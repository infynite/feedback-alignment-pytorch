# Feedback Alignment in PyTorch
**This version is forked and fixed some conflictions that main implementation had with new pytorch version and upgraded to Python3**

This is a simple implementation of [Random synaptic feedback weights support error backpropagation for deep learning](https://www.nature.com/articles/ncomms13276) in PyTorch.

Base codes are adapted from [official PyTorch tutorial](http://pytorch.org/docs/master/notes/extending.html).

It implements simple MLP with one hidden layer, without non-linear activation function.

Run train_fa_vs_bp_linear_model.py to compare performance between feedback alignment vs backpropagation.

## Test Results
Loss Comparison on MNIST:
epoch | step | feed alignment loss | back propagation loss
--- | --- | --- | ---
0 | 1000 | 0.46798 | 0.35344 
0 | 1875 | 0.42992 | 0.39659 
1 | 1000 | 0.43433 | 0.37663 
1 | 1875 | 0.29304 | 0.21735 
2 | 1000 | 0.41269 | 0.38590 
2 | 1875 | 0.23184 | 0.24429 
3 | 1000 | 0.35857 | 0.25014 
3 | 1875 | 0.08632 | 0.06498 
4 | 1000 | 0.18751 | 0.13469 
4 | 1875 | 0.45113 | 0.39115 
5 | 1000 | 0.26102 | 0.16991 
5 | 1875 | 0.16346 | 0.13278 
6 | 1000 | 0.29775 | 0.14079 
6 | 1875 | 0.50019 | 0.42758 
7 | 1000 | 0.26730 | 0.20934 
7 | 1875 | 0.18355 | 0.11935 
8 | 1000 | 0.46082 | 0.27962 
8 | 1875 | 0.16061 | 0.15758 
9 | 1000 | 0.17815 | 0.10925 
9 | 1875 | 0.23911 | 0.17510 
10 | 1000 | 0.55483 | 0.36205 
10 | 1875 | 0.09864 | 0.07822 
11 | 1000 | 0.22050 | 0.06755 
11 | 1875 | 0.30027 | 0.28331 
12 | 1000 | 0.30410 | 0.22639 
12 | 1875 | 0.23802 | 0.12401 
13 | 1000 | 0.38504 | 0.31829 
13 | 1875 | 0.31254 | 0.17021 
14 | 1000 | 0.30799 | 0.16914 
14 | 1875 | 0.08483 | 0.05910 
15 | 1000 | 0.11392 | 0.07960 
15 | 1875 | 0.33861 | 0.30033 
16 | 1000 | 0.53456 | 0.25107 
16 | 1875 | 0.29415 | 0.14761 
17 | 1000 | 0.14059 | 0.07061 
17 | 1875 | 0.10071 | 0.06098 
18 | 1000 | 0.34540 | 0.13852 
18 | 1875 | 0.32415 | 0.16791 
19 | 1000 | 0.34725 | 0.24961 
19 | 1875 | 0.34411 | 0.19213 
20 | 1000 | 0.14642 | 0.09837 
20 | 1875 | 0.06806 | 0.04413 
21 | 1000 | 0.16839 | 0.04480 
21 | 1875 | 0.15662 | 0.08321 
22 | 1000 | 0.24548 | 0.09513 
22 | 1875 | 0.24273 | 0.07480 
23 | 1000 | 0.33001 | 0.14574 
23 | 1875 | 0.27394 | 0.17840 
24 | 1000 | 0.27252 | 0.10221 
24 | 1875 | 0.39897 | 0.24693 
25 | 1000 | 0.25453 | 0.12092 
25 | 1875 | 0.51975 | 0.14524 
26 | 1000 | 0.24217 | 0.09227 
