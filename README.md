# Caltech-Bird-Classification-Using-Resnet101-t
**📖 Table of Contents**

 ➤ OverView

 ➤ DataSet

 ➤ Getting Started

      1-Data Prepration
      2-Perceptron
      3-ResNet-101
      4-Visualization


**☁️ Overview** 

 Using Caltech Bird dataset on fully connected neural network and  pretrained Resnet101 from keras  (after applying fine-tuning)
 


**🔸 DataSet**

The Caltech-UCSD Birds-200-2011  dataset of 200 bird species . it baseline experients for multi-class categorization


**📖 Getting Started**
  
_1-Data Preparation_
 
Using ImageDataGenerator  from Keras
 to  split data into train and validate and test

_2-Perceptron_
 
To implement  a fully connected neural network ( multi-layer perceptron) Therefore, need  to 
 
 -Resize the image to 32x32

 - Use Sequential API in keras
 - Import layers from keras.layers
 
![](images/img.png)
 - Build  Fully connected neural network
![](images/img_1.png)

 - Optimize the model 
![](images/img_2.png)
 - Train the model and Plot loss and accuracy 
![](images/img_3.png)
![](images/img_5.png)
 - Compare between actual classes and predicted classes
![](images/img_6.png)
_3- ResNet101_
 
this step  divided into two-step

  **First step**
 - Removing the FC layers, but leaving the other layers intact
   ![](images/img_7.png)
  

 - Plot accuracy and loss

![](images/img_8.png)
  **Second step**
 - unfreeze some convolutional layers and retrain the network
 ![](images/img_9.png)

 - Plot Accuracy and loss
      ![](images/img_10.png)     ![](images/img_11.png)

 _4- Visualization_ 
  
 Visualize the filter  by choosing  conv2_block1_2_conv layer 
![](images/img_12.png)

 Use t-SNE to observe clusters
![](images/img_13.png)

 Visualize the activation maps
![](images/img_14.png)
