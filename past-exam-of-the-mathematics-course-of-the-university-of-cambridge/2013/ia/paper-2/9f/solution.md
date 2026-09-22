<h1 id="9f/solution">Solution</h1>

↑ **Parent:** [9F](../9f.md)

The [exponential distribution](../../../../../exponential-distribution.md) has survival [probability](../../../../../probability.md) $e^{-u}$ for $u\geq0$. [Conditional probability](../../../../../conditional-probability.md) therefore gives

$$
\mathbb P(Z>s+t\mid Z>s)=\frac{e^{-(s+t)}}{e^{-s}}=e^{-t},
$$

which proves the [memoryless property](../../../../../memorylessness-of-the-exponential-distribution.md). Let $K=\lfloor Z\rfloor$ and $U=Z-K$. With $q=e^{-1}$,

$$
\boxed{\mathbb P(K=m)=(1-q)q^m,\quad m=0,1,2,\ldots}.
$$

The [geometric distribution](../../../../../geometric-distribution.md) here starts at zero. Summing its first moment gives

$$
\boxed{\mathbb E[K]=\frac q{1-q}=\frac1{e-1}}.
$$

For $0\leq u<1$, sum the density over all integer translates:

$$
\boxed{f_U(u)=\sum_{m=0}^\infty e^{-m-u}=\frac{e^{-u}}{1-e^{-1}}},
$$

with zero density outside that interval. The [integer and fractional parts of an exponential variable](../../../../../integer-and-fractional-parts-of-an-exponential-variable.md) are independent, because for every integer $m\geq0$ and measurable $A\subseteq[0,1)$,

$$
\mathbb P(K=m,U\in A)=\int_Ae^{-m-u}\,du
=\mathbb P(K=m)\int_A f_U(u)\,du.
$$

This factorization proves [independence](../../../../../independent-random-variables.md) of the discrete and continuous components, beyond just checking their separate marginals.

## ↑ Ancestors (10)

1. [9F](../9f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
