# HyViD (Synthetic Hyperspectral Array Video Database)

## Source

Since some of the source files are too big, the source can be found here: https://gitlab.lms.tf.fau.de/frank.sippel/hyvid

## Database
The actual data can be found here: https://data.fau.de/public/76/27/336172776/

Our novel synthetic <ins>Hy</ins>perspectral <ins>Vi</ins>deo <ins>D</ins>atabase (HyViD) provides seven scenes rendered from 400 nm to 700 nm in 10 nm steps, resulting in 31 hyperspectral channels. 
The videos have a length of 30 frames.
Furthermore, the scenes are rendered using a camera array using nine cameras arranged in a three times three grid. Depth maps for every camera and frame are provided as well.
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

## Framework Usage
If you execute main.py using Python3 everything should work as long as Blender is installed and executable in command line by *blender*.
You can also execute "run.py" within Blender if you want to model a new scene and execute it.
If you add textures to objects, the name of an "Image Texture" must be the same as the name of the folder.
If you want to move the camera, please move the "cam_center". This camera is used to calculate the positions of the other cameras.
Currently, if you name a light source "sun", then the spectrum of the sun is applied.
Otherwise, if the name of a light source ends with 'K', then the number in front of it determines the light spectrum according to the black body radiation, e.g., a light source with name *3200K* will lead to a light spectrum of a black body at 3200K temperature.

## License
The database and source are licensed using CC-BY-SA.
If you use the dataset or source for your research, you should cite the follwing paper:
```
@article{Sippel:23,
	author = {Frank Sippel and J\"{u}rgen Seiler and Andr\'{e} Kaup},
	journal = {J. Opt. Soc. Am. A},
	number = {3},
	pages = {479--491},
	publisher = {Optica Publishing Group},
	title = {Synthetic Hyperspectral Array Video Database with Applications to Cross-Spectral Reconstruction and Hyperspectral Video Coding},
	volume = {40},
	month = {Mar},
	year = {2023},
}
```

## Original 3D models

Family House:
House: https://www.blendswap.com/blend/23878
Trees & Bush: https://www.blendswap.com/blend/14644
Car: https://blendswap.com/blend/13575

Medieval Seaport:
Scene: https://blendswap.com/blend/6115

City:
Scene: https://www.blendswap.com/blend/25505
Car: https://www.blendswap.com/blend/16710

Outdoor:
Scene: https://www.blendswap.com/blend/5957

Indoor:
Scene: https://www.blendswap.com/blend/6468

Lab:
Small man: https://blendswap.com/blend/14431
Cups: https://blendswap.com/blend/4499
Figure: https://blendswap.com/blend/4499
Cardboard: https://blendswap.com/blend/19402
Porsche: https://blendswap.com/blend/11182
White lily: https://blendswap.com/blend/12953
Monstera: https://blendswap.com/blend/27517
Table: https://www.blendswap.com/blend/17037
