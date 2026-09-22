# Realized absolute covariation

↑ **Parent:** [Quadratic covariation](quadratic-covariation.md)

For continuous local martingales $M,N$ and a sequence in which each term is a [partition of an interval](partition-of-an-interval.md) whose mesh tends to zero, the sums

$$
\widetilde V_t^n=\sum_k|\Delta_kM|\,|\Delta_kN|
$$

converge in the sense of [uniform convergence on compacts in probability](uniform-convergence-on-compacts-in-probability.md) to a continuous increasing process. To identify the limit, put $C=[M]+[N]$ and choose [Radon-Nikodym derivatives](radon-nikodym-derivative.md)

$$
a=\frac{d[M]}{dC},\qquad b=\frac{d[N]}{dC},\qquad c=\frac{d[M,N]}{dC}.
$$

If $(U,V)$ is a centered [bivariate normal distribution](bivariate-normal-distribution.md) with covariance matrix $\left(\begin{smallmatrix}a&c\\c&b\end{smallmatrix}\right)$, then

$$
\widetilde V_t=\int_0^t\mathbb E|UV|\,dC.
$$

Localizing, representing the pair as [stochastic integrals](stochastic-integral.md) against a two-dimensional [Brownian motion](brownian-motion-split.md), and approximating the integrands by bounded predictable step processes proves the convergence. The step-process case follows from the [weak law of large numbers](weak-law-of-large-numbers.md) for independent Gaussian increments; the [Burkholder-Davis-Gundy inequality](burkholder-davis-gundy-inequalities.md) controls the approximation error. Since $|\mathbb E[UV]|\leq\mathbb E|UV|\leq\sqrt{\mathbb EU^2\mathbb EV^2}$,

$$
V_t([M,N])\leq\widetilde V_t\leq[M]_t^{1/2}[N]_t^{1/2}.
$$

## ↑ Ancestors (9)

1. [Quadratic covariation](quadratic-covariation.md)
2. [Quadratic variation](quadratic-variation.md)
3. [Stochastic calculus](stochastic-calculus-split.md)
4. [Stochastic process](stochastic-process-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202/2/b/i/solution.md)
