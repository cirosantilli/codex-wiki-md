<h1 id="3/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Only the $2d$ edges incident to $x_0$ depend on $\Gamma(x_0)$. Conditional on the remaining field, write

$$
m=\frac1{2d}\sum_{y\sim x_0}\Gamma(y).
$$

Completing the square gives

$$
\sum_{y\sim x_0}(\Gamma(x_0)-\Gamma(y))^2
=2d(\Gamma(x_0)-m)^2+\text{constant}.
$$

The conditional density is therefore proportional to $e^{-(u-m)^2}$, and hence

$$
\Gamma(x_0)\mid(\Gamma(x):x\ne x_0)
\sim N\left(\frac1{2d}\sum_{y\sim x_0}\Gamma(y),\frac12\right).
$$

This is the [Gibbs-Markov property of the discrete Gaussian free field](../../../../../../gibbs-markov-property-of-the-discrete-gaussian-free-field.md) in the normalization used by the paper.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [3](../../3.md)
3. [Paper 209](../../../paper-209-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
