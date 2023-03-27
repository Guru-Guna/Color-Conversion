# COLOUR-CONVERSION
## AIM:
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## SOFTWARE REQUIRED:
Anaconda - Python 3.7
## ALGORITHM:
### Step1:
Import cv2 and save and image as filename.png

### Step2:
Use imread(filename, flags) to read the file

### Step3:
Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.

### Step4:
Split and merge the image using cv2.split and cv2.merge commands.

### Step5:
End the program and close the output image windows.

## PROGRAM:

Developed By : Gunaseelan G

Register Number : 212221230031
# i) Original Image
```
import cv2
uni = cv2.imread('lamboo.jpg')
cv2.imshow('Original image',uni)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# ii) Convert BGR to HSV 
```
import cv2
uni = cv2.imread('lamboo.jpg')
hsv_image = cv2.cvtColor(uni, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV' ,hsv_image )
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# iii)Convert BGR to GRAY
```
import cv2
uni = cv2.imread('lamboo.jpg')
gray_image = cv2.cvtColor(uni, cv2.COLOR_BGR2GRAY)
cv2.imshow( 'BGR2GRAY', gray_image)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# iv) Convert RGB to HSV
```
import cv2
uni = cv2.imread('lamboo.jpg')
hsv_image = cv2.cvtColor(uni, cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV', hsv_image)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# v)  Convert RGB to GRAY
```
import cv2
uni = cv2.imread('flamboo.jpg')
gray_image1 = cv2.cvtColor (uni, cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
# vi) Convert HSV to RGB
```
import cv2
uni = cv2.imread('lamboo.jpg')
RGB_image = cv2.cvtColor(uni,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# vii)  Convert HSV to BGR
```
import cv2
uni = cv2.imread('lamboo.jpg')
BGR_image = cv2.cvtColor(uni,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# viii)  Convert RGB to YCrCb
```
import cv2
uni = cv2.imread('lamboo.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# ix) Convert BGR to YCrCb
```
import cv2
uni = cv2.imread('lamboo.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
# x) Merge RGB Image
```
import cv2
uni = cv2.imread('lamboo.jpg')
blue=uni[:,:,0]
green=uni[:,:,1]
red=uni[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)

merged_BGR=cv2.merge((blue,green,red))
cv2.imshow('Merged BGR Image',merged_BGR)
cv2.waitKey(0)
cv2.destoryAllWindows()
```
# xi) Split HSV Image
```
import cv2
uni = cv2.imread('lamboo.jpg')
hsv=cv2.cvtColor(uni,cv2.COLOR_BGR2HSV)
h,s,v=cv2.split(hsv)
cv2.imshow("Hue-image",h)
cv2.imshow("Saturation-image",s)
cv2.imshow("gray-image",v)
```
# xii) Merge HSV Image
```
Merged_HSV=cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()
```
## OUTPUT:
### i) Original Image
![](output1.png)

### ii) Convert BGR to HSV
![](output2.png)

### iii)Convert BGR to GRAY
![](output3.png)


### iv) Convert RGB to HSV
![](output4.png)


### v) Convert RGB to GRAY
![](output5.png)


### vi) Convert HSV to RGB
![](output6.png)


### vii) Convert HSV to BGR
![](output7.png)


### viii) Convert RGB to YCrCb
![](output8.png)


### ix) Convert BGR to YCrCb
![](output9.png)


### x) Merge RGB Image

![rchannel](https://user-images.githubusercontent.com/93427255/228011664-2ed69ee7-8d01-4eaf-99d6-50843d3559d3.png)

![gchannel](https://user-images.githubusercontent.com/93427255/228016079-66e30125-c00b-47dd-b09f-7cdb05df8e39.png)

![bchannel](https://user-images.githubusercontent.com/93427255/228014963-9204e65a-9198-46a7-b39c-fd5975f5cb49.png)

![merged bgr](https://user-images.githubusercontent.com/93427255/228011596-b3a0cf9b-2331-4e7b-8d5e-291308691691.png)



### xi) Split HSV Image and xii) Merge HSV Image

![saturation](https://user-images.githubusercontent.com/93427255/228012206-42758cbd-5dff-4bd6-90b2-ede7c4e7b723.png)

![hue](https://user-images.githubusercontent.com/93427255/228016128-20edd335-72f7-4d5f-80ec-752fc0e2c86e.png)

![grayimg](https://user-images.githubusercontent.com/93427255/228016151-deeca302-f8c6-417c-b88f-5c86b49ae692.png)

![lastone](https://user-images.githubusercontent.com/93427255/228016167-362ea6fb-771e-4d55-a463-9313d1d8995a.png)



## RESULT:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
