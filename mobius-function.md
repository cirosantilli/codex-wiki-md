<h1 id="mobius-function">Möbius function</h1>

↑ **Parent:** [Arithmetic function](arithmetic-function-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Möbius_function)

The [Möbius function](mobius-function.md) assigns a cancellation weight to each [positive integer](positive-integer.md):

$$
\mu(n)=\begin{cases}
1&n=1,\\
(-1)^r&n=p_1\cdots p_r\text{ with distinct primes }p_1,\ldots,p_r,\\
0&p^2\mid n\text{ for some prime }p.
\end{cases}
$$

Thus a [squarefree integer](square-free-integer.md) contributes a sign determined by its number of distinct [prime factors](prime-factor.md); a repeated [prime factor](prime-factor.md) makes the weight zero. This packages the alternating signs of [inclusion-exclusion](inclusion-exclusion-principle.md) into an [arithmetic function](arithmetic-function-split.md). [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.1.2](https://darijgrinberg.gitlab.io/floor.pdf)

For example, $\mu(2)=\mu(3)=-1$, $\mu(6)=1$, and $\mu(30)=(-1)^3=-1$, since $30=2\cdot3\cdot5$. In contrast, $\mu(4)=\mu(12)=\mu(60)=0$: all three have the square of the [prime number](prime-number-split.md) $2$ as a [divisor](divisor.md). On [prime powers](prime-power.md), $\mu(p)=-1$ and $\mu(p^a)=0$ for $a\geq2$.

The [Möbius function](mobius-function.md) is a [multiplicative function](multiplicative-function.md): for [coprime integers](coprime-integers.md), their [prime factors](prime-factor.md) are disjoint, so either a squared [prime factor](prime-factor.md) forces both sides of $\mu(mn)=\mu(m)\mu(n)$ to vanish, or the counts of distinct [prime factors](prime-factor.md) add and their signs multiply. It is not a [completely multiplicative function](completely-multiplicative-function.md), since $\mu(4)=0\ne1=\mu(2)^2$. Its [Möbius divisor-sum identity](mobius-divisor-sum-identity.md) makes it the inverse of the [constant-one arithmetic function](constant-one-arithmetic-function.md) under [Dirichlet convolution](dirichlet-convolution.md): $\mu*\mathbf1=\varepsilon$, the [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md). This is why the small set of weights $-1,0,1$ can undo an entire [divisor sum](divisor-sum.md).

**Table of contents**

- [Möbius divisor-sum identity](mobius-divisor-sum-identity.md)
- [Möbius harmonic logarithmic moments](mobius-harmonic-logarithmic-moments.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Mertens function](mertens-function.md)
  - [Prime number asymptotic from Mertens cancellation](prime-number-asymptotic-from-mertens-cancellation.md)
  - [Mertens bound from a log-integrable Chebyshev error](mertens-bound-from-a-log-integrable-chebyshev-error.md)
  - [Mertens function bound from the classical zeta zero-free region](mertens-function-bound-from-the-classical-zeta-zero-free-region.md)

## ↑ Ancestors (5)

1. [Arithmetic function](arithmetic-function-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Dirichlet convolution](dirichlet-convolution.md)
- [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md)
- [Mertens function](mertens-function.md)
- [Möbius divisor-sum identity](mobius-divisor-sum-identity.md)
- [Möbius function](mobius-function.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Number-theoretic sieve](number-theoretic-sieve.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-16/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-25/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/11h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-150/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-150/1/a/solution.md)
- [Pretentious distance between one and the Möbius function](pretentious-distance-between-one-and-the-mobius-function.md)
- [Ramanujan sum](ramanujan-sum.md)
- [Square-free integer](square-free-integer.md)
- [Squarefree counting function](squarefree-counting-function.md)
- [Type I sum](type-i-sum.md)
