# Exponential endpoint limit of a uniform maximum

↑ **Parent:** [Uniform order statistic](uniform-order-statistic.md)

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) $U_i$ with the [continuous uniform distribution](continuous-uniform-distribution.md) on $[0,1]$, let $M_n=\max_{1\leq i\leq n}U_i$. Its [cumulative distribution function](cumulative-distribution-function.md) is $x^n$ on $[0,1]$, so $M_n\xrightarrow{\mathrm d}1$. The endpoint error has a nonconstant limiting [probability distribution](probability-distribution-split.md): for fixed $z\geq0$ and $n\geq z$,

$$
\mathbb P(n(1-M_n)>z)=(1-z/n)^n\longrightarrow e^{-z}.
$$

This [survival function](survival-function.md) gives the displayed [exponential distribution](exponential-distribution.md) limit. More generally, for observations uniform on $[a,b]$, $n(b-M_n)/(b-a)$ has the same limit. The scaling identifies an error of order $1/n$, in contrast to the $1/\sqrt n$ fluctuations of a typical [sample mean](sample-mean.md) with nonzero finite [variance](variance-split.md).

## ↑ Ancestors (7)

1. [Uniform order statistic](uniform-order-statistic.md)
2. [Order statistic](order-statistic.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-probability-course-of-the-university-of-oxford/2015/1/a/ii/solution.md)
