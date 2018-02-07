# corner-seeker

This project motivated by thuwc2018 implements several corner detectors in C++ with provision of Python3 API, including 

+ FAST.
+ Harris. 
+ CSS.
+ He & Yung.
+ RCSS.
+ CPDA.

which have been illustrated in [1]. 

## Testing 

You should first run `make` to finish the complication. For the most simple usage, run the following command after successful complication:

```
./detector example.png -o marked.png -l keypoints.txt -m css
```

The detector then uses CSS method to extract the corners, with image IO support by project [nothing/stb](https://github.com/nothings/stb). If you would like to use the Python3 API, see `example.py` as well, where `matplotlib` deals with the image instead. Both of them allows `-h` for more information.

## Notes

All the implementations are for the purpose of study only and thus not optimized, while several techniques, e.g., complexity improvement, multiple threads, are still used for speed-up. The following table illustrates the efficiency with I5 7200U under Ubuntu 16.04.

You may find corresponding comments in codes.

## Reference