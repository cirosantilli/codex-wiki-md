# Slow exponential plus an exponential sample mean

↑ **Parent:** [Exponential distribution](exponential-distribution.md)

Let $S$ be a fixed sum of [independent](independent-random-variables.md) [exponential random variables](exponential-distribution.md) with smallest rate $\lambda>0$, and let $Z_N$ be the sum of $N-k$ independent rate-$r$ [exponential random variables](exponential-distribution.md), independent of $S$, with fixed $k$ and $r>\lambda$. At [large-deviation speed](large-deviation-speed.md) $N$, $S/N$ has [rate function](rate-function.md) $\lambda y$ for $y\geq0$; the sample mean has [rate function](rate-function.md) $K_r(z)=rz-1-\log(rz)$ for $z>0$. The [product large-deviation principle](product-large-deviation-principle.md) and [contraction principle for large deviations](contraction-principle-for-large-deviations.md) give

$$
I(x)=\inf_{0<z\leq x}\{\lambda(x-z)+rz-1-\log(rz)\}
=\begin{cases}
rx-1-\log(rx),&0<x\leq(r-\lambda)^{-1},\\
\lambda x+\log((r-\lambda)/r),&x\geq(r-\lambda)^{-1},\\
\infty,&x\leq0.
\end{cases}
$$

Indeed the derivative of the quantity minimized with respect to $z$ is $r-\lambda-1/z$. Its minimizer is $\min(x,(r-\lambda)^{-1})$. Beyond that transition, a single slow [exponential random variable](exponential-distribution.md) carries the extra excursion; the [rate function](rate-function.md) becomes affine.

## ↑ Ancestors (8)

1. [Exponential distribution](exponential-distribution.md)
2. [Continuous probability distribution](continuous-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36/2/b/solution.md)
