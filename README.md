# Non-vacuous Generalization Bounds at the ImageNet Scale: a PAC-Bayesian Compression Approach

This repository contains everything necessary to reproduce the experiments
in our paper: Non-vacuous Generalization Bounds at the ImageNet Scale: a PAC-Bayesian
Compression Approach.


## LeNet-5 pruning

The directory [compression_lenet]
contais the scripts which implement the training, pruning, quantization and evaluation of the LeNet-5 network.


## MobileNet Pruning

The directory [compression-mobilenet]
contains the scripts which implement the pruning, quantization, and evaluation of noise stability of our network.
The typical compression pipeline would be to take an already trained network (such as those available [here](https://research.googleblog.com/2017/06/mobilenets-open-source-models-for.html))
and prune then quantize the network. Please see the [readme](scripts/compression-mobilenet/README.md)
for more details on compressing MobileNet.

## CIFAR-10 randomization tests

The directory [randomization-cifar](scripts/randomization-cifar)
contains the scripts which implement the training and pruning of a ResNet-56 on the CIFAR-10 dataset
with a portion of the labels randomized.
