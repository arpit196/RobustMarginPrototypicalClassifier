This repository contains tensorflow code for a novel deep neural network, the robust large margin prototype encoder (RMPE) classifier that uses class prototypes on a sparse subspace output by a CNN. The class prototypes reduces the within class variance while sparsity further promotes robustness of model. Its greater robustness to several categories of input noises, including random noise, adversarial noises and attacks, and occlusion have been verified. Some results demonstrating this are shown in the Tables below. We show greater robustness than FGSM, PGD and Carlini Wagner attacks.

![alt text](https://private-user-images.githubusercontent.com/30366755/359680349-0602ad78-d73c-474c-a79b-840eb3ac9f11.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MjQxOTcxNDAsIm5iZiI6MTcyNDE5Njg0MCwicGF0aCI6Ii8zMDM2Njc1NS8zNTk2ODAzNDktMDYwMmFkNzgtZDczYy00NzRjLWE3OWItODQwZWIzYWM5ZjExLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDA4MjAlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwODIwVDIzMzQwMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ1MTRlN2JmYmE5MTY0MzZiOTUzYjg2MWEyNmNhYjAwZmMzMzEzYzMxZWUxYzFiYjBkZWM4NmU4YzkxYzEyZGQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.OIY6Z2miAuOAMU3Ea53TBVLTzH9LHJmBrdwCDsnv5RY)

| Attack | Softmax CNN | Robust Margin Prototype CNN |
|-------:|-------------|-----------------------------|
|Attack intensity ϵ=|0.08, 0.1, 0.15, 0.25|0.08, 0.1, 0.15, 0.25|
|FGSM    |84.05, 73.6, 31.9, 9.82| **91.31**, **85.57**, **69.72**, **41.29** |
|PGD    |66.47 39.17 16.14 0.8| **89.75**, **79.71**, **64.19**, **13.82** |
