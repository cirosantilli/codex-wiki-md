<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the standard linear [Gaussian](../../../../../normal-distribution.md) [state-space model](../../../../../state-space-model-time-series.md) convention: the initial state is independent of both mutually independent iid noise sequences. This [independence](../../../../../independent-random-variables.md) from the initial state is needed for the usual forecast recursion. Let $\mathcal Y_t=\sigma(y_1,\ldots,y_t)$ and write $m_{t-1}=x_{t-1}^{t-1}$ and $C_{t-1}=P_{t-1}^{t-1}$. Taking [conditional expectations](../../../../../conditional-expectation.md) in the state equation gives

$$
\boxed{x_t^{t-1}=\Phi m_{t-1},\qquad
P_t^{t-1}=\Phi C_{t-1}\Phi^\top+Q.}
$$

To justify the [covariance](../../../../../covariance.md), the forecast error is $\Phi(x_{t-1}-m_{t-1})+w_t$. Its two terms have zero cross-covariance because $w_t$ is independent of the previous state and observations. Their [covariances](../../../../../covariance.md) therefore add. In this [Gaussian](../../../../../normal-distribution.md) model the conditional error [covariance](../../../../../covariance.md) depends on the parameters and time but not on the realized data, so it also equals the unconditional forecast-error [covariance](../../../../../covariance.md) used in the notation of the question.

For completeness, derive the filtering step rather than leave the algorithm unspecified. Set $m_t^-=x_t^{t-1}$ and $C_t^-=P_t^{t-1}$. Conditionally on the previous data, the observation has mean $Am_t^-$ and [covariance](../../../../../covariance.md)

$$
\Sigma_t=AC_t^-A^\top+R.
$$

Define the [innovation process](../../../../../innovation-process.md) and gain by

$$
\epsilon_t=y_t-Am_t^-,\qquad K_t=C_t^-A^\top\Sigma_t^{-1}.
$$

The state forecast error and innovation are jointly normal, with cross-covariance $C_t^-A^\top$. The residual $x_t-m_t^- -K_t\epsilon_t$ is uncorrelated with $\epsilon_t$ by the definition of $K_t$, hence independent of it by joint normality. Its mean is zero and its [covariance](../../../../../covariance.md) is $C_t^- -C_t^-A^\top\Sigma_t^{-1}AC_t^-$. This proves the [conditional multivariate normal distribution](../../../../../conditional-multivariate-normal-distribution.md) update

$$
\boxed{x_t^t=m_t^-+K_t\epsilon_t,\qquad
P_t^t=C_t^- -C_t^-A^\top\Sigma_t^{-1}AC_t^-.}
$$

Initialize $x_0^0=\mu_0,P_0^0=\Sigma_0$. For $t=1,\ldots,n$, predict using the first boxed pair, store that forecast, form $\epsilon_t,\Sigma_t,K_t$, and update using the second boxed pair. The updated state then starts the next iteration. This is the [Kalman filter](../../../../../kalman-filter.md), and supplies the entire forecast sequence in one forward pass.

The requested unconditional innovation moments are

$$
\boxed{\mathbb E\epsilon_t=0,\qquad\operatorname{Var}(\epsilon_t)=\Sigma_t.}
$$

In fact $\epsilon_t\mid\mathcal Y_{t-1}\sim N_q(0,\Sigma_t)$, with $\Sigma_t$ deterministic for fixed parameters. Thus the innovation is independent of the past observations, and hence the innovations are mutually independent. Equivalently, orthogonality to the past together with joint normality gives this [independence](../../../../../independent-random-variables.md).

The chain rule for densities now yields the [Gaussian innovation likelihood](../../../../../gaussian-innovation-likelihood.md), treating the specified initial mean and [covariance](../../../../../covariance.md) as known:

$$
\boxed{L(\Theta)=\prod_{t=1}^n(2\pi)^{-q/2}|\Sigma_t|^{-1/2}
\exp\left(-\frac12\epsilon_t^\top\Sigma_t^{-1}\epsilon_t\right),}
$$



$$
\ell(\Theta)=-\frac{nq}{2}\log(2\pi)-\frac12\sum_{t=1}^n
\left[\log|\Sigma_t|+\epsilon_t^\top\Sigma_t^{-1}\epsilon_t\right].
$$

Both $\epsilon_t$ and $\Sigma_t$ are functions of the trial parameters, so the filtering recursion must be run again for each candidate $\Theta$. The ordinary density formula assumes $\Sigma_t$ positive definite; for example positive definite $R$ ensures this. Singular observation laws instead require densities on their [Gaussian](../../../../../normal-distribution.md) support.

Evaluate the [log-likelihood](../../../../../log-likelihood.md) numerically by the forward recursion, and maximize it over admissible $\Phi,A,Q,R$, enforcing the [covariance](../../../../../covariance.md) constraints. A [Cholesky decomposition](../../../../../cholesky-decomposition.md) $\Sigma_t=L_tL_t^\top$ gives $\log|\Sigma_t|=2\sum_j\log(L_t)_{jj}$ and the quadratic term $\|L_t^{-1}\epsilon_t\|^2$, avoiding an explicit matrix inverse. Covariance parameterizations or constrained optimization keep $Q,R$ positive semidefinite and the innovation [covariance](../../../../../covariance.md) nonsingular. An attained maximizer is a [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md); in general this is a numerical optimization problem and neither uniqueness nor global convergence of a local optimizer is automatic.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
