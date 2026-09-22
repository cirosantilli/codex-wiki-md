# Boundary limits of telescoping series

↑ **Parent:** [Telescoping sum](telescoping-sum.md)

For a real [sequence](sequence.md) $(a_n)$, the [partial sum](partial-sum.md) of $\sum_{k=1}^{\infty}(a_k-a_{k-1})$ is exactly $a_n-a_0$. Consequently it is a [convergent series](convergent-series.md) if and only if $a_n$ has a finite [limit](limit-of-a-function.md) $L$, and its [sum](sum.md) is $L-a_0$. Cancellation takes place inside each finite [partial sum](partial-sum.md); taking a [limit](limit-of-a-function.md) is a separate step.[Calculus Volume 2, §5.2 Telescoping Series: general boundary sequence, finite partial sums and finite-limit convergence criterion](calculus-volume-2-by-gilbert-strang-and-others/5-2-infinite-series.md)

The [partial fraction telescoping](partial-fraction-telescoping.md) example has $S_N=N/(3N+1)$ and therefore [limit](limit-of-a-function.md) $1/3$. In contrast, let $a_n=(-1)^n$. Its first entry is $a_0=1$, so $S_N=(-1)^N-1$. The [even](even-function.md) [partial sums](partial-sum.md) are zero and the [odd](odd-function.md) [partial sums](partial-sum.md) are negative two. Both finite cancellations are correct, but the [sequence](sequence.md) has no single [limit](limit-of-a-function.md), giving a [divergent series](divergent-series.md).

<a id="image-exact-cancellation-can-leave-a-convergent-or-an-oscillating-boundary-term"></a>
![](telescoping-series-boundary-convergence.png)

**[Figure 6](#image-exact-cancellation-can-leave-a-convergent-or-an-oscillating-boundary-term). Exact cancellation can leave a convergent or an oscillating boundary term**. Original calculated [partial sums](partial-sum.md). Top: $S_N=N/(3N+1)$ approaches $1/3$, with known [series remainder](series-remainder.md) $1/[3(3N+1)]$. Bottom: $S_N=(-1)^N-1$ alternates between zero and negative two. The dots are finite [partial sums](partial-sum.md), not observed data.

It is also essential to keep the two contributions paired. For example, $\sum_{k=1}^{\infty}(1/k-1/(k+1))$ is a [convergent series](convergent-series.md) with [sum](sum.md) one, as its finite [partial sum](partial-sum.md) is $1-1/(N+1)$. Writing it instead as $\sum_{k=1}^{\infty}1/k-\sum_{k=1}^{\infty}1/(k+1)$ asks to subtract two [divergent series](divergent-series.md). The permitted finite cancellation does not define that separate subtraction. Working through [partial sums](partial-sum.md) keeps the indices aligned and the operation meaningful.

## ↑ Ancestors (7)

1. [Telescoping sum](telescoping-sum.md)
2. [Summation](summation.md)
3. [Addition](addition.md)
4. [Arithmetic](arithmetic-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
