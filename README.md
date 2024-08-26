###Robust Large Margin Prototype Encoder (RMPE)

This repository contains tensorflow code for a novel deep neural network, the robust large margin prototype encoder (RMPE) classifier that uses class prototypes on a sparse subspace output by a CNN. The class prototypes reduces the within class variance while sparsity further promotes robustness of model. Its greater robustness to several categories of input noises, including random noise, adversarial noises and attacks, and occlusion have been verified. Some results demonstrating this are shown in the Tables below. We show greater robustness than softmax based CNN model on FGSM, PGD and L2-norm Carlini Wagner attacks.

![alt text](https://i.imgur.com/1Q2wPsh.png)

