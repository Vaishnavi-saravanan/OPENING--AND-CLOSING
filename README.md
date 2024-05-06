# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2:
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

 
## Program:
```
Developed by: VAISHNAVI S
Register Number:212222230165
```

``` Python
# Import the necessary packages

import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'HAKUNA MATATA', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)


# Create the Text using cv2.putText

import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'HAKUNA MATATA', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)

# Create the structuring element

struct_ele = np.ones((9, 9), np.uint8)

# Use Opening operation


opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)

# Use Closing Operation

closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)



```
## Output:

### Display the input Image
![323062992-bad781f7-6480-42d1-aa26-5f746f71e721](https://github.com/Vaishnavi-saravanan/OPENING--AND-CLOSING/assets/118541897/9e020127-06bc-4424-92db-c3c6e01da2a8)

### Display the result of Opening
![323063004-2464d703-8c36-4282-b2f1-5d8c90ae27bd](https://github.com/Vaishnavi-saravanan/OPENING--AND-CLOSING/assets/118541897/27542499-2b47-4bf2-9ca7-e4b790e88f51)



### Display the result of Closing
![323063031-979f37f9-547b-4cd7-bce4-ab3dfc1bd79d](https://github.com/Vaishnavi-saravanan/OPENING--AND-CLOSING/assets/118541897/124a69d2-e072-4eef-bc26-f65e11c1d745)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
