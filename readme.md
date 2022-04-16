# Hyperspectral City V2.0

## Download
https://pbdl-ws.github.io/pbdl2021/challenge/download.html

## Read Hyperspectral Cubic Data
In the dataset package, you will find a MATLAB file named *readHSD.m*, which is the MATLAB code to read the hyperspectral data. The data format is similar as RGB images, the different is the file has 128 channels rather than 3 channels.

## Dataset
### Train
In the __train__ folder, you will find all images, each of which is named with an index. In the folder, you will find four files for each image, which are:

$<*.hsd>, <rgb*.jpg>, <rgb*\_gray.png>, <rgb*.png>$

They are: 
1. the hyperspectral data file.
2. The RGB visualization of the hyperspectral image.
3. Semantic labelling coded from 0 to 18.
4. Visualization of the semantic labelling by overlay with the RGB image. 

The $*$ is the image index.
### Test
In the __test__ folder, you will find all images, each of which is named with an index. In the folder, you will find four files for each image, which is the same as training set.
### Val
In the __val__ folder, you will find three files for each image, which are:

$<rgb*.jpg>, <rgb*\_gray.png>, <rgb*.png>$

The $*$ is the image index. The images are a subset of the test set, so the corresponding hsd file($*.hsd$) is in the __test__ folder. The difference is that for an image, the label in the __val__ folder is coarse label and in the __test__ folder is fine label.
