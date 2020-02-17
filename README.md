[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"
[image2]: ./images/vgg16_model.png "VGG-16 Model Keras Layers"
[image3]: ./images/vgg16_model_draw.png "VGG16 Model Figure"


## Project Overview

Welcome to the Convolutional Neural Networks (CNN) project in the AI Nanodegree! In this project, you will learn how to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images.  Given an image of a dog, your algorithm will identify an estimate of the canine’s breed.  If supplied an image of a human, the code will identify the resembling dog breed.  

![Sample Output][image1]

Along with exploring state-of-the-art CNN models for classification, you will make important design decisions about the user experience for your app.  Our goal is that by completing this lab, you understand the challenges involved in piecing together a series of models designed to perform various tasks in a data processing pipeline.  Each model has its strengths and weaknesses, and engineering a real-world application often involves solving many problems without a perfect answer.  Your imperfect solution will nonetheless create a fun user experience!

## The libraries used
- sklearn
- keras
- numpy
- glob
- cv2
- matplotlib

## the motivation for the project
Mainly to develop a pipeline that can be used within a web or mobile app to process real-world, user-supplied images. Given an image of a dog, your algorithm will identify an estimate of the canine's breed. If supplied an image of a human, the code will identify the resembling dog breed.

## the files in the repository with a small description of each
- bottleneck_features: folder to store the bottleneck_features for the transfer learning models.
- haarcascades: store pre-trained face detectors.
- images: the images we are using in the readme and the description part of the jupyter notebook.
- images_for_step7: images to test our algorithm at step 7.
- requirements: the basic requirements of getting the notebook running.
- saved_models: the model saved for best validation scores.
- dog_app.ipynb: the jupuyter notebook of the whole pipeline
- extract_bottleneck_features.py: the file to extract bottleneck features

## a summary of the results of the analysis
The final results seems pretty accuracy, we can see that the dog breed prediction for dogs are all correct, and the resembling breed for human are make sense. 
Transfer learning works way more better than the CNN model I built from scratch. Mainly because the model from transfer learning is trained by a large amount of data, so the architecture already understood what kind of features are most representative for a image, which makes the classification process much more easier, and we don't need to sacrifice the accuracy even if we don't have a large amount of data.

## Acknowledgements
Thanks to the guidance of Udacity DSND!
