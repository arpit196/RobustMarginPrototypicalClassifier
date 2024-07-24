This repository contains tensorflow code for a novel Robust deep neural network classifier based on the concept of class prototypes and development of margin between the class. Its greater robustness to different categories of input noises, including random noise, and even the adversarial noises and attacks have been verified. Some results demonstrating this are shown in the Tables below. We show greater robustness than FGSM and PGD attacks.
Our classifier minimizes the class variance by clustering the data points closer to the class mean and maintains a large margin between the points to the classifier's decision boundary.
The enhanced robustness compared to other models is demonstrated in the tables below

| Attack | Softmax CNN | Robust Margin Prototype CNN |
|-------:|-------------|-----------------------------|
|Attack intensity ϵ=|0.08, 0.1, 0.15, 0.25|0.08, 0.1, 0.15, 0.25|
|FGSM    |84.05, 73.6, 31.9, 9.82| **91.31**, **85.57**, **69.72**, **41.29** |
|PGD    |66.47 39.17 16.14 0.8| **89.75**, **79.71**, **64.19**, **13.82** |
