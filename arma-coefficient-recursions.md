# ARMA coefficient recursions

↑ **Parent:** [Autoregressive moving-average model](autoregressive-moving-average-model.md)

For an [autoregressive moving-average model](autoregressive-moving-average-model.md), set $\Phi(z)=1-\sum_{k=1}^p\phi_kz^k$ and $\Theta(z)=1+\sum_{k=1}^q\theta_kz^k$. If both have no zeros on the closed unit disc, the causal and inverse filters have absolutely summable coefficients $C(z)=\Theta(z)/\Phi(z)=\sum_{j\geq0}c_jz^j$ and $D(z)=\Phi(z)/\Theta(z)=\sum_{j\geq0}d_jz^j$. Comparing [power series](power-series.md) coefficients gives $c_j=\theta_j+\sum_{k=1}^p\phi_kc_{j-k}$ and $d_j=a_j-\sum_{k=1}^q\theta_kd_{j-k}$, where $a_0=\theta_0=1$, $a_j=-\phi_j$ for $1\leq j\leq p$, and all out-of-range coefficients vanish. The [backshift operator](backshift-operator.md) then gives the corresponding time-series filters.

**Table of contents**

- [ARMA(1,1) causal and inverse coefficients](arma-1-1-causal-and-inverse-coefficients.md)

## ↑ Ancestors (6)

1. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/1/solution.md)
