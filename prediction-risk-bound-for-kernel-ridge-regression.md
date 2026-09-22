# Prediction-risk bound for kernel ridge regression

↑ **Parent:** [Kernel ridge regression](kernel-ridge-regression.md)

For the unscaled objective $\sum_i(Y_i-f(x_i))^2+\lambda\|f\|_{\mathcal H}^2$, the [kernel-ridge hat matrix](kernel-ridge-hat-matrix.md) is $H=K(K+\lambda I)^{-1}$. Its prediction variance is $\sigma^2\operatorname{tr}(H^2)/n$. For eigenvalues $d_i\geq0$, use $d_i^2/(d_i+\lambda)^2\leq\min\{d_i/(4\lambda),1\}$ and $\lambda^2d_i/(d_i+\lambda)^2\leq\lambda/4$ to bound the variance and the squared bias. The latter also uses the [reproducing property](reproducing-property.md) and [Bessel inequality](bessel-s-inequality.md), and does not require invertibility of $K$.

> EXISTING BODY EXPANSION, not a new concept: replace the present one-direction definition of Faithfulness of a directed acyclic graph in probability-and-statistics.bigb, under Causal directed acyclic graph, with the following body. Retain its existing header and parent.

## ↑ Ancestors (8)

1. [Kernel ridge regression](kernel-ridge-regression.md)
2. [Kernel method](kernel-method.md)
3. [Reproducing kernel Hilbert space](reproducing-kernel-hilbert-space.md)
4. [Positive-semidefinite kernel](positive-semidefinite-kernel.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/6/solution.md)
