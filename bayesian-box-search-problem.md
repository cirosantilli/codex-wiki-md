# Bayesian box search problem

↑ **Parent:** [Dynamic programming](dynamic-programming.md)

A hidden object lies in box $i$ with posterior probability $p_i$. Searching box $i$ costs $c_i$ and, conditional on the object being there, detects it with probability $\alpha_i$. After an unsuccessful search of box $i$, [Bayes' theorem](bayes-theorem.md) updates the probabilities to

$$
p_i^{(i)}=\frac{(1-\alpha_i)p_i}{1-\alpha_ip_i},
\qquad
p_j^{(i)}=\frac{p_j}{1-\alpha_ip_i}\quad(j\ne i).
$$

**Table of contents**

- [Optimal index for Bayesian box search](optimal-index-for-bayesian-box-search.md)
- [Rewarded Bayesian box search Bellman equation](rewarded-bayesian-box-search-bellman-equation.md)

## ↑ Ancestors (5)

1. [Dynamic programming](dynamic-programming.md)
2. [Mathematical optimization](mathematical-optimization-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/30k/a/solution.md)
