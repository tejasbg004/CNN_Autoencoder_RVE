# CNN_Autoencoder-RVE
Deep learning method to learn equivalent material constant for RVE.


# Intro
A composite material consist of various materials exhibiting multiple mechancial properties. High Fidelity model such as FE methods need lot of computational resources for extremely fine mesh grains.Representative Voolume Element(RVE) is a technique to condense these multi properties into a single property. The task in this project is to fit a Function(defined by an autoencoder and a FC NN) to map 2D RVE images to equivalent material property.

# Autoencoder
The given input is 28*28 dimensional image. Given the number of samples we have(2000) fitting a vanilla based CNN will overfit the model. Hence, it is necesary to reduce the dimension of the input to a manifold defined by an autoencoder.

# DNN
This ipynb file contains trained Fully Connected Neural Network that maps data present in the low dimensional manifold concatenated with corresponding Youngs modulous and poissons ratio to the equivalent material property.
