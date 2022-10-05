Today we'll practice building convolutional neural networks and applying transfer learning, working with our old friend the MNIST digit data.

1) Start by loading in the data for the digits [0, 1, 2] and preparing it for modeling, including a train-test split.

You can modify the code block given below, adding in the appropriate steps specified by the ### comments.
In particular, you should **filter down to only the first 3 digits**, **rescale pixel strengths to 0 to 1 scale**, 
and **repeat the pixel strengths across 2 additional channels**. We perform the last step to ensure that we can apply
transfer learning with base models that require 3 color channels of input.

*Hint*: For the 3rd modification, read the documentation for the `np.repeat` function. 

```

from sklearn.datasets import fetch_openml
import numpy as np
from sklearn.model_selection import train_test_split
from keras.utils import to_categorical 

mnist = fetch_openml('mnist_784')

X_digits, Y_digits = mnist.data, mnist.target.astype(np.int64)
### FILTER DOWN TO DIGITS [0,1,2]
### RESCALE THE PIXELS

# 28x28 images, with grey scale pixel strengths repeated across 3 channels for color representation
X_digits = X_digits.reshape((-1,28,28,1)) 
### REPEAT VALUES ACROSS 2 ADDITIONAL CHANNELS

X_train, X_test, y_train, y_test = (train_test_split(X_digits, Y_digits, 
                                                     test_size = .2, random_state = 42))

# 2D (one-hot encoded) representation of multiclass target 
y_train_cat = to_categorical(y_train)

```

2) Use keras to build a simple CNN model from scratch for this 3-class problem. 
With a very simple model, it should be possible to exceed 99% accuracy on train, validation, and test.

You may use the cnn lesson material as a reference for this and the next step.

3) Use keras to build a transfer learning CNN for this problem: VGG16 is recommended as the base model.
Make sure to freeze the layers in the pretrained base before training!

VGG16 requires a minimum input shape of 32x32 pixels, so you will need to add a `ZeroPadding2D(padding=2)` layer
after your input layer to slightly upsize the raw data (28x28) by adding 0s at the corners.

Prioritize getting a functioning, trainable model for this step. If time permits, try to adjust your parameters
to beat the validation and test scores you saw for your from scratch model.


