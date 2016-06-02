## Autoencoding Mixture of Sines Toy Dataset

# Setting yourself up!

* [Run MNIST CNN example in Keras](https://github.com/fchollet/keras/blob/master/examples/mnist_cnn.py)

* [Read Keras autoencoder tutorial and do examples yourself](http://blog.keras.io/building-autoencoders-in-keras.html)

* [Convert 2D autoencoder to 1D using 1D convolution and pooling layers from Keras linked here](https://github.com/fchollet/keras/blob/master/keras/layers/convolutional.py#L20)

# The actual task

* [Download mixture of sine dataset](https://drive.google.com/file/d/0BwvW2DIpN6dOX1RRSGZ3NXNzR2M/view?usp=sharing)

Each second of the dataset consists of 3 sine waves played simultaneously, amplitudes are randomly changed every second. One note stays the same for 10 seconds and the other two are changed every second. We will provide labels for this later as well, so you can use it in a discriminator network. The frequencies are all spaced with 55hz, lowest frequency present is 110hz, highest is 440hz. Use this information to downsample the audio reasonably according to the Nyquist-theorem. 

Your task is to set up a pipeline. Do it carefully, so you can re-use it in the rest of the project.

- Prepare the data such that it can be used for training. i) Downsample audio ii) Chop the long audio into 1second pieces that will form the examples in your minibatch iii) Write a script that loads the data for learning.
- Use the data to test your 1D autoencoder implementation.
- Train an autoencoder with it. Try a simple model first, 1-2 layers, little filters.
- Inspect your results, write scripts that plot reconstruction and data at once, listen to reconstructions and compare between different models.

Best of luck!
