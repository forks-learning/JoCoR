# JoCoR 
CVPR'20: Combating Noisy Labels by Agreement: A Joint Training Method with Co-Regularization.
(Pytorch implementation)



========
# Abstract

Deep Learning with noisy labels is a practically challenging problem in weakly-supervised learning. The state-of-the-art approaches "Decoupling" and "Co-teaching+" claim that the "disagreement" strategy is crucial for alleviating the problem of learning with noisy labels. In this paper, we start from a different perspective and propose a robust learning paradigm called JoCoR, which aims to reduce the diversity of two networks during training. Specifically, we first use two networks to make predictions on the same mini-batch data and calculate a joint loss with Co-Regularization for each training example. Then we select small-loss examples to update the parameters of both two networks simultaneously. Trained by the joint loss, these two networks would be more and more similar due to the effect of Co-Regularization. Extensive experimental results on corrupted data from benchmark datasets including MNIST, CIFAR-10, CIFAR-100 and Clothing1M demonstrate that JoCoR is superior to many state-of-the-art approaches for learning with noisy labels.

========

## Running JoCoR on benchmark datasets (MNIST, CIFAR-10 and CIFAR-100)
Here is an example: 

```bash
python main.py --dataset cifar10 --noise_type symmetric --noise_rate 0.5 
```
