This repository contains tensorflow code for a novel deep neural network, the robust large margin prototype encoder (RMPE) classifier that uses class prototypes on a sparse subspace output by a CNN. The class prototypes reduces the within class variance while sparsity further promotes robustness of model. Its greater robustness to several categories of input noises, including random noise, adversarial noises and attacks, and occlusion have been verified. Some results demonstrating this are shown in the Tables below. We show greater robustness than FGSM, PGD and Carlini Wagner attacks.

| Attack | Softmax CNN | Robust Margin Prototype CNN |
|-------:|-------------|-----------------------------|
|Attack intensity ϵ=|0.08, 0.1, 0.15, 0.25|0.08, 0.1, 0.15, 0.25|
|FGSM    |84.05, 73.6, 31.9, 9.82| **91.31**, **85.57**, **69.72**, **41.29** |
|PGD    |66.47 39.17 16.14 0.8| **89.75**, **79.71**, **64.19**, **13.82** |
