<h1 id="section-b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [exponential series](../../../../../../exponential-series.md) proves [normalization of a probability distribution](../../../../../../normalization-of-a-probability-distribution.md):

$$
\sum_{n=0}^\infty e^{-\lambda}\frac{\lambda^n}{n!}=e^{-\lambda}e^\lambda=1.
$$

Let $M$ and $F$ count the two labels. Conditional on $N=M+F=k+l$, independent labeling gives a [binomial distribution](../../../../../../binomial-distribution.md), so the [joint probability mass function](../../../../../../joint-probability-mass-function.md) is

$$
\begin{aligned}
\mathbb P(M=k,F=l)&=\mathbb P(N=k+l)\binom{k+l}{k}p^k(1-p)^l\\
&=e^{-\lambda}\frac{(\lambda p)^k}{k!}\frac{[\lambda(1-p)]^l}{l!}\\
&=\left[e^{-\lambda p}\frac{(\lambda p)^k}{k!}\right]\left[e^{-\lambda(1-p)}\frac{[\lambda(1-p)]^l}{l!}\right].
\end{aligned}
$$

Each bracket is a normalized [Poisson distribution](../../../../../../poisson-distribution.md). Summing over $l\geq0$ therefore gives

$$
\boxed{\mathbb P(M=k)=e^{-\lambda p}\frac{(\lambda p)^k}{k!},\qquad M\sim\operatorname{Poisson}(\lambda p).}
$$

The factorization also proves that $M$ and $F$ are [independent random variables](../../../../../../independent-random-variables.md). This is [Poisson thinning](../../../../../../poisson-thinning.md); the phrase about ignoring the other count refers to taking a [marginal distribution](../../../../../../marginal-distribution.md), rather than fixing that count.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [4](../../4.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
