# Dynamical loss functions for Machine Learning

This repository contains the code that reproduces the main results of our paper [Tilting the playing field: Dynamical loss functions for machine learning](https://arxiv.org/abs/2102.03793) (Miguel Ruiz-Garcia, Ge Zhang, Samuel S. Schoenholz and Andrea J. Liu).


## What is a dynamical loss function?

**Loss functions** are one of the pillars of supervised learning. They quantify the performance of a model at classifying the training data, and training a neural network reduces to minimizing one specific loss function. In this work we propose that changing the loss function during training (minimization) can lead to better results. In a **dynamical loss function**, we weight equally the contribution of each sample belonging to the same class, and then oscillate these weights during minimization. During each oscillation the model focuses more in one class, helping the system to learn it better. During training we tipically cycle through all the classes multiple times.


## Why should I care?

In our [paper](https://arxiv.org/abs/2102.03793) we show:

* Using a dynamical loss function can enable learning when the neural network was too small or the learning rate was too large for the model to learn the training data using a standard loss functions. 

* Using a dynamical loss function can improve generalization in cases where the model was already able to learn the training data using a standard loss function.

* Dynamical loss functions lead to complex learning dynamics. The loss function landscape is changing as the parameters of the neural network change to locally minimize it. The valleys that the model is descending during minimization are oscillating in high and width, what leads to instabilities when the valleys are too narrow. These instabilities appear as bifurcations in the learning dynamics that emerge when the largest eigenvalues of the Hessian cross a threshold.


## Running the code

It was brought to our attention that our code had changed its behavior and did not reproduce the results of the paper. We have updated our code to
solve this, please use this [Colab Notebook](https://github.com/miguel-rg/dynamical-loss-functions/blob/main/Updated_dynamical_loss_functions_for_machine_learning_github_no_NTK.ipynb). As a side effect, at the moment this code does not compute the NTK or the Hessian.

Our original code is still in the repository, [dynamical_loss_functions_for_machine_learning](https://github.com/miguel-rg/dynamical-loss-functions/blob/main/dynamical_loss_functions_for_machine_learning_github.ipynb). Be aware that, at the moment, this code does not reproduce the results of the paper.

