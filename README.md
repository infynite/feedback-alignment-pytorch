# Feedback Alignment in PyTorch
**This version is forked and fixed some conflictions that main implementation had with new pytorch version and upgraded to Python3**

This is a simple implementation of [Random synaptic feedback weights support error backpropagation for deep learning](https://www.nature.com/articles/ncomms13276) in PyTorch.

Base codes are adapted from [official PyTorch tutorial](http://pytorch.org/docs/master/notes/extending.html).

It implements simple MLP with one hidden layer, without non-linear activation function.

Run train_fa_vs_bp_linear_model.py to compare performance between feedback alignment vs backpropagation.

## Test Results
Loss Comparison on MNIST:
epoch 0 step 1000 loss_fa 0.46798 loss_bp 0.35344
epoch 0 step 1875 loss_fa 0.42992 loss_bp 0.39659
epoch 1 step 1000 loss_fa 0.43433 loss_bp 0.37663
epoch 1 step 1875 loss_fa 0.29304 loss_bp 0.21735
epoch 2 step 1000 loss_fa 0.41269 loss_bp 0.38590
epoch 2 step 1875 loss_fa 0.23184 loss_bp 0.24429
epoch 3 step 1000 loss_fa 0.35857 loss_bp 0.25014
epoch 3 step 1875 loss_fa 0.08632 loss_bp 0.06498
epoch 4 step 1000 loss_fa 0.18751 loss_bp 0.13469
epoch 4 step 1875 loss_fa 0.45113 loss_bp 0.39115
epoch 5 step 1000 loss_fa 0.26102 loss_bp 0.16991
epoch 5 step 1875 loss_fa 0.16346 loss_bp 0.13278
epoch 6 step 1000 loss_fa 0.29775 loss_bp 0.14079
epoch 6 step 1875 loss_fa 0.50019 loss_bp 0.42758
epoch 7 step 1000 loss_fa 0.26730 loss_bp 0.20934
epoch 7 step 1875 loss_fa 0.18355 loss_bp 0.11935
epoch 8 step 1000 loss_fa 0.46082 loss_bp 0.27962
epoch 8 step 1875 loss_fa 0.16061 loss_bp 0.15758
epoch 9 step 1000 loss_fa 0.17815 loss_bp 0.10925
epoch 9 step 1875 loss_fa 0.23911 loss_bp 0.17510
epoch 10 step 1000 loss_fa 0.55483 loss_bp 0.36205
epoch 10 step 1875 loss_fa 0.09864 loss_bp 0.07822
epoch 11 step 1000 loss_fa 0.22050 loss_bp 0.06755
epoch 11 step 1875 loss_fa 0.30027 loss_bp 0.28331
epoch 12 step 1000 loss_fa 0.30410 loss_bp 0.22639
epoch 12 step 1875 loss_fa 0.23802 loss_bp 0.12401
epoch 13 step 1000 loss_fa 0.38504 loss_bp 0.31829
epoch 13 step 1875 loss_fa 0.31254 loss_bp 0.17021
epoch 14 step 1000 loss_fa 0.30799 loss_bp 0.16914
epoch 14 step 1875 loss_fa 0.08483 loss_bp 0.05910
epoch 15 step 1000 loss_fa 0.11392 loss_bp 0.07960
epoch 15 step 1875 loss_fa 0.33861 loss_bp 0.30033
epoch 16 step 1000 loss_fa 0.53456 loss_bp 0.25107
epoch 16 step 1875 loss_fa 0.29415 loss_bp 0.14761
epoch 17 step 1000 loss_fa 0.14059 loss_bp 0.07061
epoch 17 step 1875 loss_fa 0.10071 loss_bp 0.06098
epoch 18 step 1000 loss_fa 0.34540 loss_bp 0.13852
epoch 18 step 1875 loss_fa 0.32415 loss_bp 0.16791
epoch 19 step 1000 loss_fa 0.34725 loss_bp 0.24961
epoch 19 step 1875 loss_fa 0.34411 loss_bp 0.19213
epoch 20 step 1000 loss_fa 0.14642 loss_bp 0.09837
epoch 20 step 1875 loss_fa 0.06806 loss_bp 0.04413
epoch 21 step 1000 loss_fa 0.16839 loss_bp 0.04480
epoch 21 step 1875 loss_fa 0.15662 loss_bp 0.08321
epoch 22 step 1000 loss_fa 0.24548 loss_bp 0.09513
epoch 22 step 1875 loss_fa 0.24273 loss_bp 0.07480
epoch 23 step 1000 loss_fa 0.33001 loss_bp 0.14574
epoch 23 step 1875 loss_fa 0.27394 loss_bp 0.17840
epoch 24 step 1000 loss_fa 0.27252 loss_bp 0.10221
epoch 24 step 1875 loss_fa 0.39897 loss_bp 0.24693
epoch 25 step 1000 loss_fa 0.25453 loss_bp 0.12092
epoch 25 step 1875 loss_fa 0.51975 loss_bp 0.14524
