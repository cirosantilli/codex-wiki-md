<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [coefficient](../../../../../../coefficient.md) sum is finite, so the [Weierstrass M-test](../../../../../../weierstrass-m-test.md) makes the cosine series uniformly convergent and $f$ continuous. Put $Q=5^{m+1}$ and $A_m=\sum_{k=m+1}^{\infty}a_k$. The indicated partial sum belongs to $\mathcal T_n$ because its largest frequency is $5^m\le n$. Its tail satisfies

$$
|f(x)-t_n(x)|\le A_m,
$$

and equality holds at $x=0$. Thus its [supremum norm](../../../../../../supremum-norm.md) error is exactly $A_m$.

At the $2Q$ points $x_j=j\pi/Q$, $0\le j<2Q$, every omitted frequency is an odd [integer](../../../../../../integer.md) multiple of $Q$. Indeed for $k\ge m+1$,

$$
\cos(5^kx_j)=\cos(5^{k-m-1}j\pi)=(-1)^j.
$$

[Uniform convergence](../../../../../../uniform-convergence.md) permits summing these values, giving

$$
f(x_j)-t_n(x_j)=(-1)^j A_m.
$$

These are cyclically alternating extrema. Since $n<Q$, there are $2Q\ge2n+2$ of them, so the [trigonometric Chebyshev alternation theorem](../../../../../../trigonometric-chebyshev-alternation-theorem.md) proves that the partial sum is the unique best approximant. Consequently the [positive lacunary trigonometric series](../../../../../../positive-lacunary-trigonometric-series.md) has

$$
\boxed{t_n(x)=\sum_{k=0}^ma_k\cos(5^kx),\qquad
E_n(f)=\sum_{k=m+1}^{\infty}a_k\quad(5^m\le n<5^{m+1}).}
$$

The positivity of every tail [coefficient](../../../../../../coefficient.md) makes the same tail attain its full [coefficient](../../../../../../coefficient.md) sum with alternating signs; a triangle bound alone would not establish optimality.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
