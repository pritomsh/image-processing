# image-processing
# Read image using Pillow

```bash
#import library
from PIL import Image
import numpy as np
```

```bash
image = Image.open("image_data/Sleeping.jpg")
# Show Image 
image.show()
#print type of image
print(type(image))
#check property of image 
print(image.format, image.size, image.mode)
# convert numpy array 
image_np =np.asarray(image)
print(type(image_np))
```
# Read Image using Matplotlib

```bash
#import library
import matplotlib.image as mpimg
import matplotlib.pyplot as plt
```

```bash
image = mpimg.imread("image_data/Sleeping.jpg")
print(type(image))
 image.shape
plt.imshow(image)
plt.colorbar()
plt.show()
```

# Read Image using Scikit_image
```bash
#import library
from skimage import io
```

```bash
image = io.imread("image_data/Sleeping.jpg")
print(type(image))
plt.imshow(image)
plt.show()
```

#  Read Image using OpenCV
```bash
#import library
import cv2
```

```bash
# Show Gray image
image = cv2.imread("image_data/Sleeping.jpg", 0)
cv2.imshow("Gray Image",image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
```bash
#Show  Color Image
image = cv2.imread("image_data/Sleeping.jpg", 1)
cv2.imshow("Color Image",image)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
Notebook : [Here](https://github.com/pritomsh/image-processing/blob/master/Read%20Image%20using%20Python.ipynb)


Ref : DigitalSreeni
