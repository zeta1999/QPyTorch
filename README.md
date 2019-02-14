# QPyTorch

QPyTorch is a low-precision arithmetic simulation package implemented through
PyTorch. QPyTorch is designed to support researches on low-precision machine
learning, especially in low-precision training. 

Notably, QPyTorch supports quantizing different numbers in the training process
with customized low-precision formats. This eases the process of investigating
different precision setting and developing new deep learning architectures. More
concretely, QPyTorch implements fused kernels for quantization and integrates
smoothly with existing PyTorch kernels (e.g. matrix multiplication, convolution). 

Recent researches can be reimplemented easily through QPyTorch. We offer an
example replicate of [WAGE](https://arxiv.org/abs/1802.04680) in a downstream
repo [WAGE.qpytorch](https://github.com/Tiiiger/WAGE.pytorch). We provide a list
of working examples under [Examples](#examples).

*Note*: QPyTorch relies on PyTorch functions for the underlying computation,
such as matrix multiplication. Therefore, QPyTorch is not intended to be used to
study the numerical behavior of different accumulation strategies.

## Installation
- Python >= 3.6
- PyTorch >= 1.0

Install QPyTorch through pip:
```bash
pip install qtorch
```

## Documentation
See our [read the docs](www.google.com)

## Tutorials
- [An overview of QPyTorch's features](https://github.com/Tiiiger/QPyTorch/blob/master/examples/tutorial/Functionality_Overview.ipynb)
- [CIFAR-10 Low-Precision Training Tutorial](https://github.com/Tiiiger/QPyTorch/blob/master/examples/tutorial/CIFAR10_Low_Precision_Training_Example.ipynb)

## Examples
- Low-Precision VGGs and ResNets using fixed point, block floating point on CIFAR and ImageNet. [lp_train](https://github.com/Tiiiger/QPyTorch/blob/master/examples/lp_train)
- Reproduction of WAGE in QPyTorch. [WAGE.qpytorch](https://github.com/Tiiiger/QPyTorch/blob/master/examples)
- Reproduction of 8-bit Floating Point Training in QPyTorch. [IBM8.qpytorch](https://github.com/Tiiiger/QPyTorch/blob/master/examples)

## Team
* Tianyi Zhang (Cornell University)
* Zhiqiu Lin (Cornell University)
* [Guandao Yang](http://www.guandaoyang.com/) (Cornell University)
* [Christopher De Sa](http://www.cs.cornell.edu/~cdesa/) (Cornell University)
