# Digit_Recognizer Kaggle Challenge
Python code for the kaggle challenge https://www.kaggle.com/c/digit-recognizer

## Competition Description
MNIST ("Modified National Institute of Standards and Technology") is the de facto “hello world” dataset of computer vision. Since its release in 1999, this classic dataset of handwritten images has served as the basis for benchmarking classification algorithms. As new machine learning techniques emerge, MNIST remains a reliable resource for researchers and learners alike.

In this competition, your goal is to correctly identify digits from a dataset of tens of thousands of handwritten images. We’ve curated a set of tutorial-style kernels which cover everything from regression to neural networks. We encourage you to experiment with different algorithms to learn first-hand what works well and how techniques compare.

## Data preparation script

- Description: If we reduce the train dataset to 10k records only with 28x28 pixels, it takes 10 min to train the logistic regression. 
In an attempt to overcome this problem we reduced the dimensionality of the problem by downsampling the images to 14x14 pixels.
This comes at the cost of some information loss, however one can agree that even with this resolution the class of the digit's is recognizable.

- Script: *src/data_prep.ipynb*

- Input: original Kaggle datasets: 42K labeled records with 28x28=784 features
*data/train.csv*, *data/test.csv*

- Output: new dataset with images of 14x14 pixels (which yields 196 features)
*data/train_14x14.csv*, *data/test_14x14.csv*
