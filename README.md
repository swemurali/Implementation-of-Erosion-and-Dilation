# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:

Import the necessary packages.

### Step2:

Create the Text using cv2.putText.

### Step3:

Create the structuring element.

### Step4:

Erode and Dilate the image.

### Step5:

End Program.

## Program:
```
Developed by: M.Suwetha
Register no: 212221230112
```
``` 
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt



# Create the Text using cv2.putText
img1 = np.zeros((100,270), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'aakaash',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')


# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))




# Erode the image

image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')



# Dilate the image

image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```
## Output:

### Display the input Image

![i-1](https://user-images.githubusercontent.com/94165336/235293781-f0c53be1-f3cf-491f-b448-4d4fae0c4e18.png)

### Display the Eroded Image

![i-2](https://user-images.githubusercontent.com/94165336/235293804-4cf76585-c29c-453b-bf26-697feb48e1bc.png)


### Display the Dilated Image

![i-3](https://user-images.githubusercontent.com/94165336/235293813-c5d306f7-f917-458c-bd2d-2f9061777951.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
