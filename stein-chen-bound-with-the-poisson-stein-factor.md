# Stein-Chen bound with the Poisson Stein factor

↑ **Parent:** [Stein-Chen method](stein-chen-method.md)

Let $W=\sum_i I_i$ and $\lambda=\sum_i p_i>0$, where each [indicator random variable](indicator-random-variable.md) $I_i$ is independent of all indicators outside $\{i\}\cup J_i$ jointly. Write $V_i=\sum_{j\in J_i}I_j$ and $W_i=W-I_i-V_i$. For a test-event solution of the [Poisson Stein equation](poisson-stein-equation.md), independence gives

$$
\lambda\mathbb Eg(W+1)-\mathbb EWg(W)
=\sum_i p_i\mathbb E[g(W+1)-g(W_i+1)]
+\sum_i\mathbb EI_i[g(W_i+1)-g(W)].
$$

Telescoping each difference and using $\|\Delta g\|_\infty\leq\min(1,\lambda^{-1})$ bounds the [total variation distance](total-variation-distance.md) by that factor times $\sum_i p_i^2+\sum_i\sum_{j\in J_i}(p_ip_j+\mathbb EI_iI_j)$. Directed dependence neighborhoods are allowed. If $\lambda=0$, the count is identically zero.

## ↑ Ancestors (9)

1. [Stein-Chen method](stein-chen-method.md)
2. [Poisson distribution](poisson-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-11/1/solution.md)
