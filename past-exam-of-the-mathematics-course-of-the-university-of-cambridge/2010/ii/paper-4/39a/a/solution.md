<h1 id="39a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For an explicit [Runge-Kutta method](../../../../../../runge-kutta-method.md), write its strictly lower-triangular stage matrix as $A$, weight vector as $b$, and $\mathbf1=(1,\ldots,1)^T$. Applied to the scalar test equation, its stage vector satisfies

$$
k=\lambda y_n\mathbf1+\lambda hAk.
$$

Since $A^s=0$, inversion is a finite [Neumann series](../../../../../../neumann-series.md). Putting $z=\lambda h$ gives

$$
\boxed{y_{n+1}=P_s(z)y_n,\qquad
P_s(z)=1+z\,b^T\sum_{j=0}^{s-1}z^jA^j\mathbf1.}
$$

This proves degree at most $s$. The printed statement of degree exactly $s$ needs a nondegeneracy assumption: a two-stage explicit scheme with $b=(1,0)$ is simply Euler's method with an unused second stage, and has [polynomial](../../../../../../polynomial-split.md) $1+z$ of degree one.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
