# Euclid-Euler theorem

↑ **Parent:** [Perfect number](perfect-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid–Euler_theorem)

An [even integer](even-number.md) $n>0$ is a [perfect number](perfect-number.md) **if and only if**

$$
\boxed{n=2^{p-1}(2^p-1)\quad\text{with }2^p-1\text{ prime}.}
$$

This forces $p$ to be a [prime number](prime-number-split.md), as shown under [Mersenne number](mersenne-number.md). It does not say that every [prime](prime-number-split.md) exponent works, nor classify possible [odd integers](odd-integer.md).[Theorem 1.1, pp. 1–2: even-number equivalence and proof](perfect-numbers-and-mersenne-primes-by-keith-conrad.md)

For the forward direction, put $q=2^p-1$ and use [coprimality](coprime-integers.md) of $q$ and $2^{p-1}$. [Multiplicativity](multiplicativity-of-an-arithmetic-function.md) of the [sum-of-divisors function](sum-of-divisors-function.md) and the [finite geometric series](finite-geometric-series.md) give

$$
\sigma(2^{p-1}q)=\sigma(2^{p-1})\sigma(q)=(2^p-1)(q+1)=q2^p=2n.
$$

The [prime number](prime-number-split.md) hypothesis makes $\sigma(q)=q+1$; replacing it with a [composite number](composite-number.md) changes this factor.

For a short converse outline, write $n=2^a m$ with $a\geq1$ and $m$ an [odd integer](odd-integer.md). The condition $\sigma(n)=2n$ gives

$$
\sigma(m)=m+t,\qquad t=\frac{m}{2^{a+1}-1}.
$$

Here $t$ is a positive [integer](integer-split.md) and a [proper divisor](proper-divisor.md) of $m$. If $t>1$, the distinct [divisors](divisor.md) $1,t,m$ alone exceed the required [sum](sum.md) $m+t$. Thus $t=1$ and $\sigma(m)=m+1$, forcing $m$ to be [prime](prime-number-split.md) and $m=2^{a+1}-1$.

**Table of contents**

- [Testing the prime condition in the Euclid construction](testing-the-prime-condition-in-the-euclid-construction.md)

## ↑ Ancestors (7)

1. [Perfect number](perfect-number.md)
2. [Positive integer](positive-integer.md)
3. [Integer](integer-split.md)
4. [Number theory](number-theory-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Mersenne prime](mersenne-prime.md)
- [Perfect number](perfect-number.md)
