# Multiplicativity of Dirichlet convolution

↑ **Parent:** [Dirichlet convolution](dirichlet-convolution.md)

The [Dirichlet convolution](dirichlet-convolution.md) of two [multiplicative functions](multiplicative-function.md) is a [multiplicative function](multiplicative-function.md). For positive [coprime integers](coprime-integers.md) $m,n$, every positive [integer divisor](divisor.md) of $mn$ has a unique form $de$ with $d\mid m$ and $e\mid n$, by [prime factorization](fundamental-theorem-of-arithmetic.md). The pairs $d,e$ and $m/d,n/e$ are each [coprime integers](coprime-integers.md), so the defining rules for the two [multiplicative functions](multiplicative-function.md) separate the sum:

$$
(f*g)(mn)=\sum_{d\mid m}\sum_{e\mid n}f(d)f(e)g(m/d)g(n/e)=(f*g)(m)(f*g)(n).
$$

Also $(f*g)(1)=f(1)g(1)=1$. This short argument proves [multiplicativity](multiplicativity-of-an-arithmetic-function.md) of both the [divisor function](divisor-function.md) $\mathbf1*\mathbf1$ and the [sum-of-divisors function](sum-of-divisors-function.md) $\operatorname{id}*\mathbf1$. The result need not be a [completely multiplicative function](completely-multiplicative-function.md), even when both inputs are: $\mathbf1*\mathbf1=\tau$ fails at $2\cdot2$. [Darij Grinberg, MIT 18.781 lecture notes, Theorem 2.6.1](https://darijgrinberg.gitlab.io/floor.pdf)

## ↑ Ancestors (6)

1. [Dirichlet convolution](dirichlet-convolution.md)
2. [Arithmetic function](arithmetic-function.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Divisor sum](divisor-sum.md)
