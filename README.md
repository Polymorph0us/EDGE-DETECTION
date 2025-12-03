# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:
Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## Program:
```
DEVELOPED BY: Keerthan D
REGISTER NUMBER: 212224240075
```
```
import cv2
import matplotlib.pyplot as plt
img=cv2.imread("dipt_img.jpg",0)
gray=cv2.cvtColor(img,cv2.COLOR_GRAY2RGB)
gray = cv2.GaussianBlur(gray,(3,3),0)
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### SOBEL EDGE DETECTOR

![image](https://github.com/user-attachments/assets/cc793e44-2a9f-47b5-a91b-6f027a0b1599)


### LAPLACIAN EDGE DETECTOR
![image](https://github.com/user-attachments/assets/67d773ea-a691-482d-b660-4bcd2fa6a08c)




### CANNY EDGE DETECTOR
![image](https://github.com/user-attachments/assets/b005eb93-e544-4d98-9779-fa68e6396b84)


## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.
