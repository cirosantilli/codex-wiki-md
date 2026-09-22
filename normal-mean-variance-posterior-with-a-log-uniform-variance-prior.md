# Normal mean-variance posterior with a log-uniform variance prior

↑ **Parent:** [Bayesian normal model](bayesian-normal-model.md)

For iid $N(\mu,v)$ observations, the prior density $1/v$ relative to $d\mu\,dv$ gives posterior kernel $v^{-n/2-1}\exp[-\{S+n(\mu-\bar x)^2\}/(2v)]$. It is proper exactly when $n>1$ and $S=\sum(x_i-\bar x)^2>0$. The conditionals are $\mu\mid v,x\sim N(\bar x,v/n)$ and $v\mid\mu,x\sim\operatorname{IG}(n/2,\sum_i(x_i-\mu)^2/2)$. Integrating out $\mu$ changes the inverse-gamma shape to $(n-1)/2$.

## ↑ Ancestors (5)

1. [Bayesian normal model](bayesian-normal-model.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/4/d/solution.md)
