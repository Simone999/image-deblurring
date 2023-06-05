# Image deblurring

The project is part of an exam on Deep Learning.

## Problem
Given an image $x$ affected by Gaussian noise and Gaussian blur, we want to restore the original image $y$. I.e. given
$$ x = (H * y) + \eta$$
our goal is to obtain an estimation of the original image $\hat y$, where $H$ is the Gaussian blur filter, $\eta$ is the Gaussian noise, and $*$ denotes convolution.

## Dataset
The dataset has been generated from Cifar10 by applying to each image a 5x5 Gaussian filter with randomly generated standard deviation in the interval $[1,4)$, followed by an additive Gaussian noise centered on 0 with standard deviation of $0.02$.

## Evaluation metrics
- Mean Squared Error (MSE)

## Constraints
- No pretrained models can be used
- Maximum number of trainable parameters: 7.8M