# Paper 47

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper47.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2006/Paper47.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Interpret the forecasts as [best linear prediction from a finite past](../../../time-series.md#best-linear-prediction-from-a-finite-past). For a causal [autoregressive process](../../../time-series.md#autoregressive-model), the innovations are orthogonal to previous observations. If they also have zero conditional mean given the past, the same forecasts are conditional means; [white noise](../../../time-series.md#white-noise) by itself guarantees only the linear-prediction interpretation.

Let $m$ be the process mean and write its centered autoregression as $X_t-m=\sum_{j=1}^p\phi_j(X_{t-j}-m)+\epsilon_t$. Set $\widehat X_{T,h}=X_{T+h}$ for $h\le0$, and recursively put

$$
\boxed{\widehat X_{T,k}=m+\sum_{j=1}^p\phi_j(\widehat X_{T,k-j}-m),\qquad k\ge1.}
$$

The forecast is a linear combination of the observed last $p$ values. Subtracting the recursion from the future autoregression shows that the prediction error is a linear combination of future innovations, hence orthogonal to every observed value. This proves the optimal projection property, rather than merely suggesting that future noise should be replaced by zero. In particular,

$$
\widehat X_{T,1}=m+\sum_{j=1}^p\phi_j(X_{T+1-j}-m),\qquad
\widehat X_{T,2}=m+\phi_1(\widehat X_{T,1}-m)+\sum_{j=2}^p\phi_j(X_{T+2-j}-m).
$$

The empty sum for $p=1$ is zero. Taking $m=0$ gives the centered convention. This is the [recursive forecasts of an autoregressive process](../../../time-series.md#recursive-forecasts-of-an-autoregressive-process) construction.

For the stable order-one equation, use its stationary causal solution

$$
X_t=\sum_{j=0}^{\infty}\phi^j\epsilon_{t-j}.
$$

The series converges in mean square because $\sum\phi^{2j}<\infty$ and the [white noise](../../../time-series.md#white-noise) innovations have a common finite [variance](../../../variance.md) $\sigma^2$. Orthogonality of their distinct time indices gives

$$
\mathbb EX_t=0,\qquad
\operatorname{Cov}(X_{t+h},X_t)=\frac{\sigma^2\phi^{|h|}}{1-\phi^2}.
$$

Adding the deterministic mean therefore yields [weak stationarity](../../../time-series.md#weakly-stationary-process) for $Z$, with

$$
\boxed{\mathbb EZ_t=\mu,\quad \gamma_Z(h)=\frac{\sigma^2\phi^{|h|}}{1-\phi^2},\quad \rho_Z(h)=\phi^{|h|}.}
$$

The [autocorrelation function](../../../time-series.md#autocorrelation) assumes $\sigma^2>0$; a zero-variance process has no normalized correlation. A recursion from an arbitrary nonstationary initial value would have transient moments, so the stationary-solution interpretation is important here.

Iteration gives $X_{T+k}=\phi^kX_T+\sum_{j=1}^k\phi^{k-j}\epsilon_{T+j}$. The innovation sum is orthogonal to the observed past, giving

$$
\boxed{\widehat Z_{T,k}=\mu+\phi^k(Z_T-\mu)\longrightarrow\mu.}
$$

For the integrated process, the [backshift operator](../../../time-series.md#backshift-operator) subtracts consecutive levels, so $(I-B)W_t=\mu+(I-B)Y_t=\mu+X_t=Z_t$. Consequently $W_{T+k}=W_T+\sum_{j=1}^kZ_{T+j}$. If the last increment is observed, substitute its forecast and sum the [geometric progression](../../../real-analysis.md#geometric-progression):

$$
\boxed{\widehat W_{T,k}=W_T+k\mu+
\frac{\phi(1-\phi^k)}{1-\phi}(W_T-W_{T-1}-\mu).}
$$

This is the [forecasts of an integrated AR(1) process](../../../time-series.md#forecasts-of-an-integrated-ar-1-process) formula. Its final term is bounded as $k\to\infty$, even for negative $\phi$, hence **the forecast's long-run slope is the drift**:

$$
\boxed{\widehat W_{T,k}/k\longrightarrow\mu.}
$$

With an initial level orthogonal to future innovations, the level formula is also the best linear forecast from the observed levels. Without that initial-level condition, it is the increment-based recursive forecast, and the levels could contain additional predictive information. The level formula uses $T\ge2$, or a known $W_0$ when $T=1$. With just $W_1$ and no model for the initial level, the last increment cannot be recovered from the supplied observations; a one-observation level forecast would need that additional information.

## 2

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a [weakly stationary process](../../../time-series.md#weakly-stationary-process) with mean $m$, the [autocovariance function](../../../time-series.md#autocovariance) is $\gamma_k=\mathbb E[(X_{t+k}-m)(X_t-m)]$, independent of $t$. The positive definiteness of these covariances gives a unique finite positive [spectral measure of a stationary time series](../../../time-series.md#spectral-measure-of-a-stationary-time-series) on the frequency circle. Its cumulative function is the [time-series spectral distribution](../../../time-series.md#spectral-distribution-function-of-a-stationary-time-series) $F$, with total mass $\gamma_0$, and

$$
\boxed{\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}\,dF(\lambda).}
$$

Use one representative of the identified endpoints $-\pi$ and $\pi$ when specifying atoms. For a real-valued process the measure is symmetric, so the imaginary part integrates to zero. If it has a [time-series spectral density](../../../time-series.md#spectral-density-of-a-stationary-process), then

$$
\boxed{\gamma_k=\int_{-\pi}^{\pi}e^{ik\lambda}f(\lambda)d\lambda,\qquad
f(\lambda)=\frac1{2\pi}\sum_{k\in\mathbb Z}\gamma_k e^{-ik\lambda}.}
$$

The second identity is pointwise for an absolutely summable [covariance](../../../variance.md#covariance) sequence, as will apply to part (a). Existence of a density alone does not guarantee ordinary pointwise convergence of its [Fourier series](../../../fourier-series.md); in general the reconstruction can be interpreted by its [Cesaro means](../../../real-analysis.md#cesaro-mean) in $L^1$. This fixes the frequency normalization for all three calculations below.

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Only overlapping innovations contribute to the [autocovariance function](../../../time-series.md#autocovariance) of the [moving-average process](../../../time-series.md#moving-average-model). Set $c_0=1,c_1=\theta_1,c_2=\theta_2$. The overlap formula is $\gamma_k=\sigma^2\sum_jc_jc_{j+|k|}$, with coefficients outside $0,1,2$ set to zero. Thus

$$
\boxed{\gamma_k=\begin{cases}
\sigma^2(1+\theta_1^2+\theta_2^2),&k=0,\\
\sigma^2\theta_1(1+\theta_2),&|k|=1,\\
\sigma^2\theta_2,&|k|=2,\\
0,&|k|>2.
\end{cases}}
$$

The [time-series spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) is the Fourier sum of this finite [covariance](../../../variance.md#covariance) sequence:

$$
\boxed{f(\lambda)=\frac{\sigma^2}{2\pi}\left[1+\theta_1^2+\theta_2^2+
2\theta_1(1+\theta_2)\cos\lambda+2\theta_2\cos2\lambda\right].}
$$

It also equals $\sigma^2|1+\theta_1e^{-i\lambda}+\theta_2e^{-2i\lambda}|^2/(2\pi)$, which directly verifies nonnegativity. Integrating from $-\pi$ gives the requested [time-series spectral distribution](../../../time-series.md#spectral-distribution-function-of-a-stationary-time-series):

$$
\boxed{F(\lambda)=\frac{\sigma^2}{2\pi}\left[(1+\theta_1^2+\theta_2^2)(\lambda+\pi)
+2\theta_1(1+\theta_2)\sin\lambda+\theta_2\sin2\lambda\right],\quad -\pi\le\lambda\le\pi.}
$$

Extend it by zero below $-\pi$ and by $\gamma_0$ above $\pi$. In particular its total mass is the process [variance](../../../variance.md), not necessarily one.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The even [time-series spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) makes the sine part vanish. At lag zero its integral is the area of the triangle, so $\gamma_0=\pi^2$. For any nonzero integer $k$, integration by parts gives

$$
\begin{aligned}
\gamma_k&=2\int_0^\pi(\pi-\lambda)\cos(k\lambda)d\lambda\\
&=\frac2k\int_0^\pi\sin(k\lambda)d\lambda
=\frac{2(1-\cos k\pi)}{k^2}.
\end{aligned}
$$

Therefore the [triangular spectral density of a stationary time series](../../../time-series.md#triangular-spectral-density-of-a-stationary-time-series) has [autocovariance function](../../../time-series.md#autocovariance)

$$
\boxed{\gamma_k=\begin{cases}\pi^2,&k=0,\\4/k^2,&k\text{ odd},\\0,&k\ne0\text{ even}.\end{cases}}
$$

No additional factor $1/(2\pi)$ belongs in this inverse integral under the convention stated above.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The zero means of both amplitudes give $\mathbb EX_t=0$. Their unit variances and zero [covariance](../../../variance.md#covariance) give, for arbitrary integer $s,t$,

$$
\mathbb E[X_sX_t]=\cos(\omega_0s)\cos(\omega_0t)+\sin(\omega_0s)\sin(\omega_0t)
=\cos(\omega_0(s-t)).
$$

Thus the [variance](../../../variance.md) is one and the [covariance](../../../variance.md#covariance) depends only on lag, proving [weak stationarity](../../../time-series.md#weakly-stationary-process). Independence or normality of the amplitudes is unnecessary. Since

$$
\cos(\omega_0k)=\tfrac12e^{ik\omega_0}+\tfrac12e^{-ik\omega_0},
$$

the [spectral measure of a random harmonic oscillation](../../../time-series.md#spectral-measure-of-a-random-harmonic-oscillation) assigns mass $1/2$ to each of $-\omega_0,\omega_0$. The corresponding right-continuous [time-series spectral distribution](../../../time-series.md#spectral-distribution-function-of-a-stationary-time-series) is

$$
\boxed{F(\lambda)=\begin{cases}0,&\lambda<-\omega_0,\\1/2,&-\omega_0\le\lambda<\omega_0,\\1,&\lambda\ge\omega_0.\end{cases}}
$$

These spectral atoms represent a persistent oscillation. There is no ordinary absolutely continuous spectral density for this process.

## 3

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For [rejection sampling](../../../probability-and-statistics.md#rejection-sampling), independently generate a proposal $Y$ with density $g$ and a uniform $U$ on $(0,1)$. Accept $Y$ if $U\le f(Y)/(Mg(Y))$; otherwise generate a fresh independent pair and repeat. Set the ratio to zero on $g=0$ where necessarily $f=0$. The envelope condition makes the acceptance threshold at most one.

For any measurable set $A$, a single attempt satisfies

$$
\mathbb P(Y\in A,\text{ accepted})=\int_Ag(y)\frac{f(y)}{Mg(y)}dy
=\frac1M\int_Af(y)dy.
$$

Taking the whole space shows that acceptance has probability $1/M$. Conditioning on acceptance therefore gives density $f$. Repeating rejected independent attempts preserves that conditional law and terminates almost surely; the number of attempts is geometric with mean $M$.

For fixed proposal density, admissibility requires $M\ge\sup_{g(x)>0}f(x)/g(x)$ under the pointwise convention in the question. Since $1/M$ decreases with $M$, **the smallest valid envelope gives the greatest acceptance probability**:

$$
\boxed{M_* =\sup_{g(x)>0}\frac{f(x)}{g(x)},\qquad p_{\mathrm{acc}}=1/M_*.}
$$

For densities specified only almost everywhere, replace the supremum by the essential supremum. Integration of the envelope also gives $M\ge1$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Use the uniform proposal on $[1,7]$, with density $g=1/6$. The [triangular distribution](../../../continuous-probability-distribution.md#triangular-distribution) peaks at $x=3$ with height $1/3$, so the optimal constant for this proposal is $M=2$. At each attempt take two fresh pseudo-random uniforms $U,V$, and propose $Y=1+6U$. The [rejection method](../../../probability-and-statistics.md#rejection-sampling) accepts according to

$$
\boxed{V\le\begin{cases}(Y-1)/2,&1\le Y\le3,\\(7-Y)/4,&3<Y\le7.\end{cases}}
$$

Indeed these bounds are $f(Y)/(2g(Y))=3f(Y)$. Part (a) proves that the accepted value has the required density. Acceptance probability is $1/2$, so the method needs two proposal attempts on average, and hence four uniforms on average if each attempt uses two. The validity of the ideal algorithm presumes independent uniform draws; merely belonging to $[0,1]$ does not by itself make a pseudo-random sequence uniform or independent.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Integrating the two linear pieces gives the [cumulative distribution function](../../../probability-theory.md#cumulative-distribution-function)

$$
F(x)=\begin{cases}
0,&x<1,\\(x-1)^2/12,&1\le x\le3,\\1-(7-x)^2/24,&3\le x\le7,\\1,&x>7.
\end{cases}
$$

The split probability is $F(3)=1/3$. Invert each branch to obtain the [method of inversion](../../../probability-theory.md#inverse-transform-sampling):

$$
\boxed{X=\begin{cases}1+\sqrt{12U},&0\le U\le1/3,\\7-\sqrt{24(1-U)},&1/3<U\le1.\end{cases}}
$$

Both expressions equal three at the split. For an ideal uniform draw, monotonicity gives $\mathbb P(F^{-1}(U)\le x)=\mathbb P(U\le F(x))=F(x)$, proving the target law. **Inversion is preferable here**: its quantile is explicit, it uses one uniform and one square root per output, and has no rejected draws. Rejection remains useful for densities with no convenient inverse CDF.

## 4

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The nonparametric [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) replaces the unknown sampling law by the [empirical distribution](../../../information-theory.md#type-information-theory)

$$
\widehat F_n(x)=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i\le x\}}.
$$

Generate $B$ independent [bootstrap samples](../../../statistical-modelling.md#bootstrap-sample), each containing $n$ independent draws with replacement from that law. Recompute the original estimator in each sample, obtaining $\widehat\theta_1^*,\ldots,\widehat\theta_B^*$. With $\overline\theta^*=B^{-1}\sum_b\widehat\theta_b^*$, the [bootstrap standard error](../../../statistical-modelling.md#bootstrap-standard-error) estimate is

$$
\boxed{\widehat{\operatorname{se}}_*(\widehat\theta)
=\left[\frac1{B-1}\sum_{b=1}^B(\widehat\theta_b^*-\overline\theta^*)^2\right]^{1/2}.}
$$

This estimates the conditional [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) standard deviation, which approximates the estimator's sampling standard deviation when the [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) is consistent. Dividing this expression by $\sqrt B$ would instead estimate the Monte Carlo error in the [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) mean, a different quantity.

For distinct original observations, each resample is an ordered index sequence with one of $n^n$ equally likely values. It contains no repeats precisely when it is a permutation of all $n$ original indices, giving $n!$ possibilities. Hence

$$
\boxed{\mathbb P_*(\text{at least one repeated observation})=1-\frac{n!}{n^n}.}
$$

The distinctness assumption is needed to equate repeated values with repeated indices.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Calculate the observed [sample correlation coefficient](../../../variance.md#sample-correlation-coefficient) $\widehat r$. In each [paired bootstrap](../../../statistical-modelling.md#paired-bootstrap), draw 100 indices independently with replacement from $1,\ldots,100$ and select the corresponding whole pairs. Compute the [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) correlation $r_b^*$ from each resample; do not resample the two margins independently, since that would destroy their empirical dependence.

Let $q_p$ be the empirical $p$-quantile of those [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) correlations. The [percentile bootstrap confidence interval](../../../statistical-modelling.md#percentile-bootstrap-confidence-interval) is

$$
\boxed{[q_{0.025},q_{0.975}].}
$$

This is the requested algorithmic interval; the actual endpoints require the observed pairs. Its coverage is approximate, based on the sampling law of the correlation being well approximated by the [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) law. Both sample variances must be positive. Resamples having a constant margin have undefined correlation and cannot be repaired by arbitrarily assigning correlation zero. One may regenerate these exceptional resamples, explicitly conditioning on well-defined correlations; under the usual nondegenerate large-sample conditions their probability is negligible. Frequent degeneracy instead indicates that this ordinary correlation-bootstrap construction is unsuitable.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For a [bootstrap-t confidence interval](../../../statistical-modelling.md#bootstrap-t-confidence-interval), estimate the original [standard error](../../../statistical-inference.md#standard-error) $\widehat s$ of $\widehat r$, for example by the standard deviation of the outer [paired bootstrap](../../../statistical-modelling.md#paired-bootstrap) correlations. For each outer resample $b$, estimate its own [standard error](../../../statistical-inference.md#standard-error) $s_b^*$ by drawing many inner paired resamples from that outer sample and taking the standard deviation of their correlations. The resulting studentized statistics are

$$
T_b^*=\frac{r_b^*-\widehat r}{s_b^*}.
$$

Let $t_p^*$ be their empirical quantiles. Approximating the distribution of $(\widehat r-r)/\widehat s$ by that of $T^*$ and solving the two inequalities for $r$ gives

$$
\boxed{[\widehat r-t_{0.975}^*\widehat s,\ \widehat r-t_{0.025}^*\widehat s].}
$$

The reversal of quantiles is essential. The pivot requires positive [standard errors](../../../statistical-inference.md#standard-error) and nondegenerate correlations; its claimed 95% coverage is an approximation under [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) regularity, not an exact finite-sample guarantee. One may intersect the final interval with the parameter space $[-1,1]$.

The same percentile and studentized procedures can be applied to the [sample mean](../../../variance.md#sample-mean) of $X$, and then only the $X$ observations need be resampled. They are useful when a normal approximation is doubtful. However the mean already has the simple standard-error estimate $S_X/10$ here. For normal observations, the classical exact interval is

$$
\boxed{\overline X\pm t_{99,0.975}\frac{S_X}{10},}
$$

and the same form is an asymptotic approximation for independent finite-variance observations under appropriate large-sample conditions. Thus [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) intervals are valid alternatives, but are often unnecessary for a mean with a reliable classical pivot; the correlation has no corresponding distribution-free elementary pivot. An infinite-variance distribution would require other theory rather than this ordinary standard-error argument.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

A [control variate](../../../probability-and-statistics.md#control-variates) is a random variable $C$ correlated with the estimator and with known mean $c_0$. For a fixed real coefficient $a$, define $Y_a=Y-a(C-c_0)$. Then $\mathbb EY_a=\theta$, while

$$
\operatorname{Var}(Y_a)=\operatorname{Var}(Y)-2a\operatorname{Cov}(Y,C)+a^2\operatorname{Var}(C).
$$

Assuming finite second moments and positive control [variance](../../../variance.md), complete the square to find

$$
\boxed{a_* =\frac{\operatorname{Cov}(Y,C)}{\operatorname{Var}(C)},\qquad
\min_a\operatorname{Var}(Y_a)=\operatorname{Var}(Y)-\frac{\operatorname{Cov}(Y,C)^2}{\operatorname{Var}(C)}.}
$$

When $\operatorname{Var}(Y)>0$, the minimum is $\operatorname{Var}(Y)(1-\rho_{Y,C}^2)$. A constant control cannot reduce [variance](../../../variance.md). A strongly correlated control, including a negatively correlated one with a negative coefficient, can substantially reduce it.

For [multivariate control variates](../../../probability-and-statistics.md#multivariate-control-variates), write $Y_\beta=Y-\beta^T(C-\mathbb EC)$, $\Sigma=\operatorname{Cov}(C)$ and $c=\operatorname{Cov}(C,Y)$. Completing the multivariate square gives

$$
\boxed{\beta_* =\Sigma^{-1}c,\qquad
\min_\beta\operatorname{Var}(Y_\beta)=\operatorname{Var}(Y)-c^T\Sigma^{-1}c.}
$$

If $\Sigma$ is singular, use its [Moore-Penrose inverse](../../../linear-algebra.md#moore-penrose-inverse). Indeed any null direction has a constant centered control combination and therefore zero [covariance](../../../variance.md#covariance) with $Y$, so $c$ lies in the range of $\Sigma$. The elementary unbiasedness statement assumes a deterministic coefficient; estimating it from the same simulation may introduce finite-sample bias, whereas an independently trained coefficient keeps the conditional unbiasedness argument valid.

## 5

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

For the [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm), start at a state $\theta$ with positive target density, propose $\theta'$ from $q(\theta'\mid\theta)$, and generate an independent uniform draw. Accept the proposal with probability

$$
\boxed{\alpha(\theta,\theta')=\min\left\{1,
\frac{\pi(\theta')q(\theta\mid\theta')}{\pi(\theta)q(\theta'\mid\theta)}\right\}.}
$$

On rejection retain $\theta$, including repeated states in the chain; removing repeats would generally change its stationary law. The accepted-flow density satisfies

$$
\pi(\theta)q(\theta'\mid\theta)\alpha(\theta,\theta')
=\min\{\pi(\theta)q(\theta'\mid\theta),\pi(\theta')q(\theta\mid\theta')\},
$$

which is symmetric in its two states. This proves [detailed balance](../../../markov-process.md#detailed-balance) and hence invariance of the target distribution, including the holding probabilities on the diagonal. Unknown common normalization constants cancel in the ratio. Invariance alone does not establish convergence from arbitrary initial states. Choosing proposals that yield a [positive Harris recurrent Markov chain](../../../markov-process.md#positive-harris-recurrent-markov-chain) with [aperiodicity](../../../markov-process.md#aperiodic-markov-chain) supplies the usual convergence guarantee, and the resulting sample is dependent. Use burn-in and account for autocorrelation when assessing Monte Carlo precision.

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

A [random-walk update](../../../statistical-inference.md#random-walk-metropolis-algorithm) proposes $\theta'=\theta+\eta$, with an increment distribution independent of the current state. If its density is symmetric, $q(\theta'\mid\theta)=q(\theta\mid\theta')$, reducing the [Metropolis–Hastings acceptance probability](../../../statistical-inference.md#metropolis-hastings-acceptance-probability) to $\min\{1,\pi(\theta')/\pi(\theta)\}$. For nonsymmetric increments the proposal-density ratio must remain.

Such updates need little global knowledge of the target and adapt naturally to its local scale. Their limitation is a tuning tradeoff: very small increments accept often but move slowly, while very large increments are often rejected. They can also have difficulty moving between distant modes. Covariance-scaled increments help with anisotropic targets, but the chain still explores through local steps.

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

An [independence sampler](../../../statistical-inference.md#independence-metropolis-hastings-algorithm) proposes from a fixed density $g(\theta')$, independent of the current state. Its acceptance probability is

$$
\boxed{\alpha(\theta,\theta')=\min\left\{1,
\frac{\pi(\theta')g(\theta)}{\pi(\theta)g(\theta')}\right\}.}
$$

If $g$ is close to the target, proposals can make large efficient moves and cross separated modes; $g=\pi$ gives acceptance one and independent samples. On the other hand, a good global approximation is required. A proposal with tails too light can leave the chain trapped at states having very large importance weight $\pi/g$, since most outgoing proposals then have tiny acceptance probabilities.

For perspective, if the normalized target satisfies $\pi\le Mg$, the accepted transition density is at least $\pi(\theta')/M$, because both entries in $\min\{g(\theta'),\pi(\theta')/w(\theta)\}$ have that lower bound, where $w=\pi/g\le M$. This yields a uniform refresh component. Thus a well-designed independence proposal can mix rapidly, whereas a poor global proposal can be much worse than a locally tuned random walk. The tradeoff concerns effective samples per computation, not acceptance rate alone.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

Let $v=\sigma^2>0$, $d_k=k+1$, and $S_k(a)=\|y-X_ka\|^2$. Under the standard interpretation that the two stated priors are independent, multiply the normal likelihood by the normal coefficient prior and the [inverse-gamma distribution](../../../continuous-probability-distribution.md#inverse-gamma-distribution) density. The [independent normal and inverse-gamma regression priors](../../../linear-regression.md#independent-normal-and-inverse-gamma-regression-priors) give

$$
\boxed{\pi(a_k,v\mid x,y)\propto
v^{-(\alpha+1+n/2)}
\exp\left[-\frac{\beta+S_k(a_k)/2}{v}
-\frac12(a_k-\mu_k)^T\Sigma_k^{-1}(a_k-\mu_k)\right],\quad v>0.}
$$

For a fixed model the determinant and Gaussian normalizing constants are independent of $a_k,v$ and may be omitted here; $\Sigma_k$ is assumed [positive-definite](../../../linear-algebra.md#positive-definite-bilinear-form). The coefficient prior is not scaled by $v$, so replacing its precision by $\Sigma_k^{-1}/v$ would describe a different prior.

For an additional check, completing the coefficient square and reading the [variance](../../../variance.md) kernel give the full conditional distributions

$$
a_k\mid v,x,y\sim N(m_k,V_k),\quad
V_k=(X_k^TX_k/v+\Sigma_k^{-1})^{-1},\quad
m_k=V_k(X_k^Ty/v+\Sigma_k^{-1}\mu_k),
$$

and

$$
v\mid a_k,x,y\sim\operatorname{InvGamma}(\alpha+n/2,\beta+S_k(a_k)/2).
$$

Marginal priors alone would not determine their joint prior without the independence assumption. The front-page inverse-gamma mean has a typographical error: this density has mean $\beta/(\alpha-1)$ when $\alpha>1$, not a denominator $\alpha+1$. The density itself, used in the posterior calculation, fixes the correct parameterization.

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

The cross-model target must include a model-order prior $\rho_k$. Write its joint, unnormalized density as

$$
t_k(a,v)=\rho_k\,p(y\mid a,v,k)\,p(a\mid k)\,p(v\mid k).
$$

Here the prior densities are normalized within each model. In particular their $k$-dependent determinants and powers of $2\pi$ cannot be dropped merely because the fixed-model posterior in part (i) was given up to proportionality.

For explicit [birth and death moves for Bayesian variable selection](../../../statistical-inference.md#birth-and-death-moves-for-bayesian-variable-selection), choose a birth with probability $b_k$, generate $u$ from a density $g_k(u\mid a,v)$, append $u$ as the new covariate coefficient, and leave $v$ unchanged. The map from $(a,v,u)$ to $(a',v')=((a,u),v)$ is invertible under the reverse deletion and has absolute Jacobian one. It matches dimensions: the smaller-model coefficients and [variance](../../../variance.md) have dimension $k+2$, and the one auxiliary draw supplies the larger-model dimension $k+3$. If the reverse death is selected with probability $d_{k+1}$, accept with

$$
\boxed{\alpha_b=\min\left\{1,
\frac{t_{k+1}((a,u),v)d_{k+1}}
{t_k(a,v)b_k g_k(u\mid a,v)}\right\}.}
$$

For a death, delete the last coefficient $u$, retain the others and the [variance](../../../variance.md), and use

$$
\boxed{\alpha_d=\min\left\{1,
\frac{t_k(a,v)b_k g_k(u\mid a,v)}
{t_{k+1}((a,u),v)d_{k+1}}\right\}.}
$$

To verify [detailed balance](../../../markov-process.md#detailed-balance), multiply the birth acceptance by $t_kb_kg_k$ and the reverse death acceptance by $t_{k+1}d_{k+1}$. Both equal the minimum of these two quantities in the matched coordinates. This proves reversibility without merely naming a dimension-changing algorithm. A more general bijection introduces its absolute Jacobian, and random choices among several covariates introduce the corresponding forward and reverse selection probabilities. Add within-model updates so that coefficients and [variance](../../../variance.md) can explore each model. These are [reversible-jump Markov chain Monte Carlo](../../../statistical-inference.md#reversible-jump-markov-chain-monte-carlo) updates; the unspecified model prior and proposal density must be supplied to implement them numerically.

## 6

↑ **Parent:** [Paper 47](paper-47.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

First distinguish a complete-data calculation, conditional on the missing counts, from optimization of the observed-data likelihood. Introduce death counts $D_j=\sum_{i=1}^jn_{ij}$, survivor counts $S_j=A_{1j}$, observed recapture counts $C_j=\sum_{i=1}^{j-1}m_{ij}$ and unobserved-alive counts $U_j=A_{2j}$. Terms involving these probabilities in the complete-data log likelihood are

$$
\ell=\sum_{j=1}^{J-1}[D_j\log(1-\phi_j)+S_j\log\phi_j]
+\sum_{j=2}^J[C_j\log P_j+U_j\log(1-P_j)]+\text{constant}.
$$

The survival score is $S_j/\phi_j-D_j/(1-\phi_j)$ and the detection score is $C_j/P_j-U_j/(1-P_j)$. Their derivatives are nonpositive, and strictly negative whenever their respective total counts are positive. The interior roots, with boundary interpretations if a success or failure count vanishes, are therefore

$$
\boxed{\widehat\phi_j=\frac{S_j}{S_j+D_j},\qquad
\widehat P_j=\frac{C_j}{C_j+U_j}.}
$$

Substituting the survivor and unobserved-alive totals gives

$$
\widehat\phi_j=
\frac{\sum_{i=1}^j\sum_{s=j+1}^J(m_{is}+n_{is})}
{\sum_{i=1}^j(\sum_{s=j+1}^Jm_{is}+\sum_{s=j}^Jn_{is})},
\quad
\widehat P_j=
\frac{\sum_{i=1}^{j-1}m_{ij}}
{\sum_{i=1}^{j-1}\sum_{s=j}^J(m_{is}+n_{is})}.
$$

These are the requested complete-data maximizing ratios. Here $n_{iJ}$ denotes the terminal missing count discussed in part (b); pre-release cells and nonexistent release cohorts contribute zero. If a denominator is zero, the likelihood is constant in that parameter rather than defining a $0/0$ estimate. Also $P_1$ does not occur in this likelihood and has no identified maximum. With unobserved $n$, these ratios alone do not yet supply an observed-data estimate; the [EM algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) below supplies the missing-count expectations.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

The consistent missing-data interpretation is that each never-recaptured individual either dies in an interval $j<J$ or survives unobserved through the final occasion. Define the known never-recaptured total and its allocation by

$$
N_i=R_i-\sum_{s=i+1}^Jm_{is},\qquad
\sum_{j=i}^{J-1}n_{ij}+n_{iJ}=N_i.
$$

The terminal cell $n_{iJ}$ is the source's separately named $n_i$. The printed identity equating that cell to the total observed recaptures is inconsistent with the supplied multinomial law. In particular, with no observed recaptures its printed value would be zero even though the terminal-cell probability is positive at interior parameters. The displayed accounting identity repairs that notation and makes all sums through $J$ well-defined.

For an individual released at $i$, define the unnormalized probabilities

$$
w_{ij}=(1-\phi_j)\prod_{\ell=i}^{j-1}\phi_\ell(1-P_{\ell+1})\quad(i\le j<J),\qquad
w_{iJ}=\prod_{\ell=i}^{J-1}\phi_\ell(1-P_{\ell+1}).
$$

The empty product is one. Each intermediate factor means surviving an interval and avoiding its subsequent detection; the death weight additionally includes failure to survive interval $j$. Let $K_i=\sum_{j=i}^Jw_{ij}$. This is the probability of never being recaptured. It is the source's normalizing constant $C_i$, renamed to avoid confusion with the detection-success counts above. Conditional on no recapture, division by $K_i$ gives precisely the supplied [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution) cell probabilities.

Initialize an interior parameter vector $(\phi^{(0)},P^{(0)})$. At iteration $r$, the E step of [missing-count EM for capture-recapture](../../../statistical-modelling.md#missing-count-em-for-capture-recapture) computes, for every cohort and missing cell,

$$
\boxed{\overline n_{ij}^{(r)}
=\mathbb E[n_{ij}\mid m,\phi^{(r)},P^{(r)}]
=N_i\frac{w_{ij}(\phi^{(r)},P^{(r)})}{K_i(\phi^{(r)},P^{(r)})},\quad i\le j\le J.}
$$

If $N_i=0$, set every missing count to zero without dividing, even if $K_i=0$. If $N_i>0$ and $K_i=0$, that parameter vector gives zero probability to the observations and cannot be used in the E step. These expected counts sum to $N_i$, preserving each cohort's observed accounting. The E step is [conditional expectation](../../../measure-theory.md#conditional-expectation), not replacement by the modal missing counts or a single random imputation.

The expected complete-data log likelihood is linear in the missing counts, apart from count-only terms irrelevant to the new parameter values. In the M step substitute these expectations into the success/failure ratios from part (a):

$$
\boxed{\phi_j^{(r+1)}=
\frac{\sum_{i=1}^j\sum_{s=j+1}^J(m_{is}+\overline n_{is}^{(r)})}
{\sum_{i=1}^j(\sum_{s=j+1}^Jm_{is}+\sum_{s=j}^J\overline n_{is}^{(r)})},}
$$

and

$$
\boxed{P_j^{(r+1)}=
\frac{\sum_{i=1}^{j-1}m_{ij}}
{\sum_{i=1}^{j-1}\sum_{s=j}^J(m_{is}+\overline n_{is}^{(r)})}.}
$$

If an exposure denominator vanishes, retain any admissible value of the unidentifiable parameter. Repeat until the observed likelihood and parameter updates stabilize. The conditional normalizers in the E step are evaluated at the old parameters; maximizing a newly normalized conditional missing-data distribution instead of the expected complete-data log likelihood would be the wrong M step.

One can monitor the observed likelihood directly. The probability of a first recapture at $s>i$ is

$$
p_{is}=\left[\prod_{\ell=i}^{s-2}\phi_\ell(1-P_{\ell+1})\right]\phi_{s-1}P_s,
$$

and successive death, detection and continuation alternatives partition the possibilities, giving $K_i+\sum_{s=i+1}^Jp_{is}=1$. Thus, up to count-only factors,

$$
L_{\mathrm{obs}}\propto\prod_i K_i^{N_i}\prod_{s=i+1}^Jp_{is}^{m_{is}}.
$$

The usual conditional Jensen argument for the [EM algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) makes this likelihood nondecreasing at each exact M step. It does not guarantee a unique global maximum. In this observation scheme the final survival and detection probabilities enter through the product $\phi_{J-1}P_J$ only, so these two probabilities cannot generally be estimated separately without a further constraint. The algorithm remains valid, but may converge to different points on the same likelihood ridge.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

With complete counts fixed, the likelihood factor for $P_j$ is $P_j^{C_j}(1-P_j)^{U_j}$. As a function of $P_j\in(0,1)$, normalize it to the density of a [Beta distribution](../../../probability-theory.md#beta-distribution) with parameters $C_j+1,U_j+1$. Normalization does not change its maximizing argument. The standard beta-mode formula, when both counts are positive, gives

$$
\boxed{\widehat P_j=\frac{(C_j+1)-1}{(C_j+1)+(U_j+1)-2}
=\frac{C_j}{C_j+U_j}.}
$$

This uses the standard distribution result without differentiating the likelihood, and introducing the normalized beta kernel does not require adopting a Bayesian prior. If only $C_j$ is zero the maximum is at zero; if only $U_j$ is zero it is at one; if both vanish every probability maximizes the constant factor. For the EM M step the same beta-mode argument applies to the expected, possibly noninteger counts, since positive real beta parameters are allowed.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2006](../../2006.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
