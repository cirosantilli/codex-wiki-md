<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose first that the bounded [Fredholm operator](../../../../../../fredholm-operator.md) $T:H\to H$ has [Fredholm index](../../../../../../fredholm-index.md) zero. Put $N=\ker T$ and $C=(\operatorname{ran}T)^\perp=\ker T^*$. These finite-dimensional [linear subspaces](../../../../../../vector-subspace.md) have the same [dimension](../../../../../../dimension-vector-space.md). The restricted map $T:N^\perp\to\operatorname{ran}T$ is a bounded bijection, with bounded inverse by the [bounded inverse theorem](../../../../../../bounded-inverse-theorem.md). Choose an isomorphism $J:N\to C$ and extend it by zero on $N^\perp$, writing the resulting [finite-rank operator](../../../../../../finite-rank-operator.md) as $K$.

Relative to the [orthogonal decompositions](../../../../../../orthogonal-decomposition-by-a-closed-subspace.md) $H=N\oplus N^\perp$ and $H=C\oplus\operatorname{ran}T$, the operator $T+K$ is the direct sum of $J$ and the invertible restricted map. Thus $T+K$ is invertible, and $T=(T+K)-K$ is the sum of an invertible operator and a [compact operator](../../../../../../compact-operator-split.md).

Conversely write $T=U+K$ with $U$ invertible and $K$ compact. It suffices to treat $I+C$ with $C=U^{-1}K$. A [compact operator](../../../../../../compact-operator-split.md) on a [Hilbert space](../../../../../../hilbert-space-split.md) admits arbitrary [operator norm](../../../../../../operator-norm.md) approximation by [finite-rank operators](../../../../../../finite-rank-operator.md): take a finite epsilon-net of its unit-ball image and project onto the span of the net. Choose $F$ of finite rank with $\|C-F\|<1$, put $R=C-F$, and factor

$$
I+C=(I+R)\bigl(I+(I+R)^{-1}F\bigr).
$$

The first factor is invertible by the [Neumann series](../../../../../../neumann-series.md). Set $G=(I+R)^{-1}F$ and $E=\operatorname{ran}G$, a finite-dimensional [linear subspace](../../../../../../vector-subspace.md). On $E\oplus E^\perp$, the second factor has block form

$$
I+G=\begin{pmatrix}A&B\\0&I\end{pmatrix},\qquad A=I_E+G|_E.
$$

Left multiplication by the invertible block matrix $\begin{pmatrix}I&-B\\0&I\end{pmatrix}$ reduces it to $A\oplus I$. Its range is closed, and its [kernel](../../../../../../kernel-of-a-linear-map.md) and [cokernel](../../../../../../cokernel.md) have equal [dimension](../../../../../../dimension-vector-space.md) by finite-dimensional [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) for $A:E\to E$. Invertible factors preserve all these properties. Hence $T$ is a [Fredholm operator](../../../../../../fredholm-operator.md) of [Fredholm index](../../../../../../fredholm-index.md) zero, proving both directions:

$$
\boxed{T\text{ Fredholm with index }0\iff T=U+K,\quad U\text{ invertible},\ K\text{ compact}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
