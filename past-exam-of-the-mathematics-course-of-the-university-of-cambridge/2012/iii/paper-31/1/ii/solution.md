<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\widetilde P_j(x)=x^{j-1}+\sum_{r=0}^{j-2}b_{rj}x^r$. The evaluation [matrix](../../../../../../matrix.md) $[\widetilde P_j(x_i)]$ is $V_m B$, where $B$ is upper triangular with diagonal entries $1$. Its [determinant](../../../../../../determinant.md) is therefore unchanged. This is [Vandermonde determinant invariance under monic basis change](../../../../../../vandermonde-determinant-invariance-under-monic-basis-change.md):

$$
\det[\widetilde P_j(x_i)]_{i,j=1}^m=\prod_{k<l}(x_l-x_k).
$$

For $w(x)=x^a e^{-x}$ on $[0,\infty)$, multiply row $i$ by $\sqrt{w(x_i)}$. The requested weighted product becomes the [weighted Vandermonde determinant](../../../../../../weighted-vandermonde-determinant.md) square

$$
\boxed{\prod_{j<k}(x_j-x_k)^2\prod_{i=1}^m w(x_i)=\left(\det[\sqrt{w(x_i)}\,\widetilde P_j(x_i)]_{i,j=1}^m\right)^2.}
$$

The sign difference between the two orientations of the Vandermonde product disappears on squaring. For $a=0$ interpret the weight at zero by continuity, so $w(0)=1$; for $a>0$, $w(0)=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
