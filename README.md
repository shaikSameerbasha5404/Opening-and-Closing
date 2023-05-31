# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.

### Step2:
Create the Text using cv2.putText.

### Step3:
Use Opening operation.


### Step4:
Use Opening operation.


### Step5:
Use Closing Operation.
 
## Program:

``` Python
### Developed by:shaik sameer basha
### Register No: 212222240093
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Create the Text using cv2.putText
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
im=cv2.putText(img1,'sameer',(5,70),font,2,(255),5,cv2.LINE_AA)
cv2.imshow ("image",im)
cv2.waitKey(0)
cv2.destroyAllWindows()
# Create the structuring element
Kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))
# Use Opening operation
image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,Kernel)
cv2.imshow("opening image",image1)
cv2.waitKey(0)
cv2.DestroyAllWindows()
# Use Closing Operation
image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,Kernel)
cv2.imshow("closeing image",image1)
cv2.waitKey(0)
cv2.DestroyAllWindows()
```
## Output:

### Display the input Image
![Screenshot from 2023-05-11 10-24-38](https://github.com/shaikSameerbasha5404/Opening-and-Closing/assets/118707756/98151656-2854-4f16-be1d-17936e51dccc)


### Display the result of Opening

![Screenshot from 2023-05-11 10-25-35](https://github.com/shaikSameerbasha5404/Opening-and-Closing/assets/118707756/963bfcfb-d833-4767-a898-2947f7da4994)


### Display the result of Closing
![Screenshot from 2023-05-11 10-26-28](https://github.com/shaikSameerbasha5404/Opening-and-Closing/assets/118707756/55b3bfeb-6692-497f-908c-3a46c8619689)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
