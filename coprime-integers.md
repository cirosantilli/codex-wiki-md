# Coprime integers

↑ **Parent:** [Greatest common divisor](greatest-common-divisor.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coprime_integers)

Two [integers](integer-split.md) $a,b$ are **coprime** when their [greatest common divisor](greatest-common-divisor.md) is one:

$$
a,b\text{ are coprime}\quad\Longleftrightarrow\quad\gcd(a,b)=1.
$$

For [positive integers](positive-integer.md), this says that the only positive common [divisor](divisor.md) is one. For signed [integers](integer-split.md), use $\gcd(a,b)=\gcd(|a|,|b|)$, with [absolute values](absolute-value.md); changing either sign leaves [coprimality](coprime-integers.md) unchanged. With the convention $\gcd(0,0)=0$, zero is [coprime](coprime-integers.md) precisely to $1,-1$, because $\gcd(a,0)=|a|$. Both $1,-1$ are [coprime](coprime-integers.md) to every [integer](integer-split.md). [Darij Grinberg, MIT 18.781, Section 1.2: greatest common divisors and coprimality](https://darijgrinberg.gitlab.io/floor.pdf)

The word concerns shared [prime factors](prime-factor.md), not whether either input is a [prime number](prime-number-split.md). For instance $8=2^3$ and $9=3^2$ are [coprime](coprime-integers.md) [composite numbers](composite-number.md), even though neither is a [square-free integer](square-free-integer.md). Conversely, $6=2\cdot3$ and $10=2\cdot5$ are [square-free integers](square-free-integer.md) but are not [coprime](coprime-integers.md). Consecutive [integers](integer-split.md) are always [coprime](coprime-integers.md): any common [divisor](divisor.md) of $n,n+1$ divides their difference one. Thus $14,15$ provide another pair of [coprime](coprime-integers.md) [composite numbers](composite-number.md).

For [positive integers](positive-integer.md), let $P(n)$ be the [prime support of an integer](prime-support-of-an-integer.md). The equivalent test is

$$
\gcd(a,b)=1\quad\Longleftrightarrow\quad P(a)\cap P(b)=\varnothing.
$$

The [set intersection](set-intersection.md) of the two [prime supports of an integer](prime-support-of-an-integer.md) must be the [empty set](empty-set.md). Indeed, any positive common [divisor](divisor.md) greater than one has a [prime factor](prime-factor.md), and any shared [prime factor](prime-factor.md) is a common [divisor](divisor.md) greater than one. Hence [coprimality](coprime-integers.md) depends on which [prime factors](prime-factor.md) occur, rather than on their [prime valuations](prime-valuation.md); replacing either input by its [radical of an integer](radical-of-an-integer.md) preserves [coprimality](coprime-integers.md).

For a list of at least two [integers](integer-split.md), distinguish [pairwise coprimality](pairwise-coprimality.md), requiring every pair to be [coprime](coprime-integers.md), from [joint coprimality](joint-coprimality.md), requiring only the [greatest common divisor](greatest-common-divisor.md) of the entire list to be one. For example,

$$
\gcd(6,10,15)=1,\qquad
\gcd(6,10)=2,\quad\gcd(6,15)=3,\quad\gcd(10,15)=5.
$$

No [prime factor](prime-factor.md) belongs to all three [prime supports of an integer](prime-support-of-an-integer.md), yet each pair shares one. By contrast, $4,9,25$ have [pairwise coprimality](pairwise-coprimality.md). The distinction is presented by Poritz under the names pairwise and mutually relatively prime. [Jonathan A. Poritz, Yet Another Introductory Number Theory Textbook, Section 1.5](https://math.libretexts.org/Bookshelves/Combinatorics_and_Discrete_Mathematics/Yet_Another_Introductory_Number_Theory_Textbook_-_Cryptology_Emphasis_(Poritz)/01:_Well-Ordering_and_Division/1.05:_The_Greatest_Common_Divisor)

<a id="image-prime-support-of-an-integer-distinguishes-coprime-pairs-joint-coprimality-and-pairwise-coprimality"></a>
![](coprime-squarefree-integers-prime-sharing.png)

**[Figure 1](#image-prime-support-of-an-integer-distinguishes-coprime-pairs-joint-coprimality-and-pairwise-coprimality). Prime support of an integer distinguishes coprime pairs, joint coprimality and pairwise coprimality**. Filled cells mark membership in the [prime support of an integer](prime-support-of-an-integer.md); empty cells mean the [prime number](prime-number-split.md) does not divide the row label. The first panel has two [coprime integers](coprime-integers.md); the middle has [joint coprimality](joint-coprimality.md) but fails [pairwise coprimality](pairwise-coprimality.md); the last has [pairwise coprimality](pairwise-coprimality.md). The columns exhaust all [prime factors](prime-factor.md) of these eight row entries. This original finite arithmetic diagram shows exact [divisibility](divisibility-split.md), not sampled probabilities.

One use is simplifying [fractions](fraction.md). For a [fraction](fraction.md) $a/b$ with [integer](integer-split.md) entries and $b>0$, divide its [numerator](numerator.md) and [denominator](denominator.md) by $d=\gcd(a,b)$ to obtain a [reduced fraction](reduced-fraction.md) with [coprime](coprime-integers.md) entries. For example, $42/30=7/5$ since $d=6$, and $-42/30=-7/5$ uses the same $d$. A further common [divisor](divisor.md) would make $d$ too small, so the reduction is complete. In particular, the [reduced fraction](reduced-fraction.md) for zero is $0/1$.

Another use is reversible [modular arithmetic](modular-arithmetic-split.md): for an [integer modulus](modulus-in-modular-arithmetic.md) $m>1$, an [integer](integer-split.md) $a$ has a [modular inverse](modular-multiplicative-inverse.md) precisely when $a,m$ are [coprime](coprime-integers.md). The proof outline uses [Bézout's identity](bezout-s-identity.md): $ua+vm=1$ makes $u$ a [modular inverse](modular-multiplicative-inverse.md), and any inverse relation $ua-km=1$ forces every common [divisor](divisor.md) to divide one. For example, $3\cdot5-2\cdot7=1$ gives $5^{-1}\equiv3\pmod7$, whereas $6$ has no [modular inverse](modular-multiplicative-inverse.md) modulo $10$. Thus [coprimality](coprime-integers.md) is the exact condition allowing division by a residue in [modular arithmetic](modular-arithmetic-split.md). [Ankur Moitra, MIT 18.200, Lecture 15, Lemmas 1–2 and modular inverses](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

**Table of contents**

- [Pairwise coprimality](pairwise-coprimality.md)
- [Joint coprimality](joint-coprimality.md)

## ↑ Ancestors (6)

1. [Greatest common divisor](greatest-common-divisor.md)
2. [Divisibility](divisibility-split.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (55)

- [Additive function (number theory)](additive-function-number-theory.md)
- [All solutions of a linear Diophantine equation](all-solutions-of-a-linear-diophantine-equation.md)
- [Coprime integers](coprime-integers.md)
- [Decimal period from multiplicative order](decimal-period-from-multiplicative-order.md)
- [Divisor function](divisor-function.md)
- [Divisor sum](divisor-sum.md)
- [Euler totient function](euler-totient-function.md)
- [Extended Euclidean algorithm](extended-euclidean-algorithm.md)
- [Fermat number](fermat-number.md)
- [Möbius function](mobius-function.md)
- [Möbius inversion formula](mobius-inversion-formula.md)
- [Modular multiplicative inverse](modular-multiplicative-inverse.md)
- [Modulo-sixteen obstruction for the negative unit descent class](modulo-sixteen-obstruction-for-the-negative-unit-descent-class.md)
- [Multiplicative function](multiplicative-function.md)
- [Multiplicative order](multiplicative-order.md)
- [Multiplicativity of an arithmetic function](multiplicativity-of-an-arithmetic-function.md)
- [Multiplicativity of Dirichlet convolution](multiplicativity-of-dirichlet-convolution.md)
- [Number theory](number-theory-split.md)
- [Order as the exact period of modular exponentiation](order-as-the-exact-period-of-modular-exponentiation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-4/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-4/1e/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/6d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-4/6d/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-4/2e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-25/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/1d/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-4/1d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3/1h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-4/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-124/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-324/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1/1g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/1i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/11h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-2/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-1/1i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/20h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/10d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3/1g/c/solution.md)
- [Prime omega function](prime-omega-function.md)
- [Quadratic Weyl inequality](quadratic-weyl-inequality.md)
- [Radical of an integer](radical-of-an-integer.md)
- [Reduced fraction](reduced-fraction.md)
- [Signed divisor-two obstruction for an isogeny covering](signed-divisor-two-obstruction-for-an-isogeny-covering.md)
- [Torus knot](torus-knot.md)
- [Wilson factorial congruence modulo a triangular number](wilson-factorial-congruence-modulo-a-triangular-number.md)
