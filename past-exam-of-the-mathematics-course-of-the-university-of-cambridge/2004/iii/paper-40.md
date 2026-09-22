# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2004/Paper40.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)
  - [iv](#4/iv)
    - [Solution](#4/iv/solution)
  - [v](#4/v)
    - [Solution](#4/v/solution)
  - [vi](#4/vi)
    - [Solution](#4/vi/solution)
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
  - [iv](#5/iv)
    - [Solution](#5/iv/solution)
  - [v](#5/v)
    - [Solution](#5/v/solution)
  - [vi](#5/vi)
    - [Solution](#5/vi/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
  - [iv](#6/iv)
    - [Solution](#6/iv/solution)

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For a [weakly stationary process](../../../time-series.md#weakly-stationary-process) with [mean](../../../probability-theory.md#expected-value) $m$ and nonzero [variance](../../../variance.md), put $\gamma(h)=\operatorname{Cov}(X_{t+h},X_t)$ and $\rho(h)=\gamma(h)/\gamma(0)$. The function $\rho$ is its [autocorrelation function](../../../time-series.md#autocorrelation). For observations $x_1,\ldots,x_N$, one common [sample autocorrelation function](../../../time-series.md#sample-autocorrelation-function) is

$$
\widehat\gamma(h)=\frac1N\sum_{t=1}^{N-h}(x_t-\overline x)(x_{t+h}-\overline x),
\qquad \widehat\rho(h)=\frac{\widehat\gamma(h)}{\widehat\gamma(0)}.
$$

A [correlogram](../../../time-series.md#correlogram) plots these estimates against lag; the population analogue plots $\rho(h)$.

The lag-$h$ [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) measures the [correlation](../../../variance.md#pearson-correlation-coefficient) between $X_t$ and $X_{t-h}$ after removing their [linear projections](../../../vector-space.md#projection-linear-algebra) on the intervening observations. Its sample counterpart can be calculated by the [Yule-Walker equations](../../../time-series.md#yule-walker-equations): solve

$$
\widehat R_h\widehat\phi_h=\widehat r_h,
\qquad (\widehat R_h)_{ij}=\widehat\rho(|i-j|),
\qquad (\widehat r_h)_i=\widehat\rho(i),
$$

and take $\widehat\alpha(h)=\widehat\phi_{h,h}$, assuming the matrix is nonsingular. This defines a standard [sample partial autocorrelation function](../../../time-series.md#sample-partial-autocorrelation-function).

For a minimal causal [autoregressive model](../../../time-series.md#autoregressive-model) of order $p$, the [autocorrelation](../../../time-series.md#autocorrelation) typically decays geometrically, possibly with damped oscillations, whereas the [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) is zero beyond lag $p$: after those $p$ preceding values have been projected out, the innovation is orthogonal to older values. For a [moving-average model](../../../time-series.md#moving-average-model) of order $q$, nonoverlapping sets of driving [white noise](../../../time-series.md#white-noise) give $\gamma(h)=0$ for $|h|>q$; its [partial autocorrelation function](../../../time-series.md#partial-autocorrelation-function) generally tails off when the representation is invertible. Thus **an ACF cutoff suggests an MA order; a PACF cutoff suggests an AR order**. An [ARMA](../../../time-series.md#autoregressive-moving-average-model) model generally has neither cutoff. These are population properties; sample noise makes cutoffs approximate, so fitted residuals and uncertainty should also be inspected. Under [independent](../../../random-variable.md#independent-random-variables) [white noise](../../../time-series.md#white-noise), fixed-lag sample [correlations](../../../variance.md#pearson-correlation-coefficient) have approximate standard error $N^{-1/2}$, giving a rough diagnostic band rather than a universal simultaneous test.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For a discrete-time [weakly stationary process](../../../time-series.md#weakly-stationary-process), the [spectral density of a stationary process](../../../time-series.md#spectral-density-of-a-stationary-process), when it exists, is a nonnegative function satisfying

$$
\gamma(h)=\int_{-\pi}^{\pi}e^{ih\omega}f_X(\omega)\,d\omega.
$$

If $\sum_h|\gamma(h)|<\infty$, then

$$
f_X(\omega)=\frac1{2\pi}\sum_{h\in\mathbb Z}\gamma(h)e^{-ih\omega}.
$$

A general second-order stationary process has a [spectral measure of a stationary time series](../../../time-series.md#spectral-measure-of-a-stationary-time-series), which need not have a [spectral density](../../../time-series.md#spectral-density-of-a-stationary-process): a centered random constant has an atom at zero. Thus the [spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) calculation below assumes that $f_X$ exists; the corresponding measure identity holds without that extra assumption.

Absolute summability of the filter coefficients gives [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) because

$$
\left\|\sum_{s\in E}a_sX_{t-s}\right\|_2
\leq\|X_0\|_2\sum_{s\in E}|a_s|.
$$

Consequently the bilateral filtered process is well defined, with constant [mean](../../../probability-theory.md#expected-value) $m\sum_sa_s$. Its [covariance](../../../variance.md#covariance) is

$$
\gamma_Y(h)=\sum_{r,s\in\mathbb Z}a_ra_s\gamma_X(h-r+s).
$$

The sum is absolutely convergent, since $|\gamma_X(j)|\leq\gamma_X(0)$ and $\sum|a_s|<\infty$. It depends only on lag, proving [weak stationarity](../../../time-series.md#weakly-stationary-process) of $Y$.

Insert the spectral representation and interchange summation and integration using absolute summability and the finite total spectral mass. For real coefficients,

$$
\begin{aligned}
\gamma_Y(h)
&=\int_{-\pi}^{\pi}e^{ih\omega}
\left(\sum_ra_re^{-ir\omega}\right)
\left(\sum_sa_se^{is\omega}\right)f_X(\omega)\,d\omega\\
&=\int_{-\pi}^{\pi}e^{ih\omega}|A(e^{i\omega})|^2f_X(\omega)\,d\omega.
\end{aligned}
$$

Therefore the [spectral density transformation under a linear filter](../../../time-series.md#spectral-density-transformation-under-a-linear-filter) is

$$
\boxed{f_Y(\omega)=|A(e^{i\omega})|^2f_X(\omega).}
$$

For a bilateral sequence, $A$ is guaranteed to converge on the unit circle. Its negative powers need not converge inside the disk: for example, $a_{-j}=2^{-j}$ makes the series diverge at $z=1/4$. Only the unit-circle values are used here, so the unnecessarily broad domain printed for $A$ does not affect the proof.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Center the five coefficients at lags $-2,-1,0,1,2$. Their transfer function is real:

$$
H(\omega)=\frac{-e^{-2i\omega}+2e^{-i\omega}+4+2e^{i\omega}-e^{2i\omega}}6
=\frac{4+4\cos\omega-2\cos(2\omega)}6.
$$

Choosing consecutive causal lags instead only adds a phase and leaves the squared modulus unchanged. After $k$ applications, the [white noise](../../../time-series.md#white-noise) [spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) has become

$$
\boxed{f_k(\omega)=\frac{\sigma^2}{2\pi}|H(\omega)|^{2k}.}
$$

Write $c=\cos\omega$. Completing the square gives

$$
H(\omega)=1+\frac23c-\frac23c^2
=\frac76-\frac23(c-\tfrac12)^2.
$$

For $-1\leq c\leq1$, its range is $[-1/3,7/6]$, and its absolute maximum is $7/6$, attained exactly when $c=1/2$. Consequently, on the conventional nonnegative frequency range $[0,\pi]$,

$$
\boxed{\frac{f_k(\omega)}{f_k(\pi/3)}
=\left(\frac{|H(\omega)|}{7/6}\right)^{2k}\longrightarrow0
\quad\text{for }\omega\ne\pi/3.}
$$

On the two-sided range $[-\pi,\pi]$ there is also a peak at $-\pi/3$; the ratio there is one for every $k$. This is a counterexample to the claim if read literally on a signed frequency domain. The correct two-sided exclusion is $\omega\ne\pm\pi/3$.

The result illustrates how [repeated symmetric filtering can amplify an oscillation](../../../time-series.md#repeated-symmetric-filtering-can-amplify-an-oscillation). Although $H(0)=1$ preserves a constant component, $H(\pi/3)=7/6>1$ amplifies period-six oscillations. Repetition selects an increasingly narrow frequency band around those peaks; it does not simply smooth all noise away. In fact the unnormalized output [variance](../../../variance.md) eventually grows without bound, since a fixed interval around either peak has $|H|>1$.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Difference the [local-level state-space model](../../../time-series.md#local-level-state-space-model) to eliminate its latent level:

$$
D_t=X_t-X_{t-1}=w_t+v_t-v_{t-1}.
$$

[Independence](../../../random-variable.md#independent-random-variables) and Gaussianity give a stationary Gaussian process with

$$
\gamma_D(0)=W+2V,
\qquad\gamma_D(1)=\gamma_D(-1)=-V,
\qquad\gamma_D(h)=0\quad(|h|>1).
$$

For $V,W>0$, let

$$
q=\frac{W+2V+\sqrt{W^2+4WV}}2,
\qquad\vartheta=-\frac Vq\in(-1,0).
$$

These satisfy $q(1+\vartheta^2)=W+2V$ and $q\vartheta=-V$. Therefore $D$ has the [covariance](../../../variance.md#covariance) of the [moving-average model](../../../time-series.md#moving-average-model) $\varepsilon_t+\vartheta\varepsilon_{t-1}$, where $\varepsilon$ is Gaussian [white noise](../../../time-series.md#white-noise) of [variance](../../../variance.md) $q$. This is an actual representation, not just [covariance](../../../variance.md#covariance) matching: define $\varepsilon_t=\sum_{j\geq0}(-\vartheta)^jD_{t-j}$. The convergent inverse filter has constant [spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) $q/(2\pi)$, so its Gaussian coordinates are [independent](../../../random-variable.md#independent-random-variables), and multiplication by $1+\vartheta B$ recovers $D$.

Thus

$$
\boxed{(1-B)X_t=(1+\vartheta B)\varepsilon_t,
\qquad \operatorname{Var}(\varepsilon_t)=q.}
$$

This is the formal [ARMA](../../../time-series.md#autoregressive-moving-average-model) equation with autoregressive coefficient one. Its unit root [means](../../../probability-theory.md#expected-value) that the levels are generally not stationary: if the initial state has finite [variance](../../../variance.md) and is [independent](../../../random-variable.md#independent-random-variables) of future noises, $\operatorname{Var}(S_t)=\operatorname{Var}(S_0)+tW$. In stationary-model terminology the correct classification is [ARIMA](../../../time-series.md#autoregressive-integrated-moving-average)(0,1,1). The requested ARMA description must therefore allow a unit-root equation.

When $V=0$, the differences are just $w_t$; when $W=0$ and $V>0$, they are $v_t-v_{t-1}$, a noninvertible MA(1) with coefficient $-1$. If both [variances](../../../variance.md) vanish, the model is deterministic apart from a possible initial random level. These limits explain the qualifications on the invertible representation above.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Conditionally on past observations, adding the [independent](../../../random-variable.md#independent-random-variables) state increment gives the prediction

$$
S_t\mid\mathcal F_{t-1}\sim N(\widehat S_{t-1},R_t),
\qquad R_t=P_{t-1}+W.
$$

The new observation then has [conditional distribution](../../../probability-theory.md#conditional-distribution) $N(\widehat S_{t-1},R_t+V)$, and its conditional [covariance](../../../variance.md#covariance) with $S_t$ is $R_t$. Equivalently, multiplying the state prediction [probability density function](../../../continuous-probability-distribution.md#probability-density-function) by the observation [likelihood](../../../statistical-modelling.md#likelihood-function) and completing the square gives

$$
\frac1{P_t}=\frac1{R_t}+\frac1V,
\qquad
\frac{\widehat S_t}{P_t}=\frac{\widehat S_{t-1}}{R_t}+\frac{X_t}V.
$$

For positive [variances](../../../variance.md), rearrangement yields the [scalar Gaussian Kalman recursion](../../../control-theory.md#scalar-gaussian-kalman-recursion)

$$
\boxed{K_t=\frac{P_{t-1}+W}{P_{t-1}+W+V},\quad
\widehat S_t=\widehat S_{t-1}+K_t(X_t-\widehat S_{t-1}),\quad
P_t=\frac{V(P_{t-1}+W)}{P_{t-1}+W+V}.}
$$

Here the innovation is the observation minus its predicted [mean](../../../probability-theory.md#expected-value). The displayed [covariance](../../../variance.md#covariance) formula also handles zero [variances](../../../variance.md) whenever its denominator is nonzero; a completely deterministic prediction and observation require no probabilistic update. [Independence](../../../random-variable.md#independent-random-variables) of the new noises from the past and the initial state is the usual state-space assumption needed for this conditional calculation.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A constant posterior [variance](../../../variance.md) must be a fixed point of the recursion in part (b). Multiplying $P=V(P+W)/(P+W+V)$ by its positive denominator gives

$$
\boxed{P^2+PW=WV.}
$$

Conversely, if a nonnegative $P$ solves this equation and the filter is initialized with $P_0=P$, the recursion preserves $P_t=P$ at every step. The fixed-point equation alone does not force an arbitrary initial [covariance](../../../variance.md#covariance) to be constant.

For $W,V>0$, the admissible root and its [steady-state local-level Kalman gain](../../../control-theory.md#steady-state-local-level-kalman-gain) are

$$
P=\frac{\sqrt{W^2+4WV}-W}2,
\qquad K=\frac{P+W}{P+W+V}=\frac PV\in(0,1).
$$

The state estimate then obeys [exponential smoothing](../../../time-series.md#exponential-smoothing):

$$
\boxed{\widehat S_t=KX_t+(1-K)\widehat S_{t-1}.}
$$

Iteration makes the weights explicit:

$$
\widehat S_t=(1-K)^t\widehat S_0
+K\sum_{j=0}^{t-1}(1-K)^jX_{t-j}.
$$

Thus older observations receive geometrically decreasing weights. Consistently with part (a), the innovations [variance](../../../variance.md) is $q=P+W+V$ and the differenced MA coefficient is $\vartheta=-(1-K)$. The degeneracies $W=0,P=0$ and $V=0,P=0$ give gain zero and gain one respectively when the denominator is positive.

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Treat the supplied uniform variates as [independent](../../../random-variable.md#independent-random-variables) $U(0,1)$ draws, as required for Monte Carlo simulation. Use $n$ of them and return

$$
\boxed{X=\sum_{j=1}^n\mathbf1_{\{U_j\leq p\}}.}
$$

Each indicator has a [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) of parameter $p$, and the indicators are [independent](../../../random-variable.md#independent-random-variables). For any subset of $r$ successes the [probability](../../../probability-theory.md#probability) is $p^r(1-p)^{n-r}$; there are $\binom nr$ such subsets. Thus $\mathbb P(X=r)=\binom nrp^r(1-p)^{n-r}$, the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution). The construction includes the cases $p=0,1$ and $n=0$.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

For rate $\lambda>0$, return

$$
\boxed{X=-\frac1\lambda\log U_1.}
$$

For $x\geq0$, $\mathbb P(X>x)=\mathbb P(U_1<e^{-\lambda x})=e^{-\lambda x}$, so $X$ has the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\lambda$. This is [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling); using $-\log(1-U_1)/\lambda$ is equivalent. Uniform draws at exact endpoints can be excluded, since those events have [probability](../../../probability-theory.md#probability) zero under the ideal continuous law.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Use [uniform-envelope rejection sampling for a beta distribution](../../../probability-and-statistics.md#uniform-envelope-rejection-sampling-for-a-beta-distribution). Put $r(x)=x^{a-1}(1-x)^{b-1}$ for $0<x<1$ and choose $M=\sup r$. For $a,b>1$, [differentiation](../../../calculus.md#differentiation) of $\log r$ gives the mode $(a-1)/(a+b-2)$, so

$$
M=\left(\frac{a-1}{a+b-2}\right)^{a-1}
\left(\frac{b-1}{a+b-2}\right)^{b-1}.
$$

If $a=1$ or $b=1$, take $M=1$; this also covers $a=b=1$. Draw $X=U_{2j-1}$ and accept it if

$$
\boxed{U_{2j}\leq\frac{r(X)}M.}
$$

Otherwise continue with the next [independent](../../../random-variable.md#independent-random-variables) pair. The [probability](../../../probability-theory.md#probability) of acceptance is $\int_0^1r(x)\,dx/M=B(a,b)/M>0$, so the procedure terminates almost surely. Conditional on acceptance, the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is proportional to $r(x)$, hence is exactly the [Beta distribution](../../../probability-theory.md#beta-distribution) of parameters $a,b$. The restriction $a,b\geq1$ guarantees the bounded uniform envelope.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

For $\sigma>0$, use the unnormalized normal shape $h(x)=e^{-x^2/(2\sigma^2)}$. The [ratio-of-uniforms method](../../../probability-and-statistics.md#ratio-of-uniforms-method) samples uniformly from

$$
\mathcal A=\{(u,v):0<u<1,\ u^2\leq h(v/u)\}.
$$

Its boundary is $|v|\leq2\sigma u\sqrt{-\log u}$. The largest possible $|v|$ occurs at $u=e^{-1/2}$ and equals $b=\sigma\sqrt{2/e}$, giving the [normal ratio-of-uniforms envelope](../../../probability-and-statistics.md#normal-ratio-of-uniforms-envelope) $0<u<1$, $-b<v<b$.

Use [independent](../../../random-variable.md#independent-random-variables) uniform pairs to propose $u=U_{2j-1}$ and $v=b(2U_{2j}-1)$. Accept precisely when

$$
\boxed{v^2\leq-4\sigma^2u^2\log u,\qquad\text{then return }X=v/u.}
$$

To verify its distribution, change coordinates from $(u,v)$ to $(u,x)$, with $v=ux$ and [Jacobian determinant](../../../calculus.md#jacobian-determinant) $u$. The accepted point is uniform on $\mathcal A$, and the marginal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) of $x$ is proportional to

$$
\int_0^{\sqrt{h(x)}}u\,du=\frac12h(x).
$$

Thus the result is $N(0,\sigma^2)$. The region has positive finite area $\sigma\sqrt{\pi/2}$, and the acceptance [probability](../../../probability-theory.md#probability) is $\sqrt{\pi e}/4$. The case $\sigma=0$ requires simply returning zero.

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Assume the draws are [independent](../../../random-variable.md#independent-random-variables) from $g$, that the target-weighted integrand is covered by its support, and that $\int|\theta(x)|f(x)\,dx<\infty$. Define the [importance weight](../../../probability-and-statistics.md#importance-weight) $w(x)=f(x)/g(x)$. The change-of-density identity is

$$
\mathbb E_g[w(X)\theta(X)]=\int\frac{f(x)}{g(x)}\theta(x)g(x)\,dx
=\int\theta(x)f(x)\,dx=\mu.
$$

Therefore [importance sampling](../../../probability-and-statistics.md#importance-sampling) uses the unbiased estimator

$$
\boxed{\widehat\mu_g=\frac1n\sum_{i=1}^nw(x_i)\theta(x_i).}
$$

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) gives consistency. A finite [second moment](../../../probability-theory.md#second-moment) of the weighted integrand additionally gives finite [variance](../../../variance.md) and a usual independent-sample [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem). A useful proposal places enough [probability](../../../probability-theory.md#probability) where $f|\theta|$ is large and avoids tiny proposal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) there; common support alone does not guarantee finite [variance](../../../variance.md).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Write $f=f_0/C_f$ and $g=g_0/C_g$, where $f_0,g_0$ are known nonnegative kernels. If both constants are known, the ordinary weight is $(C_g/C_f)f_0/g_0$. If their ratio is unknown, use [self-normalized importance sampling](../../../probability-and-statistics.md#self-normalized-importance-sampling):

$$
\boxed{\widehat\mu_{\mathrm{SN}}
=\frac{\sum_i\theta(x_i)f_0(x_i)/g_0(x_i)}{\sum_i f_0(x_i)/g_0(x_i)}.}
$$

Indeed, under the normalized proposal law,

$$
\mathbb E_g\!\left[\frac{f_0(X)}{g_0(X)}\theta(X)\right]
=\frac{C_f}{C_g}\mu,
\qquad
\mathbb E_g\!\left[\frac{f_0(X)}{g_0(X)}\right]=\frac{C_f}{C_g}.
$$

The [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) makes their empirical ratio converge to $\mu$, provided the numerator is absolutely [integrable](../../../measure-theory.md#integrability) and $0<C_f,C_g<\infty$. Multiplicative constants cancel, whether the unknown one belongs to the target, proposal, or both. Unlike the estimator in part (i), this ratio is generally biased at finite sample size. Exact sampling from $g$ is still presumed; knowing only an unnormalized proposal does not itself supply a sampler.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Set $H_i=f(x_i)\theta(x_i)/g(x_i)$. [Independence](../../../random-variable.md#independent-random-variables) gives $\operatorname{Var}(n^{-1}\sum_iH_i)=\operatorname{Var}(H_1)/n$, while part (i) gives $\mathbb E_gH_1=\mu$. Its [second moment](../../../probability-theory.md#second-moment) is

$$
\mathbb E_gH_1^2=\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx.
$$

Consequently

$$
\boxed{\operatorname{Var}(\widehat\mu_g)
=\frac1n\int\frac{f(x)^2\theta(x)^2}{g(x)}\,dx-\frac{\mu^2}n.}
$$

The [variance](../../../variance.md) is finite exactly when the displayed second-moment [integral](../../../calculus.md#integral) is finite, assuming $\mu$ exists. An infinite [integral](../../../calculus.md#integral) [means](../../../probability-theory.md#expected-value) infinite [variance](../../../variance.md), not failure of the change-of-density identity.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

For the standard [Cauchy distribution](../../../probability-theory.md#cauchy-distribution) tail, use the indicator

$$
\boxed{\theta(x)=\mathbf1_{\{x\geq k\}}.}
$$

Then $\int\theta(x)f(x)\,dx$ is the desired [probability](../../../probability-theory.md#probability), and the ordinary [importance sampling](../../../probability-and-statistics.md#importance-sampling) estimator is $n^{-1}\sum_i f(x_i)\mathbf1_{\{x_i\geq k\}}/g(x_i)$. The proposal must cover the nonzero integrand, namely the upper tail. A proposal restricted to $[0,k]$ cannot directly estimate this indicator [integral](../../../calculus.md#integral); part (v) instead uses a complementary bounded-interval identity.

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Take $k>0$, so the proposal is the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,k]$, with [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $g(x)=1/k$. Symmetry of the standard [Cauchy distribution](../../../probability-theory.md#cauchy-distribution) gives

$$
\mu=\frac12-\int_0^kf(x)\,dx
=\frac12-k\mathbb E_g[f(X)].
$$

Thus the proposed expression is exactly the unbiased [importance sampling](../../../probability-and-statistics.md#importance-sampling) estimator of this complementary [integral](../../../calculus.md#integral):

$$
\boxed{\widehat\mu=\frac12-\frac{k}{n}\sum_{i=1}^n\frac1{\pi(1+x_i^2)}.}
$$

It has finite [variance](../../../variance.md) because $f$ is bounded on $[0,k]$. Explicitly,

$$
\begin{aligned}
\mathbb E_gf(X)&=\frac{\arctan k}{\pi k},\\
\mathbb E_gf(X)^2&=\frac1{2\pi^2k}\left(\arctan k+\frac{k}{1+k^2}\right),\\
\operatorname{Var}(\widehat\mu)
&=\frac1{n\pi^2}\left[\frac{k}{2}\left(\arctan k+\frac{k}{1+k^2}\right)-(\arctan k)^2\right].
\end{aligned}
$$

These follow from the antiderivatives of $(1+x^2)^{-1}$ and $(1+x^2)^{-2}$. The target itself is $\mu=1/2-\arctan(k)/\pi$. At $k=0$ it is exactly $1/2$ without simulation; for negative $k$ the printed uniform-interval construction must be changed.

<h3 id="4/vi">vi</h3>

↑ **Parent:** [4](#4)

<h4 id="4/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#4/vi)

[Antithetic variates](../../../probability-and-statistics.md#antithetic-variates) preserve each draw's marginal law but couple two estimates negatively. For an average of identically distributed $H,H'$,

$$
\operatorname{Var}\left(\frac{H+H'}2\right)
=\frac12\left(\operatorname{Var}(H)+\operatorname{Cov}(H,H')\right).
$$

Negative [covariance](../../../variance.md#covariance) improves on two [independent](../../../random-variable.md#independent-random-variables) evaluations at the same computational budget.

Here generate [independent](../../../random-variable.md#independent-random-variables) $U_1,\ldots,U_r\sim U(0,1)$ and pair $x_j=kU_j$ with $x_j'=k(1-U_j)$. Both are uniform on $[0,k]$. The [antithetic Cauchy-tail integration on a finite interval](../../../probability-and-statistics.md#antithetic-cauchy-tail-integration-on-a-finite-interval) estimator is

$$
\boxed{\widehat\mu_A=\frac12-\frac{k}{2r}\sum_{j=1}^r
\left[f(kU_j)+f(k(1-U_j))\right].}
$$

It is unbiased. Put $h(u)=f(ku)$. This decreases, whereas $h(1-u)$ increases. For an [independent](../../../random-variable.md#independent-random-variables) copy $U'$ of $U$, the [covariance](../../../variance.md#covariance) identity gives

$$
\operatorname{Cov}(h(U),h(1-U))
=\frac12\mathbb E[(h(U)-h(U'))(h(1-U)-h(1-U'))]\leq0.
$$

Each product is nonpositive, and for $k>0$ it is strictly negative off the diagonal. Therefore

$$
\operatorname{Var}(\widehat\mu_A)
=\frac{k^2}{2r}\left[\operatorname{Var}(h(U))+
\operatorname{Cov}(h(U),h(1-U))\right]
<\frac{k^2}{2r}\operatorname{Var}(h(U)),
$$

which is the [variance](../../../variance.md) using $2r$ [independent](../../../random-variable.md#independent-random-variables) evaluations in part (v). Thus the comparison accounts for the doubled number of [probability density function](../../../continuous-probability-distribution.md#probability-density-function) evaluations in each pair.

## 5

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

The linear predictor is unchanged by $\alpha_j\mapsto\alpha_j+c$, $\beta_t\mapsto\beta_t+d$, $\mu\mapsto\mu-c-d$. Without constraints, different parameter triples therefore give the same rates and [likelihood](../../../statistical-modelling.md#likelihood-function). [Identifiability](../../../statistical-model.md#identifiability) requires choosing one representative of this redundancy.

Taking the first levels as reference yields $\alpha_1=\beta_1=0$. Then

$$
\mu=\log\lambda_{11},\qquad
\alpha_2=\log\lambda_{21}-\log\lambda_{11},\qquad
\beta_2=\log\lambda_{12}-\log\lambda_{11}.
$$

These identify all three free parameters, while $\lambda_{22}=\lambda_{21}\lambda_{12}/\lambda_{11}$ is the model's no-interaction constraint. **The zero reference effects fix a parametrization; they do not remove the baseline rate or impose equal rates across groups.**

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Use the standard interpretation that the counts are conditionally [independent](../../../random-variable.md#independent-random-variables) given the parameters, with mutually [independent](../../../random-variable.md#independent-random-variables) stated priors. Let $a_2=\alpha_2$, $b_2=\beta_2$, and define

$$
T=\sum_{i,j,t}x_{ijt},\qquad
R=\sum_{i,t}x_{i2t},\qquad
C=\sum_{i,j}x_{ij2},\qquad
E=I(1+e^{a_2})(1+e^{b_2}).
$$

Under the reference constraints, the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) [likelihood](../../../statistical-modelling.md#likelihood-function), up to data-only factors, is

$$
L(\theta,a_2,b_2)=\theta^T\exp\{Ra_2+Cb_2-\theta E\}.
$$

Multiplying by the shape-rate gamma prior gives the [Poisson-gamma conjugacy with unequal exposures](../../../statistical-inference.md#poisson-gamma-conjugacy-with-unequal-exposures)

$$
\boxed{\theta\mid a_2,b_2,\mathbf x
\sim\Gamma(a+T,b+I(1+e^{a_2})(1+e^{b_2})).}
$$

Here $b$ is a rate, matching the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) convention on the PDF's first page. The factor $I$ represents the number of replicates per cell, not the total count.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

An exact [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) update is available despite the non-Gaussian intercept: draw $\theta'$ from the conditional [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) law in part (ii), then set

$$
\boxed{\mu'=\log\theta'.}
$$

Together with conditional updates of the two remaining effects, this targets the required joint posterior in the log-intercept coordinates. The [log-gamma prior for a Poisson log-intercept](../../../statistical-inference.md#log-gamma-prior-for-a-poisson-log-intercept) includes the change-of-variable factor: with $d\theta/d\mu=e^\mu$,

$$
\pi(\mu\mid a_2,b_2,\mathbf x)
\propto\exp\{(a+T)\mu-(b+E)e^\mu\}.
$$

Using $(a+T-1)\mu$ instead would omit the Jacobian and give the wrong conditional law for $\mu$.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

The full conditional log [probability density functions](../../../continuous-probability-distribution.md#probability-density-function) of the effects are, up to constants,

$$
\begin{aligned}
\ell_\alpha(a_2)&=Ra_2-I\theta(1+e^{b_2})e^{a_2}-\frac{a_2^2}{2\sigma_1^2},\\
\ell_\beta(b_2)&=Cb_2-I\theta(1+e^{a_2})e^{b_2}-\frac{b_2^2}{2\sigma_2^2}.
\end{aligned}
$$

These are [Gaussian-prior Poisson log-effect conditional](../../../statistical-modelling.md#gaussian-prior-poisson-log-effect-conditional) [probability density functions](../../../continuous-probability-distribution.md#probability-density-function). The exponential [likelihood](../../../statistical-modelling.md#likelihood-function) term prevents a standard [normal distribution](../../../probability-theory.md#normal-distribution) conjugate update. A [Metropolis-within-Gibbs algorithm](../../../statistical-inference.md#metropolis-within-gibbs-algorithm) conveniently updates one effect at a time without computing its conditional [normalizing constant](../../../continuous-probability-distribution.md#normalizing-constant).

For example, propose $a_2'=a_2+s_\alpha Z$ with $Z\sim N(0,1)$, and accept with

$$
\boxed{\min\{1,\exp(\ell_\alpha(a_2')-\ell_\alpha(a_2))\}.}
$$

Use an analogous [normal distribution](../../../probability-theory.md#normal-distribution) random-walk proposal for $b_2$. The proposal is symmetric and lives on the appropriate unrestricted real parameter space, so no proposal ratio is needed. It makes local moves compatible with a unimodal conditional [probability density function](../../../continuous-probability-distribution.md#probability-density-function). Tune the positive scale in a pilot or freeze it after warm-up; a scale far too large causes rejection and a scale far too small moves slowly.

A useful scale can be inferred from the conditional curvature: $\ell_\alpha''(a_2)=-I\theta(1+e^{b_2})e^{a_2}-\sigma_1^{-2}<0$, with the analogous formula for $b_2$. A normal proposal near the conditional mode with [variance](../../../variance.md) approximately $-1/\ell''$ is another sensible choice, but an asymmetric or state-dependent proposal must include its full reverse-to-forward proposal-density ratio. Metropolis–Hastings is convenient, not logically mandatory; these [concave](../../../real-analysis.md#concave-function) conditionals also admit other specialized samplers.

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

Introduce a model indicator $M\in\{0,1\}$. In $M=0$, set $\mu=0$, hence $\theta=1$, and retain the two group effects. In $M=1$, include $\mu$ with the prior induced by the gamma baseline. Choose positive prior model [probabilities](../../../probability-theory.md#probability) $p_0,p_1$ summing to one; the supplied within-model parameter priors alone do not specify these [probabilities](../../../probability-theory.md#probability).

Let $r=(a_2,b_2)$, use the same proper prior $p(r)$ in both models, and denote their likelihoods by $L_0(r)$ and $L_1(\mu,r)$. The unnormalized joint model targets are

$$
t_0(r)=p_0p(r)L_0(r),\qquad
t_1(\mu,r)=p_1p(r)p_\mu(\mu)L_1(\mu,r),
\qquad
p_\mu(u)=\frac{b^a}{\Gamma(a)}e^{au-be^u}.
$$

For a birth move, draw an auxiliary $u$ from a positive [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $q(u)$ and map $(r,u)$ to $(\mu'=u,r'=r)$. The reverse death move simply deletes $\mu$. This is a dimension-matching bijection with absolute Jacobian one. If the birth and death selection [probabilities](../../../probability-theory.md#probability) are $b_0$ and $d_1$, respectively, the [birth and death moves for Bayesian variable selection](../../../statistical-inference.md#birth-and-death-moves-for-bayesian-variable-selection) rule gives

$$
\boxed{A_{0\to1}=\min\!\left(1,
\frac{p_1p_\mu(u)L_1(u,r)d_1}{p_0L_0(r)b_0q(u)}\right).}
$$

The reverse acceptance is the reciprocal ratio, capped at one, evaluated at the current $\mu$. Choosing $q=p_\mu$ cancels the added-parameter prior; a data-informed proposal may mix better but must retain its proposal factor. Within each model, also update its continuous parameters to ensure exploration.

For an explicit [likelihood](../../../statistical-modelling.md#likelihood-function) ratio, with $E$ and $T$ from part (ii),

$$
\frac{L_1(u,r)}{L_0(r)}=\exp\{Tu-(e^u-1)E\}.
$$

This supplies a complete [reversible-jump Markov chain Monte Carlo](../../../statistical-inference.md#reversible-jump-markov-chain-monte-carlo) move. Its acceptance [probabilities](../../../probability-theory.md#probability) enforce [detailed balance](../../../markov-process.md#detailed-balance) between the two dimensions. The lower-dimensional state is a separate point-mass model, not a zero-probability equality test inside the continuous full-model prior.

<h3 id="5/vi">vi</h3>

↑ **Parent:** [5](#5)

<h4 id="5/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#5/vi)

Under the reference convention $\alpha_1=0$, the hypothesis becomes absence of the free group contrast $\alpha_2$. Introduce an inclusion indicator $J$: set $\alpha_2=0$ when $J=0$, and use its stated proper normal prior when $J=1$. Assign positive prior [probabilities](../../../probability-theory.md#probability) $q_0,q_1$ to those models, and retain $\mu,\beta_2$ in both.

A birth draws $u$ from a proposal [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $g(u)$ and appends it as $\alpha_2'=u$; the reverse death deletes it. The Jacobian is one. At fixed $\theta,\beta_2$, the [likelihood](../../../statistical-modelling.md#likelihood-function) ratio is

$$
\frac{L(\alpha_2=u)}{L(\alpha_2=0)}
=\exp\{Ru-I\theta(1+e^{\beta_2})(e^u-1)\}.
$$

Thus the birth acceptance ratio before capping is

$$
\frac{q_1p_\alpha(u)d_1}{q_0b_0g(u)}
\exp\{Ru-I\theta(1+e^{\beta_2})(e^u-1)\},
$$

where $p_\alpha$ is the normalized $N(0,\sigma_1^2)$ prior. Again, taking $g=p_\alpha$ cancels that factor. Use the reciprocal death rule and ordinary within-model parameter updates.

After warm-up, the [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) occupation fraction estimates the desired [probability](../../../probability-theory.md#probability):

$$
\boxed{\mathbb P(\alpha_1=\alpha_2=0\mid\mathbf x)
\approx\frac1N\sum_{s=1}^N\mathbf1_{\{J^{(s)}=0\}}.}
$$

This requires the chain to explore both models and satisfy its usual ergodic convergence conditions. Under the original continuous normal prior alone, the equality event has posterior [probability](../../../probability-theory.md#probability) zero; the explicit model indicator supplies the necessary prior atom. If intercept selection from part (v) is also performed, use two indicators and count all sampled states with $J=0$, regardless of the intercept indicator.

## 6

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

The parameter range is $0\leq\theta\leq1$. Omitting data-only constants from the [multinomial distribution](../../../discrete-probability-distribution.md#multinomial-distribution) [likelihood](../../../statistical-modelling.md#likelihood-function), its log is

$$
\ell(\theta)=(x_1+x_2)\log(1-\theta)+x_3\log\theta
+x_4\log(7+4\theta)+\mathrm{constant}.
$$

For an interior maximizer, the [likelihood](../../../statistical-modelling.md#likelihood-function) score must vanish:

$$
-\frac{x_1+x_2}{1-\theta}+\frac{x_3}{\theta}
+\frac{4x_4}{7+4\theta}=0.
$$

Multiply by $\theta(1-\theta)(7+4\theta)$ and collect powers to obtain

$$
\boxed{-4(x_1+x_2+x_3+x_4)\theta^2
+(-7x_1-7x_2-3x_3+4x_4)\theta+7x_3=0.}
$$

The [likelihood](../../../statistical-modelling.md#likelihood-function) is [concave](../../../real-analysis.md#concave-function): its second [derivative](../../../calculus.md#derivative) in the interior is

$$
\ell''(\theta)=-\frac{x_1+x_2}{(1-\theta)^2}
-\frac{x_3}{\theta^2}-\frac{16x_4}{(7+4\theta)^2}<0.
$$

Therefore an admissible interior root is the unique maximum. Endpoints must also be handled if some counts vanish. If $x_3>0$ and $x_1+x_2>0$, both endpoints have zero [likelihood](../../../statistical-modelling.md#likelihood-function) and the root is interior. If the maximum is at zero then $x_3=0$, and zero also satisfies the displayed polynomial; a maximum at one requires $x_1+x_2=0$, and one likewise satisfies it. Multiplying the score can introduce other endpoint roots, so not every polynomial root is an MLE: evaluate the actual [likelihood](../../../statistical-modelling.md#likelihood-function) on the feasible candidates.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Let $Z$ be the unobserved part of the fourth count associated with the component of [probability](../../../probability-theory.md#probability) $\theta/3$. Its complementary subcount has [probability](../../../probability-theory.md#probability) $7/12$. Conditional on the observed fourth count and a parameter value,

$$
\boxed{Z\mid x_4,\theta\sim\operatorname{Bin}\left(x_4,\frac{4\theta}{7+4\theta}\right).}
$$

The complete-data [log-likelihood](../../../statistical-modelling.md#log-likelihood) now has the simple form

$$
\ell_c(\theta)=(x_3+Z)\log\theta+(x_1+x_2)\log(1-\theta)
+\mathrm{constant}.
$$

The constant term can depend on the completed counts, but not on $\theta$. The split therefore converts the troublesome $\log(7+4\theta)$ term into a binomial-like maximization problem. Since $Z$ is unobserved, it should be averaged conditionally in an [EM algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm), not guessed or treated as observed.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

For observed data $x$ and missing data $z$, let $p_\theta(x,z)$ be the complete-data model. Starting at $\theta^{(0)}$, the [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) alternates

$$
Q(\theta\mid\theta^{(r)})
=\mathbb E_{\theta^{(r)}}[\log p_\theta(x,Z)\mid x],
\qquad
\theta^{(r+1)}\in\operatorname*{arg\,max}_\theta Q(\theta\mid\theta^{(r)}).
$$

The E-step computes the [conditional expectation](../../../measure-theory.md#conditional-expectation) of the complete-data [log-likelihood](../../../statistical-modelling.md#log-likelihood), using the current parameter for the missing-data [conditional distribution](../../../probability-theory.md#conditional-distribution). The M-step maximizes that expected [log-likelihood](../../../statistical-modelling.md#log-likelihood) over a new parameter. Maximizing the [likelihood](../../../statistical-modelling.md#likelihood-function) of imputed [mean](../../../probability-theory.md#expected-value) data is equivalent only when the complete-data [log-likelihood](../../../statistical-modelling.md#log-likelihood) has the necessary linear dependence on the missing sufficient statistics.

For the monotonicity argument, let $q_r(z)=p_{\theta^{(r)}}(z\mid x)$. [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives

$$
\log p_\theta(x)-\log p_{\theta^{(r)}}(x)
=\log\mathbb E_{q_r}\left[\frac{p_\theta(x,Z)}{p_{\theta^{(r)}}(x,Z)}\right]
\geq Q(\theta\mid\theta^{(r)})-Q(\theta^{(r)}\mid\theta^{(r)}).
$$

Therefore an M-step increasing $Q$ cannot decrease the observed-data [likelihood](../../../statistical-modelling.md#likelihood-function). Standard support and [integrability](../../../measure-theory.md#integrability) conditions are understood. EM need not find a global maximum for a general model; its behavior depends on the objective and starting point.

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

For these counts, start with any $0<\theta^{(0)}<1$. The conditional missing count from part (ii) has [mean](../../../probability-theory.md#expected-value)

$$
z_r=\mathbb E[Z\mid\mathbf x,\theta^{(r)}]
=\frac{340\theta^{(r)}}{7+4\theta^{(r)}}.
$$

The E-step objective is

$$
Q(\theta\mid\theta^{(r)})=(5+z_r)\log\theta+30\log(1-\theta)+\mathrm{constant}.
$$

Its strictly [concave](../../../real-analysis.md#concave-function) M-step is explicit:

$$
\boxed{\theta^{(r+1)}=\frac{5+z_r}{35+z_r},\qquad
z_r=\frac{340\theta^{(r)}}{7+4\theta^{(r)}}.}
$$

Equivalently, the update map is $F(\theta)=(35+360\theta)/(245+480\theta)$. Its fixed-point equation is

$$
480\theta^2-115\theta-35=0.
$$

The unique root in $(0,1)$ is the [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator)

$$
\boxed{\widehat\theta=\frac{115+\sqrt{80425}}{960}\approx0.4152.}
$$

For example, starting at $1/2$ gives $0.443299$, then approximately $0.425065$, and subsequent iterates approach the displayed root. Convergence is also transparent without relying only on the general EM theorem: $F$ is increasing and

$$
F(\theta)-\theta=\frac{35+115\theta-480\theta^2}{245+480\theta}.
$$

This is positive below the feasible fixed point and negative above it. Monotonicity of $F$ prevents crossing that fixed point, so the iterates converge monotonically toward it from either side. The original [log-likelihood](../../../statistical-modelling.md#log-likelihood) is strictly [concave](../../../real-analysis.md#concave-function) and diverges to minus infinity at both endpoints, establishing that the fixed point is the unique global maximum.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2004](../../2004.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
