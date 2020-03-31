# Deep Learning: Logistic Regression with a Neural Network Mindset
This repo contains the Python code for the Logistic Regression with a Neural Network mindset assignment. The training data set consists of 209 images (and the test set, 50) , each with an associated label as cat (y=1) or not a cat (y=0). 

The goal is to predict which images are cats based off the image files.

The basic process is as follows:

Each image is loaded into Python and transformed first into a (64,64,3) numpy array. That is a 64 pixel wide , 64 pixel high , Red/Green/Blue array. Hence each image conists of 64x64x3=12288 pixels. The whole of the training data set can hence be stored as an array with shape (12288,209). Similarly, the test data set consists of 50 labeled images and hence can be stored as an array with shape (12288,50). Furthermore, we "flatten" the images by dividing every pixel by the maximum pixel intensity of 255.

For this example we use the sigmoid function for our output layer. We create functions that allow for the random inilization of weight parameters(W) and associated bias terms (b).

Foward propagation is used, followed by backpropagation to obtain gradients. Finally, gradient descent is applied to optimize the weights. 

Using a two layer neural network gives a high training accuracy , but only a 68% accuracy on the test set.
We improve by using a larger network to 80% accuracy on the training set.

You can test this algorithm by uploading your own images as well, the code is provided for that.
