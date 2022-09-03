# CarDamageDetection_NN
The aim of this project is to implement a method to detect car damages using convolutional neural network. 

# Table of Contents
 1. Introduction '
 2. Motivation
 3. Data 
 4. Model
 5. Evaluation 
 6. Validation Results
 7. Conclusion
 8. Credit

# Introduction
In this world of data, deep learning techniques have helped us in creating models which reduces time and labour. Detecting car damages with the help of deep learning technqiues is easier than a person checking the damage out. This project mainly focuses on predicting whether a car has damage or not.

# Motivation 
The idea behind this project was to focus on a real world issue faced by the insurance companies. Usually when an insured car gets damaged, the owner has to notify the insurance company and the police  immediately. The insurance company then assigns a surveyor to take a look at the damage and has to come with an evaluation for the loss. As the world gets more digital day by day, this process of having a surveyor to look at the damage can be eliminated and Artificial Intelligence can take up this task making the process less time consuming and more efficient.

# Data
The data used for this project has been collected from google. The training set contains 1840 images belonging to two classes - ‘damaged’ and ‘no damage’. The testing dataset contains 460 images, belonging to two classes. The images were downloaded using the google extension ‘Image Downloader’ and later unwanted or unrelated images were deleted, making the data clean for the process.

![Screenshot (6)](https://user-images.githubusercontent.com/81976818/188277937-601f8371-8188-45d2-8731-962ea01409c9.png)


# Model 
The main aim of the model is to detect whether the car has damage or not. So, this is a case of binary classification. We have only two classes- ‘Damaged’ & ‘Not Damaged’. A normal convolutional neural network has been used as the model here. 
  1. The model contains one convolutional layer with relu as its activation function. 
  2. A pooling layer is given afterwards. Another convolutional layer was added with 128 units. 
  3. Flattening process was done. 
  4. Fully connected layers were added and the output layer was defined with sigmoid as its activation function as it is a binary classification problem.

# Evaluation 
As the images in the dataset have different sizes, the first step was to resize the images to 150x150. The model was built using the tensorflow framework. It was first trained and then predicted on the test dataset. 

If the result was 0 then the product would predict the car as damaged and if it was 1 then the model would predict the car as not damaged. 
![Screenshot (8)](https://user-images.githubusercontent.com/81976818/188278135-ed2a4e09-8aa2-4315-a1ed-6a622311f81e.png)

This is the graph showing the train and test error. The validation loss was found to be 0.6 and the
loss was 0.1. The testing error needs to be lowered. But both the losses are considerable for the
model.

![Screenshot (7)](https://user-images.githubusercontent.com/81976818/188278061-2f9376f9-b1a5-45e6-ac4a-9214cc62b82b.png)

# Validation Results 
The below images show two of the validation results obtained. One result shows that the car is damaged and the other has predicted that the car is not damaged. 

![Screenshot (9)](https://user-images.githubusercontent.com/81976818/188278203-a5ceadc1-a837-4f7d-b13a-74e1a73d0b16.png)

![Screenshot (10)](https://user-images.githubusercontent.com/81976818/188278286-2473a615-6291-4008-b4d1-7948cdd7e20d.png)

# Conclusion
1. The model can be made better by using the Mask R CNN as it deals with bounding boxes and it will show us the exact area where the damage has occured 
2. The accuracy of the model can be increased by adding more layers and working that out

# Credit 
Google Images Download - This project wouldn't have been possible without this tool. It saved my enormous amount of time while collecting the data.
