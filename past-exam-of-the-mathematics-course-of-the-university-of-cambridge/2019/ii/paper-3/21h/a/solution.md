<h1 id="21h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $B$ for the [open unit ball](../../../../../../open-unit-ball.md). Because $T$ is a [linear map](../../../../../../linear-map.md), the hypothesis scales to

$$
sB\subseteq\overline{T(sB)}
\qquad(s>0).
$$

Fix $y\in B$. Choose numbers $r$ and $\theta$ such that

$$
\lVert y\rVert<r<1,
\qquad 0<\theta<1-r;
$$

then $r/(1-\theta)<1$.

Set $z_0=y$. Inductively, if $\lVert z_{j-1}\rVert<r\theta^{j-1}$, the scaled density statement lets us choose

$$
x_j\in r\theta^{j-1}B
\quad\text{such that}\quad
\lVert z_{j-1}-Tx_j\rVert<r\theta^j,
$$

and we put $z_j=z_{j-1}-Tx_j$. The [geometric series](../../../../../../geometric-series.md) gives

$$
\sum_{j=1}^{\infty}\lVert x_j\rVert
<\sum_{j=1}^{\infty}r\theta^{j-1}
=\frac r{1-\theta}<1.
$$

Because $X$ is a [Banach space](../../../../../../banach-space-split.md), $x=\sum_{j\geq1}x_j$ exists and lies in $B$. Since $T$ is a [bounded linear operator](../../../../../../continuous-linear-operator.md), it is continuous, while

$$
y-T\sum_{j=1}^Nx_j=z_N\longrightarrow0.
$$

Therefore $Tx=y$. As $y\in B$ was arbitrary,

$$
\boxed{T(B)\supseteq B.}
$$

This is the [dense open-unit-ball image criterion](../../../../../../dense-open-unit-ball-image-criterion.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21H](../../21h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
