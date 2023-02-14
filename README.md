# LeNet-5
LeNet was introduced in the research paper “Gradient-Based Learning Applied To Document Recognition” in the year 1998 by Yann LeCun, Leon Bottou, Yoshua Bengio,
and Patrick Haffner. Many of the listed authors of the paper have gone on to provide several significant academic contributions to the field of deep learning.

we implemented LeNet-5 CNN for the classification of images from the MNIST dataset.

What to find in this :
->Understanding of components within a convolutional neural network

->Key definitions of terms commonly used in deep learning and machine learning

->Understanding of LeNet-5 as presented in the original research paper

->Implementation of a neural network using TensorFlow and Keras


LeNet-5 CNN architecture is made up of 7 layers.
The layer composition consists of 3 convolutional layers, 2 subsampling layers and 2 fully connected layers.

![image](https://user-images.githubusercontent.com/36032464/218644301-bde6520a-8f02-4d27-98c3-69568571d08e.png)

The first layer is the input layer — this is generally not considered a layer of the network as nothing is learnt in this layer.
The input layer is built to take in 32x32, and these are the dimensions of images that are passed into the next layer. 
Those who are familiar with the MNIST dataset will be aware that the MNIST dataset images have the dimensions 28x28.
To get the MNIST images dimension to the meet the requirements of the input layer, the 28x28 images are padded.

The grayscale images used in the research paper had their pixel values normalized from 0 to 255, to values between -0.1 and 1.175.
The reason for normalization is to ensure that the batch of images have a mean of 0 and a standard deviation of 1, the benefits of
this is seen in the reduction in the amount of training time. In the image classification with LeNet-5 example below, we’ll be normalizing
the pixel values of the images to take on values between 0 to 1.

The LeNet-5 architecture utilizes two significant types of layer construct: convolutional layers and subsampling layers.

->Convolutional layers
->Sub-sampling layers
