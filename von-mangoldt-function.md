# Von Mangoldt function

↑ **Parent:** [Arithmetic function](arithmetic-function-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Mangoldt_function)

The [Von Mangoldt function](von-mangoldt-function.md) assigns a [natural logarithm](natural-logarithm.md) weight to each positive power of a [prime number](prime-number-split.md). For a [positive integer](positive-integer.md) $n$,

$$
\Lambda(n)=\begin{cases}
\log p,&n=p^k,\quad p\text{ prime},\ k\geq1,\\
0,&\text{otherwise}.
\end{cases}
$$

Here and throughout the [Chebyshev functions](chebyshev-function.md), **$\log$ means the [natural logarithm](natural-logarithm.md)**. In particular, $\Lambda(1)=0$: the exponent must be positive, even though the convention in [prime power](prime-power.md) allows exponent zero. The [support of a function](support.md) of $\Lambda$ therefore consists precisely of the [prime powers](prime-power.md) greater than one. [254A, Notes 1: Elementary multiplicative number theory](254a-analytic-prime-number-theory/254a-notes-1-elementary-multiplicative-number-theory.md)

For example, $\Lambda(2)=\Lambda(4)=\Lambda(8)=\log2$ and $\Lambda(3)=\Lambda(9)=\log3$, whereas $\Lambda(6)=\Lambda(12)=0$. A [composite number](composite-number.md) can have a nonzero weight: $8$ has just one distinct [prime factor](prime-factor.md). But $12=2^2\cdot3$ has two distinct [prime factors](prime-factor.md), so its weight is zero. At $p^k$ the weight is **$\log p$, not $\log(p^k)=k\log p$**. This choice lets successive powers record successive copies of the same [prime factor](prime-factor.md) in the [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md).

The [Von Mangoldt function](von-mangoldt-function.md) is useful because it connects two views of the [prime numbers](prime-number-split.md): the [prime factorization](fundamental-theorem-of-arithmetic.md) of an individual [integer](integer-split.md), through a [divisor sum](divisor-sum.md), and the accumulated weights below a cutoff, through the [Second Chebyshev function](second-chebyshev-function.md). The latter turns questions about the distribution of [prime numbers](prime-number-split.md) into questions about a [partial sum](partial-sum.md) of an [arithmetic function](arithmetic-function-split.md).

**Table of contents**

- [Selberg symmetry formula](selberg-symmetry-formula.md)
- [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md)
- [Chebyshev function](chebyshev-function.md)
  - [Second Chebyshev function](second-chebyshev-function.md)
    - [First integral of the Chebyshev function](first-integral-of-the-chebyshev-function.md)
      - [Smoothed explicit formula for the Chebyshev function](smoothed-explicit-formula-for-the-chebyshev-function.md)
    - [Integrated Chebyshev sum](integrated-chebyshev-sum.md)
    - [Chebyshev estimate](chebyshev-estimate.md)
      - [Chebyshev estimate from central binomial coefficients](chebyshev-estimate-from-central-binomial-coefficients.md)
    - [Riemann–von Mangoldt explicit formula](riemann-von-mangoldt-explicit-formula.md)
      - [Truncated explicit formula for the second Chebyshev function](truncated-explicit-formula-for-the-second-chebyshev-function.md)
- [Vaughan's identity](vaughan-s-identity.md)
  - [Prime exponential-sum estimate from Vaughan identity](prime-exponential-sum-estimate-from-vaughan-identity.md)
  - [Logarithmic coefficient bound in Vaughan identity](logarithmic-coefficient-bound-in-vaughan-identity.md)
  - [Vaughan identity for the Möbius function](vaughan-identity-for-the-mobius-function.md)
    - [Type I–type II inverse principle for Möbius correlation](type-i-type-ii-inverse-principle-for-mobius-correlation.md)
  - [Vaughan identity proof](vaughan-identity-proof.md)

## ↑ Ancestors (5)

1. [Arithmetic function](arithmetic-function-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (22)

- [Chebyshev function in an arithmetic progression](chebyshev-function-in-an-arithmetic-progression.md)
- [Log-weighted convolution bound for three to the prime omega](log-weighted-convolution-bound-for-three-to-the-prime-omega.md)
- [Logarithmic coefficient bound in Vaughan identity](logarithmic-coefficient-bound-in-vaughan-identity.md)
- [Major-arc value of the prime exponential sum](major-arc-value-of-the-prime-exponential-sum.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-76/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-25/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-22/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/7/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-25/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-150/3/c/solution.md)
- [Second Chebyshev function](second-chebyshev-function.md)
- [Short-interval Perron bound for the second Chebyshev function](short-interval-perron-bound-for-the-second-chebyshev-function.md)
- [Type II sum](type-ii-sum.md)
- [Vinogradov Type I–II method](vinogradov-type-i-ii-method.md)
- [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md)
- [Von Mangoldt function](von-mangoldt-function.md)
