# Image_Recognition_pretrainedmodel

Face Recognition System Using Transfer Learning

VGG16 is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. The model achieves 92.7% top-5 test accuracy in ImageNet, which is a dataset of over 14 million images belonging to 1000 classes. It was one of the famous model submitted to ILSVRC-2014. It makes the improvement over AlexNet by replacing large kernel-sized filters (11 and 5 in the first and second convolutional layer, respectively) with multiple 3×3 kernel-sized filters one after another. VGG16 was trained for weeks and was using NVIDIA Titan Black GPU’s.


Facial recognition system : A facial recognition system is a technology capable of identifying or verifying a person from a digital image or a video frame from a video source.

ImageNet is a dataset of over 15 million labeled high-resolution images belonging to roughly 22,000 categories. The images were collected from the web and labeled by human labelers using Amazon’s Mechanical Turk crowd-sourcing tool. Starting in 2010, as part of the Pascal Visual Object Challenge, an annual competition called the ImageNet Large-Scale Visual Recognition Challenge (ILSVRC) has been held. ILSVRC uses a subset of ImageNet with roughly 1000 images in each of 1000 categories. In all, there are roughly 1.2 million training images, 50,000 validation images, and 150,000 testing images. ImageNet consists of variable-resolution images. Therefore, the images have been down-sampled to a fixed resolution of 256×256. Given a rectangular image, the image is rescaled and cropped out the central 256×256 patch from the resulting image.

Approach:

In this task, I am using Pretrained model(MobileNet) to predict the image of the persons.

In my dataset, there is the pictures of Salman Khan and Akshay Kumar.

In step 1 - I import the MobileNet pretrained model and Freeze the layers of MobileNet

In step 2 - I make the function which help to connect the FC into MobileNet

In step 3 - In this step I add the fc Head to the end of MobileNet layers

In step 4 - In this step I load my dataset

   In this dataset

     2 classes have 108 images of Salman Khan and Akshay Kumar for training the model
     
     2 classes have 26 images of Salman Khan and Akshay Kumar for testing the model   

In step 5 - Now I start traing the model
 
In the  further step I load the trained model then start predicting the images of Salman Khan and Akshay Kumar.  
