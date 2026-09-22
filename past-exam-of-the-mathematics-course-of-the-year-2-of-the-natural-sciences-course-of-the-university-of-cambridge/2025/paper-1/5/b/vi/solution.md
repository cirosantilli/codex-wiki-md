<h1 id="5/b/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Complete the square in the [Hermitian matrix](../../../../../../hermitian-operator.md) polynomial:

$$
H=\left(A+\frac\alpha2I\right)^2+\left(\beta-\frac{\alpha^2}4\right)I.
$$

For every nonzero [vector](../../../../../../vector.md) $v$,

$$
v^\dagger Hv=\left\|\left(A+\frac\alpha2I\right)v\right\|^2+\left(\beta-\frac{\alpha^2}4\right)\|v\|^2>0.
$$

Thus $H$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), so $\boxed{0\text{ is not an eigenvalue of }H}$. In [finite-dimensional spectral theorem](../../../../../../finite-dimensional-spectral-theorem.md) terms, each [eigenvalue](../../../../../../eigenvalue.md) is

$$
h_j=\lambda_j^2+\alpha\lambda_j+\beta=\left(\lambda_j+\frac\alpha2\right)^2+\beta-\frac{\alpha^2}4>0.
$$

If $\alpha^2\geq4\beta$, the scalar [polynomial](../../../../../../polynomial-split.md) has real [roots of a polynomial](../../../../../../root-of-a-polynomial.md)

$$
r_\pm=\frac{-\alpha\pm\sqrt{\alpha^2-4\beta}}2.
$$

An allowed nonzero root can be an [eigenvalue](../../../../../../eigenvalue.md) of $A$, a [Hermitian matrix](../../../../../../hermitian-operator.md) which is also an [invertible matrix](../../../../../../invertible-matrix.md), in which case $H$ has a zero [eigenvalue](../../../../../../eigenvalue.md). For example, $\alpha=2$, $\beta=1$, $A=-I$ gives $H=0$. The weaker inequality does not force failure for every $A$; it removes the general positive lower bound. There is also the harmless corner $\alpha=\beta=0$, for which $H=A^2$ stays positive definite because $A$ is invertible, even though the strict discriminant hypothesis is absent.

## ↑ Ancestors (14)

1. [Vi](../vi.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
