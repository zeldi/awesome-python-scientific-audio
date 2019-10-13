# Python for Scientific Audio 

The aim of this repository is to create a comprehensive, curated list of python software/tools related and used for scientific research in audio/music applications.


### Counting Sliding Sindows

``skimage.util`` library can be used to count number the sliding window that is used during MFCC calculation

```
from skimage import util

M = 1024 # Windos or Frame Size (samples)

slices = util.view_as_windows(audio, window_shape=(M,), step=100)
print(f'Audio shape: {audio.shape}, Sliced audio shape: {slices.shape}')
```
