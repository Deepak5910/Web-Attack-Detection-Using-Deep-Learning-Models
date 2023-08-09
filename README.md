
# Web-Attack-Detection-Using-Deep-Learning-Models
<h2>Team Members</h2>
Deepak Mina (201IT117)</br>
Nimish Saket (201IT139)</br>
Vishal Kumar (201IT166)</br>
<h2>Data Collection:-</h2>
The HTTP dataset CSIC 2010 was created by the Computer Security Group at the University of Madrid, and it was made available to the public in 2010. The dataset includes more than 60,000 HTTP requests and responses captured while interacting with 36 web applications. 
The dataset includes requests and responses that are associated with various types of web application vulnerabilities, including cross-site scripting (XSS), SQL injection, and directory traversal attacks. </br>

<img src="https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/download.png" width = "600px">


Dataset link:-https:  //www.kaggle.com/datasets/ispangler/csic-2010-web-application-attacks</br>
Code :- https://colab.research.google.com/drive/131SIfaaKkeMFk14TOoazsydkr2j1JvRa?usp=sharing</br>

<h2>Data Cleaning</h2>
in this dataset, 8 columns contain only unique values that's why we need to remove this column to improve the quality of the dataset
</br> Features that contain only Sigle values  ['User-Agent', 'Pragma', 'Cache-Control', 'Accept', 'Accept-encoding', 'Accept-charset', 'language', 'content-type']

<h3>Clear Missing Values</h3>
The dataset Contains some Missing values and Duplicates values so we need to handle these values to improve the efficiency of the model.</br>
<h3>Encode DataSet</h3> we used Ordinal Encoder to encode the data set</br>
Standardization of dataset:- to improve the model's efficiency we need to  Standardize the data.</br>
Z =  (Xi-mean)/std


<img src = "https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/download%20(1).png" width = "800px">
<img src = "https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/download%20(2).png" width = "800px">


<h2>Model Traning</h1>
<h3>Train-Test Split</h3>for model training and testing we need to split the dataset. while implementation we used sklearn library to split the dataset.</br>
training dataset = 80%</br>
testing dataset = 20%</br>
</br>
<h2>ANN Model:</h2></br>
<h3>Number of epochs:</h3> This parameter determines the number of times the model should iterate over the entire training dataset. and the goal is to find the best set of weights that minimize the loss function.</br>
Number of Epochs = 10
<h3>Batch size:</h3> This parameter determines the number of samples to use in each update of the model weights. A larger batch size reduces the noise in the weight updates
Batch size = 128
<h3>Optimization algorithm:</h3> This parameter determines the method used to update the model weights during training.</br></br>
Optimization algorithm: Adam</br></br>
<h3>Activation function:</h3> This parameter determines the non-linearity of the hidden layers in the ANN.</br></br>
Common activation functions = sigmoid</br>
<h3>Testing Model</h3>
<img src = "https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/ann.png" width = "800px">
<h2>CNN Model</h2>
<img src = "https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/cnn.png" width = "800px">
<h2>RNN Model</h2>
<img src = "https://github.com/Deepak5910/Web-Attack-Detection-Using-Deep-Learning-Models/blob/main/rnn.png" width = "800px">











