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
```py
Developed by: RAJA R
Register Number:212222100041
```
### Display the input Image
```py
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'RAJA R(CS)', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```py
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```py
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```java
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![Screenshot 2024-04-16 214225](https://github.com/Raja8334/OPENING--AND-CLOSING/assets/120719634/b6b2eae4-b84f-4be2-bc46-3851672017df)


### Display the result of Opening
![Screenshot 2024-04-16 214259](https://github.com/Raja8334/OPENING--AND-CLOSING/assets/120719634/fd61348f-c146-4116-83bc-8ddc353ced57)


### Display the result of Closing
![Screenshot 2024-04-16 214324](https://github.com/Raja8334/OPENING--AND-CLOSING/assets/120719634/dd93aedd-78de-43bd-9af7-a48a753d9640)


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
