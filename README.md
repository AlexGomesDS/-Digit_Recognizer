# Digit_Recognizer Kaggle Challenge
Python code for the kaggle challenge https://www.kaggle.com/c/digit-recognizer

## Competition Description
MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

In this competition, your goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. We’ve curated a set of tutorial-style kernels which cover everything from regression to neural networks. We encourage you to experiment with different algorithms to learn first-hand what works well and how techniques compare.

## Data preparation
The original Kaggle train dataset has 42k labeled records with 28x28=784 features. This means it takes 10 min to train a logistic regression with 10k records only. In an attempt to overcome this problem we reduced the dimensionality of the problem by downsampling the images to 14x14 pixels (which yields 196 features) and storing it in the */input* folder. This comes at the cost of some information loss, however one can agree that even with this resolution the class of the digit's is recognizable.  
The code used to generate this images can be found in the file */src/data_prep.ipynb*.
