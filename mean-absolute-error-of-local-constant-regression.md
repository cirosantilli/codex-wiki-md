# Mean absolute error of local constant regression

↑ **Parent:** [Nadaraya–Watson estimator](nadaraya-watson-estimator.md)

For an equally spaced design with independent errors of variance at most $\sigma^2$ and a regression function with [Lipschitz constant](lipschitz-constant.md) $L$, the [unit-width box kernel](unit-width-box-kernel.md) estimator averages the $N_x$ observations in the window. Its bias is at most $Lh/2$, and its variance is at most $\sigma^2/N_x$. The [window occupancy for an equally spaced regression design](window-occupancy-for-an-equally-spaced-regression-design.md) gives, whenever $nh\ge2$,

$$
\mathbb E|\widehat m(x)-m(x)|\le\frac{2\sigma}{\sqrt{n\min(h,1)}}+\frac{Lh}{2}.
$$

In the usual range $h\le1$, this is $O(\sigma/\sqrt{nh}+Lh)$ uniformly up to the boundary. For arbitrarily large bandwidth, the stochastic error cannot continue to decrease as $1/\sqrt{nh}$: once all observations are included the estimator is simply their mean.

## ↑ Ancestors (9)

1. [Nadaraya–Watson estimator](nadaraya-watson-estimator.md)
2. [Local polynomial regression](local-polynomial-regression.md)
3. [Nonparametric regression](nonparametric-regression.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/4/solution.md)
