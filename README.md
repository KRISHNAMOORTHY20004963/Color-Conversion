# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
 Convert BGR and RGB to HSV and GRAY

### Step2:
Convert HSV TO RGB AND BGR

### Step3:
Convert RGB and BGR to YCrCb

### Step4:
To Split and merge RGB Image

### Step5:
To Split and merge HSV Image

## Program:
```python
# Developed By: S.krishnamoorthy
# Register Number: 212220230025

# i) Convert BGR and RGB to HSV and GRAY
import cv2
img = cv2.imread('kimo.jpg')
cv2.imshow('Original Image',img)
img1 = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',img1)
img2 = cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',img2)

img3 = cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',img3)

img4 = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',img4)
cv2.waitKey(0)





# ii)Convert HSV to RGB and BGR
cv2.imshow('Original Image',img)

img5 = cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',img5)
img6 = cv2.cvtColor(img,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV2RGB',img6)
cv2.waitKey(0)





# iii)Convert RGB and BGR to YCrCb
cv2.imshow('Original Image',img)

img7 = cv2.cvtColor(img,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',img7)

img8 = cv2.cvtColor(img,cv2.COLOR_BGR2YCrCb)
cv2.imshow('RCB2YCrCb',img8)
cv2.waitKey(0)




# iv)Split and Merge RGB Image
red = img[:,:,0]
green = img[:,:,1]

blue = img[:,:,2]
img9=cv2.merge((blue,green,red))
cv2.imshow('Merged',img9)
cv2.waitKey(0)



# v) Split and merge HSV Image
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow("ORIGINAL HSV_IMAGE",hsv)
h,s,v = cv2.split(hsv)
img10=cv2.merge((h,s,v))
cv2.imshow('Merged',img10)
cv2.waitKey(0)





```
## Output:
### i) BGR and RGB to HSV and GRAY

![kimo exp3](https://user-images.githubusercontent.com/75241177/165580022-dfd0be32-0854-4a84-8c3c-d428b8013e60.jpg)


### ii) HSV to RGB and BGR
![kimo exp3 1](https://user-images.githubusercontent.com/75241177/165580080-76e8ce4e-9932-4c2a-a1fe-08510e756044.jpg)


### iii) RGB and BGR to YCrCb


![kimo exp3 2](https://user-images.githubusercontent.com/75241177/165580918-ebdfc6a0-7caf-4221-ad07-4f8af888191b.jpg)


### iv) Split and merge RGB Image

![kimo exp3 3](https://user-images.githubusercontent.com/75241177/165580623-89f79826-bda4-4f66-b2ce-11deaf7159af.jpg)




### v) Split and merge HSV Image

![kimo exp3 4](https://user-images.githubusercontent.com/75241177/165580693-89462834-ba00-4c9c-8880-7a464d6ebf47.jpg)



## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.

