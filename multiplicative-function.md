# Multiplicative function

↑ **Parent:** [Arithmetic function](arithmetic-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplicative_function)

An [arithmetic function](arithmetic-function.md) $f$ is a [multiplicative function](multiplicative-function.md) when $f(1)=1$ and $f(mn)=f(m)f(n)$ for all [coprime integers](coprime-integers.md) $m,n>0$, meaning their [greatest common divisor](greatest-common-divisor.md) is $1$. The condition $f(1)=1$ excludes the identically zero [function](function-split.md). This definition makes no assertion about a pair whose [greatest common divisor](greatest-common-divisor.md) exceeds $1$. [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.2.1](https://darijgrinberg.gitlab.io/floor.pdf)

For the [divisor function](divisor-function.md), the [integer divisors](divisor.md) of $2$ are $1,2$, those of $3$ are $1,3$, and those of $6$ are $1,2,3,6$. Hence

$$
\tau(6)=4=\tau(2)\tau(3)=2\cdot2.
$$

Here $2$ and $3$ are [coprime integers](coprime-integers.md). In contrast, $\tau(4)=3\ne4=\tau(2)^2$, because the [integer divisors](divisor.md) of $4$ are $1,2,4$. Thus the [divisor function](divisor-function.md) is a [multiplicative function](multiplicative-function.md) but not a [completely multiplicative function](completely-multiplicative-function.md).

The practical gain is that [prime factorization](fundamental-theorem-of-arithmetic.md) reduces all values to values at [prime powers](prime-power.md). For distinct [prime numbers](prime-number.md) $p_1,\ldots,p_r$ and positive exponents $a_1,\ldots,a_r$,

$$
n=\prod_{k=1}^r p_k^{a_k}\quad\Longrightarrow\quad f(n)=\prod_{k=1}^r f(p_k^{a_k}).
$$

For instance, $f(12)=f(4)f(3)$ since $4$ and $3$ are [coprime integers](coprime-integers.md); replacing $f(4)$ by $f(2)^2$ additionally requires a [completely multiplicative function](completely-multiplicative-function.md). The short proof repeatedly applies the defining rule to [prime powers](prime-power.md) belonging to different [prime numbers](prime-number.md), which are [coprime integers](coprime-integers.md).

**Table of contents**

- [Multiplicativity of an arithmetic function](multiplicativity-of-an-arithmetic-function.md)
- [Completely multiplicative function](completely-multiplicative-function.md)
- [Divisor sum](divisor-sum.md)
  - [Sum-of-divisors function](sum-of-divisors-function.md)
    - [Proper-divisor sum](proper-divisor-sum.md)
- [Pretentious distance](pretentious-distance.md)
  - [Large Fourier coefficient criterion for pretentiousness](large-fourier-coefficient-criterion-for-pretentiousness.md)
  - [Pretentious distance between one and the Möbius function](pretentious-distance-between-one-and-the-mobius-function.md)
  - [Prime-restriction metric for pretentious distance](prime-restriction-metric-for-pretentious-distance.md)
  - [Triangle inequality for pretentious distance](triangle-inequality-for-pretentious-distance.md)
  - [Archimedean character](archimedean-character.md)
  - [Halász theorem](halasz-theorem.md)
  - [Strong aperiodicity of the Möbius function](strong-aperiodicity-of-the-mobius-function.md)

## ↑ Ancestors (5)

1. [Arithmetic function](arithmetic-function.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Divisor function](divisor-function.md)
- [Divisor sum](divisor-sum.md)
- [Möbius function](mobius-function.md)
- [Multiplicative function](multiplicative-function.md)
- [Multiplicativity of an arithmetic function](multiplicativity-of-an-arithmetic-function.md)
- [Multiplicativity of Dirichlet convolution](multiplicativity-of-dirichlet-convolution.md)
- [Radical of an integer](radical-of-an-integer.md)
- [Sum-of-divisors function](sum-of-divisors-function.md)
