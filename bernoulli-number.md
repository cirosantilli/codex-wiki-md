# Bernoulli number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_number)

The [Bernoulli numbers](bernoulli-number.md) are a [sequence](sequence-and-series.md#sequence) of [rational numbers](number-theory.md#rational-number) that turns [integer power sums](#integer-power-sum) into exact [polynomials](polynomial.md). The same numbers describe corrections when a discrete [summation](arithmetic.md#summation) is compared with an [integral](integral.md). For example, the [sum of squares](arithmetic.md#sum-of-squares) $1^2+\cdots+N^2$ is $N^3/3+N^2/2+N/6$: the leading term is an [integral](integral.md), while the last two terms repair the difference between area and sampled values.

We use **$B_1=-\tfrac12$ throughout**. The defining [exponential generating function](sequence-and-series.md#exponential-generating-function) is

$$
\frac{t}{e^t-1}=\sum_{n=0}^{\infty}B_n\frac{t^n}{n!}
=1-\frac t2+\frac{t^2}{12}-\frac{t^4}{720}+\frac{t^6}{30240}-\cdots.
$$

Here $e^t$ is the [exponential function](calculus.md#exponential-function) and $n!$ is a [factorial](combinatorics.md#factorial); in particular, the [coefficient](vector-space.md#coefficient) of $t^2$ is $B_2/2!$, rather than $B_2$. At $t=0$ the quotient has limiting value one. The identity can be read algebraically as a [formal power series](commutative-algebra.md#formal-power-series), or as a [convergent series](sequence-and-series.md#convergent-series) for $|t|<2\pi$.[Karl Dilcher, Chapter 24, §24.2(i), equation 24.2.1: defining generating function and convergence domain](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

To compute the numbers, multiply by $e^t-1$ and compare [coefficients](vector-space.md#coefficient). The resulting [recurrence relation](sequence-and-series.md#recurrence-relation), with [binomial coefficients](binomial-coefficient.md), is

$$
B_0=1,\qquad \sum_{k=0}^{m}\binom{m+1}{k}B_k=0\quad(m\geq1),\qquad
B_m=-\frac{1}{m+1}\sum_{k=0}^{m-1}\binom{m+1}{k}B_k.
$$

Thus $1+2B_1=0$, $1+3B_1+3B_2=0$, and $1+4B_1+6B_2+4B_3=0$ give $B_1=-1/2$, $B_2=1/6$, and $B_3=0$. Continuing gives

$$
\begin{array}{c|rrrrrrrrrrr}
n&0&1&2&3&4&5&6&7&8&9&10\\\hline
B_n&1&-\tfrac12&\tfrac16&0&-\tfrac1{30}&0&\tfrac1{42}&0&-\tfrac1{30}&0&\tfrac5{66}
\end{array}
$$

The [recurrence relation](sequence-and-series.md#recurrence-relation) agrees with equation 24.5.3 after replacing its index $n$ by $m+1$.[Karl Dilcher, Chapter 24, §24.5(i), equation 24.5.3; first values also in Table 24.2.1](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

Why do so many values vanish? Put $F(t)=t/(e^t-1)$. Direct substitution gives $F(-t)=F(t)+t$, so $F(t)+t/2$ is an [even function](calculus.md#even-function). Its odd [power series](sequence-and-series.md#power-series) [coefficients](vector-space.md#coefficient) vanish: $B_{2r+1}=0$ for every [positive integer](integer.md#positive-integer) $r$. The exception $B_1$ matters. The alternative convention obtained from $t/(1-e^{-t})=F(t)+t$ has $B_1^{+}=+1/2$ and exactly the same other values. A formula copied between conventions must also retain its summation endpoints.

Historically, [integer power sums](#integer-power-sum) were studied before the modern [Bernoulli number](bernoulli-number.md) notation. A historical study examines formulas published in 1631 and distinguishes those separate formulas from encoding all exponents using one [sequence](sequence-and-series.md#sequence) of constants. This is a useful motivation for the [generating function](sequence-and-series.md#generating-function), without assigning all discovery to a single moment. [Donald E. Knuth, Johann Faulhaber and sums of powers, 1992 preprint, pp. 2 and 14: the 1631 power-sum formulas and the uniform Bernoulli-number formula](mathematics-bibliography.md#johann-faulhaber-and-sums-of-powers-by-donald-e-knuth)

**Table of contents**

- [von Staudt-Clausen theorem](#von-staudt-clausen-theorem)
- [Bernoulli polynomial](#bernoulli-polynomial)
  - [Integer power sum](#integer-power-sum)
    - [Bernoulli corrections for polynomial sums](#bernoulli-corrections-for-polynomial-sums)
- [Hyperbolic cotangent generating function for Bernoulli numbers](#hyperbolic-cotangent-generating-function-for-bernoulli-numbers)
- [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values)
  - [Zeta series truncation error](#zeta-series-truncation-error)
  - [Cotangent coefficient proof of the even zeta values](#cotangent-coefficient-proof-of-the-even-zeta-values)
- [Generalized Bernoulli number](#generalized-bernoulli-number)

## von Staudt-Clausen theorem

↑ **Parent:** [Bernoulli number](bernoulli-number.md)

## Bernoulli polynomial

↑ **Parent:** [Bernoulli number](bernoulli-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_polynomial)

The [Bernoulli polynomials](#bernoulli-polynomial) extend the [Bernoulli numbers](bernoulli-number.md) by inserting the [exponential function](calculus.md#exponential-function) $e^{xt}$ into their [exponential generating function](sequence-and-series.md#exponential-generating-function):

$$
\frac{te^{xt}}{e^t-1}=\sum_{n=0}^{\infty}B_n(x)\frac{t^n}{n!},\qquad
B_n(x)=\sum_{j=0}^{n}\binom nj B_jx^{n-j},\qquad B_n(0)=B_n.
$$

For example, $B_0(x)=1$, $B_1(x)=x-1/2$, $B_2(x)=x^2-x+1/6$, and $B_3(x)=x^3-3x^2/2+x/2$.[Karl Dilcher, Chapter 24, equations 24.2.3–24.2.5 and Table 24.2.2](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

Their crucial property is a [finite difference](finite-difference.md) identity:

$$
B_n(x+1)-B_n(x)=nx^{n-1}\quad(n\geq1).
$$

Indeed, subtracting the two [exponential generating functions](sequence-and-series.md#exponential-generating-function) cancels $e^t-1$ and leaves $te^{xt}$. Thus $B_{p+1}(x)/(p+1)$ plays for discrete [summation](arithmetic.md#summation) the role that $x^{p+1}/(p+1)$ plays for [integration](integral.md): taking a unit [finite difference](finite-difference.md) recovers $x^p$.[Karl Dilcher, Chapter 24, §24.4(i), equation 24.4.1](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

### Integer power sum

↑ **Parent:** [Bernoulli polynomial](#bernoulli-polynomial)

An integer power sum adds a fixed nonnegative [integer](integer.md) power of consecutive [integers](integer.md). Let $N$ be a [nonnegative integer](arithmetic.md#natural-number) and $p$ a [nonnegative integer](arithmetic.md#natural-number). For $p=0$, use the constant [polynomial](polynomial.md) $x^0=1$, including at zero, so $S_0(N)=N$. Summing the [Bernoulli polynomial](#bernoulli-polynomial) [finite difference](finite-difference.md) identity makes the intermediate terms cancel and gives

$$
S_p(N)=\sum_{k=0}^{N-1}k^p
=\frac{B_{p+1}(N)-B_{p+1}(0)}{p+1}
=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_jN^{p+1-j}.
$$

The sum is empty when $N=0$. For the endpoints $1,\ldots,N$, the formula valid also at $p=0$ is instead

$$
\sum_{k=1}^{N}k^p=\frac{B_{p+1}(N+1)-B_{p+1}(1)}{p+1}.
$$

For $p\geq1$, $B_{p+1}(1)=B_{p+1}(0)$, and this becomes the standard positive-endpoint formula. The exception at $p=0$ is essential: $B_1(1)-B_1(0)=1$.[Karl Dilcher, Chapter 24, equations 24.4.1 and 24.4.7; the displayed equation 24.4.7 needs the endpoint adjustment at exponent zero](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

For $p\geq1$, adding $N^p$ to $S_p(N)$ changes the $B_1$ contribution from $-N^p/2$ to $+N^p/2$. Equivalently,

$$
\sum_{k=1}^{N}k^p=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_j^{+}N^{p+1-j}\quad(p\geq1),
$$

where only $B_1^{+}$ differs from our [Bernoulli numbers](bernoulli-number.md). A quick endpoint check is $p=1$: the sums over $0,\ldots,N-1$ and $1,\ldots,N$ are $N(N-1)/2$ and $N(N+1)/2$, respectively. The latter is a [triangular number](arithmetic.md#triangular-number).

#### Bernoulli corrections for polynomial sums

↑ **Parent:** [Integer power sum](#integer-power-sum)

For a concrete comparison, take $f(x)=x^2$ on $[0,6]$. The [integral](integral.md) is $I=\int_0^6x^2\,dx=72$, whereas the unit-width left and right [Riemann sums](real-analysis.md#riemann-sum) are $L=55$ and $R=91$. The exact [integer power sum](#integer-power-sum) formula gives

$$
L=I-\frac{6^2}{2}+\frac66=55,\qquad
R=I+\frac{6^2}{2}+\frac66=91.
$$

The endpoint choice explains the opposite signs of the $18$ correction. The remaining correction is one in both cases.

<a id="image-left-and-right-riemann-sums-for-x-2-differ-from-its-integral-by-exact-bernoulli-number-corrections"></a>
![](bernoulli-square-sums-versus-integral.png)

**[Figure 1](#image-left-and-right-riemann-sums-for-x-2-differ-from-its-integral-by-exact-bernoulli-number-corrections). Left and right Riemann sums for $x^2$ differ from its integral by exact Bernoulli number corrections**. Six rectangles of width one sample $x^2$ at $0,\ldots,5$ on the left and $1,\ldots,6$ on the right. Their areas are $55$ and $91$; the smooth area is $72$. The endpoint terms are $-18$ and $+18$, while the $B_2$ correction adds one in each case.

The same method is useful far beyond [squares of numbers](arithmetic.md#square-of-a-number). Substituting $B_0$, $B_1$, $B_2$ and $B_4$ into the [integer power sum](#integer-power-sum) formula gives the exact fourth-power result

$$
\sum_{k=1}^{N}k^4=\frac{N^5}{5}+\frac{N^4}{2}+\frac{N^3}{3}-\frac{N}{30}.
$$

At $N=10$, this is

$$
\underbrace{20000}_{\text{integral}}+\underbrace{5000}_{\text{endpoint}}+
\underbrace{\frac{1000}{3}}_{B_2\text{ term}}-
\underbrace{\frac13}_{B_4\text{ term}}=25333.
$$

Thus a finite [polynomial](polynomial.md) calculation replaces ten additions, or a million additions if $N$ is a million. Although the individual corrections can be [rational numbers](number-theory.md#rational-number), the result is the exact [integer](integer.md) sum.

<a id="image-exact-bernoulli-number-corrections-turn-an-integral-into-the-fourth-power-sum-1-4-plus-cdots-plus-10-4"></a>
![](bernoulli-fourth-power-exact-corrections.png)

**[Figure 2](#image-exact-bernoulli-number-corrections-turn-an-integral-into-the-fourth-power-sum-1-4-plus-cdots-plus-10-4). Exact Bernoulli number corrections turn an integral into the fourth-power sum $1^4+\cdots+10^4$**. The first panel builds the sum from integral $20000$, endpoint term $5000$, and $B_2$ term $1000/3$. The enlarged second panel resolves the final $B_4$ correction $-1/3$, reaching $25333$, checked independently by direct addition.

There is also a useful [numerical integration](numerical-integration.md) interpretation. The average of the left and right [Riemann sums](real-analysis.md#riemann-sum) is the composite [trapezoidal rule](runge-kutta-method.md#trapezoidal-rule). For $x^2$, the endpoint corrections cancel but its value is $73$, one above the true [integral](integral.md). Subtracting the $B_2$ correction makes this particular [polynomial](polynomial.md) example exact. For $f(x)=x^4$, the two interior corrections above can be written $B_2(f'(N)-f'(0))/2!$ and $B_4(f'''(N)-f'''(0))/4!$. These are exact identities for these [polynomials](polynomial.md); extending such corrections to general [functions](function.md) requires a separate error analysis.

## Hyperbolic cotangent generating function for Bernoulli numbers

↑ **Parent:** [Bernoulli number](bernoulli-number.md)

The defining generating function of the [Bernoulli numbers](bernoulli-number.md), with $B_1=-1/2$, gives this identity of formal [Laurent series](analysis.md#laurent-series) by $\coth z=1+2/(e^{2z}-1)$. Therefore $a\coth(az)-\coth z$ is regular and odd. Integrating it gives the even formal logarithm of $\sinh(az)/(a\sinh z)$. Its even derivatives of order $k$ at zero are $2^k(a^k-1)B_k/k$, while the odd derivatives vanish. This computes the [cyclotomic higher logarithmic derivatives](algebraic-number-theory.md#cyclotomic-higher-logarithmic-derivative) of symmetric [cyclotomic units](galois-theory.md#cyclotomic-unit) without introducing a spurious linear term.

## Euler evaluation of even zeta values

↑ **Parent:** [Bernoulli number](bernoulli-number.md)

The [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values) turns a family of [series](sequence-and-series.md#series-mathematics) into exact expressions using [Bernoulli numbers](bernoulli-number.md), [factorials](combinatorics.md#factorial) and powers of $\pi$. For every [positive integer](integer.md#positive-integer) $r$,

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^{2r}}=\zeta(2r)=\frac{(-1)^{r+1}B_{2r}(2\pi)^{2r}}{2(2r)!}}.
$$

Here $\zeta$ is the [Riemann zeta function](analytic-number-theory.md#riemann-zeta-function), defined by its [convergent series](sequence-and-series.md#convergent-series) at these arguments, and the [Bernoulli number](bernoulli-number.md) convention is $B_1=-1/2$. The alternating sign combines with the sign of $B_{2r}$ to give a positive [sum](arithmetic.md#sum).[§25.6(i), equations 25.6.1–25.6.2: positive even arguments](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions/25-6-integer-arguments)

Substituting $B_2=1/6$, $B_4=-1/30$ and $B_6=1/42$ gives

$$
\boxed{\zeta(2)=\frac{\pi^2}{6},\qquad\zeta(4)=\frac{\pi^4}{90},\qquad\zeta(6)=\frac{\pi^6}{945}}.
$$

The first identity answers the [Basel problem](analytic-number-theory.md#basel-problem). It is surprising because the original [series](sequence-and-series.md#series-mathematics) only mentions reciprocal squares of [integers](integer.md), while its exact [sum](arithmetic.md#sum) involves the circle constant $\pi$. The [cotangent partial-fraction expansion](geometry-and-topology.md#cotangent-partial-fraction-expansion) supplies a connection between the two: [trigonometric functions](geometry-and-topology.md#trigonometric-function) encode equally spaced integer [poles](isolated-singularity.md#pole), whose expansion brings the reciprocal powers into view.

For an original numerical comparison, the first ten terms give $\sum_{n=1}^{10}n^{-2}\approx1.549767731$, while $\pi^2/6\approx1.644934067$. The omitted positive terms still contribute approximately $0.095166336$. For fourth powers, the ten-term [partial sum](sequence-and-series.md#partial-sum) is approximately $1.082036583$, only $0.000286650$ below $\pi^4/90\approx1.082323234$. Both are [convergent series](sequence-and-series.md#convergent-series), but the second approaches its [limit](calculus.md#limit-of-a-function) much faster.

<a id="image-reciprocal-square-and-reciprocal-fourth-power-partial-sums-approach-exact-zeta-values"></a>
![](zeta-even-power-partial-sums.png)

**[Figure 3](#image-reciprocal-square-and-reciprocal-fourth-power-partial-sums-approach-exact-zeta-values). Reciprocal-square and reciprocal-fourth-power partial sums approach exact zeta values**. Original computed [partial sums](sequence-and-series.md#partial-sum) for the first thirty terms. Each panel has its own vertical scale. Dashed horizontal lines mark $\pi^2/6$ and $\pi^4/90$; neither finite [partial sum](sequence-and-series.md#partial-sum) equals its limiting value.

Exact evaluation is useful beyond obtaining more digits. It supplies an independent check on a numerical [summation](arithmetic.md#summation), exposes how [Bernoulli numbers](bernoulli-number.md) organize infinitely many identities, and makes the remaining [series truncation error](numerical-analysis.md#series-truncation-error) measurable without knowing any omitted terms individually. The [even integer](integer.md#even-number) condition is essential to this formula: putting $r=3/2$ into it is not a way to evaluate $\zeta(3)$, since the required [Bernoulli number](bernoulli-number.md) index and [factorial](combinatorics.md#factorial) expression here are indexed by [positive integers](integer.md#positive-integer).

Historically, [Leonhard Euler](mathematics.md#leonhard-euler) announced reciprocal-square and reciprocal-fourth-power evaluations in §2 of [On the sums of series of reciprocals by Leonhard Euler](mathematics-bibliography.md#on-the-sums-of-series-of-reciprocals-by-leonhard-euler). That paper was presented on 5 December 1735 and published in 1740, as the English translation's first-page note records. His §§3–8 develop a route through the [sine](geometry-and-topology.md#sine) [power series](sequence-and-series.md#power-series) and relationships between roots and [coefficients](vector-space.md#coefficient). The [cotangent](geometry-and-topology.md#cotangent) calculation below is a concise modern presentation of the connection.[English translation, p. 1, §2 and publication note; pp. 3–4, §§3–8: sine series, roots and coefficients](mathematics-bibliography.md#on-the-sums-of-series-of-reciprocals-by-leonhard-euler)

### Zeta series truncation error

↑ **Parent:** [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values)

For a real [exponent](arithmetic.md#exponent) $s>1$ and a [positive integer](integer.md#positive-integer) $N$, the [series truncation error](numerical-analysis.md#series-truncation-error) in the defining [Riemann zeta function](analytic-number-theory.md#riemann-zeta-function) [series](sequence-and-series.md#series-mathematics) is

$$
R_N(s)=\sum_{n=N+1}^{\infty}n^{-s}>0.
$$

The [integral comparison](sequence-and-series.md#integral-comparison-for-a-nonincreasing-nonnegative-function) for the positive decreasing [function](function.md) $x^{-s}$ gives the explicit bounds

$$
\boxed{\frac{(N+1)^{1-s}}{s-1}\leq R_N(s)\leq\frac{N^{1-s}}{s-1}}.
$$

On each unit [interval](real-analysis.md#interval-mathematics), the area under $x^{-s}$ lies between its endpoint heights. Summing from the first omitted term gives the lower [integral](integral.md) from $N+1$ to infinity and the upper [integral](integral.md) from $N$ to infinity. This uses positivity and monotonicity, not an assumption that the last computed term equals the remaining error.

At $N=10$, the bounds are $1/11\leq R_{10}(2)\leq1/10$, whereas $1/(3\cdot11^3)\leq R_{10}(4)\leq1/(3\cdot10^3)$. The errors above fit both intervals. Merely looking at the eleventh term would give $1/121\approx0.008264$ for squares, far smaller than the actual remaining $0.095166$.

<a id="image-integral-bounds-enclose-the-full-remaining-error-of-two-zeta-series"></a>
![](zeta-even-power-tail-bounds.png)

**[Figure 4](#image-integral-bounds-enclose-the-full-remaining-error-of-two-zeta-series). Integral bounds enclose the full remaining error of two zeta series**. Original computed errors, obtained by subtracting finite [partial sums](sequence-and-series.md#partial-sum) from the exact even zeta values. Shaded bands show the upper and lower [integral comparison](sequence-and-series.md#integral-comparison-for-a-nonincreasing-nonnegative-function) bounds. The logarithmic axes reveal decay proportional to $1/N$ for squares and $1/N^3$ for fourth powers. These are mathematical computations, not measured data.

For a chosen absolute error target $\varepsilon>0$, the sufficient condition is $N\geq((s-1)\varepsilon)^{-1/(s-1)}$, rounded upward to an [integer](integer.md). Thus $\varepsilon=10^{-4}$ requires $N=10000$ by this bound for squares but only $N=15$ for fourth powers. This is a guarantee from an upper bound, not a claim that those are the smallest successful term counts.

### Cotangent coefficient proof of the even zeta values

↑ **Parent:** [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values)

The [cotangent partial-fraction expansion](geometry-and-topology.md#cotangent-partial-fraction-expansion) gives, on $0<|z|<1$,

$$
\pi\cot(\pi z)=z^{-1}-2\sum_{r\geq1}\zeta(2r)z^{2r-1}.
$$

The [Bernoulli number](bernoulli-number.md) [generating function](sequence-and-series.md#generating-function) gives the same [Laurent series](analysis.md#laurent-series) in another form:

$$
\pi\cot(\pi z)=\pi i+\frac{2\pi i}{e^{2\pi iz}-1}
=z^{-1}+\sum_{r\geq1}\frac{B_{2r}(2\pi i)^{2r}}{(2r)!}z^{2r-1}.
$$

The $B_1$ term cancels the separate $\pi i$; the higher odd [Bernoulli numbers](bernoulli-number.md) vanish. Comparing [Laurent coefficients](analysis.md#laurent-coefficient) therefore gives $-2\zeta(2r)=B_{2r}(2\pi i)^{2r}/(2r)!$, which is the stated real formula because $i^{2r}=(-1)^r$. The [cotangent partial-fraction expansion](geometry-and-topology.md#cotangent-partial-fraction-expansion) justifies the convergent expansion before the [coefficient](vector-space.md#coefficient) comparison; a finite plot of [partial sums](sequence-and-series.md#partial-sum) alone would not prove the infinite identity.

## Generalized Bernoulli number

↑ **Parent:** [Bernoulli number](bernoulli-number.md)

For a [Dirichlet character](algebraic-number-theory.md#dirichlet-character) $\chi$ of conductor $f$, define the generalized Bernoulli numbers by

$$
\sum_{a=1}^{f}\chi(a)\frac{z e^{az}}{e^{fz}-1}
=\sum_{k\geq0}B_{k,\chi}\frac{z^k}{k!}.
$$

They express special values of [Dirichlet L-functions](algebraic-number-theory.md#dirichlet-l-function) at nonpositive integers and occur in the interpolation formula for [Kubota-Leopoldt p-adic L-functions](analytic-number-theory.md#kubota-leopoldt-p-adic-l-function).

## ↑ Ancestors (4)

1. [Number theory](number-theory.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (19)

- [Basel problem](analytic-number-theory.md#basel-problem)
- [Bernoulli corrections for polynomial sums](#bernoulli-corrections-for-polynomial-sums)
- [Bernoulli number](bernoulli-number.md)
- [Bernoulli polynomial](#bernoulli-polynomial)
- [Cotangent coefficient proof of the even zeta values](#cotangent-coefficient-proof-of-the-even-zeta-values)
- [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values)
- [Euler-Maclaurin formula](arithmetic.md#euler-maclaurin-formula)
- [Hyperbolic cotangent generating function for Bernoulli numbers](#hyperbolic-cotangent-generating-function-for-bernoulli-numbers)
- [Integer power sum](#integer-power-sum)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-27.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-30.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-26.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1.md#9/b/iii/solution)
- [Rational structure of level-one modular forms](modular-function.md#rational-structure-of-level-one-modular-forms)
