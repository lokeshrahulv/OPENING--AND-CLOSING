# OPENING--AND-CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages

### Step2
Create the Text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

## Program:
```
Developed by: LOKESH RAHUL V V
Register Number:212222100024
```
### Display the input Image
```python
import cv2
import numpy as np

img = np.zeros((350, 1400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img, 'LokeshRahul', (15, 200), font, 5, (255), 10, cv2.LINE_AA)
cv2.imshow('created_text', img)
cv2.waitKey(0)
```
### Create ths structured element
```python
struct_ele = np.ones((9, 9), np.uint8)
```
### Display the result of Opening
```python
opening = cv2.morphologyEx(img, cv2.MORPH_OPEN, struct_ele)
cv2.imshow('Opening', opening)
cv2.waitKey(0)
```
### Display the result of Closing
```python
closing = cv2.morphologyEx(img, cv2.MORPH_CLOSE, struct_ele)
cv2.imshow('Closing', closing)
cv2.waitKey(0)
```
## Output:

### Display the input Image
![Screenshot 2024-05-01 155758](https://github.com/lokeshrahulv/OPENING--AND-CLOSING/assets/118423842/75140c6f-e790-49f8-957b-d63559f58e27)

### Display the result of Opening
![Screenshot 2024-05-01 155819](https://github.com/lokeshrahulv/OPENING--AND-CLOSING/assets/118423842/2ad4cd12-a8fa-451b-ab8c-d71e53318ec7)

### Display the result of Closing
![Screenshot 2024-05-01 155831](https://github.com/lokeshrahulv/OPENING--AND-CLOSING/assets/118423842/85a89446-ea1b-4190-8462-3f189b82f91e)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
