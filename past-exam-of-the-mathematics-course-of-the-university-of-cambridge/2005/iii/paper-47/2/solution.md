<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\Phi(z)=1-\phi_1z-\cdots-\phi_pz^p$. The [causality root criterion for an autoregressive model](../../../../../causality-root-criterion-for-an-autoregressive-model.md),

$$
\boxed{\Phi(z)\ne0\quad\text{for }|z|\leq1,}
$$

is a sufficient condition for a [weakly stationary process](../../../../../weakly-stationary-process.md) solution, and gives the causal solution $X_t=\sum_{j\geq0}\psi_j\varepsilon_{t-j}$. Indeed $1/\Phi$ is analytic in a disk of radius greater than one, so its Taylor coefficients $\psi_j$ decay geometrically. The series therefore has [mean-square convergence](../../../../../convergence-in-l2.md) and defines a [linear filter of a stationary time series](../../../../../linear-filter-of-a-stationary-time-series.md); multiplying by $\Phi$ verifies the equation.

For the specified order-two model, put $\varphi=(1+\sqrt5)/2$. Since $\varphi-\varphi^{-1}=1$,

$$
\Phi(z)=1-\alpha z-\alpha^2z^2
=(1-\alpha\varphi z)(1+\alpha z/\varphi).
$$

When $\alpha\ne0$, its roots are $1/(\alpha\varphi)$ and $-\varphi/\alpha$. Both have modulus greater than one exactly when $|\alpha|<1/\varphi$. The case $\alpha=0$ is [white noise](../../../../../white-noise.md) and satisfies the same inequality. Consequently

$$
\boxed{\alpha_0=\frac{\sqrt5-1}{2},\qquad|\alpha|<\alpha_0.}
$$

This is the causal [stationarity](../../../../../stationary-process.md) condition selected above. Without causality, a two-sided [autoregressive model](../../../../../autoregressive-model.md) can also have a [noncausal stationary autoregression](../../../../../noncausal-stationary-autoregression.md) when its [polynomial](../../../../../polynomial-split.md) has no unit-circle zeros. Thus the inequality is not a necessary condition for all conceivable [weak stationarity](../../../../../weakly-stationary-process.md) solutions; the causal interpretation is the one required by the subsequent innovations and forecasting questions.

To find the [Wold representation](../../../../../wold-decomposition.md), expand $1/\Phi(z)=\sum_{j\geq0}\psi_jz^j$. Matching coefficients gives $\psi_0=1$, $\psi_1=\alpha$ and $\psi_j=\alpha\psi_{j-1}+\alpha^2\psi_{j-2}$. Hence

$$
\boxed{X_t=\sum_{j=0}^{\infty}F_{j+1}\alpha^j\varepsilon_{t-j},\qquad
F_{j+1}=\frac{\varphi^{j+1}-(-1/\varphi)^{j+1}}{\sqrt5}.}
$$

Here $F_1=F_2=1$ are the [Fibonacci numbers](../../../../../fibonacci-number.md). The coefficient formula also follows by partial fractions in the displayed factorization. Absolute summability follows from $|\alpha\varphi|<1$ and $|\alpha/\varphi|<1$. The past observation span equals the past noise span, because the causal series gives one inclusion and $\varepsilon_t=X_t-\alpha X_{t-1}-\alpha^2X_{t-2}$ gives the reverse inclusion. Thus these noises are the [linear innovations](../../../../../linear-innovation-process.md), and there is no additional deterministic component. This is the [Fibonacci-coefficient autoregression](../../../../../fibonacci-coefficient-autoregression.md).

The [best linear prediction from an infinite past](../../../../../best-linear-prediction-from-an-infinite-past.md) is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the closed span of $X_T,X_{T-1},\ldots$. Future [white noise](../../../../../white-noise.md) is orthogonal to that span. Substitution in the recursion therefore gives

$$
\boxed{\widehat X_{T+1}=\alpha X_T+\alpha^2X_{T-1},\qquad
\widehat X_{T+2}=2\alpha^2X_T+\alpha^3X_{T-1}.}
$$

The respective errors are $\varepsilon_{T+1}$ and $\alpha\varepsilon_{T+1}+\varepsilon_{T+2}$, so their [mean squared errors](../../../../../mean-squared-error.md) are $\sigma^2$ and $(1+\alpha^2)\sigma^2$. No [normal distribution](../../../../../normal-distribution.md) assumption is needed for these linear forecasts.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 47](../../paper-47-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
