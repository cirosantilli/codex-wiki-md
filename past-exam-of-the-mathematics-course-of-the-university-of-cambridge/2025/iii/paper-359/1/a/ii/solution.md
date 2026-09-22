<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpolation between $L^2$ and $L^6$, followed by the three-dimensional [Sobolev inequality](../../../../../../../sobolev-inequality.md), gives

$$
\|v\|_{L^3}
\leq\|v\|_{L^2}^{1/2}\|v\|_{L^6}^{1/2}
\leq c|v|^{1/2}\|v\|^{1/2}.
$$

Apply this with $v=P_Nw$ and use part i:

$$
\|P_Nw\|_{L^3}
\leq c|P_Nw|^{1/2}
\left(\lambda_N^{1/2}|P_Nw|\right)^{1/2}
=c\lambda_N^{1/4}|P_Nw|.
$$

Orthogonal projection is contractive in $H$, so

$$
\boxed{\|P_Nw\|_{L^3}
\leq c\lambda_N^{1/4}|w|}.
$$

The Sobolev constant is dimensionless after using the periodic-domain normalization, so the estimate is scale invariant.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
