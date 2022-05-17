# HyViD (Synthetic Hyperspectral Array Video Database)

[CURRENTLY FOR REVIEWERS ONLY]

The actual data can be found here: https://drive.google.com/drive/folders/1JWPaA_w0LW-v4JmYigPaMVVSA0pi6IDZ?usp=sharing

The watermarks will be removed in the final version of this database.

Our novel synthetic <ins>Hy</ins>perspectral <ins>Vi</ins>deo <ins>D</ins>atabase (HyViD) provides seven scenes rendered from 400 nm to 700 nm in 30 nm steps, resulting in 31 hyperspectral channels. 
The videos have a length of 30 frames.
Furthermore, the scenes are rendered using a camera array using nine cameras arranged in a three times three grid.
The camera array is arranged as follows:
```
[View from front onto the sensor]
0 - 1 - 2
|   |   |
3 - 4 - 5
|   |   |
6 - 7 - 8
```

Thus, camera 4 is the center camera.

The folder structure is:
```
camera -> channel -> frame
```

For more details please refer to the paper "A Synthetic Hyperspectral Array Video Database with Applications to Cross-Spectral Reconstruction and Hyperspectral Video Coding".

If you are interested in the source files, e.g., because you want to render the scenes using a different camera array, please write to frank.sippel[at]fau.de.
