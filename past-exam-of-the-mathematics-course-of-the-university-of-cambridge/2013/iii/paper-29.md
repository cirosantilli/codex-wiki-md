# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2013/paper_29.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A [causal time-series representation](../../../time-series.md#causal-time-series-representation) uses only the present and past driving [white noise](../../../time-series.md#white-noise). Thus the coefficient condition is

$$
\boxed{a_r=0\quad\text{for }r<0.}
$$

The series must have its stated convergence meaning. For centered [white noise](../../../time-series.md#white-noise) of positive finite [variance](../../../variance.md), $\sum_{r\geq0}|a_r|^2<\infty$ is sufficient and necessary for [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2). In the usual stable-filter convention one imposes the stronger $\sum_{r\geq0}|a_r|<\infty$. A bilateral stationary [linear process](../../../time-series.md#linear-process-time-series) need not be causal: terms with $r<0$ involve future driving values.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

An [invertible time-series representation](../../../time-series.md#invertible-time-series-representation) recovers the driving [white noise](../../../time-series.md#white-noise) from current and past observations. In the inverse series the support condition is therefore

$$
\boxed{b_r=0\quad\text{for }r<0.}
$$

Again the series must converge. Stable invertibility uses $\sum_{r\geq0}|b_r|<\infty$, which ensures [mean-square convergence](../../../convergence-of-random-variables.md#convergence-in-l2) when $X_t$ has finite [variance](../../../variance.md). Merely writing a bilateral inverse is not invertibility in this one-sided sense: it may require future observations. For a general correlated input $X$, square summability of $b_r$ alone is not the same sufficient condition as it is for a [white noise](../../../time-series.md#white-noise) input.

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

For an [autoregressive moving-average model](../../../time-series.md#autoregressive-moving-average-model), the driving-to-output transfer function is $A(z)=\theta(z)/\phi(z)$, and the inverse transfer function is $A(z)^{-1}=\phi(z)/\theta(z)$. The [causality and invertibility root criteria for an ARMA model](../../../time-series.md#causality-and-invertibility-root-criteria-for-an-arma-model) require these respective rational functions to have power series about zero converging on a disk larger than the unit disk. If the two polynomials have no common factor, the conditions become

$$
\boxed{\phi(z)\ne0\text{ for }|z|\leq1\quad\text{(causality)},\qquad
\theta(z)\ne0\text{ for }|z|\leq1\quad\text{(invertibility)}.}
$$

Indeed, outside-disk roots leave a radius of convergence greater than one, so the coefficients decay geometrically and are absolutely summable. Conversely an uncancelled pole inside or on the unit disk prevents the required stable power series. If factors are common, apply the criterion after cancellation, to the noise-driven solution rather than additional homogeneous components. The [backshift operator](../../../time-series.md#backshift-operator) translates these power series into the desired one-sided filters.

The original representation has $\phi(z)=1-2z$ and $\theta(z)=1+2z$, with roots $1/2$ and $-1/2$. There is no cancellation. Hence **it is neither causal nor invertible** relative to its specified driving noise. [Stationarity](../../../time-series.md#stationary-process) is nevertheless possible through a two-sided solution: expanding the autoregressive inverse in negative powers gives

$$
X_t=-\epsilon_t-2\sum_{j\geq1}2^{-j}\epsilon_{t+j}.
$$

This is an [anticausal time series](../../../time-series.md#anticausal-time-series) representation with square-summable coefficients.

To establish the alternative representation on the same process, define

$$
\eta_t=\frac{1-\tfrac12B}{1+\tfrac12B}X_t
=X_t+2\sum_{j\geq1}\left(-\frac12\right)^jX_{t-j}.
$$

The inverse of $1+\tfrac12B$ is a stable one-sided filter. For $|z|=1$, the identities $|1+2z|^2=4|1+z/2|^2$ and $|1-2z|^2=4|1-z/2|^2$ give

$$
\left|\frac{1-z/2}{1+z/2}\right|^2
\left|\frac{1+2z}{1-2z}\right|^2=1.
$$

The [time-series spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) of $X$ is $\sigma^2|1+2e^{-i\omega}|^2/(2\pi|1-2e^{-i\omega}|^2)$; therefore the defined $\eta$ has constant [time-series spectral density](../../../time-series.md#spectral-density-of-a-stationary-process) $\sigma^2/(2\pi)$. Its mean is zero, its [variance](../../../variance.md) is $\sigma^2$, and all its nonzero-lag [autocovariances](../../../time-series.md#autocovariance) vanish. It is thus [weak white noise](../../../time-series.md#weak-white-noise). Its definition directly gives

$$
\boxed{X_t=\frac12X_{t-1}+\frac12\eta_{t-1}+\eta_t.}
$$

This [root reflection of an ARMA representation](../../../time-series.md#root-reflection-of-an-arma-representation) has roots $2,-2$, so is causal and invertible. A constant spectrum proves whiteness, not independence of non-Gaussian coordinates; no Gaussian assumption is needed for the required [white noise](../../../time-series.md#white-noise) representation.

For [best linear prediction from an infinite past](../../../time-series.md#best-linear-prediction-from-an-infinite-past), let $\mathcal H_0$ be the closed linear span of $X_t$ with $t\leq0$. The causal representation expresses every such $X_t$ in present and past $\eta$ values, while invertibility puts every $\eta_t$ with $t\leq0$ in $\mathcal H_0$. In particular $\eta_1$ is orthogonal to $\mathcal H_0$. The representation at time one then gives the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection)

$$
\widehat X_1=\frac12X_0+\frac12\eta_0
=X_0-\frac12X_{-1}+\frac14X_{-2}-\cdots.
$$

Consequently **the best linear predictor and its error variance are**

$$
\boxed{\widehat X_1=\sum_{j\geq0}\left(-\frac12\right)^jX_{-j},\qquad
X_1-\widehat X_1=\eta_1,\qquad \operatorname{Var}(X_1-\widehat X_1)=\sigma^2.}
$$

Orthogonality proves optimality among linear predictors in the closed past span, without asserting that the predictor must be the conditional mean for a non-Gaussian process.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For a real [weakly stationary process](../../../time-series.md#weakly-stationary-process), extend its [autocovariance](../../../time-series.md#autocovariance) by $\gamma_{-k}=\gamma_k$. The exact [existence of a time-series spectral density](../../../time-series.md#existence-of-a-time-series-spectral-density) condition is that its [spectral measure of a stationary time series](../../../time-series.md#spectral-measure-of-a-stationary-time-series) be [absolutely continuous with respect to](../../../measure-theory.md#absolute-continuity-of-measures) [Lebesgue measure](../../../measure-theory.md#lebesgue-measure). Absolute summability $\gamma_0+2\sum_{k\geq1}|\gamma_k|<\infty$ is a useful sufficient condition, not a necessary one.

We use the conventional angular-frequency density on $[-\pi,\pi]$, restricted to $[0,\pi]$ by symmetry. Under the absolute-summability condition, the [Fourier series](../../../fourier-series.md) and its inverse relation are

$$
\boxed{f(\omega)=\frac1{2\pi}\left(\gamma_0+2\sum_{k\geq1}\gamma_k\cos(k\omega)\right),\qquad
\gamma_k=2\int_0^\pi f(\omega)\cos(k\omega)\,d\omega.}
$$

Thus $2\int_0^\pi f=\gamma_0$. If a one-sided density is instead normalized to integrate to the full [variance](../../../variance.md), use $g=2f$ and omit the factor two in the inverse formula. This is the [positive-frequency spectral normalization](../../../time-series.md#positive-frequency-spectral-normalization) convention difference. With merely an integrable spectral density, the inverse relation remains valid; one must not assume pointwise convergence of the unweighted Fourier series. Its [Fejér sums](../../../fourier-series.md#fejer-sum) recover the density in $L^1$:

$$
f_N(\omega)=\frac1{2\pi}\left[\gamma_0+2\sum_{k=1}^N\left(1-\frac{k}{N+1}\right)\gamma_k\cos(k\omega)\right]\longrightarrow f.
$$

If $X$ and $Y$ are [independent](../../../random-variable.md#independent-random-variables) stationary processes, the cross [covariances](../../../variance.md#covariance) vanish, so

$$
\gamma_Z(k)=\operatorname{Cov}(X_{t+k}+Y_{t+k},X_t+Y_t)=\gamma_X(k)+\gamma_Y(k).
$$

Linearity of the inverse [Fourier series](../../../fourier-series.md) relation, or addition of the [spectral measures of a stationary time series](../../../time-series.md#spectral-measure-of-a-stationary-time-series), gives **$f_Z=f_X+f_Y$**. Independence can in fact be weakened to zero cross-covariances at every lag.

For the [ARMA](../../../time-series.md#autoregressive-moving-average-model)$(1,1)$ representation, away from an uncancelled unit root the transfer function gives

$$
\boxed{f_X(\omega)=\frac v{2\pi}\frac{1+\theta^2+2\theta\cos\omega}{1+\phi^2-2\phi\cos\omega}.}
$$

The usual causal case has $|\phi|<1$; the same expression holds for the two-sided stationary solution when $|\phi|>1$. We work in the nondegenerate case $v,w>0$ and $\phi\ne\pm1$; cancellations and zero-noise cases are obtained by the appropriate reduced representation or limits. Since [independent](../../../random-variable.md#independent-random-variables) [white noise](../../../time-series.md#white-noise) of [variance](../../../variance.md) $w$ contributes $w/(2\pi)$, put

$$
A=v(1+\theta^2)+w(1+\phi^2),\qquad C=v\theta-w\phi.
$$

Then

$$
\boxed{f_Z(\omega)=\frac1{2\pi}\frac{A+2C\cos\omega}{1+\phi^2-2\phi\cos\omega}.}
$$

The [white-noise addition to an ARMA(1,1) process](../../../time-series.md#white-noise-addition-to-an-arma-1-1-process) problem is therefore the factorization

$$
A+2C\cos\omega=\lambda(1+\alpha^2+2\alpha\cos\omega).
$$

Define

$$
P=A+2C=v(1+\theta)^2+w(1-\phi)^2,\qquad
Q=A-2C=v(1-\theta)^2+w(1+\phi)^2.
$$

Both are positive under the stated nondegeneracy conditions. An invertible choice is

$$
\boxed{\alpha=\frac{\sqrt P-\sqrt Q}{\sqrt P+\sqrt Q},\qquad
\lambda=\frac{(\sqrt P+\sqrt Q)^2}{4}.}
$$

These satisfy $|\alpha|<1$, $\lambda(1+\alpha)^2=P$, and $\lambda(1-\alpha)^2=Q$. Hence

$$
\boxed{\left(\frac{1+\alpha}{1-\alpha}\right)^2=
\frac{v(1+\theta)^2+w(1-\phi)^2}{v(1-\theta)^2+w(1+\phi)^2}.}
$$

In particular, it is the autoregressive coefficient $\phi$ that enters the terms from the added observation noise.

To obtain a representation of the actual $Z$, define

$$
\xi_t=(1+\alpha B)^{-1}(1-\phi B)Z_t.
$$

The stable inverse exists because $|\alpha|<1$, and spectral filtering gives $f_\xi=\lambda/(2\pi)$. Thus $\xi$ is [weak white noise](../../../time-series.md#weak-white-noise), and

$$
\boxed{Z_t=\phi Z_{t-1}+\alpha\xi_{t-1}+\xi_t.}
$$

Its [variance](../../../variance.md) can equivalently be written

$$
\boxed{\lambda=\frac{v(1+\theta^2)+w(1+\phi^2)}{1+\alpha^2}
=\frac{A+\sqrt{A^2-4C^2}}2.}
$$

When $\alpha\ne0$, also $\lambda=(v\theta-w\phi)/\alpha$; when $\alpha=0$, necessarily $C=0$ and $\lambda=A$, so the latter quotient should not be used. The model may reduce in order through cancellation. Boundary limits with $P=0$ or $Q=0$ give $|\alpha|=1$ and need not be stably invertible; the displayed stable reconstruction applies to the nondegenerate case above.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

For the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform), draw [independent](../../../random-variable.md#independent-random-variables) $U,V$ from the [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$ and set

$$
R=\sqrt{-2\log U},\qquad \Theta=2\pi V,\qquad
\boxed{G_1=R\cos\Theta,\quad G_2=R\sin\Theta.}
$$

The radial density is $r e^{-r^2/2}$ for $r>0$, with an [independent](../../../random-variable.md#independent-random-variables) uniform angle. The polar-to-Cartesian [Jacobian determinant](../../../calculus.md#jacobian-determinant) is $r$, so the joint density of $(G_1,G_2)$ is

$$
\frac1{2\pi}\exp\left[-\frac{g_1^2+g_2^2}{2}\right]
=\frac{e^{-g_1^2/2}}{\sqrt{2\pi}}\frac{e^{-g_2^2/2}}{\sqrt{2\pi}}.
$$

This factorization proves that both outputs have the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution) and are [independent](../../../random-variable.md#independent-random-variables). Repeating the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform) with fresh [independent](../../../random-variable.md#independent-random-variables) uniform pairs gives [independent](../../../random-variable.md#independent-random-variables) normal outputs; discard one extra output if the desired sample size is odd.

For the prescribed binary probabilities, generate [independent](../../../random-variable.md#independent-random-variables) standard normal values $G_i$ in this way and use

$$
\boxed{Y_i=\mathbf1_{\{G_i\leq x_i\}}.}
$$

The [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function) gives $\mathbb P(Y_i=1)=\Phi(x_i)$, and [independence](../../../random-variable.md#independent-random-variables) is preserved because each threshold uses a different [independent](../../../random-variable.md#independent-random-variables) normal value.

For the [probit regression](../../../statistical-modelling.md#probit-model) posterior, introduce latent variables

$$
Z_i=\beta x_i+G_i,\qquad Y_i=\mathbf1_{\{Z_i>0\}}.
$$

Given $\beta$, these are [independent](../../../random-variable.md#independent-random-variables) $N(\beta x_i,1)$ variables, and normal symmetry gives $\mathbb P(Z_i>0\mid\beta)=\Phi(\beta x_i)$. Thus this [data augmentation](../../../statistical-inference.md#data-augmentation) has exactly the observed binary [likelihood](../../../statistical-modelling.md#likelihood-function). With the specified normal [prior distribution](../../../statistical-inference.md#prior-probability), the augmented joint [posterior](../../../statistical-inference.md#bayesian-posterior) is proportional to

$$
\exp\left[-\frac{\beta^2}{2}-\frac12\sum_i(z_i-\beta x_i)^2\right]
\prod_i\mathbf1_{\{z_i>0\text{ if }y_i=1;\ z_i\leq0\text{ if }y_i=0\}}.
$$

The [latent-normal Gibbs sampler for probit regression](../../../statistical-modelling.md#latent-normal-gibbs-sampler-for-probit-regression) alternates two blocks. First, given the current $\beta$, draw each $Z_i$ independently from its [truncated normal distribution](../../../probability-theory.md#truncated-normal-distribution), namely $N(\beta x_i,1)$ restricted to the sign fixed by $y_i$. One exact method is to use the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform) for $G_i$, form $\beta x_i+G_i$, and reject until the sign is correct. The probability of success is positive at every finite parameter value, so the method is valid, although it can be slow for a rare sign.

For direct [sign-truncated normal sampling](../../../probability-theory.md#sign-truncated-normal-sampling), let $\mu_i=\beta x_i$, $a_i=\Phi(-\mu_i)$ and draw $U_i\sim\operatorname{Unif}(0,1)$. An [inverse transform sampling](../../../probability-theory.md#inverse-transform-sampling) implementation is

$$
\boxed{Z_i=\mu_i+\Phi^{-1}(a_i+(1-a_i)U_i)\quad(y_i=1),\qquad
Z_i=\mu_i+\Phi^{-1}(a_iU_i)\quad(y_i=0).}
$$

Use suitable tail or survival-function evaluations when floating-point probabilities approach zero or one; the rejection construction remains a valid alternative.

Second, completing the square in $\beta$ yields its [full conditional distribution](../../../probability-theory.md#full-conditional-distribution):

$$
\boxed{\beta\mid z,y\sim N\left(\frac{\sum_i x_i z_i}{1+\sum_i x_i^2},\ \frac1{1+\sum_i x_i^2}\right).}
$$

Generate a fresh standard normal value by the [Box-Muller transform](../../../probability-and-statistics.md#box-muller-transform), multiply by the conditional standard deviation, and add the conditional mean. Start from any finite $\beta$, alternate these steps, discard an initial transient and use the retained $\beta$ values to approximate its [posterior distribution](../../../statistical-inference.md#bayesian-posterior). These are dependent [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) samples, rather than [independent](../../../random-variable.md#independent-random-variables) posterior draws. Each block is an exact [Gibbs sampling](../../../statistical-inference.md#gibbs-sampler) update for the augmented [posterior](../../../statistical-inference.md#bayesian-posterior), whose marginal in $\beta$ is the requested posterior.

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The [reversible-jump Markov chain Monte Carlo](../../../statistical-inference.md#reversible-jump-markov-chain-monte-carlo) state comprises the model index and that model's parameter. Its unnormalized posterior density in model $j$ is

$$
h_j(\theta)=\varpi_j p_j(x\mid\theta)\pi_j(\theta).
$$

For models of equal dimension, choose model $k\ne j$ with probability $s_{jk}(\theta)$ and propose $\theta'$ using density $q_{jk}(\theta'\mid\theta)$ on the destination parameter space. The [equal-dimension reversible-jump acceptance probability](../../../statistical-inference.md#equal-dimension-reversible-jump-acceptance-probability) is

$$
\boxed{a((j,\theta),(k,\theta'))=
\min\left\{1,\frac{h_k(\theta')s_{kj}(\theta')q_{kj}(\theta\mid\theta')}
{h_j(\theta)s_{jk}(\theta)q_{jk}(\theta'\mid\theta)}\right\}.}
$$

On acceptance change both model and parameter; on rejection retain both. Choose model proposals connecting all models of positive posterior mass and within-model kernels exploring their supports, with aperiodicity, to obtain an ergodic chain. Include within-model updates targeting its conditional [posterior](../../../statistical-inference.md#bayesian-posterior), and use model occupation proportions after the initial transient to estimate [posterior](../../../statistical-inference.md#bayesian-posterior) model probabilities. The formula includes the model [prior probabilities](../../../statistical-inference.md#prior-probability), parameter [prior densities](../../../statistical-inference.md#prior-density), [likelihoods](../../../statistical-modelling.md#likelihood-function), reverse model-selection probability, and reverse parameter-proposal density.

This direct-density formula is [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm) on a disjoint union of equal-dimensional spaces. If instead a move uses a deterministic bijection $T:(\theta,u)\mapsto(\theta',u')$ with auxiliary proposal densities $g_{jk}(u\mid\theta)$ and $g_{kj}(u'\mid\theta')$, use

$$
\min\left\{1,\frac{h_k(\theta')s_{kj}(\theta')g_{kj}(u'\mid\theta')}
{h_j(\theta)s_{jk}(\theta)g_{jk}(u\mid\theta)}
\left|\det\frac{\partial(\theta',u')}{\partial(\theta,u)}\right|\right\}.
$$

The [Jacobian determinant](../../../calculus.md#jacobian-determinant) is one for identity matching, but equal model dimensions alone do not make a nonlinear map volume-preserving. For a direct proposal density the change of variables is already included in that density, so no additional Jacobian factor is inserted.

For the two Poisson models, use the shape-rate convention for the [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution):

$$
\pi(g)=\frac{b^a}{\Gamma(a)}g^{a-1}e^{-bg},\qquad g>0.
$$

If $b$ denotes scale instead, replace every occurrence of the rate $b$ below by $1/b$. Introduce the inactive $\gamma_2$ under model $2$ with the proper [pseudo-prior](../../../statistical-inference.md#pseudo-prior) $\pi(\gamma_2)$, [independent](../../../random-variable.md#independent-random-variables) of $\gamma_1$. This [pseudo-prior augmentation for model comparison](../../../statistical-inference.md#pseudo-prior-augmentation-for-model-comparison) does not change model $2$'s marginal likelihood because the inactive density integrates to one. The two augmented targets on the same positive quadrant are

$$
h_1=\tfrac12 L_1(\gamma_1,\gamma_2)\pi(\gamma_1)\pi(\gamma_2),\qquad
h_2=\tfrac12 L_2(\gamma_1)\pi(\gamma_1)\pi(\gamma_2),
$$

where

$$
L_1=\frac{e^{-(\gamma_1+\gamma_2)}\gamma_1^{x_1}\gamma_2^{x_2}}{x_1!x_2!},\qquad
L_2=\frac{e^{-2\gamma_1}\gamma_1^{x_1+x_2}}{x_1!x_2!}.
$$

Use a symmetric cross-model proposal that flips the model label and leaves both parameters unchanged. The matching map is the identity, with unit [Jacobian determinant](../../../calculus.md#jacobian-determinant), and the common prior factors cancel. Hence the **model-switch acceptance probabilities** are

$$
\boxed{a_{1\to2}=\min\left\{1,e^{\gamma_2-\gamma_1}\left(\frac{\gamma_1}{\gamma_2}\right)^{x_2}\right\},\qquad
a_{2\to1}=\min\left\{1,e^{\gamma_1-\gamma_2}\left(\frac{\gamma_2}{\gamma_1}\right)^{x_2}\right\}.}
$$

Only the second observation's factor changes because $\gamma_1$ is retained as its shared candidate mean. Evaluate the ratio on a logarithmic scale as $\gamma_2-\gamma_1+x_2(\log\gamma_1-\log\gamma_2)$ for the first direction.

For within-model moves, [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy) gives exact [Gibbs sampling](../../../statistical-inference.md#gibbs-sampler) refreshes:

$$
\begin{aligned}
M_1:\quad&\gamma_1\mid x\sim\operatorname{Gamma}(a+x_1,b+1),\quad
\gamma_2\mid x\sim\operatorname{Gamma}(a+x_2,b+1),\\
M_2:\quad&\gamma_1\mid x\sim\operatorname{Gamma}(a+x_1+x_2,b+2),\quad
\gamma_2\mid x\sim\operatorname{Gamma}(a,b).
\end{aligned}
$$

The two draws are conditionally [independent](../../../random-variable.md#independent-random-variables) within either model. Choose with fixed positive probabilities between this block refresh and the cross-model proposal. Both moves preserve the augmented [posterior](../../../statistical-inference.md#bayesian-posterior); refreshing the inactive parameter maintains its correct distribution and supports mixing. **The fraction of retained states labelled $M_j$ estimates $\mathbb P(M_j\mid x)$**.

An equivalent literal dimension-changing implementation deletes $\gamma_2$ on a proposed $1\to2$ move, and on a $2\to1$ move draws an auxiliary $u\sim\operatorname{Gamma}(a,b)$ and sets $\gamma_2=u$. The birth matching has $1+1=2+0$ dimensions and unit [Jacobian determinant](../../../calculus.md#jacobian-determinant). Its proposal density cancels the new parameter's prior density, giving the same acceptance ratios above for symmetric selection of move directions. This provides suitable moves without storing an inactive parameter.

For an independent check of [Poisson mean equality model comparison](../../../statistical-inference.md#poisson-mean-equality-model-comparison), the exact [Bayes factor](../../../statistical-inference.md#bayes-factor) is

$$
\frac{m_2(x)}{m_1(x)}=
\frac{\Gamma(a+x_1+x_2)\Gamma(a)}{\Gamma(a+x_1)\Gamma(a+x_2)}
\frac{(b+1)^{2a+x_1+x_2}}{b^a(b+2)^{a+x_1+x_2}}.
$$

It follows by integrating the two gamma likelihood kernels; the common factorial terms cancel. With equal model priors, the exact posterior probability of $M_2$ is $m_2/(m_1+m_2)$, which can also be used to check the [RJ-MCMC](../../../statistical-inference.md#reversible-jump-markov-chain-monte-carlo) occupation estimate.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2013](../../2013.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
