<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $\theta_\gamma=(\gamma,0,\ldots,0)^T$, every moved observation has residual

$$
\gamma\tau-(\tau,0,\ldots,0)\theta_\gamma=0.
$$

Every original observation has

$$
|y_i-x_i^T\theta_\gamma|
=|y_i-\gamma x_{i1}|
\leq M_y+\gamma\max_i|x_{i1}|.
$$

Selecting any $h$ losses and adding $\lambda\|\theta_\gamma\|_1=\lambda\gamma$ gives

$$
\boxed{L_{Z_{\gamma,\tau}}(\theta_\gamma)
\leq h\rho\!\left(M_y+\gamma\max_i|x_{i1}|\right)+\lambda\gamma.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
