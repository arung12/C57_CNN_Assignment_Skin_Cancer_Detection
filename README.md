# Project Name
> Melanoma Detection Assignment

## Table of Contents
* [General Info](#general-information)
* [Approach](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)

## General Information
This Assignment will aim to build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Approach

1. [Importing Necessary Modules](#Importing-all-the-important-libraries)
2. [Data Understanding](#Data-Understanding)
3. [Create a dataset](#Create-a-dataset)
4. [Visualize the data](#Visualize-the-data)
5. [Create the model](#Create-the-model)
    - [Simple Model](#Simple-Model)
    - [Model With Dropouts](#Model-With-Dropouts)
    - [Model With Increased Feature Maps](#Model-With-Increased-Feature-Maps)
    - [Model with Additional Layers](#Model-with-Additional-Layers)
6. [Data Augmentation](#Data-Augmentation)
     - [Using Preprocessing Data Augmentation Layer](#Using-Preprocessing-Data-Augmentation-Layer)
     - [Using ImageDataGenerator](#Using-ImageDataGenerator)
7. [Handling Class Imbalance](#Handling-Class-Imbalance)
     - [Ploting Class Distriubution](#Ploting-Class-Distriubution)
     - [Generating images with Augmentor](#Generating-images-with-Augmentor)
     - [Model building on updated Augmentor data](#Model-building-on-updated-Augmentor-data)
8. [Conclusion](#Conclusion)


## Conclusions


 1. created a simple model and observed the training accuracy of 90% and validation accuracy of 51%
 2. it is observed that the model is overfitting and tried to resolve with dropouts
 3. the model with dropout had a training accuracy of 89% and a validation accuracy of 50%
 4. created another model with more feature maps which resulted in  a training accuracy of 87% and validation accuracy of 51%
 5. created another model with one more layer which resulted in  a training accuracy of 84% and validation accuracy of 52%
 6. All the above experiments failed to resolve the overfitting of the model, so started experimenting with data augmentation
 7. Created a model with a data augmentation layer using the TensorFlow preprocessing library which resulted in  a training accuracy of 45% and validation accuracy of 41%. Which is actually underfitting the model
 8. Tried different Data Augmentation strategies with ImageDataGenerator, the model resulted in  a training accuracy of 72% and validation accuracy of 42%. Which is still an underfitting model
 9. Verified the dataset for class imbalance and found that actually seborrheic keratosis, dermatofibrom, actinic keratosis has least samples and pigmented benign keratosis, Melanoma has more sample
10. handling the class imbalance by adding 500 samples to each of them using an augmentor 
11. Created a new model on the updated dataset with dropouts, so we can close the gap between training and validation accuracy and achieved  a training accuracy of 89% and validation accuracy of 86%
12. Using the above model verified the predictions on some random images


## Technologies Used
- numpy - version 1.5.3
- pandas - version 1.24.3
- matplotlib - version 3.7.1
- tensorflow - version 2.10

## Contact
Created by [@arung12] - feel free to contact me!