<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Weierstrass M-test](../../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../../uniform-convergence.md) and [continuity](../../../../../../continuous-function.md) of the series. For the proposed [trigonometric polynomial](../../../../../../trigonometric-polynomial.md), set $q=5^{m+1}$ and $A=\sum_{k=m+1}^\infty a_k$. The tail satisfies

$$
r(x):=f(x)-t_n(x)=\sum_{k=m+1}^\infty a_k\cos(5^kx),\qquad \|r\|_\infty\le A.
$$

At $x_j=j\pi/q$, for $j=0,\ldots,2q-1$, the [integer](../../../../../../integer.md) $5^k/q$ is odd for every omitted frequency. Thus $\cos(5^kx_j)=(-1)^j$ and $r(x_j)=(-1)^jA$. In particular $\|r\|_\infty=A$.

Since $n<q$, these $2q$ points include at least $2n+2$ consecutive alternating extrema in a single period. Also $5^m\le n$, so $t_n\in\mathcal T_n$. The [trigonometric Chebyshev alternation theorem](../../../../../../trigonometric-chebyshev-alternation-theorem.md) proves that **the proposed partial sum is the unique best approximant**, with

$$
\boxed{E_n(f)=\sum_{k=m+1}^\infty a_k\qquad(5^m\le n<5^{m+1}).}
$$

This is an instance of [positive lacunary trigonometric series](../../../../../../positive-lacunary-trigonometric-series.md): all omitted odd frequency ratios align their extrema.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
