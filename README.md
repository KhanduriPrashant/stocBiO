# stocBiO and ITD-BiO for hyperparameter optimization and meta-learning
Codes for paper [Bilevel Optimization: Nonasymptotic Analysis and Faster Algorithms](https://arxiv.org/pdf/2010.07962.pdf).

Our hyperparameter optimization implementation is bulit on [HyperTorch](https://github.com/prolearner/hypertorch), where we propose stoc-BiO algorithm with better performance than other bilevel algorithms.
The implementation of stoc-BiO is located in two experiments [l2reg_on_twentynews.py](https://github.com/JunjieYang97/StocBio_hp/tree/master/experimental/l2reg_on_twentynews.py) and [mnist_exp.py](https://github.com/JunjieYang97/StocBio_hp/tree/master/experimental/mnist_exp.py). We will implement our stoc-BiO as a class for an independent use soon!  

Our meta-learning part is built on [learn2learn](https://github.com/learnables/learn2learn), where we show the bilevel optimizer ITD-BiO converges faster than MAML and ANIL.

In the following, we provide some experiments to demonstrate the better performance of the proposed stoc-BiO algorithm. 

We compare our algorithm to various hyperparameter baseline algorithms on newspaper dataset:

<img src="Hyperparameter-optimization/results/test_loss_alg.png" width="350">

We evaluate the performance of our algorithm with respect to different batch sizes:

<img src="Hyperparameter-optimization/results/test_loss_batch.png" width="350">

The comparison results on MNIST dataset:

<img src="Hyperparameter-optimization/results/test_loss_mnist.png" width="350">

This repo is still under construction and any comment is welcome! 
