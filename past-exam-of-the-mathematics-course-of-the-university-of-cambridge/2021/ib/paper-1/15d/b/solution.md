<h1 id="15d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The magnetostatic [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) is $\nabla\times B=\mu_0J$. Substituting $B=\nabla\times A$ and using the [Coulomb gauge](../../../../../../coulomb-gauge.md) $\nabla\mathbin{\cdot}A=0$ gives

$$
\mu_0J=\nabla\times(\nabla\times A)
=\nabla(\nabla\mathbin{\cdot}A)-\nabla^2A
=-\nabla^2A.
$$

The free-space [Green function of the Laplacian](../../../../../../green-function-of-the-laplacian.md) therefore gives

$$
A(x)=\frac{\mu_0}{4\pi}
\int_{\mathbb R^3}\frac{J(x')}{|x-x'|}\,d^3x'.
$$

For the thin wire current stated in the question this becomes

$$
\boxed{
A(x)=\frac{\mu_0I}{4\pi}\oint_C\frac{dx'}{|x-x'|}}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [15D](../../15d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
