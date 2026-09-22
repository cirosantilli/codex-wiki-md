<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each $n$, choose the [best uniform approximation](../../../../../../best-uniform-approximation.md) $p_n^*$. If its error is nonzero, take its $n+2$ alternating extrema. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) supplies a point $y_j$ strictly between the $j$th and $(j+1)$st extrema such that $f(y_j)=p_n^*(y_j)$, for $0\le j\le n$. These $n+1$ points are distinct. The [polynomial interpolation](../../../../../../polynomial-interpolation.md) problem at them has a unique solution of degree at most $n$, so its solution is exactly $p_n^*$. This constructs the [interpolation nodes from best uniform approximation](../../../../../../interpolation-nodes-from-best-uniform-approximation.md).

If $E_n(f)=0$, then $f$ itself belongs to the [polynomial](../../../../../../polynomial-split.md) space, and any $n+1$ distinct nodes give the same conclusion. In either case, take $x_{n,j}=y_j$ or the arbitrary nodes just described. Then

$$
\|\ell_n(f)-f\|_\infty=E_n(f).
$$

The [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md) gives $E_n(f)\to0$; alternatively, the bound derived in part 4(b), combined with [uniform continuity](../../../../../../uniform-continuity.md), gives this convergence directly. Therefore

$$
\boxed{\|\ell_n(f)-f\|_\infty\longrightarrow0.}
$$

The nodes may depend on $f$ and on $n$. The conclusion does not assert a universal sequence of interpolation grids working for every continuous target.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
