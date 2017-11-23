# CameraCalibration
[![Build Status](https://travis-ci.org/MuteBardTison/CameraCalibration.svg?branch=master)](https://travis-ci.org/MuteBardTison/CameraCalibration)
[![release](http://github-release-version.herokuapp.com/github/MuteBardTison/CameraCalibration/release.svg?style=flat)](https://github.com/MuteBardTison/CameraCalibration/releases)

This is an implementation of Camera Calibration method with OpenCV in C++.

Using image-processing program GIMP to find the coordinates of the frame and the corresponding pixel coordinates on the image.

Each square of the chessboard is 60mm.

To remove the perspective distortion on Donald's image.

## Usage

```
cd <source directory>
mkdir build
cd build
cmake ..
make
./CV_donald_annotated_points ../donald_annotated_points.jpg
```

## Input
![donald_annotated_points](https://user-images.githubusercontent.com/25029380/33165125-fb2762ea-d035-11e7-94c4-57ce5ca82388.jpg)

## Output
Showing the homography matrix from the pixel coordinates to the coordinates in the frame

Demonstrating with iTerm2

<img width="565" alt="screen shot 2017-11-23 at 10 34 14 am" src="https://user-images.githubusercontent.com/25029380/33166275-facdde24-d039-11e7-9f0a-9acec4c2ebaf.png">
Calibrated Donald's figure:
<img width="335" alt="screenshot" src="https://user-images.githubusercontent.com/25029380/33164898-15fe8bc6-d035-11e7-9e54-010be8d9116b.png">

## License
[MIT](https://github.com/MuteBardTison/CameraCalibration/blob/master/LICENSE) © Zihan Qi
