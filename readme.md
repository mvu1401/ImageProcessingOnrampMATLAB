# Image Processing Onramp #
This is a note for information in the course "Image Processing Onramp" <br />
Link: https://matlabacademy.mathworks.com/details/image-processing-onramp/imageprocessing

## outcome of the course:
1. import -> Import, display, and manipulate color and grayscale images.
2. preprocess & postprocess -> Improve image segmentation by using common pre- and postprocessing techniques.
3. segment -> Create binary images by thresholding pixel intensity values.
4. classify -> Develop a metric to classify an image, and apply that metric to a set of image files.
## Import & Export image

### loading image
-> imread() <br/>
eg: I = imread("0001.jpg")

### showing image
-> imshow() <br/>
eg: imshow(I)

### view images
-> imshowpair() <br/>
The "montage" option places the images A1 and A2 side by side, with A1 on the left and A2 on the right.
eg: imshowpair(I, I2, montage)

### export processed image
-> imwrite() <br/>
eg: imwrite(I1, "img.png")

## Colors in image
Matlab store image in array of intensity <br/>
size of picture = size of array = [row; cols] = [height; width] <br/>
### extract specific color of RGB image
-> I(:, :, X) with X: red =1, green =2, blue =3 <br/>
we can also use Image Processing Toolbox: using imsplit() <br/>
eg: [R, G, B] = imsplit(A)

### display color planes at once
-> montage({R,G,B})

### get max/min intensity of specific color
-> Rmax = max(R, [], "all") <br/>
-> Rmin = min(R, [], "all") <br/>
Using the "all" option finds the maximum across all values in the array. The brackets are required; they are placeholders for an unused input. 