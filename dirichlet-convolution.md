# Dirichlet convolution

↑ **Parent:** [Arithmetic function](arithmetic-function.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_convolution)

The [Dirichlet convolution](dirichlet-convolution.md) of [arithmetic functions](arithmetic-function.md) $f,g$ is the [arithmetic function](arithmetic-function.md)

$$
(f*g)(n)=\sum_{d\mid n}f(d)g(n/d)=\sum_{\substack{a,b>0\\ab=n}}f(a)g(b),\qquad n>0.
$$

In the first sum, $d$ runs over the positive [integer divisors](divisor.md) of $n$; the second uses [ordered pairs](ordered-pair.md) of [positive integers](positive-integer.md) whose product is $n$. Both sums are finite. Each pair contributes one weight from $f$ and one from $g$, so [Dirichlet convolution](dirichlet-convolution.md) combines information attached to complementary factors. It turns a [divisor sum](divisor-sum.md) into an operation on [arithmetic functions](arithmetic-function.md). [Darij Grinberg, MIT 18.781 lecture notes, Sections 2.3 and 2.4: Dirichlet convolution and examples](https://darijgrinberg.gitlab.io/floor.pdf)

For $n=12$ the six [ordered pairs](ordered-pair.md) are $(1,12),(2,6),(3,4),(4,3),(6,2),(12,1)$. The [constant-one arithmetic function](constant-one-arithmetic-function.md) gives one per pair, while the [identity arithmetic function](identity-arithmetic-function.md) weights the first factor by its size:

$$
\begin{aligned}
\tau&=\mathbf1*\mathbf1,&\tau(12)&=1+1+1+1+1+1=6,\\
\sigma_1&=\operatorname{id}*\mathbf1,&\sigma_1(12)&=1+2+3+4+6+12=28.
\end{aligned}
$$

Here $\tau$ is the [divisor function](divisor-function.md) and $\sigma_1$ is the [sum-of-divisors function](sum-of-divisors-function.md). By comparison, the [pointwise product of arithmetic functions](pointwise-product-of-arithmetic-functions.md) gives $(\mathbf1\cdot\mathbf1)(12)=1$ and $(\operatorname{id}\cdot\mathbf1)(12)=12$.

<a id="image-six-ordered-pairs-of-positive-integers-with-product-12-contribute-to-dirichlet-convolution-one-per-pair-for-the-divisor-function-or-the-first-factor-for-the-sum-of-divisors-function"></a>
![](dirichlet-convolution-factor-pairs.png)

**[Figure 15](#image-six-ordered-pairs-of-positive-integers-with-product-12-contribute-to-dirichlet-convolution-one-per-pair-for-the-divisor-function-or-the-first-factor-for-the-sum-of-divisors-function). Six ordered pairs of positive integers with product 12 contribute to Dirichlet convolution: one per pair for the divisor function, or the first factor for the sum-of-divisors function**.

[Commutativity](commutativity.md) follows by swapping the two entries of every [ordered pair](ordered-pair.md). [Associativity](associative-property.md) follows by reindexing either grouping over the same ordered [tuples](finite-tuple.md) of three [positive integers](positive-integer.md):

$$
((f*g)*h)(n)=\sum_{\substack{a,b,c>0\\abc=n}}f(a)g(b)h(c)=(f*(g*h))(n).
$$

For example, $((\mathbf1*\mathbf1)*\mathbf1)(12)$ counts ordered [tuples](finite-tuple.md) of three [positive integers](positive-integer.md) with product $12$. Distribute the two occurrences of the [prime factor](prime-factor.md) $2$ among three entries in $\binom{2+2}{2}=6$ ways, and the one occurrence of the [prime factor](prime-factor.md) $3$ in $\binom{1+2}{2}=3$ ways. These [binomial coefficients](binomial-coefficient.md) are the [stars and bars](stars-and-bars-combinatorics.md) counts of exponent choices in the [nonnegative integers](natural-number.md); [prime factorization](fundamental-theorem-of-arithmetic.md) therefore gives $6\cdot3=18$ such [tuples](finite-tuple.md). Directly, the same [Dirichlet convolution](dirichlet-convolution.md) is $\sum_{d\mid12}\tau(d)=1+2+2+3+4+6=18$.

The [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md) is $\varepsilon$, and the [Möbius function](mobius-function.md) reverses a [divisor sum](divisor-sum.md) because $\mu*\mathbf1=\varepsilon$. This makes [Dirichlet convolution](dirichlet-convolution.md) useful both for counting factorizations and for recovering an [arithmetic function](arithmetic-function.md) from its [divisor sum](divisor-sum.md).

**Table of contents**

- [Multiplicativity of Dirichlet convolution](multiplicativity-of-dirichlet-convolution.md)
- [Constant-one arithmetic function](constant-one-arithmetic-function.md)
- [Identity arithmetic function](identity-arithmetic-function.md)
- [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md)
- [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
  - [Divisor summatory function](divisor-summatory-function.md)
  - [Asymmetric Dirichlet hyperbola split](asymmetric-dirichlet-hyperbola-split.md)
  - [Arithmetic work of the Dirichlet hyperbola method](arithmetic-work-of-the-dirichlet-hyperbola-method.md)
  - [Divisor summatory asymptotic](divisor-summatory-asymptotic.md)
  - [Harmonic divisor sum](harmonic-divisor-sum.md)

## ↑ Ancestors (5)

1. [Arithmetic function](arithmetic-function.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (36)

- [Arithmetic function](arithmetic-function.md)
- [Arithmetic work of the Dirichlet hyperbola method](arithmetic-work-of-the-dirichlet-hyperbola-method.md)
- [Asymmetric Dirichlet hyperbola split](asymmetric-dirichlet-hyperbola-split.md)
- [Constant-one arithmetic function](constant-one-arithmetic-function.md)
- [Dirichlet convolution](dirichlet-convolution.md)
- [Dirichlet hyperbola method](dirichlet-hyperbola-method.md)
- [Dirichlet series](dirichlet-series.md)
- [Divisor function](divisor-function.md)
- [Divisor sum](divisor-sum.md)
- [Identity arithmetic function](identity-arithmetic-function.md)
- [Identity for Dirichlet convolution](identity-for-dirichlet-convolution.md)
- [Log-weighted convolution bound for three to the prime omega](log-weighted-convolution-bound-for-three-to-the-prime-omega.md)
- [Mertens bound from a log-integrable Chebyshev error](mertens-bound-from-a-log-integrable-chebyshev-error.md)
- [Möbius divisor-sum identity](mobius-divisor-sum-identity.md)
- [Möbius function](mobius-function.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Multiplicativity of Dirichlet convolution](multiplicativity-of-dirichlet-convolution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-28/7/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-29/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/11h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-150/1/a/solution.md)
- [Pointwise product of arithmetic functions](pointwise-product-of-arithmetic-functions.md)
- [Prime number asymptotic from Mertens cancellation](prime-number-asymptotic-from-mertens-cancellation.md)
- [Selberg sieve denominator asymptotic](selberg-sieve-denominator-asymptotic.md)
- [Sum-of-divisors function](sum-of-divisors-function.md)
- [Totient divisor-sum identity](totient-divisor-sum-identity.md)
- [Vaughan identity proof](vaughan-identity-proof.md)
- [Von Mangoldt divisor identity](von-mangoldt-divisor-identity.md)
