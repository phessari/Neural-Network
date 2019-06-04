# Neural-Network- FeedForward NN, CNN, RNN

A feedforward neural network model, also known as deep neural network (DNN) or multi-layer perceptron (MLP), is the most common type of Deep Neural Network. Neural Networks can be visualized as a series of connected layers that form a network. It contains three types of layers:

1.Input Layer: Each unit of the layer contains a feature


2.Hidden Layers: there could be several hidden layers in a NN. They successively transform feature values from input layer to out layer.


3.Output Layer: contains the output resulted from hidden layers


It is called feedforward because the features are fed forward through the Network. All parameters are initialized randomly by Gaussian or normal uniform distribution. It would be a good idea to scale the features before training. Then the features are fed to the network. The output values are compared to the true values by loss function (Forward Propagation). Then the algorithm goes backward (Backward Propagation) through the network and changes the weight in order to improve the output. 

Several other types of DNNs are popular as well, such as Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs). MLPs work well on transactional (tabular) data; however if you have image data, then CNNs are a great choice. If you have sequential data (e.g. text, audio, time-series), then RNNs are a good choice. 

Here we construct a feedforward NN for binary classification. The design of NN is NOT an easy matter. For each NN, the number of hidden layer, the number of units in each hidden layer and its activation function should be defined. For compiling the NN, we also need to define loss function, optimizer and metrics depends on the problem at hand. 

Here, we used the IMDB datasets. Dataset of 25,000 movies reviews from IMDB, labeled by sentiment (positive/negative). Reviews have been preprocessed, and each review is encoded as a sequence of word indexes (integers). 

