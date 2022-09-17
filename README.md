# TMLC-Problem  Bark Texture Images Classification 

Problem Statement - Train any neural network of your choice on the given 50 bark texture dataset. Prepare an in-depth notebook on the same. Explain each and every step in suitable words. Unique approach will carry more grade.
Dataset source:- https://www.kaggle.com/datasets/saurabhshahane/barkvn50 

The Dataset consists of bark texture of 50 trees using deep learning. There is a total of 5,578 images in the dataset.
 
### Problem with the Dataset:
Class Imbalance was prevalent in the dataset as some classes had around 60-80 images(minority classes) while some had 100+ & 200+(majority classes). This could affect the model training and its performance so it must be solved.

### Model and Data split 
The dataset is train,validation and test using pre-trained model which is MobileNetV3Small.The dataset is split into  90% for training and 10% for testing. In 90% of training  dataset  again split to  90% for training  and  10% for validation . 

###Model summary
Model: "model"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 input_2 (InputLayer)        [(None, 224, 224, 3)]     0         
                                                                 
 MobilenetV3small (Functiona  (None, 7, 7, 576)        939120    
 l)                                                              
                                                                 
 global_average_pooling2d (G  (None, 576)              0         
 lobalAveragePooling2D)                                          
                                                                 
 dense (Dense)               (None, 50)                28850     
                                                                 
=================================================================
Total params: 967,970
Trainable params: 28,850
Non-trainable params: 939,120
_________________________________________________________________


### Training Accuracy : 99.80%

### Testing Accuracy : 96.05%
