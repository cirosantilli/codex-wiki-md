# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_36.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Series 1 wanders over a changing level rather than fluctuating around a stable local mean. Its sample [autocorrelation function](../../../time-series.md#autocorrelation) is strongly positive and decreases very slowly. This is the usual diagnostic evidence for an ordinary [unit root](../../../time-series.md#unit-root): an autoregressive polynomial containing $1-z$, with a zero at $z=1$, and a stationary model after first [differencing](../../../time-series.md#differencing). The plots support an integrated model, rather than specifying the number of its remaining stationary autoregressive or moving-average terms.

Series 2 has a pronounced oscillation with period about six observations. Its sample [autocorrelation](../../../time-series.md#autocorrelation) alternates between large positive and negative values with little damping: approximately positive at multiples of six and negative halfway between. Together with the changing amplitude, this suggests a conjugate pair of unit-circle zeros near

$$
\boxed{z=e^{\pm i\pi/3}.}
$$

The associated real autoregressive factor is $1-2\cos(\pi/3)z+z^2=1-z+z^2$. A targeted filter $1-B+B^2$ removes this pair; the broader [seasonal difference operator](../../../time-series.md#seasonal-difference-operator) $1-B^6$ also contains it but introduces additional [differencing](../../../time-series.md#differencing) factors. This is the [oscillatory unit-root diagnosis from an undamped sample autocorrelation](../../../time-series.md#oscillatory-unit-root-diagnosis-from-an-undamped-sample-autocorrelation).

Thus **Series 1 suggests a zero at 1; Series 2 suggests a conjugate pair on the unit circle at a seasonal frequency**. These are model diagnoses, not deductions of exact roots from a finite sample. A stationary model very close to a [unit root](../../../time-series.md#unit-root) can look similar, and an undamped periodic [covariance](../../../variance.md#covariance) can also arise from a stationary random sinusoid. The figure does not identify exact orders or prove nonstationarity by itself.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Among the supplied candidates, **choose [ARMA](../../../time-series.md#autoregressive-moving-average-model)(2,1)**. It has the smallest [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion). Relative to [ARMA](../../../time-series.md#autoregressive-moving-average-model)(2,2), its AIC improvement is $1.71$; the additional second moving-average estimate is only half a standard error from zero and increases the log [likelihood function](../../../statistical-modelling.md#likelihood-function) by only about $0.14$. Dropping it is a reasonable parsimony choice, although that AIC gap is small. [ARMA](../../../time-series.md#autoregressive-moving-average-model)(1,1) has AIC larger by $17.55$, a much clearer loss of fit. In the chosen model the second autoregressive term is about seven standard errors from zero, so it should not be dropped merely to obtain order one. The first autoregressive term is less precisely estimated; this does not justify automatically deleting it without fitting and comparing the reduced candidate.

Using the usual positive-sign moving-average convention, the fitted [autoregressive moving-average model](../../../time-series.md#autoregressive-moving-average-model) is

$$
\boxed{X_t=-0.30X_{t-1}+0.28X_{t-2}+Z_t+0.50Z_{t-1},\qquad Z\sim\operatorname{WN}(0,4).}
$$

These are plug-in values rounded as given, not exact population parameters. The model has zero mean. Its polynomials are $\phi(z)=1+0.30z-0.28z^2=(1-0.4z)(1+0.7z)$ and $\theta(z)=1+0.5z$.

With angular frequency $\omega\in[-\pi,\pi]$, so that the [autocovariance](../../../time-series.md#autocovariance) is $\gamma(h)=\int_{-\pi}^{\pi}e^{ih\omega}f_X(\omega)\,d\omega$, the [spectral density of a stationary process](../../../time-series.md#spectral-density-of-a-stationary-process) is

$$
\boxed{f_X(\omega)=\frac4{2\pi}\frac{|1+0.5e^{-i\omega}|^2}{|1+0.30e^{-i\omega}-0.28e^{-2i\omega}|^2}
=\frac2\pi\frac{1.25+\cos\omega}{(1.16-0.8\cos\omega)(1.49+1.4\cos\omega)}.}
$$

The frequency convention makes the normalization unambiguous.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The autoregressive polynomial factors as $(1-0.4z)(1+0.7z)$, with zeros

$$
\boxed{z=2.5,\qquad z=-10/7.}
$$

Both have modulus greater than one. The [causality root criterion for an autoregressive model](../../../time-series.md#causality-root-criterion-for-an-autoregressive-model) therefore gives a causal stationary solution. The moving-average polynomial has its only zero at $-2$, also outside the unit circle, so the [invertibility of a moving-average model](../../../time-series.md#invertibility-of-a-moving-average-model) holds. There is no common root to cancel.

To use unit-[variance](../../../variance.md) [white noise](../../../time-series.md#white-noise), put $W_t=Z_t/2$. One suitable pair is

$$
\boxed{\widetilde\phi(z)=1+0.30z-0.28z^2,\qquad\widetilde\theta(z)=2+z.}
$$

Then $\widetilde\phi(B)X_t=\widetilde\theta(B)W_t$ with $W\sim\operatorname{WN}(0,1)$. The factor two changes the innovation scale, not the zero of the moving-average polynomial.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Write $X_t=\sum_{j\geq0}\psi_jZ_{t-j}$, with innovation [variance](../../../variance.md) four. The generating function of this [linear process](../../../time-series.md#linear-process-time-series) is

$$
\Psi(z)=\frac{1+0.5z}{1+0.30z-0.28z^2}.
$$

Equating coefficients gives $\psi_0=1$, $\psi_1=0.2$ and $\psi_j=-0.3\psi_{j-1}+0.28\psi_{j-2}$ for $j\geq2$. Thus the first five coefficients, including lag zero, are

$$
\boxed{(\psi_0,\psi_1,\psi_2,\psi_3,\psi_4)=(1,\ 0.2,\ 0.22,\ -0.01,\ 0.0646).}
$$

For all remaining lags, partial fractions give

$$
\Psi(z)=\frac{9/11}{1-0.4z}+\frac{2/11}{1+0.7z},\qquad
\boxed{\psi_j=\frac9{11}(0.4)^j+\frac2{11}(-0.7)^j\quad(j\geq0).}
$$

The coefficients are absolutely summable, so the series converges in mean square and defines the causal moving-average expansion. In the unit-[variance](../../../variance.md) convention of part (c), $X_t=\sum_{j\geq0}c_jW_{t-j}$ with $c_j=2\psi_j$; its first five coefficients are $(2,0.4,0.44,-0.02,0.1292)$. This is the [two-geometric-coefficient expansion of a causal ARMA(2,1) process](../../../time-series.md#two-geometric-coefficient-expansion-of-a-causal-arma-2-1-process).

[White noise](../../../time-series.md#white-noise) orthogonality gives, for any integer $h$,

$$
\boxed{\gamma(h)=4\sum_{j=0}^\infty\psi_j\psi_{j+|h|}=\sum_{j=0}^\infty c_jc_{j+|h|},\qquad
\rho(h)=\frac{\sum_{j\geq0}\psi_j\psi_{j+|h|}}{\sum_{j\geq0}\psi_j^2}.}
$$

To see this directly, expand the [covariance](../../../variance.md#covariance) of the two convergent series. Only matching noise indices contribute. [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) makes the coefficient-product sum finite, justifying the [covariance](../../../variance.md#covariance) limit.

There is also a closed expression. Set $a=9/11$, $d=2/11$, $r=0.4$, $s=-0.7$. For $h\geq0$,

$$
\gamma(h)=4\left[\frac{a^2r^h}{1-r^2}+\frac{d^2s^h}{1-s^2}+\frac{ad(r^h+s^h)}{1-rs}\right],
$$

and negative lags follow by symmetry. Dividing by the expression at zero gives the same [autocorrelation function](../../../time-series.md#autocorrelation).

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Interpret stationarity in the usual second-order time-series sense and assume nondegenerate noise, $\sigma_z^2>0$. For a two-sided autoregressive equation, the missing existence condition is

$$
\boxed{|\phi|\ne1.}
$$

It is important to separate this from causality. If $|\phi|<1$, the unique stationary solution is $X_t=\sum_{j\geq0}\phi^jZ_{t-j}$. If $|\phi|>1$, there is still a stationary solution, but it is [anticausal](../../../time-series.md#anticausal-time-series):

$$
\boxed{X_t=-\sum_{j=1}^\infty\phi^{-j}Z_{t+j}.}
$$

Both expansions converge in L2 because their coefficients are square summable. Substitution verifies the equation. Their means are zero and their [covariance](../../../variance.md#covariance) functions depend only on lag. Uniqueness follows by iterating the equation backward in the first case and forward in the second: the remainders $\phi^nX_{t-n}$ or $\phi^{-n}X_{t+n}$ tend to zero in L2 for any stationary finite-[variance](../../../variance.md) solution. This is the [stationary versus causal solution of a two-sided AR(1) equation](../../../time-series.md#stationary-versus-causal-solution-of-a-two-sided-ar-1-equation).

For $\phi=\pm1$, iteration gives

$$
X_t-\phi^nX_{t-n}=\sum_{j=0}^{n-1}\phi^jZ_{t-j}.
$$

The [variance](../../../variance.md) of the right side is $n\sigma_z^2$. The [variance](../../../variance.md) of the left side is at most $4\operatorname{Var}(X_t)$ by stationarity and [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). These are incompatible as $n\to\infty$. Thus no weakly stationary finite-[variance](../../../variance.md) solution exists at those [unit roots](../../../time-series.md#unit-root).

If the intended claim includes a causal innovation representation, its condition is instead **$|\phi|<1$**, as in the next part. The stated [white noise](../../../time-series.md#white-noise) equation alone does not say that $Z_t$ is orthogonal to the past of $X$. If zero innovation [variance](../../../variance.md) is allowed, the unit-root exclusion has degenerate exceptions, such as random constant solutions when $\phi=1$; the nondegenerate convention is necessary for the asserted nonexistence.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The condition for a causal linear-filter solution is **$|\phi|<1$**. Its mean-square expansion is $X_t=\sum_{j\geq0}\phi^jZ_{t-j}$. Summing the matching [white noise](../../../time-series.md#white-noise) terms gives

$$
\gamma_X(h)=\frac{\sigma_z^2}{1-\phi^2}\phi^{|h|}.
$$

The assumed orthogonality of every $W_s$ to every $Z_t$ extends to every $X_t$ by L2 convergence of that expansion. Hence the added-noise process has mean zero and

$$
\boxed{\gamma_Y(h)=\frac{\sigma_z^2}{1-\phi^2}\phi^{|h|}+\sigma_w^2\mathbf1_{\{h=0\}}.}
$$

This depends only on lag, proving [weak stationarity](../../../time-series.md#weakly-stationary-process). Its [autocorrelation](../../../time-series.md#autocorrelation) has the same geometric tail as the latent autoregression, but its positive-lag correlations are reduced by the additional [variance](../../../variance.md) at lag zero. This is the [autocovariance of an AR(1) process observed with white noise](../../../time-series.md#autocovariance-of-an-ar-1-process-observed-with-white-noise). Strict stationarity or Gaussianity is not implied by [white noise](../../../time-series.md#white-noise) [covariance](../../../variance.md#covariance) assumptions alone.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Apply $1-\phi B$ to the observed process and call the result $V_t$. Then

$$
V_t=Z_t+W_t-\phi W_{t-1}.
$$

Its only nonzero [covariance](../../../variance.md#covariance) lags are

$$
A=\gamma_V(0)=\sigma_z^2+(1+\phi^2)\sigma_w^2,\qquad C=\gamma_V(1)=-\phi\sigma_w^2.
$$

Seek an invertible moving-average factor $V_t=\varepsilon_t+\vartheta\varepsilon_{t-1}$ with $\operatorname{Var}(\varepsilon_t)=\nu$. Matching these covariances requires $\nu(1+\vartheta^2)=A$ and $\nu\vartheta=C$. Solving gives

$$
\boxed{\nu=\frac{A+\sqrt{A^2-4\phi^2\sigma_w^4}}2,\qquad
\vartheta=-\frac{\phi\sigma_w^2}{\nu},\qquad\phi_{\rm AR}=\phi.}
$$

These are the three requested parameters in the positive-sign moving-average convention. For nonzero total noise [variance](../../../variance.md),

$$
A-2|C|=\sigma_z^2+(1-|\phi|)^2\sigma_w^2>0,
$$

so $|\vartheta|<1$ and the larger quadratic root gives the invertible factor.

[Covariance](../../../variance.md#covariance) matching alone would not identify arbitrary processes in distribution. To obtain an actual representation on the given space, define

$$
\varepsilon_t=(1+\vartheta B)^{-1}V_t=\sum_{j\geq0}(-\vartheta)^jV_{t-j}.
$$

The series converges in L2. The spectrum of $V$ is $(A+2C\cos\omega)/(2\pi)=\nu|1+\vartheta e^{-i\omega}|^2/(2\pi)$, so this filtered process has constant spectrum $\nu/(2\pi)$ and is [white noise](../../../time-series.md#white-noise). Thus

$$
\boxed{(1-\phi B)Y_t=(1+\vartheta B)\varepsilon_t,\qquad\varepsilon\sim\operatorname{WN}(0,\nu).}
$$

This is the [invertible ARMA factorization of an AR(1)-plus-noise process](../../../time-series.md#invertible-arma-factorization-of-an-ar-1-plus-noise-process). If $\sigma_w^2=0$, it reduces to AR(1); if $\phi=0$, it reduces to [white noise](../../../time-series.md#white-noise). If $\sigma_z^2=0$ and $\sigma_w^2>0$, then $\vartheta=-\phi$, the common factor cancels and $Y=W$. Therefore the orders are at most (1,1); no unnecessarily minimal-order claim is made in those degenerate cases.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Take the latent autoregression as the scalar state $S_t$. A [state-space model](../../../time-series.md#state-space-model-time-series) is

$$
\boxed{\text{state: }S_t=\phi S_{t-1}+Z_t,\qquad\text{observation: }Y_t=S_t+W_t.}
$$

The transition and observation matrices are both scalar, $F=\phi$, $H=1$. State-noise [variance](../../../variance.md) is $Q=\sigma_z^2$, observation-noise [variance](../../../variance.md) is $R=\sigma_w^2$, and the cross-noise [covariance](../../../variance.md#covariance) is zero at every pair of times.

A complete stationary initialization is

$$
S_0=\sum_{j\geq0}\phi^jZ_{-j},\qquad\mathbb ES_0=0,\qquad\operatorname{Var}(S_0)=\frac{\sigma_z^2}{1-\phi^2}.
$$

It is orthogonal to future state noise and to all observation noise. This is the [stationary initialization of a scalar linear state-space model](../../../time-series.md#stationary-initialization-of-a-scalar-linear-state-space-model). This specifies the initial state in terms of the actual given two-sided [white noise](../../../time-series.md#white-noise) sequence, as well as its second-order law; simply starting from zero would give transient rather than stationary observations.

If a Gaussian state-space specification is intended, the complete specialization is $S_0\sim N(0,Q/(1-\phi^2))$, independent of the future iid Gaussian state and observation noises, themselves independent with variances $Q,R$. Under the printed assumptions alone, Gaussian distributions and independence cannot be deduced from [white noise](../../../time-series.md#white-noise) orthogonality; the equations and stationary-series initialization above give the exact second-order representation without adding them.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Generate independent $U,V\sim\operatorname{Unif}(0,1)$ and use the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform)

$$
\boxed{G_1=\sqrt{-2\log U}\cos(2\pi V),\qquad G_2=\sqrt{-2\log U}\sin(2\pi V).}
$$

For $R=\sqrt{-2\log U}$, $\mathbb P(R>r)=e^{-r^2/2}$, so its density is $re^{-r^2/2}$ on $r>0$. The angle $2\pi V$ is uniform on $[0,2\pi)$ and independent of $R$. Dividing the joint radial-angular density by the polar-coordinate Jacobian $r$ gives

$$
f_{G_1,G_2}(x,y)=\frac1{2\pi}e^{-(x^2+y^2)/2}
=\frac{e^{-x^2/2}}{\sqrt{2\pi}}\frac{e^{-y^2/2}}{\sqrt{2\pi}}.
$$

Thus **both outputs are independent and have the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution)**. Independent pairs of uniforms give further independent normal observations. The null event $U=0$ is excluded in implementation so the logarithm is finite.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

For fixed parameters $(a,b)$, every new error is independent of the previous observations. Put $\varphi_0(z)=(2\pi)^{-1/2}e^{-z^2/2}$. Since $X_0=X_1=0$, the first three conditional densities are

$$
\boxed{f_{X_2\mid X_1}(x_2\mid0)=\varphi_0(x_2),\qquad
f_{X_3\mid X_2,X_1}(x_3\mid x_2,0)=\varphi_0(x_3-ax_2),}
$$

and

$$
\boxed{f_{X_4\mid X_3,X_2,X_1}(x_4\mid x_3,x_2,0)=\varphi_0(x_4-ax_3-bx_2).}
$$

In general,

$$
\boxed{X_{t+2}\mid(X_{t+1},\ldots,X_1),a,b\sim N(aX_{t+1}+bX_t,1).}
$$

Its density is $\varphi_0(x_{t+2}-ax_{t+1}-bx_t)$. The recursion is interpreted from $t=0$, as required to define $X_2$ from the two given initial values. These are parameter-conditional sampling distributions; integrating over the prior would instead give predictive mixtures.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the chain rule for conditional densities. With $x_0=x_1=0$, the [likelihood function](../../../statistical-modelling.md#likelihood-function) of the nondegenerate observations is

$$
\boxed{L(a,b;x_1,\ldots,x_n)=(2\pi)^{-(n-1)/2}\exp\left[-\frac12\sum_{t=0}^{n-2}(x_{t+2}-ax_{t+1}-bx_t)^2\right].}
$$

The first residual is $x_2$ and carries no parameter information. There is no ordinary joint Lebesgue density for $X_1,\ldots,X_n$ because $X_1=0$ deterministically; this expression is the conditional [likelihood function](../../../statistical-modelling.md#likelihood-function) given the fixed initial values, or the [likelihood function](../../../statistical-modelling.md#likelihood-function) on $x_2,\ldots,x_n$. The initial point mass is parameter independent and has no effect on inference. This is the [conditional likelihood of an initialized Gaussian AR(2) process](../../../time-series.md#conditional-likelihood-of-an-initialized-gaussian-ar-2-process).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Define the sufficient data sums, all over $0\leq t\leq n-2$,

$$
A=1+\sum x_{t+1}^2,\quad D=1+\sum x_t^2,\quad C=\sum x_{t+1}x_t,\quad
r=\sum x_{t+1}x_{t+2},\quad s=\sum x_tx_{t+2}.
$$

Multiplying the [likelihood function](../../../statistical-modelling.md#likelihood-function) by the independent standard-normal priors and collecting the quadratic terms gives

$$
\pi(a,b)\propto\exp\left[-\frac12(Aa^2+2Cab+Db^2-2ra-2sb)\right].
$$

Let $\Lambda=\begin{pmatrix}A&C\\C&D\end{pmatrix}$ and $\Delta=AD-C^2$. This precision matrix is $I+\sum v_tv_t^T$, where $v_t=(x_{t+1},x_t)^T$, so it is positive definite even for a short or singular design. Completing the square proves

$$
\boxed{\begin{pmatrix}a\\b\end{pmatrix}\Bigm|x\sim N_2(\mu,\Sigma),\quad
\Sigma=\frac1\Delta\begin{pmatrix}D&-C\\-C&A\end{pmatrix},\quad
\mu=\frac1\Delta\begin{pmatrix}Dr-Cs\\As-Cr\end{pmatrix}.}
$$

The fully normalized [posterior](../../../statistical-inference.md#bayesian-posterior) density is

$$
\boxed{\pi(a,b)=\frac{\sqrt\Delta}{2\pi}\exp\left[-\frac12\left(\begin{pmatrix}a\\b\end{pmatrix}-\mu\right)^T\Lambda\left(\begin{pmatrix}a\\b\end{pmatrix}-\mu\right)\right].}
$$

This is [Gaussian conjugacy for an initialized AR(2) regression](../../../statistical-modelling.md#gaussian-conjugacy-for-an-initialized-ar-2-regression).

Completing each one-dimensional square, or using the supplied conditional-normal identity, gives

$$
\boxed{b\mid a,x\sim N\left(\frac{s-Ca}{D},\frac1D\right),\qquad
a\mid b,x\sim N\left(\frac{r-Cb}{A},\frac1A\right).}
$$

When $n=2$, all regressor sums vanish and the [posterior](../../../statistical-inference.md#bayesian-posterior) remains the independent standard-normal prior. No stationary-parameter restriction is imposed: the specified prior is on all of $\mathbb R^2$, and the finite initialized chain is defined for all $(a,b)$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Start from any $(a^{(0)},b^{(0)})$. For independent draws $G_{1,k},G_{2,k}$ from the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) at each sweep, the [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) can be implemented as

$$
\boxed{a^{(k+1)}=\frac{r-Cb^{(k)}}A+\frac{G_{1,k}}{\sqrt A},\qquad
b^{(k+1)}=\frac{s-Ca^{(k+1)}}D+\frac{G_{2,k}}{\sqrt D}.}
$$

The second update must use the newly drawn first coordinate. The transform in part (a) supplies the needed independent Gaussian draws. Each conditional update preserves the joint [posterior](../../../statistical-inference.md#bayesian-posterior), so their composition does too.

Convergence is particularly transparent here. Centering at the [posterior](../../../statistical-inference.md#bayesian-posterior) mean gives

$$
b^{(k+1)}-\mu_b=\frac{C^2}{AD}(b^{(k)}-\mu_b)-\frac{C}{D\sqrt A}G_{1,k}+\frac{G_{2,k}}{\sqrt D}.
$$

Positive definiteness gives $C^2/(AD)<1$, so this is a stable Gaussian autoregression. The full sampler has the desired [posterior](../../../statistical-inference.md#bayesian-posterior) as its limiting invariant law. This is the [linear contraction of a two-coordinate Gaussian Gibbs sweep](../../../statistical-inference.md#linear-contraction-of-a-two-coordinate-gaussian-gibbs-sweep).

For a [posterior](../../../statistical-inference.md#bayesian-posterior)-integrable function $\phi$, its [posterior](../../../statistical-inference.md#bayesian-posterior) expectation is estimated after a burn-in $K$ by

$$
\boxed{\widehat{\mathbb E}_\pi\phi=\frac1L\sum_{k=K+1}^{K+L}\phi(a^{(k)},b^{(k)}).}
$$

The ergodic theorem justifies this Monte Carlo average. The retained values of $\phi$ also approximate its [posterior](../../../statistical-inference.md#bayesian-posterior) distribution and quantiles. If a Bayesian point estimate is requested under squared-error loss, the [posterior](../../../statistical-inference.md#bayesian-posterior) mean is the appropriate estimate, when its needed moments exist. An arbitrary function need not have a finite [posterior](../../../statistical-inference.md#bayesian-posterior) mean; integrability must be assumed for the displayed target. Successive Gibbs draws are correlated, so uncertainty in the Monte Carlo average should use chain-aware error estimates rather than treating them as iid.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $w(x)=f(x)/g(x)$ where $g(x)>0$, and set it to zero on the g-null set where $g=0$. The domination assumption makes $f=0$ there and gives $0\leq w\leq M$. Integrating it also gives $M\geq1$. For iid proposals $X_i\sim g$, the [importance sampling](../../../probability-and-statistics.md#importance-sampling) estimator is

$$
\boxed{\widehat\theta_1=\frac1n\sum_{i=1}^n\phi(X_i)w(X_i).}
$$

[Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) under $f$ gives $|\theta|\leq(\int\phi^2f)^{1/2}<\infty$. Direct integration proves unbiasedness, $\mathbb E_g[\phi(X)w(X)]=\theta$. Moreover

$$
\mathbb E_g[\phi(X)^2w(X)^2]=\int_{g>0}\phi(x)^2\frac{f(x)^2}{g(x)}\,dx\leq M\int\phi(x)^2f(x)\,dx<\infty.
$$

Thus

$$
\boxed{\mathbb E\widehat\theta_1=\theta,\qquad\operatorname{Var}(\widehat\theta_1)=\frac{v_{\rm IS}}n,\quad
v_{\rm IS}=\int\phi^2\frac{f^2}{g}-\theta^2.}
$$

The iid [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) applies to these finite-[variance](../../../variance.md) weighted observations:

$$
\boxed{\sqrt n(\widehat\theta_1-\theta)\ \Longrightarrow\ N(0,v_{\rm IS}).}
$$

If the [variance](../../../variance.md) is zero, this denotes the point mass at zero. This is the [bounded-weight importance-sampling moment bound](../../../probability-and-statistics.md#bounded-weight-importance-sampling-moment-bound).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For each proposal $X\sim g$, independently draw $U\sim\operatorname{Unif}(0,1)$ and accept it when

$$
\boxed{U\leq\frac{f(X)}{Mg(X)}.}
$$

The ratio is at most one, as required. For any measurable set $A$,

$$
\mathbb P(X\in A,\text{accept})=\frac1M\int_Af(x)\,dx,
$$

so the acceptance probability is $p=1/M$ and the conditional distribution of an accepted proposal has density $f$. Repeating independent trials until acceptance therefore gives an exact draw from $f$, and repeating the whole procedure gives iid target draws. This proves [rejection sampling](../../../probability-and-statistics.md#rejection-sampling).

The number of proposals for one successful draw is geometric with mean $M$. Thus $M$ is also the expected proposal cost of this exact simulation method.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Apply independent uniforms to the $n$ proposals, and let $I_i$ indicate acceptance. Each $I_i$ is Bernoulli with success probability $p=1/M$, and the indicators are independent because the pairs $(X_i,U_i)$ are independent. Hence

$$
\boxed{N=\sum_{i=1}^nI_i\sim\operatorname{Bin}(n,1/M),\qquad
\mathbb EN=\frac nM,\qquad\operatorname{Var}(N)=\frac nM\left(1-\frac1M\right).}
$$

For a fixed acceptance pattern, the values at accepted positions are independent with density $f$, by the single-trial conditional density calculation. The same product law holds for every pattern of a given size. Consequently, conditional on $N=m$, the ordered accepted observations have joint density $\prod_{j=1}^mf(y_j)$. This is the [binomial count and iid values in fixed-budget rejection sampling](../../../probability-and-statistics.md#binomial-count-and-iid-values-in-fixed-budget-rejection-sampling); the count provides no information about those target values.

There is a finite-sample empty-output event, with probability $(1-1/M)^n$. Any estimator dividing by $N$ must be defined separately on $N=0$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Write $p=1/M$ and $v_f=\int\phi^2f-\theta^2$. The Bernoulli [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives

$$
\boxed{\frac{N-\mathbb EN}{\sqrt n}\ \Longrightarrow\ N(0,p(1-p)).}
$$

If $M=1$, all proposals are accepted and this limit is degenerate.

Conditional on $N=m$, the accepted sample is iid from $f$. Since $N/n\to p>0$, its size tends to infinity, and the ordinary target-sample CLT therefore gives

$$
\boxed{\sqrt N\left(\frac1N\sum_{i=1}^N\phi(Y_i)-\theta\right)\ \Longrightarrow\ N(0,v_f).}
$$

Assign any fixed value to the estimator on $N=0$; the probability of that event tends to zero, so it does not change this limit. This is the [random-count central limit theorem for accepted rejection samples](../../../probability-and-statistics.md#random-count-central-limit-theorem-for-accepted-rejection-samples).

For comparison at the same budget of $n$ proposals, Slutsky's theorem rescales this as

$$
\boxed{\sqrt n(\widehat\theta_2-\theta)\ \Longrightarrow\ N(0,Mv_f).}
$$

The distinction between accepted-sample size and proposal count is essential for the final efficiency comparison.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

At a common proposal budget, the two asymptotic variances are

$$
v_{\rm IS}=\int\phi^2\frac{f^2}{g}-\theta^2,\qquad v_{\rm rej}=M\left(\int\phi^2f-\theta^2\right).
$$

Thus **prefer the estimator with the smaller proposal-budget [variance](../../../variance.md); the stated assumptions do not give a universal winner**. [Importance sampling](../../../probability-and-statistics.md#importance-sampling) uses every proposal and avoids an empty accepted sample, but those facts alone do not establish [variance](../../../variance.md) dominance. The bound from part (a) only says $v_{\rm IS}\leq Mv_f+(M-1)\theta^2$. If $\theta=0$, it does imply that [importance sampling](../../../probability-and-statistics.md#importance-sampling) is at least as efficient asymptotically.

For explicit nonconstant counterexamples in both directions, take $g(x)=1$ and $f(x)=2x$ on $0<x<1$, and zero outside, with the sharp envelope $M=2$. For $\phi(x)=x$, direct integration gives $\theta=2/3$, $v_f=1/18$ and

$$
\boxed{v_{\rm IS}=16/45>1/9=v_{\rm rej}.}
$$

The accepted-sample mean is better. For the same densities but $\phi(x)=x-1$, the target [variance](../../../variance.md) is unchanged, while $\theta=-1/3$ and

$$
\boxed{v_{\rm IS}=1/45<1/9=v_{\rm rej}.}
$$

[Importance sampling](../../../probability-and-statistics.md#importance-sampling) is now better. This is the [variance reversal under additive shifts of an importance-sampling integrand](../../../probability-and-statistics.md#variance-reversal-under-additive-shifts-of-an-importance-sampling-integrand).

There is a useful distinction about the [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem). The weighted importance estimator is the conditional expectation, given the proposals, of the fixed-denominator rejection estimator $(M/n)\sum_i I_i\phi(X_i)$. It is not the conditional expectation of the random-denominator mean $N^{-1}\sum_i I_i\phi(X_i)$. Rao-Blackwell [variance](../../../variance.md) reduction for the former therefore does not prove a comparison with the latter. This is the [Rao-Blackwell identity for a fixed-denominator rejection estimator](../../../probability-and-statistics.md#rao-blackwell-identity-for-a-fixed-denominator-rejection-estimator). The appropriate answer is the [proposal-budget variance comparison of importance and rejection sampling](../../../probability-and-statistics.md#proposal-budget-variance-comparison-of-importance-and-rejection-sampling), with the empty-output convention specified.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
