<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a mesh of $[-1,1]$ and the conforming space of [Cubic Hermite finite elements](../../../../../../cubic-hermite-finite-element.md): piecewise cubic functions that are globally $C^1$ and satisfy $v(\pm1)=v'(\pm1)=0$. Let $\phi_1,\ldots,\phi_n$ be its nodal value-and-slope basis. For $u_n=\sum_ka_k\phi_k$, the [Ritz method](../../../../../../rayleigh-ritz-method.md) imposes

$$
a(u_n,\phi_j)=\int_{-1}^1f\phi_jdx
\qquad(1\leq j\leq n).
$$

Hence the coefficient vector solves

$$
Ka=F,
\qquad
K_{jk}=\int_{-1}^1
\left(p\phi_k''\phi_j''+q\phi_k'\phi_j'+r\phi_k\phi_j\right)dx,
\qquad
F_j=\int_{-1}^1f\phi_jdx.
$$

The stiffness matrix is symmetric positive definite by part a.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
