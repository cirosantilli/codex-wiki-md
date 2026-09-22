# Sudakov-Fernique inequality

↑ **Parent:** [Gaussian process](gaussian-process.md)

For centered [multivariate normal distributions](multivariate-normal-distribution.md), if $\mathbb E(U_i-U_j)^2\leq\mathbb E(V_i-V_j)^2$ for every pair, then the displayed comparison holds. For a quick proof, make $U,V$ [independent](independent-random-variables.md) and set $Z_r=\sqrt{1-r}U+\sqrt rV$. Apply [Gaussian integration by parts](stein-s-lemma-probability.md) to $F_\tau(z)=\tau^{-1}\log\sum_i e^{\tau z_i}$. With [softmax function](softmax-function.md) weights $p_i$ and $D=\operatorname{Cov}(V)-\operatorname{Cov}(U)$, the derivative of $\mathbb EF_\tau(Z_r)$ is $\tfrac\tau4\mathbb E\sum_{i,j}p_ip_j(D_{ii}+D_{jj}-2D_{ij})\geq0$. Since $\max z_i\leq F_\tau(z)\leq\max z_i+\tau^{-1}\log n$, let $\tau\to\infty$. Singular [covariance matrices](covariance-matrix.md) follow by adding identical small [independent](independent-random-variables.md) [normal](normal-distribution.md) noise to both vectors and taking a limit.

## ↑ Ancestors (7)

1. [Gaussian process](gaussian-process.md)
2. [Stochastic process](stochastic-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/4/solution.md)
- [Slepian's lemma](slepian-s-lemma.md)
