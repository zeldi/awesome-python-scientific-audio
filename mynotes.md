# Notes on using python for Audio Signal Processing (DSP)

The aim of this notes is to create a comprehensive, curated list of python related code and used for scientific research in audio/music applications.


### Counting Sliding Windows

[``skimage.util``](https://scikit-image.org/docs/dev/api/skimage.util.html?highlight=view_as_windows#skimage.util.view_as_windows) library can be used to count number the sliding window that is used during MFCC calculation

```python
from skimage import util

M = 1024 # Windows or Frame Size (samples)

slices = util.view_as_windows(audio, window_shape=(M,), step=100)
print(f'Audio shape: {audio.shape}, Sliced audio shape: {slices.shape}')
```
