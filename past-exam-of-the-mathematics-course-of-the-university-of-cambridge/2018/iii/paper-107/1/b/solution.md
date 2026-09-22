<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x,z\in B_\rho(y)$, the [open balls](../../../../../../open-ball.md) satisfy $B_\rho(x)\subset B_{3\rho}(z)\subset B_{4\rho}(y)$. Nonnegativity and the [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) give

$$
u(x)=\frac1{\omega_n\rho^n}\int_{B_\rho(x)}u
\leq\frac1{\omega_n\rho^n}\int_{B_{3\rho}(z)}u=3^nu(z).
$$

Taking the supremum over $x$ and the infimum over $z$ proves the [Harnack inequality for harmonic functions](../../../../../../harnack-inequality-for-harmonic-functions.md):

$$
\boxed{\sup_{B_\rho(y)}u\leq3^n\inf_{B_\rho(y)}u.}
$$

This includes a zero infimum, which forces $u=0$ on the smaller ball.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
