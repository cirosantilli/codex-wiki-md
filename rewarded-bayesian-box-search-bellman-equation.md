# Rewarded Bayesian box search Bellman equation

↑ **Parent:** [Bayesian box search problem](bayesian-box-search-problem.md)

If discovery in box $i$ earns reward $R_i$ and stopping earns zero, the [Bellman equation](bellman-equation.md) is

$$
V(p)=\max\left\{0,
\max_i\left[-c_i+\alpha_ip_iR_i
+(1-\alpha_ip_i)V(p^{(i)})\right]\right\}.
$$

If $\sum_i c_i/(\alpha_iR_i)<1$, every posterior state has some $i$ with $\alpha_ip_iR_i>c_i$, so stopping is never optimal.

## ↑ Ancestors (6)

1. [Bayesian box search problem](bayesian-box-search-problem.md)
2. [Dynamic programming](dynamic-programming.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/30k/b/solution.md)
