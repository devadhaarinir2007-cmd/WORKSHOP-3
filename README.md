# WORKSHOP-3-Canny Edge Detection
## PROGRAM:
DEVELOPED BY:DEVADHAARINI.R
REGISTER NO:212225040061.
```
import cv2
import matplotlib.pyplot as plt
```
```
img = cv2.imread('boy.jpg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150)
```
```
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```
## OUTPUT:
<img width="490" height="391" alt="image" src="https://github.com/user-attachments/assets/e4d024e1-1fac-4757-83b0-39b1727e1753" />
<img width="538" height="402" alt="image" src="https://github.com/user-attachments/assets/ce46eaa9-13ea-4d4f-9e67-e8604ed96381" />
