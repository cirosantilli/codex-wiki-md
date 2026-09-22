# Euler evaluation of even zeta values

↑ **Parent:** [Bernoulli number](bernoulli-number-split.md)

The [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md) turns a family of [series](series-mathematics.md) into exact expressions using [Bernoulli numbers](bernoulli-number-split.md), [factorials](factorial.md) and powers of $\pi$. For every [positive integer](positive-integer.md) $r$,

$$
\boxed{\sum_{n=1}^{\infty}\frac1{n^{2r}}=\zeta(2r)=\frac{(-1)^{r+1}B_{2r}(2\pi)^{2r}}{2(2r)!}}.
$$

Here $\zeta$ is the [Riemann zeta function](riemann-zeta-function.md), defined by its [convergent series](convergent-series.md) at these arguments, and the [Bernoulli number](bernoulli-number-split.md) convention is $B_1=-1/2$. The alternating sign combines with the sign of $B_{2r}$ to give a positive [sum](sum.md).[§25.6(i), equations 25.6.1–25.6.2: positive even arguments](nist-digital-library-of-mathematical-functions/25-6-integer-arguments.md)

Substituting $B_2=1/6$, $B_4=-1/30$ and $B_6=1/42$ gives

$$
\boxed{\zeta(2)=\frac{\pi^2}{6},\qquad\zeta(4)=\frac{\pi^4}{90},\qquad\zeta(6)=\frac{\pi^6}{945}}.
$$

The first identity answers the [Basel problem](basel-problem.md). It is surprising because the original [series](series-mathematics.md) only mentions reciprocal squares of [integers](integer-split.md), while its exact [sum](sum.md) involves the circle constant $\pi$. The [cotangent partial-fraction expansion](cotangent-partial-fraction-expansion.md) supplies a connection between the two: [trigonometric functions](trigonometric-function.md) encode equally spaced integer [poles](pole.md), whose expansion brings the reciprocal powers into view.

For an original numerical comparison, the first ten terms give $\sum_{n=1}^{10}n^{-2}\approx1.549767731$, while $\pi^2/6\approx1.644934067$. The omitted positive terms still contribute approximately $0.095166336$. For fourth powers, the ten-term [partial sum](partial-sum.md) is approximately $1.082036583$, only $0.000286650$ below $\pi^4/90\approx1.082323234$. Both are [convergent series](convergent-series.md), but the second approaches its [limit](limit-of-a-function.md) much faster.

<a id="image-reciprocal-square-and-reciprocal-fourth-power-partial-sums-approach-exact-zeta-values"></a>
![](zeta-even-power-partial-sums.png)

**[Figure 3](#image-reciprocal-square-and-reciprocal-fourth-power-partial-sums-approach-exact-zeta-values). Reciprocal-square and reciprocal-fourth-power partial sums approach exact zeta values**. Original computed [partial sums](partial-sum.md) for the first thirty terms. Each panel has its own vertical scale. Dashed horizontal lines mark $\pi^2/6$ and $\pi^4/90$; neither finite [partial sum](partial-sum.md) equals its limiting value.

Exact evaluation is useful beyond obtaining more digits. It supplies an independent check on a numerical [summation](summation.md), exposes how [Bernoulli numbers](bernoulli-number-split.md) organize infinitely many identities, and makes the remaining [series truncation error](series-truncation-error.md) measurable without knowing any omitted terms individually. The [even integer](even-number.md) condition is essential to this formula: putting $r=3/2$ into it is not a way to evaluate $\zeta(3)$, since the required [Bernoulli number](bernoulli-number-split.md) index and [factorial](factorial.md) expression here are indexed by [positive integers](positive-integer.md).

Historically, [Leonhard Euler](leonhard-euler.md) announced reciprocal-square and reciprocal-fourth-power evaluations in §2 of [On the sums of series of reciprocals by Leonhard Euler](on-the-sums-of-series-of-reciprocals-by-leonhard-euler.md). That paper was presented on 5 December 1735 and published in 1740, as the English translation's first-page note records. His §§3–8 develop a route through the [sine](sine.md) [power series](power-series.md) and relationships between roots and [coefficients](coefficient.md). The [cotangent](cotangent.md) calculation below is a concise modern presentation of the connection.[English translation, p. 1, §2 and publication note; pp. 3–4, §§3–8: sine series, roots and coefficients](on-the-sums-of-series-of-reciprocals-by-leonhard-euler.md)

**Table of contents**

- [Zeta series truncation error](zeta-series-truncation-error.md)
- [Cotangent coefficient proof of the even zeta values](cotangent-coefficient-proof-of-the-even-zeta-values.md)

## ↑ Ancestors (5)

1. [Bernoulli number](bernoulli-number-split.md)
2. [Number theory](number-theory-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Basel problem](basel-problem.md)
- [Euler evaluation of even zeta values](euler-evaluation-of-even-zeta-values.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-33/2/solution.md)
