# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:LOGESHWARI.P
### Register Number: 212221230055
i) #To Read,display the image
```
import cv2
color_img=cv2.imread('puppy.jpeg',1)
cv2.imshow('Logeshwari',color_img)
cv2.waitKey(0)

  

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('puppy.jpeg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('Logeshwari',color_img)
cv2.waitKey(0)



```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('puppy.jpeg',1)
print(color_img.shape)



```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('puppy.jpeg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('Logeshwari',color_img)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```
import cv2
color_img=cv2.imread('puppy.jpeg',-1)
tag=color_img[300:400,300:400]
color_img[50:150,50:150]=tag
cv2.imshow('Logeshwari',color_img)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image


![exp1 DIP](https://user-images.githubusercontent.com/94211349/225381867-7a8581df-83aa-4b86-bce5-de15fe8254d4.png)

### ii)Write the image


![exp1a DIP](https://user-images.githubusercontent.com/94211349/225381945-1d9fa9bb-6b9d-47f6-a86c-d2950aaf0961.png)

### iii)Shape of the Image


![exp1d DIP](https://user-images.githubusercontent.com/94211349/225381992-d1e90b42-3480-4d60-a7a3-96b97d5de0bf.png)


### iv)Access rows and columns


![exp1b DIP](https://user-images.githubusercontent.com/94211349/225382073-43621d8d-8dd0-4955-b678-02af16989a8e.png)

### v)Cut and paste portion of image

![exp1c DIP](https://user-images.githubusercontent.com/94211349/225382177-e35556f1-30de-45ed-99fe-779af9fe160d.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


