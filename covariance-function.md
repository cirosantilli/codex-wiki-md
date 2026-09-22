# Covariance function

↑ **Parent:** [Stochastic process](stochastic-process-split.md)

For a real-valued [stochastic process](stochastic-process-split.md) $(X_t)$ with finite [second moments](second-moment.md), write $m(t)=\mathbb E X_t$. Its covariance function is

$$
C(s,t)=\operatorname{Cov}(X_s,X_t)=\mathbb E[(X_s-m(s))(X_t-m(t))].
$$

The diagonal gives the [variance](variance-split.md) at each time; off-diagonal values record linear dependence between times. For the independent [standard normal random variables](standard-normal-random-variable.md) above, $C_X(m,n)=\mathbf1_{\{m=n\}}$, whereas the shared [Gaussian process](gaussian-process-split.md) $Y_n=Z$ has $C_Y(m,n)=1$ for all $m,n$. For a fair [simple random walk on the integer line](simple-random-walk-on-the-integer-line.md), $C(m,n)=\min(m,n)$; [Brownian motion](brownian-motion-split.md) has the continuous-time counterpart $C(s,t)=\min(s,t)$. These formulas quantify how much random history the observations share.

Every covariance function is a [positive-semidefinite kernel](positive-semidefinite-kernel-split.md). Indeed, for any real coefficients $a_1,\ldots,a_k$,

$$
\sum_{i,j=1}^k a_i a_j C(t_i,t_j)=\operatorname{Var}\!\left(\sum_{i=1}^k a_i X_{t_i}\right)\ge0.
$$

Thus a proposed covariance function must make every finite [covariance matrix](covariance-matrix.md) [positive semidefinite](positive-semidefinite-matrix.md). For a [Gaussian process](gaussian-process-split.md), the [mean](expected-value-split.md) function and the covariance function determine every [finite-dimensional distribution](finite-dimensional-distribution.md), including degenerate ones such as the shared process. Conversely, any real [positive-semidefinite kernel](positive-semidefinite-kernel-split.md) satisfying $C(s,t)=C(t,s)$, together with a specified [mean](expected-value-split.md) function, defines consistent [multivariate normal distributions](multivariate-normal-distribution.md); the [Kolmogorov extension theorem](kolmogorov-extension-theorem.md) then constructs a [Gaussian process](gaussian-process-split.md). For a general [stochastic process](stochastic-process-split.md), [covariance](covariance.md) alone does not determine the full law. The exceptional completeness of this description is what makes [Gaussian process regression](gaussian-process-regression.md) possible with a mean and a covariance model.

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (28)

- [Autocovariance](autocovariance.md)
- [Brownian snake](brownian-snake.md)
- [Canonical pseudometric of a Gaussian process](canonical-pseudometric-of-a-gaussian-process.md)
- [Covariance of a squared random field](covariance-of-a-squared-random-field.md)
- [Differentiable modification of a stationary Gaussian process](differentiable-modification-of-a-stationary-gaussian-process.md)
- [Exponential Brownian time change to a stationary Ornstein-Uhlenbeck process](exponential-brownian-time-change-to-a-stationary-ornstein-uhlenbeck-process.md)
- [Fractional Brownian motion](fractional-brownian-motion.md)
- [Gaussian process regression](gaussian-process-regression.md)
- [Kriging](kriging.md)
- [Mathematical model](mathematical-model.md)
- [Mean-square derivative of a Gaussian process](mean-square-derivative-of-a-gaussian-process.md)
- [Ordinary kriging](ordinary-kriging.md)
- [Ornstein-Uhlenbeck stationary initialization](ornstein-uhlenbeck-stationary-initialization.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-41/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72/1/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-220/2/a/ii/solution.md)
- [Periodic covariance function](periodic-covariance-function.md)
- [Phase covariance in the first Rytov approximation](phase-covariance-in-the-first-rytov-approximation.md)
- [Phase folding of a light curve](phase-folding-of-a-light-curve.md)
- [Power spectrum of surface height](power-spectrum-of-surface-height.md)
- [Random field](random-field.md)
- [Stochastic process](stochastic-process-split.md)
- [Uncentered wave-field correlation](uncentered-wave-field-correlation.md)
