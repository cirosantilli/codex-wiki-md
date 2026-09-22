<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $D_k=\sum_{i:z_i=k}d_i$ and $T_k=\sum_{i:z_i=k}x_i$. Since the cumulative hazard is $\theta e^{z_i\beta}x_i$,

$$
\ell(\theta,\beta)
=(D_0+D_1)\log\theta+D_1\beta
-\theta(T_0+e^\beta T_1).
$$

The score equations imply $D_1=\theta e^\beta T_1$ and $D_0=\theta T_0$. Therefore

$$
\widehat\theta=\frac{D_0}{T_0},
\qquad
\widehat\beta=log\frac{D_1/T_1}{D_0/T_0},
$$

when both event counts are positive, with the usual infinite boundary estimates otherwise.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
