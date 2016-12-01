"# CSC421Assginment4Question5" 

README

To run, type the following commands:

import os

os.chdir("Your Download Directory Here")

ex.) os.chdir("C:\Users\Clami\OneDrive\University\CSC 421\Assignment4")

from src import mnist_loader

training_data, validation_data, test_data = mnist_loader.load_data_wrapper()

import network

net = network.Network([784, 10])

net.SGD(training_data, 10, 3.0, test_data=test_data)
