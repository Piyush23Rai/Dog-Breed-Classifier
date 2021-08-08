
### Table of Contents

1. [Installation](#installation)
2. [Project Overview](#overview)
3. [Files in the Repository](#files)
4. [Instructions](#Instructions)
5. [Observations](#observations)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

Install all necessary libraries given in requirements.txt file.  The code should run with no issues using Python versions 3.*. 

## Project Overview<a name="overview"></a>

Welcome to the Convolutional Neural Networks (CNN) project! In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

Along with exploring state-of-the-art CNN models for classification, you will make important design decisions about the user experience for your app.  Our goal is that by completing this lab, you understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer

## Files in the Repository<a name="files"></a>

    • bottleneck_features
	|- DogInceptionV3Data.npz #file that contains bottlneck features corresponding to InceptionV3 Network.
	|- DogResnet50Data.npz #f file that contains bottlneck features corresponding to Resenet-50 Network data.
	|- DogVGG16Data.npz #f file that contains bottlneck features corresponding to VGG16 Network.
    • haarcascades
     	|- haarcascade_frontalface_alt.xml #xml file that has features extracted on the basis haarcascade implementation of OpenCV.
    • images #folder that contain all the samples images over which the algorithm will be tested
    • saved_models 
      |- weights.best.from_scratch.hdf5 #file that contains weights corresponding to CNN model built from scratch.
      |- weights.best.InceptionV3.hdf5 #file that contains weights corresponding to InceptionV3 CNN model.
	|- weights.best.Resnet50.hdf5 #file that contains weights corresponding to Resnet-50 CNN model.
	|- weights.best.VGG16.hdf5 #file that contains weights corresponding to VGG16 CNN model.
    • requirements #folder containing all the requirements for the project along with the requirements.txt file for libraries.
    • dog_app.ipynb #jupyter notebook where the project implementation is carried out.
    • extract_bottleneck_features.py #utility file to extract bottleneck features.
    • LICENSE.txt
    • README.md



## Instructions <a name="Instructions"></a>


1. Install all the necessary libraries in the requirements.txt file
2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/dogImages`. 

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder. 

4. You may download the botteneck features from the link provided in the notebook should you wish to use any other than what is already downloaded (I have used InceptionV3 and VGG16 which will need to be downloaded).
	
3. Run the Jupyter notebook Starbucks.ipynb till the end to get the results.

## Observations<a name="observations"></a>

The Observations corresponding to each technique is discussed in the notebook.


## Licensing, Authors, Acknowledgements<a name="licensing"></a>

The entire project in partial fulfilment towards completing Udacity's Data Science Nanodegree Program.

The videos and lectures guided me to understand and implement each technique.
There were quite a lot of medium posts that helped me with the implementation, links to which are given below.

1. [MTCNN](https://medium.com/r?url=https%3A%2F%2Ftowardsdatascience.com%2Fhow-does-a-face-detection-program-work-using-neural-networks-17896df8e6ff)
2.[Resnet-50](https://medium.com/r?url=https%3A%2F%2Ftowardsdatascience.com%2Funderstanding-and-coding-a-resnet-in-keras-446d7ff84d33%23%3A%7E%3Atext%3DThe%2520ResNet%252D50%2520model%2520consists%2Cover%252023%2520million%2520trainable%2520parameters.%26text%3DOur%2520ResNet%252D50%2520gets%2520to%2Cin%252025%2520epochs%2520of%2520training)
3.[VGG-16](https://medium.com/r?url=https%3A%2F%2Ftowardsdatascience.com%2Fstep-by-step-vgg16-implementation-in-keras-for-beginners-a833c686ae6c%23%3A%7E%3Atext%3DVGG16%2520is%2520a%2520convolution%2520neural%2Cvision%2520model%2520architecture%2520till%2520date.%26text%3DIt%2520follows%2520this%2520arrangement%2520of%2Cconsistently%2520throughout%2520the%2520whole%2520architecture)





