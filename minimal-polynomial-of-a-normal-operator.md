# Minimal polynomial of a normal operator

↑ **Parent:** [Minimal polynomial](minimal-polynomial.md)

On a real or complex [inner product space](inner-product-space.md) of finite [dimension](dimension-vector-space.md), a [normal operator](normal-operator.md) has a [square-free polynomial](square-free-polynomial.md) as its [minimal polynomial](minimal-polynomial.md). To prove this without the [spectral theorem](spectral-theorem.md), suppose an [irreducible polynomial](irreducible-polynomial.md) $f$ occurs at least twice in $m_T$. Put $h=m_T/f^2$ and $N=f(T)$. Since [polynomials of a normal operator are normal](polynomials-of-a-normal-operator-are-normal.md), $N$ is a [normal operator](normal-operator.md). For every $v$,

$$
N^2h(T)v=m_T(T)v=0.
$$

By [kernel stabilization for a normal operator](kernel-stabilization-for-a-normal-operator.md), $Nh(T)v=0$. Hence the smaller-degree [monic polynomial](monic-polynomial.md) $m_T/f$ annihilates $T$, contradicting minimality.

Over the [complex numbers](complex-number.md), all [irreducible polynomials](irreducible-polynomial.md) are linear, so the [primary decomposition theorem for linear maps](primary-decomposition-theorem-for-linear-maps.md) now gives a [basis](basis.md) of [eigenvectors](eigenvector.md). Over the [real numbers](real-number.md), irreducible quadratics can remain: a nontrivial planar [rotation](rotation-mathematics.md) need not have any real [eigenvectors](eigenvector.md), although its [minimal polynomial](minimal-polynomial.md) is square-free.

## ↑ Ancestors (7)

1. [Minimal polynomial](minimal-polynomial.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-linear-algebra-course-of-the-university-of-oxford/2023/3/b/iv/solution.md)
