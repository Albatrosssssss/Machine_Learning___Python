

# How do Machines Store Images?
~~~
pyimport pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
from skimage.io import imread, imshow

image = imread('image_8_original.png', as_gray=True)
imshow(image)

#checking image shape 
image.shape, image
~~~
# Method #1: Grayscale Pixel Values as Features
# pixel features

~~~
features = np.reshape(image, (660*450))

features.shape, features
~~~
