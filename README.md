# Multi-Class-Image-Classification-with-CNN
Multi - Class Image Classification using Convolutional Neural Network

##

**Main dataset**
  - **url source:** https://www.kaggle.com/trolukovich/apparel-images-dataset
  - **size:** consists of 24 categories
 
 We, later, split the dataset to:
  1. Training data
  2. Validation data
  3. Test data
  
 ##
 
 **CNN architecture**
 
        Model: "sequential_1"
        _________________________________________________________________
        Layer (type)                 Output Shape              Param #   
        =================================================================
        conv2d_1 (Conv2D)            (None, 222, 222, 32)      896       
        _________________________________________________________________
        max_pooling2d_1 (MaxPooling2 (None, 111, 111, 32)      0         
        _________________________________________________________________
        conv2d_2 (Conv2D)            (None, 109, 109, 32)      9248      
        _________________________________________________________________
        max_pooling2d_2 (MaxPooling2 (None, 54, 54, 32)        0         
        _________________________________________________________________
        conv2d_3 (Conv2D)            (None, 52, 52, 64)        18496     
        _________________________________________________________________
        max_pooling2d_3 (MaxPooling2 (None, 26, 26, 64)        0         
        _________________________________________________________________
        dropout_1 (Dropout)          (None, 26, 26, 64)        0         
        _________________________________________________________________
        flatten_1 (Flatten)          (None, 43264)             0         
        _________________________________________________________________
        dense_1 (Dense)              (None, 128)               5537920   
        _________________________________________________________________
        dropout_2 (Dropout)          (None, 128)               0         
        _________________________________________________________________
        dense_2 (Dense)              (None, 24)                3096      
        =================================================================
        Total params: 5,569,656
        Trainable params: 5,569,656
        Non-trainable params: 0
        
        
 ##
 
 **Results**
 
 Test Accuracy (after 10 epochs): **0.87**
 
 ##
 
 **Tools**
 
 - Keras
 - Tensorflow
 - scikit-learn (for splitting the dataset)
 - jupyter notebook
 - Pillow (Python Image Library)
