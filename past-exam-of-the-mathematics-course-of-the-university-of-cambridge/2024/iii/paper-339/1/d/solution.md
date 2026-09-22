<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $a_i^T$ for row $i$ of $A$, and define affine functions

$$
\ell_0(x)=c^Tx,
\qquad
\ell_i(x)=(c+Ma_i)^Tx-Mb_i
\quad(1\leq i\leq m).
$$

Then

$$
f(x)=\max_{0\leq i\leq m}\ell_i(x).
$$

The [pointwise maximum of convex functions](../../../../../../pointwise-maximum-of-convex-functions.md) is convex, so $f$ is a [convex function](../../../../../../convex-function.md). Moreover,

$$
|f(x)-f(y)|
\leq L\lVert x-y\rVert_2,
\qquad
L=\max\left\{\lVert c\rVert_2,
\max_i\lVert c+Ma_i\rVert_2\right\},
$$

so $f$ has [Lipschitz continuity](../../../../../../lipschitz-continuity.md). The simpler bound $L\leq\lVert c\rVert_2+M\max_i\lVert a_i\rVert_2$ is also valid.

Let $I(x)=\{i:\ell_i(x)=f(x)\}$ be the active set. The [subdifferential](../../../../../../subdifferential.md) is

$$
\partial f(x)=
\operatorname{conv}\left(
\{c:0\in I(x)\}\cup
\{c+Ma_i:i\in I(x),\ i\geq1\}
\right),
$$

the [convex hull](../../../../../../convex-hull.md) of all active slopes. In particular, choosing any active index gives the [subgradient](../../../../../../subgradient.md)

$$
g(x)=
\begin{cases}
c,&0\in I(x),\\
c+Ma_j,&j\in I(x),\ j\geq1.
\end{cases}
$$

At a tie, every convex combination of the tied slopes is also valid.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
