# Image Processing Onramp #
This is a note for information in the course "Image Processing Onramp"
Link: https://matlabacademy.mathworks.com/details/image-processing-onramp/imageprocessing

## outcome of the course:
1. import -> Import, display, and manipulate color and grayscale images.
2. preprocess -> 
3. segment -> Create binary images by thresholding pixel intensity values.
4. postprocess -> Improve image segmentation by using common pre- and postprocessing techniques.
5. classify -> Develop a metric to classify an image, and apply that metric to a set of image files.

## loading image ## 
-> imread()
eg: I = imread("0001.jpg")

## showing image ## 
-> imshow()
eg: imshow(I)

## view images
-> imshowpair()
The "montage" option places the images A1 and A2 side by side, with A1 on the left and A2 on the right.
eg: imshowpair(I, I2, montage)

## export processed image
-> imwrite()
eg: imwrite(I1, "img.png")