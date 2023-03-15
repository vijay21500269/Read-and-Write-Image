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
i) # To Read,display the image
```
import cv2
color_image = cv2.imread('lion.jpeg',1)
cv2.imshow('vijay-212221230121',color_image)
cv2.waitKey(0) 
cv2.destroyAllWindows

```
ii) # To write the image
```
import cv2
color_image = cv2.imread('lion.jpeg',1)
cv2.imwrite('lion.png',color_image)
cv2.waitKey(0)
```
iii) # Find the shape of the Image
```
import cv2
img=cv2.imread('lion.jpeg',-1)
print(img.shape)

```
iv) # To access rows and columns

```
import cv2
img=cv2.imread('lion.jpeg',-1)
for i in range(100,150):
    for j in range(10,255):
        img[i][j]=[255,100,255] #blue green red
cv2.imshow('212221230121-R.Vijay',img);
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) # To cut and paste portion of image
```
import cv2
img1=cv2.imread('lion.jpeg',-1)
copied_portion=img1[10:60,10:120]
img1[110:160,110:220]=copied_portion
cv2.imshow('212221230121',img1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image

![OP1](https://user-images.githubusercontent.com/94381788/225405591-1f5da5d0-698d-4b4f-bd73-2a0b0efa22e1.png)



### ii)Write the image

![op2](https://user-images.githubusercontent.com/94381788/225405645-096796b6-d778-46f4-8948-35746dc25500.png)

### iii)Shape of the Image

![op3](https://user-images.githubusercontent.com/94381788/225405648-4a3ab7a9-e88f-4e6f-b154-97804936547a.png)

### iv)Access rows and columns
![op4](https://user-images.githubusercontent.com/94381788/225405653-c915bfd2-fe5b-4cb0-804f-5fa5e6edf014.png)

### v)Cut and paste portion of image

![op5](https://user-images.githubusercontent.com/94381788/225405676-25217f2a-929d-41dc-bd93-a67c7809e5df.png)
## Result:
Thus the images are read, displayed, and written successfully using the python program.


