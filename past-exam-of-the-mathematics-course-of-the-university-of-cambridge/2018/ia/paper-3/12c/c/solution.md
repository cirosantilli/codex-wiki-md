<h1 id="12c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The relation is

$$
A_{ij}=\alpha\delta_{ij}B_{kk}+\beta B_{ij}+\gamma B_{ji}.
$$

Taking its trace, symmetric traceless part, and antisymmetric part separately gives

$$
B_{kk}=\frac{A_{kk}}{3\alpha+\beta+\gamma},\qquad
B_{(ij)}-\frac13\delta_{ij}B_{kk}
=\frac{A_{(ij)}-\frac13\delta_{ij}A_{kk}}{\beta+\gamma},
\qquad
B_{[ij]}=\frac{A_{[ij]}}{\beta-\gamma}.
$$

Equivalently,

$$
\boxed{
B_{ij}=
\frac{A_{ij}+A_{ji}}{2(\beta+\gamma)}
+\frac{A_{ij}-A_{ji}}{2(\beta-\gamma)}
-\frac{\alpha\delta_{ij}A_{kk}}{(\beta+\gamma)(3\alpha+\beta+\gamma)}.}
$$

If $\beta=-\gamma\ne0$, $\alpha\ne0$, and $A_{ij}=0$, its symmetric part forces $B_{kk}=0$ and its antisymmetric part forces $B_{[ij]}=0$. Thus **the solutions are exactly the symmetric traceless tensors $B_{ij}$**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12C](../../12c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
