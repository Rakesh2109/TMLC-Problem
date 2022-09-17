# TMLC-Problem  Bark Texture Images Classification 

Problem Statement - Train any neural network of your choice on the given 50 bark texture dataset. Prepare an in-depth notebook on the same. Explain each and every step in suitable words. Unique approach will carry more grade.
Dataset source:- https://www.kaggle.com/datasets/saurabhshahane/barkvn50 

The Dataset consists of bark texture of 50 trees using deep learning. There is a total of 5,578 images in the dataset.
 
### Problem with the Dataset:
Class Imbalance was prevalent in the dataset as some classes had around 60-80 images(minority classes) while some had 100+ & 200+(majority classes). This could affect the model training and its performance so it must be solved.

### Model and Data split 
The dataset is train,validation and test using pre-trained model which is MobileNetV3Small.The dataset is split into  90% for training and 10% for testing. In 90% of training  dataset  again split to  90% for training  and  10% for validation . 

### Model Parameters
Total params: 967,970

Trainable params: 28,850

Non-trainable params: 939,120


### Training Accuracy : 99.80%

### Testing Accuracy : 96.05%
### Model  Classification Report

test accuracy = 96.05734767025089 %

              precision    recall  f1-score   support

           0       1.00      1.00      1.00        12
           1       1.00      0.86      0.92         7
           2       1.00      1.00      1.00        11
           3       1.00      1.00      1.00        21
           4       1.00      1.00      1.00        13
           5       1.00      1.00      1.00        18
           6       1.00      0.94      0.97        16
           7       1.00      1.00      1.00        12
           8       1.00      1.00      1.00        12
           9       1.00      1.00      1.00        26
          10       1.00      1.00      1.00        10
          11       1.00      1.00      1.00        11
          12       1.00      1.00      1.00         6
          13       1.00      1.00      1.00         7
          14       0.89      1.00      0.94         8
          15       1.00      1.00      1.00         9
          16       0.83      1.00      0.91        10
          17       0.67      0.50      0.57         8
          18       0.94      0.94      0.94        18
          19       1.00      1.00      1.00        14
          20       1.00      0.88      0.93         8
          21       0.95      0.95      0.95        19
          22       1.00      1.00      1.00        14
          23       1.00      1.00      1.00         7
          24       1.00      1.00      1.00        12
          25       1.00      0.80      0.89        10
          26       1.00      1.00      1.00        13
          27       1.00      1.00      1.00         7
          28       0.92      0.86      0.89        14
          29       1.00      1.00      1.00         5
          30       1.00      1.00      1.00         8
          31       0.83      1.00      0.91        10
          32       1.00      1.00      1.00        10
          33       1.00      1.00      1.00        13
          34       0.89      0.89      0.89         9
          35       1.00      1.00      1.00        13
          36       0.88      0.88      0.88         8
          37       1.00      1.00      1.00         5
          38       0.89      1.00      0.94         8
          39       1.00      1.00      1.00        11
          40       0.86      1.00      0.92         6
          41       0.88      0.70      0.78        10
          42       1.00      1.00      1.00         9
          43       1.00      1.00      1.00         6
          44       1.00      0.91      0.95        11
          45       0.79      1.00      0.88        11
          46       0.76      0.87      0.81        15
          47       1.00      1.00      1.00        18
          48       1.00      1.00      1.00         9
          49       1.00      0.90      0.95        10
    accuracy                           0.96       558
    macro_avg      0.96      0.96      0.96       558
    weighted avg   0.96      0.96      0.96       558
