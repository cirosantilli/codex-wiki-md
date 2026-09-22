<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

In an affine chart, the [Zariski tangent space](../../../../../zariski-tangent-space.md) at $P$ consists of vectors $v$ with $df_P(v)=0$ for every [polynomial](../../../../../polynomial-split.md) vanishing on the variety. Intrinsically it is the dual of $\mathfrak m_P/\mathfrak m_P^2$. For a finite set of generators in an ambient $N$-space, its dimension is $N-\operatorname{rank}J(P)$. The condition that this be at least $r$ is the vanishing of all $(N-r+1)$-minors, hence is closed. The affine-chart descriptions agree intrinsically; being closed is local on the variety, so the same conclusion holds projectively.

For the two given quadrics the gradient rows are

$$
J=\begin{pmatrix}0&X_2&X_1&X_4&X_3\\X_1&X_0&0&2X_3&2X_4\end{pmatrix}.
$$

Their intersection has dimension two: the quadrics have no common factor, so form a codimension-two complete intersection. Its singular points are where the two rows are dependent. If the first row vanishes, one obtains $[1:0:0:0:0]$. Otherwise write a dependence with nonzero coefficient of the second row. Its first coordinate forces $X_1=0$. The defining equations then imply $X_3X_4=0$ and $X_3^2+X_4^2=0$, hence $X_3=X_4=0$. Conversely every point of the resulting line lies on the variety and has dependent rows. Therefore

$$
\boxed{\operatorname{Sing}V=\{[X_0:0:X_2:0:0]\}\cong\mathbb P^1.}
$$

On this line at least one of $X_0,X_2$ is nonzero, so the Jacobian [rank](../../../../../rank-one-quadratic-form.md) is exactly one. The projective ambient tangent dimension is four, giving **$\dim T_{V,P}=3$ at every singular point**. Away from the line the [rank](../../../../../rank-one-quadratic-form.md) is two and the tangent dimension is two.

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
