<h1 id="13k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Weighted least squares uses the known conditional variances and should be at least as efficient, so $\rho\leq1$. Indeed, apply Cauchy--Schwarz to

$$
\frac{|X_1|}{\sqrt{v(X_1)}}\quad\text{and}\quad |X_1|\sqrt{v(X_1)}.
$$

It gives

$$
\bigl(\mathbb E[X_1^2]\bigr)^2
\leq\mathbb E[X_1^2/v(X_1)]\,\mathbb E[v(X_1)X_1^2],
$$

which is exactly $\rho\leq1$. Equality holds precisely when $v(X_1)$ is constant on the part of the support where $X_1\ne0$, up to null sets.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [13K](../../13k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
