<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [bipartite graph](../../../../../../bipartite-graph.md) property means that a walk starting in $V_0$ ends there precisely when its length is even. Thus the [even-length walk generating function on a bipartite graph](../../../../../../even-length-walk-generating-function-on-a-bipartite-graph.md) is $Z_G^0(x)=\sum_{k\geq0}\sigma_{2k}x^{2k}$. Deleting the last [edge](../../../../../../edge-of-a-graph.md) of an odd-length [self-avoiding walk](../../../../../../self-avoiding-walk.md) leaves an even-length one; each such prefix has at most $\Delta$ possible last-edge choices. Hence $\sigma_{2k+1}\leq\Delta\sigma_{2k}$, and for $x\geq0$,

$$
\boxed{Z_G^0(x)\leq Z_G(x)=Z_G^0(x)+\sum_{k\geq0}\sigma_{2k+1}x^{2k+1}\leq(1+\Delta x)Z_G^0(x)}.
$$

These inequalities also hold with infinite values. Their finite positive prefactor shows that the two [power series](../../../../../../power-series.md) have the same [radius of convergence](../../../../../../radius-of-convergence.md) $1/\mu$; alternatively apply the root formula to the even subsequence.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 26](../../../paper-26-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
