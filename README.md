# Face Mask detection using Convolutional Neural Network
# Overview
A Convolutional Neural network (CNN) is a type of Artificial Neural network designed to process pixel data. They are used explicitly in Image Processing and Image Recognition.
# CNN Model Pipeline
First, we will input RGB images with a resolution of 128×128 pixels. These images will then be processed by a Convolutional Neural Network (CNN) model, which will extract 128 relevant feature vectors. Subsequently, these feature vectors will be used to train various machine learning classifiers.

We will import all the necessary libraries required for this project. These include libraries such as NumPy, which is used for performing complex mathematical calculations, and TensorFlow, which is used for machine learning tasks, among others.

Next, we will label these images: images with masks will be assigned a label of 1, and images without masks will be assigned a label of 0. Finally, we will split the dataset into training and testing sets using the "train_test_split" function from the sklearn library.

We combined both arrays into a single array and normalized each pixel value to be between 0 and 1 by dividing them by 255.
Next, we will build our Convolutional Neural Network (CNN). First, we will use an image data generator to augment our dataset by creating additional images from the existing ones. This image generator will perform operations such as resizing, and adjusting contrast.

After applying transfer learning, we will add a flattening layer to convert the 2D matrix into a 1D array. Next, we will apply dense and dropout layers to perform the classification.Finally, we will train our model with a batch size of 32 and for epochs=5. The computational power requirements can be adjusted as needed.

Now, we will generate additional images from our dataset using the Image Data Generator. Next, we will set our hyperparameters, such as learning rate, batch size, and number of epochs. Finally, we will train our pre-trained CNN model and evaluate its accuracy on the test set.
