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
### Developed By:
### Register Number: 
```
Developed by: Akash A
Register Number: 212221230003
```
i) #To Read,display the image
```python3
import cv2
import numpy as np
import matplotlib.pyplot as plt
img=cv2.imread('kimi_no_nawa.jpg')
img1=img
cv2.imshow("Original",img)
cv2.waitKey(0)
# plt.imshow(img1)
```
ii) #To write the image
```python3
cv2.imwrite("final.jpg",img1)
```
iii) #Find the shape of the Image
```python3
img.shape
```
iv) #To access rows and columns

```python3
import random
for i in range(100,500):
    for j in range(1000,1920):
        img2[i][j]=[random.randint(100,1920),random.randint(100,1920),random.randint(100,1920)]
cv.imshow("ROW_COL",img2)
cv2.waitKey(0)
# plt.imshow(img2)
```
v) #To cut and paste portion of image
```python3
end=cv2.imread('final.jpg',1)
cv2.imwrite("final2.jpg",img3)
end1=cv2.imread('final2.jpg',1)
tag=end[65:1269,950:1520]
tag1=end[65:1269,380:950]
end1[65:1269,950:1520]=tag1
end1[65:1269,380:950]=tag
cv.imshow("Inter",end1)
cv2.waitKey(0)
#plt.imshow(end1)
cv2.imwrite("rotate.jpeg",end1)
rot= cv2.imread('rotate.jpeg',1)
for i in range(950,1520):
    for j in range(65,1269):
        rot[j][570-i]=end1[j][i]
sam=rot
dam=rot
doom=rot
cv2.imwrite("IMAGE1.jpg",rot)
aot=cv2.imread('IMAGE1.jpg',1)
for i in range(380,950):
    for j in range(65,1269):
        sam[j][570-i]=doom[j][i]
cv2.imwrite('dam.jpg',dam)
name=cv2.imread('dam.jpg',1)
tagr=name[65:1269,1520:1920]
tagr1=name[65:1269,0:170]
cv2.imwrite("kimi.jpg",aot)
kimi=cv2.imread('kimi.jpg',1)
plt.imshow(kimi)
kimi[65:1269,380:780]=tagr
kimi[65:1269,780:950]=tagr1
cv.imshow("FInal",kimi)
cv2.waitKey(0)
# plt.imshow(kimi)
```

## Output:

### i) Read and display the image
[](./main.png)
### ii)Write the image
[](./write.png)
### iii)Shape of the Image
[](./shape.png)
### iv)Access rows and columns
[](./row.png)
### v)Cut and paste portion of image
[](./final.png)
## Result:
Thus the images are read, displayed, and written successfully using the python program.


