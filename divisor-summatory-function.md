# Divisor summatory function

↑ **Parent:** [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisor_summatory_function)

The [divisor summatory function](divisor-summatory-function.md) adds the [divisor function](divisor-function.md) up to a cutoff $x\ge1$. It counts all [ordered pairs](ordered-pair.md) of [positive integers](positive-integer.md) whose product is at most $x$. For $N=12$, the twelve individual [divisor function](divisor-function.md) values are

$$
(\tau(1),\ldots,\tau(12))=(1,2,2,3,2,4,2,4,3,4,2,6),
\qquad D(12)=35.
$$

Counting columns of [lattice points](lattice-point.md) instead gives $12+6+4+3+2+2+1+1+1+1+1+1=35$. The [Dirichlet hyperbola method](dirichlet-hyperbola-method.md) needs only the first three column counts:

$$
D(12)=2(12+6+4)-3^2=44-9=35.
$$

The [arithmetic work of the Dirichlet hyperbola method](arithmetic-work-of-the-dirichlet-hyperbola-method.md) is much smaller even though the answer is identical.

This is useful for elementary averages: individual [divisor function](divisor-function.md) values fluctuate, but their [summation](summation.md) has the regular behavior given by the [divisor summatory asymptotic](divisor-summatory-asymptotic.md). Dividing that estimate by a [positive integer](positive-integer.md) $N$ gives

$$
\frac1N\sum_{n=1}^N\tau(n)
=\log N+2\gamma-1+O(N^{-1/2})\qquad(N\longrightarrow\infty),
$$

where $\log$ is the [natural logarithm](natural-logarithm.md), $\gamma$ is the [Euler--Mascheroni constant](euler-s-constant.md), and $O$ uses [big O notation](big-o-notation.md). This describes an average, rather than an estimate for every individual [divisor function](divisor-function.md) value. [§1.1.4, p. 8, equation (1.1.13): the divisor summatory asymptotic](multiplicative-number-theory-the-pretentious-approach-by-andrew-granville-and-k-soundararajan.md)

## ↑ Ancestors (7)

1. [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
2. [Dirichlet convolution](dirichlet-convolution.md)
3. [Arithmetic function](arithmetic-function.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Arithmetic work of the Dirichlet hyperbola method](arithmetic-work-of-the-dirichlet-hyperbola-method.md)
- [Asymmetric Dirichlet hyperbola split](asymmetric-dirichlet-hyperbola-split.md)
- [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
- [Divisor summatory function](divisor-summatory-function.md)
