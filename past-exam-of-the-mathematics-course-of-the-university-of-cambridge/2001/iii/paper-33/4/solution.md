<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For the [three-coordinate state realization of an ARMA(1,1) process](../../../../../three-coordinate-state-realization-of-an-arma-1-1-process.md), the observation row and transition [matrix](../../../../../matrix.md) are

$$
\boxed{F=(\phi,1,\theta),\qquad
G=\begin{pmatrix}\phi&1&\theta\\0&0&0\\0&1&0\end{pmatrix}.}
$$

The first row of $GS_{t-1}$ is $x_{t-1}$ by the previous-time recursion; the second row is zero until the new [white noise](../../../../../white-noise.md) value is added; and the third row copies $\varepsilon_{t-1}$. Hence the state equation has noise [covariance](../../../../../covariance.md)

$$
Q=\operatorname{Cov}(w_t)
=\begin{pmatrix}0&0&0\\0&\sigma^2&0\\0&0&0\end{pmatrix}.
$$

We use the causal state model, in which the new driving noise is independent of the previous state. The [Gaussian filtering with exact observations](../../../../../gaussian-filtering-with-exact-observations.md) form of the [Kalman filter](../../../../../kalman-filter.md) alternates prediction through the state equation with conditioning on the next observation. Given the posterior [expected value](../../../../../expected-value.md) and [covariance](../../../../../covariance.md) at time $t-1$, [independence](../../../../../independent-random-variables.md) of the new [white noise](../../../../../white-noise.md) value gives predictive [expected value](../../../../../expected-value.md) $a_t=G\widehat S_{t-1}$ and predictive [covariance](../../../../../covariance.md)

$$
R_t=GP_{t-1}G^\top+Q.
$$

Project through the observation row to get

$$
\widehat x_t=Fa_t,\qquad
\boxed{V_t=FR_tF^\top=FGP_{t-1}G^\top F^\top+\sigma^2.}
$$

The residual $v_t=x_t-\widehat x_t$ is the [innovation](../../../../../innovation-process.md). Conditioning the joint [Gaussian](../../../../../normal-distribution.md) state-observation vector adjusts the [expected value](../../../../../expected-value.md) according to this residual and reduces the [covariance](../../../../../covariance.md). In this exact-observation model, the updates can be written

$$
K_t=\frac{R_tF^\top}{V_t},\qquad
\widehat S_t=a_t+K_tv_t,\qquad
P_t=R_t-\frac{R_tF^\top FR_t}{V_t}.
$$

Thus $F\widehat S_t=x_t$ and $FP_tF^\top=0$: the observed [linear combination](../../../../../linear-combination.md) of the state is now known exactly, though other state combinations remain uncertain.

The PDF's stated prediction [variance](../../../../../variance-split.md) omits $FQF^\top=\sigma^2$. This omission cannot be used in a valid [likelihood](../../../../../likelihood-function.md): for the AR(1) specialization below it would give zero prediction [variance](../../../../../variance-split.md) after the first observation. The required [likelihood](../../../../../likelihood-function.md) calculation uses the corrected [innovation](../../../../../innovation-process.md) [variance](../../../../../variance-split.md) just derived.

For [stationary initialization of an ARMA(1,1) state](../../../../../stationary-initialization-of-an-arma-1-1-state.md) with $|\phi|<1$, take $\widehat S_0=0$ and the unconditional stationary [covariance](../../../../../covariance.md). The causal coefficients are $1$ at lag zero and $(\phi+\theta)\phi^{j-1}$ at lags $j\geq1$, giving

$$
\gamma_0=\operatorname{Var}(x_t)
=\sigma^2\left[1+\frac{(\phi+\theta)^2}{1-\phi^2}\right]
=\frac{\sigma^2(1+\theta^2+2\phi\theta)}{1-\phi^2}.
$$

Since $S_0=(x_{-1},\varepsilon_0,\varepsilon_{-1})^\top$, the cross-covariance with $\varepsilon_0$ is zero and that with $\varepsilon_{-1}$ is $\sigma^2$. Therefore

$$
\boxed{P_0=
\begin{pmatrix}
\gamma_0&0&\sigma^2\\
0&\sigma^2&0\\
\sigma^2&0&\sigma^2
\end{pmatrix}.}
$$

Direct substitution verifies $P_0=GP_0G^\top+Q$. If prior state information is available, instead use its conditional [expected value](../../../../../expected-value.md) and [covariance](../../../../../covariance.md). A diffuse initialization is another option when the initial state is genuinely unknown, but it changes the finite-sample [likelihood](../../../../../likelihood-function.md) and should not silently replace the stationary initial law.

By the [Gaussian](../../../../../normal-distribution.md) prediction step,

$$
x_t\mid x_1,\ldots,x_{t-1}\sim N(\widehat x_t,V_t).
$$

The [chain rule for probabilities](../../../../../chain-rule-for-probabilities.md) for the joint [probability density function](../../../../../probability-density-function.md) therefore gives

$$
L(\phi,\theta,\sigma^2)
=\prod_{t=1}^T(2\pi V_t)^{-1/2}
\exp\!\left[-\frac{(x_t-\widehat x_t)^2}{2V_t}\right].
$$

Taking minus twice its logarithm shows that **[maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) is equivalent to minimizing**

$$
\boxed{\sum_{t=1}^T\left[\log(2\pi)+\log V_t+
\frac{(x_t-\widehat x_t)^2}{V_t}\right],}
$$

with each $V_t$ and $\widehat x_t$ evaluated at the candidate parameters and the specified initialization. The corrected $+\sigma^2$ is essential in every $V_t$.

For the stationary causal AR(1) case, $\theta=0$ and $|\phi|<1$. The first observation is $N(0,\sigma^2/(1-\phi^2))$, whereas each later conditional observation is $\phi x_{t-1}+\varepsilon_t$. Hence

$$
\boxed{V_1=\frac{\sigma^2}{1-\phi^2},
\qquad V_t=\sigma^2\quad(2\leq t\leq T).}
$$

This also gives a direct counterexample to the uncorrected PDF [variance](../../../../../variance-split.md): with $\theta=0$, $FG=\phi F$ and $FP_{t-1}F^\top=0$ after observing $x_{t-1}$, so its printed expression would give $V_t=0$ for $t\geq2$.

To compare the [conditional and stationary AR1 likelihood estimators](../../../../../conditional-and-stationary-ar1-likelihood-estimators.md), put

$$
Q_T(\phi)=(1-\phi^2)x_1^2+
\sum_{t=2}^T(x_t-\phi x_{t-1})^2.
$$

Then its negative twice log-likelihood is

$$
T\log(2\pi)+T\log\sigma^2-\log(1-\phi^2)+
\frac{Q_T(\phi)}{\sigma^2}.
$$

For fixed $\phi$, $\widehat{\sigma^2}=Q_T(\phi)/T$. Writing

$$
C_T=\sum_{t=2}^Tx_{t-1}^2,\qquad
D_T=\sum_{t=2}^Tx_tx_{t-1},
$$

the exact interior score equation is

$$
0=\frac{\phi}{1-\phi^2}+
\frac{\phi(C_T-x_1^2)-D_T}{\sigma^2}.
$$

The stationary initial contribution is order one for a fixed interior parameter, while $C_T$ is order $T$. Discarding this lower-order contribution gives

$$
\boxed{\widehat\phi\approx
\frac{D_T}{C_T}
=\frac{\sum_{t=2}^Tx_tx_{t-1}}{\sum_{t=2}^Tx_{t-1}^2}.}
$$

Conditioning on $x_1$ makes this ratio the exact unconstrained [conditional maximum likelihood](../../../../../conditional-maximum-likelihood.md) estimate. Under the stationary initial law it is only the leading approximation: at an interior optimum,

$$
\widehat\phi-\frac{D_T}{C_T}
=\frac{\widehat\phi}{C_T}
\left(x_1^2-\frac{\widehat{\sigma^2}}{1-\widehat\phi^2}\right)
=O_{\mathbb P}(T^{-1}).
$$

This approximation presumes a nondegenerate sample denominator and a true coefficient fixed away from the unit-root boundary; a finite-sample constrained optimum must respect $|\phi|<1$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
