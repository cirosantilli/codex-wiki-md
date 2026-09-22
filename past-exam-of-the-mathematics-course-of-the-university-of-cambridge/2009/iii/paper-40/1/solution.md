<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $\theta_0=1$ and define the [autoregressive polynomial](../../../../../autoregressive-polynomial.md) and [moving-average polynomial](../../../../../moving-average-polynomial.md) by

$$
\Phi(z)=1-\sum_{k=1}^p\phi_kz^k,\qquad\Theta(z)=\sum_{k=0}^q\theta_kz^k.
$$

For a minimal, coprime [ARMA](../../../../../autoregressive-moving-average-model.md) representation, the usual simultaneous [causality and invertibility root criteria for an ARMA model](../../../../../causality-and-invertibility-root-criteria-for-an-arma-model.md) are

$$
\boxed{\Phi(z)\ne0\text{ and }\Theta(z)\ne0\quad\text{for all }|z|\le1.}
$$

The autoregressive condition makes $\Theta/\Phi$ a stable one-sided filter and gives the causal second-order [stationary process](../../../../../stationary-process.md). The moving-average condition makes its inverse a stable one-sided filter, so the [white noise](../../../../../white-noise.md) can be reconstructed from present and past observations. If the two polynomials have a common factor, first use [common factor cancellation in an ARMA model](../../../../../common-factor-cancellation-in-an-arma-model.md); necessary-and-sufficient root statements apply to the reduced noise-driven representation. Stationarity here is second-order stationarity; [weak white noise](../../../../../weak-white-noise.md) alone does not assert strict stationarity of all finite-dimensional laws.

For $p=1$, write $\phi=\phi_1$, so $|\phi|<1$. Expanding $(1-\phi z)^{-1}=\sum_{r\ge0}\phi^rz^r$ gives the [Wold representation](../../../../../wold-decomposition.md)

$$
X_t=\sum_{j\ge0}c_j\epsilon_{t-j},\qquad\boxed{c_j=\sum_{k=0}^{\min(j,q)}\theta_k\phi^{j-k}.}
$$

In particular $c_0=1$, $c_j=\phi c_{j-1}+\theta_j$ for $1\le j\le q$, and $c_j=\phi^{j-q}c_q$ for $j\ge q$. The coefficients are square-summable, so this series converges in mean square. Causality and invertibility identify the driver with the [linear innovation process](../../../../../linear-innovation-process.md), justifying the Wold terminology. For $\phi=0$, powers with exponent zero equal one and the formula reduces to the finite moving average.

To obtain the [covariance](../../../../../covariance.md) equations, subtract $\phi X_{t-1}$ and take [covariance](../../../../../covariance.md) with $X_{t-k}$. Orthogonality of the [white noise](../../../../../white-noise.md) and the causal expansion imply

$$
\operatorname{Cov}(\epsilon_{t-i},X_{t-k})=\begin{cases}\sigma^2c_{i-k},&i\ge k,\\0,&i<k.\end{cases}
$$

Thus the [innovation coefficients of an ARMA(1,q) process](../../../../../innovation-coefficients-of-an-arma-1-q-process.md) give the entire triangular system in one formula:

$$
\boxed{\gamma_k-\phi\gamma_{k-1}=\sigma^2\sum_{i=k}^q\theta_i c_{i-k}\quad(0\le k\le q),\qquad\gamma_k-\phi\gamma_{k-1}=0\quad(k>q).}
$$

At $k=0$, use $\gamma_{-1}=\gamma_1$, since the [autocovariance](../../../../../autocovariance.md) of a real [stationary process](../../../../../stationary-process.md) is symmetric. The terms are consequently $\sigma^2(c_0+\theta_1c_1+\cdots+\theta_qc_q)$ at zero, $\sigma^2\theta_qc_0$ at $q$, and the intervening partial sums as required.

For $q=1$, put $\theta=\theta_1$ and $c_1=\phi+\theta$. The equations become

$$
\gamma_0-\phi\gamma_1=\sigma^2(1+\theta\phi+\theta^2),\quad\gamma_1-\phi\gamma_0=\sigma^2\theta,\quad\gamma_k=\phi\gamma_{k-1}\ (k\ge2).
$$

Substitution of the second into the first, followed by the geometric recursion, yields the [autocovariance of a causal ARMA(1,1) process](../../../../../autocovariance-of-a-causal-arma-1-1-process.md):

$$
\boxed{\gamma_0=\frac{\sigma^2(1+\theta^2+2\phi\theta)}{1-\phi^2},\qquad\gamma_k=\frac{\sigma^2(\phi+\theta)(1+\phi\theta)}{1-\phi^2}\phi^{|k|-1}\quad(k\ne0).}
$$

This includes $\phi=0$: only lags $\pm1$ survive, as for an MA(1) process.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
