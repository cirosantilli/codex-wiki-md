<h1 id="31j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

With the other coordinates fixed, the smooth part of the objective has derivative at $\beta_1=0$

$$
\frac1n\left(\kappa_1-(\kappa_2-\kappa_1)\right)
=\frac{2\kappa_1-\kappa_2}{n}.
$$

The subdifferential of the $\ell^1$ penalty at zero is $\gamma[-1,1]$. Therefore

$$
\partial_{\beta_1}f(0,\beta_2,\ldots,\beta_p)
=\frac{2\kappa_1-\kappa_2}{n}+\gamma[-1,1].
$$

The stated condition $|2\kappa_1-\kappa_2|\leq\gamma$ is stronger than the needed condition $|2\kappa_1-\kappa_2|\leq n\gamma$, and hence places zero in this subdifferential. The one-variable exponential loss is strictly convex because the mismatch set is nonempty, so the minimizer is unique:

$$
\boxed{\operatorname{argmin}_{\beta_1\in\mathbb R}f(\beta_1,\beta_2,\ldots,\beta_p)=\{0\}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
