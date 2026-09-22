<h1 id="4e/solution">Solution</h1>

↑ **Parent:** [4E](../4e.md)

The key fact is that convergence of a [power series](../../../../../power-series.md) at one nonzero point forces [absolute convergence](../../../../../absolute-convergence.md) at every smaller modulus. Indeed, if $\sum a_nw^n$ converges and $w\ne0$, its terms form a [bounded sequence](../../../../../bounded-sequence.md), say $|a_nw^n|\le M$. For $|z|<|w|$,

$$
\sum_{n=0}^{\infty}|a_nz^n|\le M\sum_{n=0}^{\infty}\left|\frac zw\right|^n<\infty
$$

by convergence of a [geometric series](../../../../../geometric-series.md).

Let $S$ be the set of moduli of points at which the [power series](../../../../../power-series.md) converges, and put $R=\sup S$, allowing $R=\infty$. The set contains zero, so its [supremum](../../../../../supremum.md) is defined in $[0,\infty]$. Whenever $|z|<R$, the definition of [supremum](../../../../../supremum.md) provides a convergence point $w$ with $|w|>|z|$. The preceding estimate gives [absolute convergence](../../../../../absolute-convergence.md) at $z$. Whenever $|z|>R$, convergence at $z$ would put $|z|$ in $S$, contradicting its upper bound. This proves the asserted [radius of convergence](../../../../../radius-of-convergence.md) property, including $R=0$ and $R=\infty$. Nothing in the argument decides convergence on $|z|=R$.

For the requested boundary behavior, take the [power series](../../../../../power-series.md)

$$
\boxed{\sum_{k=1}^{\infty}\frac{z^{2k}}k.}
$$

Its coefficients are $a_{2k}=1/k$ for $k\ge1$, $a_{2k+1}=0$ and $a_0=0$. At either $z=1$ or $z=-1$ it is the divergent [harmonic series](../../../../../harmonic-series.md). At either $z=i$ or $z=-i$ it is $\sum_{k\ge1}(-1)^k/k$, which converges by the [alternating series test](../../../../../alternating-series-test.md). In fact its [radius of convergence](../../../../../radius-of-convergence.md) is one, since inside the unit circle the terms are bounded by a [geometric series](../../../../../geometric-series.md), and outside it they do not tend to zero.

## ↑ Ancestors (10)

1. [4E](../4e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
