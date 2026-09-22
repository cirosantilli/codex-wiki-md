<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the inverse [tensor](../../../../../tensor.md) as

$$
Y_{ij}=\delta_{ij}+\lambda A_{ij}+\lambda^2C_{ij}+\lambda^3D_{ij}+O(\lambda^4).
$$

Insert this into $(\delta_{ik}+\lambda X_{ik})Y_{kj}=\delta_{ij}$ and equate powers of $\lambda$. One obtains successively

$$
A_{ij}=-X_{ij},\qquad C_{ij}=-X_{ik}A_{kj}=X_{ik}X_{kj},\qquad
D_{ij}=-X_{ik}C_{kj}=-X_{ik}X_{kl}X_{lj}.
$$

Thus the [Neumann series](../../../../../neumann-series.md) gives

$$
\boxed{Y_{ij}=\delta_{ij}-\lambda X_{ij}+\lambda^2X_{ik}X_{kj}-\lambda^3X_{ik}X_{kl}X_{lj}+O(\lambda^4).}
$$

Every contraction is an ordinary ordered [matrix product](../../../../../matrix-product.md). No transpose or symmetry assumption is used. Multiplying the truncated series on either side by $I+\lambda X$ leaves $I-\lambda^4X^4$, which verifies the error order. For a fixed finite matrix this expansion converges whenever $|\lambda|\,\|X\|<1$ in a submultiplicative [matrix norm](../../../../../matrix-norm.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
