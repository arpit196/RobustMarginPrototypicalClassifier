A Robust deep neural network classifier based on the concept of class prototypes that is robust to different categories of input noises, including random noise, as well as the adversarial noises and attacks.
Our classifier minimizes the class variance by clustering the data points closer to the class mean and maintains a large margin between the points to the classifier's decision boundary.
The enhanced robustness compared to other models is demonstrated in the tables below

| Attack | Softmax CNN | Robust Margin Prototype CNN |
|--------|-------------|-----------------------------|
|        |ϵ=0.08 0.1 0.15 0.25|ϵ=0.08 0.1 0.15 0.25|
|FGSM    |84.05 73.6 31.9 9.82 91.31| 91.31 85.57 69.72 41.29 |
