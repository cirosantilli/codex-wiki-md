# Bernoulli polynomial

↑ **Parent:** [Bernoulli number](bernoulli-number.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_polynomial)

The [Bernoulli polynomials](bernoulli-polynomial.md) extend the [Bernoulli numbers](bernoulli-number.md) by inserting the [exponential function](exponential-function.md) $e^{xt}$ into their [exponential generating function](exponential-generating-function.md):

$$
\frac{te^{xt}}{e^t-1}=\sum_{n=0}^{\infty}B_n(x)\frac{t^n}{n!},\qquad
B_n(x)=\sum_{j=0}^{n}\binom nj B_jx^{n-j},\qquad B_n(0)=B_n.
$$

For example, $B_0(x)=1$, $B_1(x)=x-1/2$, $B_2(x)=x^2-x+1/6$, and $B_3(x)=x^3-3x^2/2+x/2$.[Karl Dilcher, Chapter 24, equations 24.2.3–24.2.5 and Table 24.2.2](nist-digital-library-of-mathematical-functions.md)

Their crucial property is a [finite difference](finite-difference-split.md) identity:

$$
B_n(x+1)-B_n(x)=nx^{n-1}\quad(n\geq1).
$$

Indeed, subtracting the two [exponential generating functions](exponential-generating-function.md) cancels $e^t-1$ and leaves $te^{xt}$. Thus $B_{p+1}(x)/(p+1)$ plays for discrete [summation](summation.md) the role that $x^{p+1}/(p+1)$ plays for [integration](integral.md): taking a unit [finite difference](finite-difference-split.md) recovers $x^p$.[Karl Dilcher, Chapter 24, §24.4(i), equation 24.4.1](nist-digital-library-of-mathematical-functions.md)

**Table of contents**

- [Integer power sum](integer-power-sum.md)
  - [Bernoulli corrections for polynomial sums](bernoulli-corrections-for-polynomial-sums.md)

## ↑ Ancestors (5)

1. [Bernoulli number](bernoulli-number.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Bernoulli polynomial](bernoulli-polynomial.md)
- [Integer power sum](integer-power-sum.md)
