<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) states that $p\in\mathcal P_n$ is a [best uniform approximation](../../../../../../best-uniform-approximation.md) to real $f$ precisely when there are $n+2$ increasingly ordered points $x_0<\cdots<x_{n+1}$ with

$$
f(x_i)-p(x_i)=\eta(-1)^iE,\qquad \eta\in\{-1,1\},\quad E=\|f-p\|_\infty.
$$

For sufficiency, an improving [polynomial](../../../../../../polynomial-split.md) direction $h$ would have to share these alternating signs, by the [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md). The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) would give at least $n+1$ distinct [roots of a polynomial](../../../../../../root-of-a-polynomial.md) between consecutive points. A nonzero [polynomial](../../../../../../polynomial-split.md) of degree at most $n$ cannot do that. If $E=0$, no improvement is possible anyway.

For necessity, suppose $E>0$ and the active set $M$ has no alternating sequence of length $n+2$. Its positive-error and negative-error subsets are disjoint [compact sets](../../../../../../compact-space.md), hence separated by a positive distance. Reading them from left to right splits $M$ into finitely many consecutive sign blocks. If there are $L$ blocks, choosing one point per block gives an alternating sequence, so $L\le n+1$. Choose $z_j$ in the gap between each consecutive pair of blocks. The [polynomial](../../../../../../polynomial-split.md) $h(x)=C\prod_{j=1}^{L-1}(x-z_j)$ has degree at most $n$; choose the sign of $C$ to match the error on the first block. Its sign then matches the error on every block, and it is nonzero throughout $M$. Thus $rh>0$ on $M$, contradicting the [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md). There must therefore be $n+2$ alternating extrema.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
