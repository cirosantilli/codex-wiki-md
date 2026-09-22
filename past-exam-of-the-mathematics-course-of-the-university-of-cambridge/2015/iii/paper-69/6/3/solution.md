<h1 id="6/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix $i$. If $t<t_i$, all knot values of the function $x\mapsto(x-t)_+^{k-1}$ agree with a [polynomial](../../../../../../polynomial-split.md) of degree $k-1$. Its order-$k$ [divided difference](../../../../../../divided-difference.md) vanishes. If $t>t_{i+k}$, all the knot values are zero, so the same [divided difference](../../../../../../divided-difference.md) again vanishes. Thus **the support is finite**:

$$
\boxed{\operatorname{supp}M_i\subseteq[t_i,t_{i+k}],\qquad\operatorname{supp}N_i\subseteq[t_i,t_{i+k}].}
$$

The [support and Gram bandwidth of B-splines](../../../../../../support-and-gram-bandwidth-of-b-splines.md) also holds at repeated knots: the same conclusion follows with the standard limiting convention. If $j\geq i+k$, then $t_j\geq t_{i+k}$, so the two supports have no positive-length overlap. An endpoint intersection contributes zero to the integral defining $G_{ij}$. The case $i\geq j+k$ is identical. Hence

$$
\boxed{G_{ij}=0\quad\text{when }|i-j|\geq k,\qquad d=k.}
$$

For strictly increasing knots, [B-splines](../../../../../../b-spline.md) whose indices differ by $k-1$ overlap on a positive-length interval and their product is positive there, so this universal bound is sharp. In standard matrix terminology the half-bandwidth is $k-1$ and the full bandwidth is $2k-1$; the paper's integer $d$ is $k$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [6](../../6.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
