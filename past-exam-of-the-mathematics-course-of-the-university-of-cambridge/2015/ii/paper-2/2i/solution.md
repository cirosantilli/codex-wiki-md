<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

To prove [convergence of positive quadrature on continuous functions](../../../../../convergence-of-positive-quadrature-on-continuous-functions.md), for a continuous $f$, the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) supplies a [polynomial](../../../../../polynomial-split.md) $p$ with $\|f-p\|_\infty<\varepsilon$. For every sufficiently large $n$, the [Gaussian quadrature](../../../../../gaussian-quadrature.md) rule is exact for this fixed [polynomial](../../../../../polynomial-split.md). Positivity of its weights and their sum $2$ then give

$$
\left|Q_n(f)-\int_{-1}^1f\right|\leq\sum_jA_j|f(x_j)-p(x_j)|+\int_{-1}^1|f-p|\leq4\varepsilon.
$$

Since $\varepsilon$ is arbitrary, **$Q_n(f)\to\int_{-1}^1f$**. Notice that no differentiability of $f$ is needed; uniform [polynomial](../../../../../polynomial-split.md) approximation and positivity provide the whole argument.

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
