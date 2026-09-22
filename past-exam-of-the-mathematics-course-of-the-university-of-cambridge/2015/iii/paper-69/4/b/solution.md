<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $p\in\mathcal P_n$ and $e=f-p$, with $d=\|e\|_\infty>0$. **The [Chebyshev alternation theorem](../../../../../../equioscillation-theorem.md) is**

$$
\boxed{p\text{ is best}\iff\exists x_0<\cdots<x_{n+1},\quad e(x_i)=\varepsilon(-1)^id,\quad\varepsilon\in\{1,-1\}.}
$$

If such points exist and a [polynomial](../../../../../../polynomial-split.md) $v\in\mathcal P_n$ had $e(x)v(x)>0$ at every extremum, its signs at those $n+2$ points would alternate. The [intermediate value theorem](../../../../../../intermediate-value-theorem.md) would give at least $n+1$ distinct zeros, impossible for a nonzero degree-at-most-$n$ [polynomial](../../../../../../polynomial-split.md). The [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md) therefore proves sufficiency.

For necessity, let $E_+=\{e=d\}$ and $E_-=\{e=-d\}$. They are disjoint compact sets. If one set is empty there is just one sign block. Otherwise their positive separation implies that, reading the extremal set from left to right, its signs form finitely many alternating blocks. If there are fewer than $n+2$ alternating extrema, there are at most $n+1$ blocks. Place one point $\xi_j$ in each extremum-free gap between consecutive blocks. A scalar multiple of $v(x)=\prod_j(x-\xi_j)$ can be chosen to have exactly the sign of $e$ on every block. Its degree is at most $n$, and $ev>0$ throughout $E$, contradicting the [Kolmogorov criterion for uniform approximation](../../../../../../kolmogorov-criterion-for-uniform-approximation.md). Thus there must be at least $n+2$ alternating extrema. If $d=0$, the exact [polynomial](../../../../../../polynomial-split.md) is already best and the equalities with zero error are automatic.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
