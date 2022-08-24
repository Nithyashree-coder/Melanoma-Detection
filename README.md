# Melanoma Detection
To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
* [Overview](#Overview)
* [Observations](#Observations)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## Overview
The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.

The data set contains the following diseases:

    * Basal cell carcinoma
    * Actinic keratosis
    * Dermatofibroma
    * Pigmented benign keratosis
    * Nevus
    * Squamous cell carcinoma
    * Melanoma
    * Seborrheic keratosis
    * Vascular lesion

## Observations
- The data set contained 2357 images of 9 skin cancer types.
- The target class lebels were 'actinic keratosis', 'basal cell carcinoma', 'dermatofibroma', 'melanoma', 'nevus', 'pigmented benign keratosis', 'seborrheic keratosis', 'squamous cell carcinoma' and 'vascular lesion'
- Train-test Split - 80% of the images were used for training, and 20% for validation.
- On the initial dataset, training accuracy is observed to be around 90% whereas validation accuracy is around 56%. This shows the model is overfitting
- To eliminate class imbalance, data augmentation was used to generate more images to the training set.
- seborrheic keratosis class has the least number of samples.
- melanoma and pigmented benign keratosis dominate the data in terms of proportionate number of samples.
- When epoch is increased to a high value around 50, the training accuracy is increased but the validation accuracy remains static as the training progresses.
- The gap of validation and train accuracy is increasing with epoch more than 10. Similar trend is there for loss function as well.
- When number of epochs are increased to 20, we observed overfitting. If the number of epochs are lesser than 10, the model was learning properly with less accuracy in the training.
- After increasing epochs and class rebalancing, the accuracy improved.


## Acknowledgements
This project is created as part of upgrad assignment on melanoma detection. With this, complex problems like convolutional neural networks built from scratch was learnt.  

## Contact
Created by [@Nithyashree-coder] - feel free to contact me!
