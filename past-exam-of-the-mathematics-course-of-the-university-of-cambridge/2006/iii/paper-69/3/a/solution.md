<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The strain is an [Ornstein-Uhlenbeck process](../../../../../../ornstein-uhlenbeck-process.md). Multiplying its equation by the [integrating factor](../../../../../../integrating-factor.md) $e^{t/\tau}$ and using the zero initial condition gives

$$
\widetilde\sigma(t)=\int_0^t e^{-(t-s)/\tau}f(s)\,ds=\sqrt\kappa\int_0^t e^{-(t-s)/\tau}\,dW_s.
$$

The second expression is a [stochastic integral](../../../../../../stochastic-integral.md) against [Brownian motion](../../../../../../brownian-motion-split.md). A deterministic linear functional of [Gaussian white noise](../../../../../../gaussian-white-noise.md) is [Gaussian](../../../../../../normal-distribution.md), and its [expected value](../../../../../../expected-value.md) is zero. For $t\ge t'$, the noise [covariance](../../../../../../covariance.md) gives

$$
\begin{aligned}
\mathbb E[\widetilde\sigma(t)\widetilde\sigma(t')]
&=\kappa\int_0^{t'}e^{-(t-s)/\tau}e^{-(t'-s)/\tau}\,ds\\
&=\frac{\kappa\tau}{2}\left[e^{-(t-t')/\tau}-e^{-(t+t')/\tau}\right].
\end{aligned}
$$

For $t'\gg\tau$, the initial-condition term is negligible. The stationary [autocorrelation](../../../../../../autocorrelation.md) is therefore

$$
\boxed{\mathbb E[\widetilde\sigma(t)\widetilde\sigma(t')]\simeq\frac{\kappa\tau}{2}e^{-|t-t'|/\tau}.}
$$

Its normalized exponential decay has [correlation time](../../../../../../correlation-time.md) $\tau$. The [zero-start Ornstein-Uhlenbeck covariance](../../../../../../zero-start-ornstein-uhlenbeck-covariance.md) also shows how stationarity is approached.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
