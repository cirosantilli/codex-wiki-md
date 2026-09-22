<h1 id="autocovariance-of-an-ma-1-process">Autocovariance of an MA(1) process</h1>

↑ **Parent:** [Moving-average process of order one](moving-average-process-of-order-one.md)

For the [MA(1)](moving-average-process-of-order-one.md) $X_t=\mu+\varepsilon_t+\theta\varepsilon_{t-1}$, centered [white noise](white-noise.md) gives

$$
\gamma(h)=\begin{cases}
\sigma^2(1+\theta^2),&h=0,\\
\sigma^2\theta,&|h|=1,\\
0,&|h|\ge2,
\end{cases}
\qquad
\rho(h)=\begin{cases}
1,&h=0,\\
\theta/(1+\theta^2),&|h|=1,\\
0,&|h|\ge2.
\end{cases}
$$

Only products of noise values with matching time indices have nonzero [expectation](expected-value-split.md). At lag zero there are two squared weights, $1$ and $\theta^2$; at lag one there is one shared noise term with weight product $\theta$; at higher lags there are none. The calculation needs zero [covariance](covariance.md) between distinct noise values, not independence. This tridiagonal finite [covariance](covariance.md) structure makes the [finite-sample innovations of an MA(1) process](finite-sample-innovations-of-an-ma-1-process.md) particularly simple.

The lag-one [autocorrelation](autocorrelation.md) can never exceed $1/2$ in magnitude, since $1+\theta^2\ge2|\theta|$. For $\theta\ne0$, replacing $\theta$ by $1/\theta$ leaves the entire [ACF](autocorrelation.md) unchanged. For example $\theta=2$ and $\theta=1/2$ both give $\rho(1)=2/5$; rescaling the latter noise [variance](variance-split.md) by $4$ also matches every [autocovariance](autocovariance.md). [Moving-average root reflection](moving-average-root-reflection.md) explains this ambiguity and why a stable invertibility convention helps identify a representation. Equality of second-order laws need not imply equality of all joint [probability distributions](probability-distribution-split.md) unless the processes are [Gaussian processes](gaussian-process-split.md). See [Bartlett, lecture 6: equivalent representations and covariance of ARMA processes](https://www.stat.berkeley.edu/~bartlett/courses/153-fall2010/lectures/6.pdf).

## ↑ Ancestors (8)

1. [Moving-average process of order one](moving-average-process-of-order-one.md)
2. [Moving-average model](moving-average-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Moving-average process of order one](moving-average-process-of-order-one.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38/2/solution.md)
