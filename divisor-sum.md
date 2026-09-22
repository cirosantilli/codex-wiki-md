# Divisor sum

↑ **Parent:** [Multiplicative function](multiplicative-function.md)

The [divisor sum](divisor-sum.md) of an [arithmetic function](arithmetic-function-split.md) $f$ assigns to each [positive integer](positive-integer.md) $n$ the [sum](sum.md)

$$
F(n)=\sum_{d\mid n}f(d).
$$

Only positive [integer divisors](divisor.md) are included, so $F(1)=f(1)$. The weights $f(d)$ can count the [integer divisors](divisor.md), measure their sizes, or record other arithmetic information: the [constant-one arithmetic function](constant-one-arithmetic-function.md) gives the [divisor function](divisor-function.md), whereas the [identity arithmetic function](identity-arithmetic-function.md) gives the [sum-of-divisors function](sum-of-divisors-function.md).

Equivalently, $F=f*\mathbf1$, where $*$ is [Dirichlet convolution](dirichlet-convolution.md) and $\mathbf1$ is the [constant-one arithmetic function](constant-one-arithmetic-function.md). If $f$ is a [multiplicative function](multiplicative-function.md), then $F$ is a [multiplicative function](multiplicative-function.md) by [Multiplicativity of Dirichlet convolution](multiplicativity-of-dirichlet-convolution.md). [Darij Grinberg, MIT 18.781 notes on floor and arithmetic functions, Proposition 2.4.2 and Theorem 2.6.1](https://darijgrinberg.gitlab.io/floor.pdf)

Here is the mechanism. For positive [coprime integers](coprime-integers.md) $m,n$, every positive [integer divisor](divisor.md) of $mn$ has a unique form $ab$ with $a\mid m$ and $b\mid n$; moreover, $a,b$ are [coprime integers](coprime-integers.md). Thus a [multiplicative function](multiplicative-function.md) satisfies

$$
F(mn)=\sum_{a\mid m}\sum_{b\mid n}f(a)f(b)=F(m)F(n).
$$

At a [prime power](prime-power.md), the [divisor sum](divisor-sum.md) becomes $F(p^a)=f(1)+f(p)+\cdots+f(p^a)$. This turns a calculation over many [integer divisors](divisor.md) into short local calculations at [prime powers](prime-power.md).

**Table of contents**

- [Sum-of-divisors function](sum-of-divisors-function.md)
  - [Proper-divisor sum](proper-divisor-sum.md)

## ↑ Ancestors (6)

1. [Multiplicative function](multiplicative-function.md)
2. [Arithmetic function](arithmetic-function-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Constant-one arithmetic function](constant-one-arithmetic-function.md)
- [Dirichlet convolution](dirichlet-convolution.md)
- [Divisor sum](divisor-sum.md)
- [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md)
- [Möbius divisor-sum identity](mobius-divisor-sum-identity.md)
- [Möbius function](mobius-function.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-23/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-126/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/1i/solution.md)
- [Selberg symmetry formula](selberg-symmetry-formula.md)
- [Sum-of-divisors function](sum-of-divisors-function.md)
- [Totient divisor-sum identity](totient-divisor-sum-identity.md)
- [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md)
- [Von Mangoldt function](von-mangoldt-function.md)
