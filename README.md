### READ AND WRITE AN IMAGE
### AIM:
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

### Software Required:
Anaconda - Python 3.7

### Algorithm:

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
### Program:
### Developed By: Guruprasad B
### Register Number: 212221230032
i) #To Read,display the image
```
import cv2
pic=cv2.imread("Husky.jpg",1)
cv2.imshow("212221240005",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
ii) #To write the image
```
import cv2
pic=cv2.imread("Husky.jpg",1)
cv2.imshow("212221240005",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
iii) #Find the shape of the Image
```python3

import cv2
pic = cv2.imread('Husky.jpg',1)
print(pic.shape)

```
iv) #To access rows and columns

```python3
import random
import cv2
pic=cv2.imread("Husky.jpg",1)
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212221230005",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```python3
import cv2
pic=cv2.imread("Husky.jpg",1)
crop=pic[300:400,300:400]
pic[50:150,50:150]=crop
cv2.imshow("212221240005",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()


```

### Output:

### i) Read and display the image

![out1](https://user-images.githubusercontent.com/95342910/224757698-0c79a028-3fc9-4d9f-8d43-cb6e525c170e.png)


### ii)Write the image

![out2](https://user-images.githubusercontent.com/95342910/224757797-abbc14ae-f879-43a1-962f-383ab5cf6324.png)


### iii)Shape of the Image

![out3](https://user-images.githubusercontent.com/95342910/224758075-bea33050-e784-4686-9464-c9fa8210a5b9.png)


### iv)Access rows and columns

![out4](https://user-images.githubusercontent.com/95342910/224758134-0e819ea7-903f-41af-88d4-90b5167b6ac5.png)


### v)Cut and paste portion of image

![out5](https://user-images.githubusercontent.com/95342910/224758185-044b47a2-5a3e-4ff7-8132-191c44d3ecef.png)


### Result:
Thus the images are read, displayed, and written successfully using the python program.


