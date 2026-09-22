# Integer power sum

↑ **Parent:** [Bernoulli polynomial](bernoulli-polynomial.md)

An integer power sum adds a fixed nonnegative [integer](integer.md) power of consecutive [integers](integer.md). Let $N$ be a [nonnegative integer](natural-number.md) and $p$ a [nonnegative integer](natural-number.md). For $p=0$, use the constant [polynomial](polynomial-split.md) $x^0=1$, including at zero, so $S_0(N)=N$. Summing the [Bernoulli polynomial](bernoulli-polynomial.md) [finite difference](finite-difference-split.md) identity makes the intermediate terms cancel and gives

$$
S_p(N)=\sum_{k=0}^{N-1}k^p
=\frac{B_{p+1}(N)-B_{p+1}(0)}{p+1}
=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_jN^{p+1-j}.
$$

The sum is empty when $N=0$. For the endpoints $1,\ldots,N$, the formula valid also at $p=0$ is instead

$$
\sum_{k=1}^{N}k^p=\frac{B_{p+1}(N+1)-B_{p+1}(1)}{p+1}.
$$

For $p\geq1$, $B_{p+1}(1)=B_{p+1}(0)$, and this becomes the standard positive-endpoint formula. The exception at $p=0$ is essential: $B_1(1)-B_1(0)=1$.[Karl Dilcher, Chapter 24, equations 24.4.1 and 24.4.7; the displayed equation 24.4.7 needs the endpoint adjustment at exponent zero](nist-digital-library-of-mathematical-functions.md)

For $p\geq1$, adding $N^p$ to $S_p(N)$ changes the $B_1$ contribution from $-N^p/2$ to $+N^p/2$. Equivalently,

$$
\sum_{k=1}^{N}k^p=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_j^{+}N^{p+1-j}\quad(p\geq1),
$$

where only $B_1^{+}$ differs from our [Bernoulli numbers](bernoulli-number.md). A quick endpoint check is $p=1$: the sums over $0,\ldots,N-1$ and $1,\ldots,N$ are $N(N-1)/2$ and $N(N+1)/2$, respectively. The latter is a [triangular number](triangular-number.md).

**Table of contents**

- [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)

## ↑ Ancestors (6)

1. [Bernoulli polynomial](bernoulli-polynomial.md)
2. [Bernoulli number](bernoulli-number.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)
- [Bernoulli number](bernoulli-number.md)
