<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\{\phi_j\}_{j=1}^{N-1}$ be the [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) on a mesh, and put

$$
u_h=\sum_{j=1}^{N-1}U_j\phi_j.
$$

The [Ritz method](../../../../../../rayleigh-ritz-method.md) requires

$$
\sum_{j=1}^{N-1}K_{ij}U_j=F_i,
\qquad i=1,\ldots,N-1,
$$

where, for $f\equiv1$,

$$
\boxed{
K_{ij}=\int_0^1
\left[(1+x^2)\phi_j'\phi_i'
+x^2\phi_j\phi_i\right]dx,
\qquad
F_i=\int_0^1\phi_i\,dx.
}
$$

Local support makes $K$ symmetric tridiagonal, and coercivity makes it positive definite.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
