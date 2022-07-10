# cats_and_dogs_classification
This repository contains the python script that is used to classify a given image as an image of a dog or an image of a cat. This is a simple binary classification. 

The dataset uesed for this is available for free download on kaggle. The link to the dataset is given below.
[Kaggle] (https://www.kaggle.com/c/dogs-vs-cats)

If you do not wish to download the dataset from the website, then the datset is also available in the repository. 

# Networks used and their performance

There are two networks used for the classification. 

First network has 4 convolutional layers and 4 max pooling layers followed by a fully-connected layer. The performance of this network is not optimal because this 
arrangement leads to the overfitting of the data. 

This can be clearly seen by the graph of training accuracy and the validation accuracy which is attached below. 

The details of the network are also attached below. 

Model: "sequential_1"


Total params: 3,453,121
Trainable params: 3,453,121
Non-trainable params: 0 




![Model_Performance_sequential_1](https://github.com/ShubhamAbhayDeshpande/cats_and_dogs_classification/blob/main/Sequential_1.png)

To overcome this problem, random dropouts method was used with the dropout rate 50%. This leads to reduced overfitting and better results. 
The details of this model and the results from this model for the model and the validation accuracy are as shown in the table and the image below.


Total params: 3,453,121
Trainable params: 3,453,121
Non-trainable params: 0


![Model_Performance_sequential_2](https://github.com/ShubhamAbhayDeshpande/cats_and_dogs_classification/blob/main/Sequential_2.png)
