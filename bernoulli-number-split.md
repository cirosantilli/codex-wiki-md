# Bernoulli number

↑ **Parent:** [Number theory](number-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_number)

The [Bernoulli numbers](bernoulli-number-split.md) are a [sequence](sequence.md) of [rational numbers](rational-number.md) that turns [integer power sums](integer-power-sum.md) into exact [polynomials](polynomial-split.md). The same numbers describe corrections when a discrete [summation](summation.md) is compared with an [integral](integral-split.md). For example, the [sum of squares](sum-of-squares.md) $1^2+\cdots+N^2$ is $N^3/3+N^2/2+N/6$: the leading term is an [integral](integral-split.md), while the last two terms repair the difference between area and sampled values.

We use **$B_1=-\tfrac12$ throughout**. The defining [exponential generating function](exponential-generating-function.md) is

$$
\frac{t}{e^t-1}=\sum_{n=0}^{\infty}B_n\frac{t^n}{n!}
=1-\frac t2+\frac{t^2}{12}-\frac{t^4}{720}+\frac{t^6}{30240}-\cdots.
$$

Here $e^t$ is the [exponential function](exponential-function.md) and $n!$ is a [factorial](factorial.md); in particular, the [coefficient](coefficient.md) of $t^2$ is $B_2/2!$, rather than $B_2$. At $t=0$ the quotient has limiting value one. The identity can be read algebraically as a [formal power series](formal-power-series.md), or as a [convergent series](convergent-series.md) for $|t|<2\pi$.[Karl Dilcher, Chapter 24, §24.2(i), equation 24.2.1: defining generating function and convergence domain](nist-digital-library-of-mathematical-functions.md)

To compute the numbers, multiply by $e^t-1$ and compare [coefficients](coefficient.md). The resulting [recurrence relation](recurrence-relation.md), with [binomial coefficients](binomial-coefficient-split.md), is

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

The [recurrence relation](recurrence-relation.md) agrees with equation 24.5.3 after replacing its index $n$ by $m+1$.[Karl Dilcher, Chapter 24, §24.5(i), equation 24.5.3; first values also in Table 24.2.1](nist-digital-library-of-mathematical-functions.md)

Why do so many values vanish? Put $F(t)=t/(e^t-1)$. Direct substitution gives $F(-t)=F(t)+t$, so $F(t)+t/2$ is an [even function](even-function.md). Its odd [power series](power-series.md) [coefficients](coefficient.md) vanish: $B_{2r+1}=0$ for every [positive integer](positive-integer.md) $r$. The exception $B_1$ matters. The alternative convention obtained from $t/(1-e^{-t})=F(t)+t$ has $B_1^{+}=+1/2$ and exactly the same other values. A formula copied between conventions must also retain its summation endpoints.

Historically, [integer power sums](integer-power-sum.md) were studied before the modern [Bernoulli number](bernoulli-number-split.md) notation. A historical study examines formulas published in 1631 and distinguishes those separate formulas from encoding all exponents using one [sequence](sequence.md) of constants. This is a useful motivation for the [generating function](generating-function.md), without assigning all discovery to a single moment. [Donald E. Knuth, Johann Faulhaber and sums of powers, 1992 preprint, pp. 2 and 14: the 1631 power-sum formulas and the uniform Bernoulli-number formula](johann-faulhaber-and-sums-of-powers-by-donald-e-knuth.md)

**Table of contents**

- [von Staudt-Clausen theorem](von-staudt-clausen-theorem.md)
- [Bernoulli polynomial](bernoulli-polynomial.md)
  - [Integer power sum](integer-power-sum.md)
    - [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)
- [Hyperbolic cotangent generating function for Bernoulli numbers](hyperbolic-cotangent-generating-function-for-bernoulli-numbers.md)
- [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md)
  - [Zeta series truncation error](zeta-series-truncation-error.md)
  - [Cotangent coefficient proof of the even zeta values](cotangent-coefficient-proof-of-the-even-zeta-values.md)
- [Generalized Bernoulli number](generalized-bernoulli-number.md)

## ↑ Ancestors (4)

1. [Number theory](number-theory-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Basel problem](basel-problem.md)
- [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)
- [Bernoulli number](bernoulli-number-split.md)
- [Bernoulli polynomial](bernoulli-polynomial.md)
- [Cotangent coefficient proof of the even zeta values](cotangent-coefficient-proof-of-the-even-zeta-values.md)
- [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md)
- [Euler-Maclaurin formula](euler-maclaurin-formula.md)
- [Hyperbolic cotangent generating function for Bernoulli numbers](hyperbolic-cotangent-generating-function-for-bernoulli-numbers.md)
- [Integer power sum](integer-power-sum.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-26/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-24/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-27/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-30/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-26/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-137/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-137/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-1/9/b/iii/solution.md)
- [Rational structure of level-one modular forms](rational-structure-of-level-one-modular-forms.md)
