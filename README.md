# Feedback Alignment in PyTorch
**This version is forked and fixed some conflictions that main implementation had with new pytorch version and upgraded to Python3**

This is a simple implementation of [Random synaptic feedback weights support error backpropagation for deep learning](https://www.nature.com/articles/ncomms13276) in PyTorch.

Base codes are adapted from [official PyTorch tutorial](http://pytorch.org/docs/master/notes/extending.html).

It implements simple MLP with one hidden layer, without non-linear activation function.

Run train_fa_vs_bp_linear_model.py to compare performance between feedback alignment vs backpropagation.
