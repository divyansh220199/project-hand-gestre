# Hand Gesture Recognition
Goal is to recognize hand gestures. I've trained the model on my own dataset using Perceptron. I've included my the dataset in the repository itself. In it's present state the model is trained to recognize just five gestures but can easily be trained for many hand gestures. I'll also upload the code that I'm using for capturing the hand an processing it for training the model.

Model gives a high testing accuracy of about 95% using just two convolution and three Dense layers. But if you want to train more hand gestures then you'll probably need more a complex network.

Images in the dataset are of dimension 275 by 275. But for performance reasons they have been resized to 50 by 50. You can use them as it is if you have a powerful setup otherwise program displays a Tensorflow error tensorflow/core/framework/allocator.cc:101] Allocation of X exceeds 10% of system memory.

# What's in the Repository 
* `capturing hand images.ipynb` - This program can capture new hand gestures and write them in the specified directory
* `recognizer.ipynb` - This is the main program that uses pretrained model (in the repo) for recognizing hand gestures
* `demo.mp4` - This is the main program that uses pretrained model (in the repo) for recognizing hand gestures
* `combining images and getting a single file.ipynb` - This is the main program that uses pretrained model (in the repo) for recognizing                                                        hand gestures
* `sample images` - This is the main program that uses pretrained model (in the repo) for recognizing hand gestures
* `loading dataset and training model.ipynb` - This program uses the given dataset to train the Perceptron model

# Required External libraries
* `cv2 (opencv)`
* `pickle`
* `glob`
* `sklearn (scikit-learn)`
* `keras`
* `numpy`

# Future
I hope to implement more than five gestures in the future. There will be further improvements in the code itself too.

# CNN Implementation
As of Jan, 2020 I have used CNN for the recognition of 5 gestures. 

# Improvements and Differences
I've used both the Perceptron as well as the CNN Model for recognition of 5 hand gestures. And I can easily say CNN works better for extracting features of an image. There's and improvement of Error %age from 32% to 5%. This happens because Perceptron model is a simple 1 dimensional set of neurons, therefore it reduces a lot of features in the images whereas the CNN is specially designed to work with images and works on 2 dimensional set of neurons.
