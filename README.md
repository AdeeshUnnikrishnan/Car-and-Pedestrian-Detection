# Car-and-Pedestrian-Detection

Car and People Detection by using OpenCV and haar-fullbody-cascade classifier

# Interpolation :
Resizing image. Image interpolation occurs when you resize or distort your image from one pixel grid to another. Zooming refers to increase the quantity of pixels, so that when you zoom an image, you will see more detail. 

Interpolation works by using known data to estimate values at unknown points.

Types of Interpolation - 

i) INTER-NEAREST =  uses nearest-neighor, probalby the fastest fo all

ii) INTER-AREA = resamples the image using pixel area, it gives more-free results

iii) INTER-CUBIC = a biubic interpolation, i.e it is used for sharpening and enlarging the image

iv) INTER-LANCZOS4 = used for sampling the rate of digital image, it is used to rotate or resize a digital image

v) INTER-LINEAR = a bilinear interpolation (used by default)


# Parameters under detectMultiscale :

scaleFactor - specifies how much the image size is reduced to image scale.

minNeighbors - how many neighbors each candidate rectangle should have to retain it.

minSize – Minimum possible object size. Objects smaller than that are ignored.

maxSize – Maximum possible object size. Objects bigger than this are ignored.

example :

rects = cascade.detectMultiScale(img, scaleFactor=1.3,  minNeighbors=4,  minSize=(30, 30),flags=cv.CASCADE_SCALE_IMAGE)
