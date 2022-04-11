# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:Import cv2 and save and image as filename.jpg
<br>

### Step2:Use imread(filename, flags) to read the file.
<br>

### Step3:Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.
<br>

### Step4:Split and merge the image using cv2.split and cv2.merge commands.
<br>

### Step5:End the program and close the output image windows.
<br>

## Program:

### Developed By:Aadheeshwar.A
### Register Number:21001368
## i) Convert BGR and RGB to HSV and GRAY
~~~
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
hsv_image = cv2.cvtColor(sun_color_image, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV' ,hsv_image )
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
~~~



## ii)Convert HSV to RGB and BGR
~~~
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
hsv_image = cv2.cvtColor(sun_color_image, cv2.COLOR_HSV2RGB)
cv2.imshow('HSV2RGB' ,hsv_image )
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_HSV2BGR)
cv2.imshow('HSV2BGR', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
~~~
## iii)Convert RGB and BGR to YCrCb
~~~
mport cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb', gray_image1)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
~~~



## iv)Split and Merge RGB Image
~~~
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb', gray_image1)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()

~~~
# v) Split and merge HSV Image
~~~
import cv2
image = cv2.imread('image.jpg')
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue-Image',h)
cv2.imshow('Saturation-Image',s)
cv2.imshow('Gray-Image',v)
Merged_HSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()
~~~




## Output:
### i) BGR and RGB to HSV and GRAY
![sda](first.png)
![asd](second.png)
![saf](third.png)
<br>
<br>

### ii) HSV to RGB and BGR
![dfd](2.png)
<br>
<br>

### iii) RGB and BGR to YCrCb
![sf](3.png)
<br>
<br>

### iv) Split and merge RGB Image
![saf](4%20(1).png)
![fgfg](4%20(2).png)
<br>
<br>

### v) Split and merge HSV Image
![ghg](Screenshot%20(228).png)
![vbc](Screenshot%20(229).png)
<br>
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
