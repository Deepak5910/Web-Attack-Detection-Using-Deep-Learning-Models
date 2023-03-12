
# Web-Attack-Detection-Using-Deep-Learning-Models

</br>

Team Members</br>
Deepak Mina (201IT117)</br>
Nimish Saket (201IT139)</br>
Vishal Kumar (201IT166)</br>
##
1). Data Collection:-</br>

The HTTP dataset CSIC 2010 was created by the Computer Security Group at the University of Madrid, and it was made available to the public in 2010. The dataset includes more than 60,000 HTTP requests and responses, which were captured while interacting with 36 different web applications. 
The dataset includes requests and responses that are associated with various types of web application vulnerabilities, including cross-site scripting (XSS), SQL injection, and directory traversal attacks. </br>


Dataset link:-https:  //www.kaggle.com/datasets/ispangler/csic-2010-web-application-attacks</br>
Code :- https://colab.research.google.com/drive/131SIfaaKkeMFk14TOoazsydkr2j1JvRa?usp=sharing</br>

##

</br>
2) Data Cleaning</br>
in this dataset 8 columns contain only unique values that's why we need to remove this columns to improve the quality of dataset
</br> Features that contain only Sigle values  ['User-Agent', 'Pragma', 'Cache-Control', 'Accept', 'Accept-encoding', 'Accept-charset', 'language', 'content-type']

a)Clear Missing Values</br>
Dataset Contain some Misssing values and Duplicates values so we need to handle these values to improve the efficiency of the model.</br>

b)Encode DataSet :- we used Ordinal Encoder to encode the data set</br>
c)Standardization of dataset:- inorder to improve the efficiency of the model we need to  Standardize the data.</br>
Z =  (Xi-mean)/std
##


3) Model Traning</br>
a)Train-Test Split:-for model training and testing we need to split the dataset. while implementation we used sklearn library to split the dataset.</br>
</br>
training dataset = 80%</br>
testing dataset = 20%</br>
</br>
b) ANN Model:</br>
a)Number of epochs: This parameter determines the number of times the model should iterate over the entire training dataset.and the goal is to find the best set of weights that minimize the loss function.</br></br>
Number of Epochs = 10</br>
b)Batch size: This parameter determines the number of samples to use in each update of the model weights. A larger batch size reduces the noise in the weight updates</br></br>
Batch size = 128</br></br>
c)Optimization algorithm:This parameter determines the method used to update the model weights during training.</br></br>
Optimization algorithm: Adam</br></br>
d)Activation function: This parameter determines the non-linearity of the hidden layers in the ANN.</br></br>
Common activation functions = sigmoid</br>
</br>




<br>
4) Testing Model:-
while testing the model we got the below output:-</br>
Epoch 1/10</br>
382/382 [==============================] - 3s 3ms/step - loss: 0.0513 - accuracy: 0.9931</br>
Epoch 2/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 2.5919e-04 - accuracy: 1.0000</br>
Epoch 3/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 8.2901e-05 - accuracy: 1.0000</br>
Epoch 4/10</br>
382/382 [==============================] - 2s 4ms/step - loss: 4.3180e-05 - accuracy: 1.0000</br>
Epoch 5/10</br>
382/382 [==============================] - 2s 4ms/step - loss: 2.5956e-05 - accuracy: 1.0000</br>
Epoch 6/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 1.7169e-05 - accuracy: 1.0000</br>
Epoch 7/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 1.1629e-05 - accuracy: 1.0000</br>
Epoch 8/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 7.8827e-06 - accuracy: 1.0000</br>
Epoch 9/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 6.9083e-06 - accuracy: 1.0000</br>
Epoch 10/10</br>
382/382 [==============================] - 1s 3ms/step - loss: 5.1903e-06 - accuracy: 1.0000</br>
382/382 [==============================] - 1s 1ms/step</br>
Test accuracy: 1.0</br>











