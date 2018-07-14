---
title: "Differentially Private Model Fitting Using Genetic Algorithms"
date: 2018-06-29T20:48:04+08:00
draft: true
---
## ABSTRACT
- Propose PrivGene, a general-purpose differentially private model fitting solution based on genetic algorithms(GA).
- PrivGene performs the random perturbations using a novel technique called the **enhanced exponential mechanism**.
- Apply PrivGene to three common analysis tasks involving model fitting: logistic regression, SVM classification, and kmeans clustering.

## BACKGROUND
Given the set of all possible output values, the user assigns each possible output value ω ∈ Ω a **quality score** Q(ω); higher scores correspond to better values. 

- 行内插图，![]()
![GitHub](https://avatars2.githubusercontent.com/u/3265208?v=3&s=100 "GitHub,Social Coding")
[![https://gyazo.com/467a551f09dfb6dc66efa150b1a1c516](https://i.gyazo.com/467a551f09dfb6dc66efa150b1a1c516.png)](https://gyazo.com/467a551f09dfb6dc66efa150b1a1c516)
## PRIVGENE
- Let D ∈ T n be a sensitive database containing n tuples sampled
from domain T , and f(D, ω) be the fitting function that measures
how well a parameter vector ω fits the data D. 
- Goal is to find
the best parameter vector ω∗ that maximizes f(D, ω∗).
[![https://gyazo.com/ba5797124a51b309470ad52bde96ffdc](https://i.gyazo.com/ba5797124a51b309470ad52bde96ffdc.png)](https://gyazo.com/ba5797124a51b309470ad52bde96ffdc)
- 算法1过程：初始化Ω，由Ω通过调用DP_Select得到Ω·，Ω·通过遗传算法交叉，变异再得到新的Ω，如此循环往复，直到达到指定循环次数。
[![https://gyazo.com/5af486381169f16d539b756c9d4c8eb9](https://i.gyazo.com/5af486381169f16d539b756c9d4c8eb9.png)](https://gyazo.com/5af486381169f16d539b756c9d4c8eb9)