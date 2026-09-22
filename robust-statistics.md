# Robust statistics

↑ **Parent:** [Statistical inference](statistical-inference.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Robust_statistics)

Robust statistics studies procedures whose behavior remains controlled under outliers and deviations from an assumed model.

**Table of contents**

- [Translation-invariant estimator](#translation-invariant-estimator)
- [Minimax asymptotic bias](#minimax-asymptotic-bias)
- [Trimmed mean](#trimmed-mean)
  - [Influence function of a trimmed mean](#influence-function-of-a-trimmed-mean)
- [M-estimator](#m-estimator)
  - [Sandwich variance of an M-estimator](#sandwich-variance-of-an-m-estimator)
  - [Argmin consistency under uniform convergence in probability](#argmin-consistency-under-uniform-convergence-in-probability)
    - [Global argmin may escape a compact convergence set](#global-argmin-may-escape-a-compact-convergence-set)
  - [Scale M-estimator](#scale-m-estimator)
- [Catoni mean estimator](#catoni-mean-estimator)
- [B-robust estimator](#b-robust-estimator)
- [Contamination (statistics)](#contamination-statistics)
  - [Kolmogorov neighborhood of a distribution](#kolmogorov-neighborhood-of-a-distribution)
  - [Epsilon-contamination neighborhood](#epsilon-contamination-neighborhood)
    - [Huber contamination](#huber-contamination)
- [Influence function](#influence-function)
  - [Influence function of the mean](#influence-function-of-the-mean)
  - [Influence function of a Huber location estimator](#influence-function-of-a-huber-location-estimator)
  - [Normal-location influence curves](#normal-location-influence-curves)
  - [Finite contamination bias of normal location](#finite-contamination-bias-of-normal-location)
  - [Local influence versus replacement breakdown](#local-influence-versus-replacement-breakdown)
  - [Rejection point of an influence function](#rejection-point-of-an-influence-function)
  - [Local-shift sensitivity](#local-shift-sensitivity)
  - [Influence function of a quantile](#influence-function-of-a-quantile)
  - [Empirical influence function](#empirical-influence-function)
  - [Sensitivity curve](#sensitivity-curve)
  - [One-step estimator](#one-step-estimator)
  - [Asymptotic linear representation](#asymptotic-linear-representation)
  - [Gross-error sensitivity](#gross-error-sensitivity)
  - [Influence function of the sample median](#influence-function-of-the-sample-median)
- [Breakdown point](#breakdown-point)
  - [Finite-sample maximum bias](#finite-sample-maximum-bias)
  - [Replacement breakdown point](#replacement-breakdown-point)
- [Huber location estimator](#huber-location-estimator)
  - [Huber location response to one outlier](#huber-location-response-to-one-outlier)
  - [Huber score](#huber-score)
    - [Optimal bounded influence function for normal location](#optimal-bounded-influence-function-for-normal-location)
  - [Huber loss](#huber-loss)
    - [Huber gradient regularizer](#huber-gradient-regularizer)
- [Median-of-means estimator](#median-of-means-estimator)
- [Tukey median](#tukey-median)
- [Asymptotic distribution of a sample median](#asymptotic-distribution-of-a-sample-median)

## Translation-invariant estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)

A location estimator $T_n$ is translation-invariant when

$$
T_n(x_1+a,\ldots,x_n+a)=T_n(x_1,\ldots,x_n)+a
$$

for every real shift $a$.

## Minimax asymptotic bias

↑ **Parent:** [Robust statistics](robust-statistics.md)

The minimax asymptotic-bias problem chooses an estimator to minimize its largest limiting bias over a specified neighborhood of a reference distribution.

## Trimmed mean

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trimmed_mean)

The $\alpha$-trimmed mean deletes the smallest and largest $\lfloor\alpha n\rfloor$ observations and averages the rest. Its population functional is

$$
T(F)=\frac1{1-2\alpha}\int_\alpha^{1-\alpha}F^{-1}(s)\,ds.
$$

### Influence function of a trimmed mean

↑ **Parent:** [Trimmed mean](#trimmed-mean)

At a differentiable distribution symmetric about zero, put $k=-F^{-1}(\alpha)$. The influence function of the $\alpha$-trimmed mean is

$$
\operatorname{IF}(x;T,F)
=\frac{\max(-k,\min(x,k))}{1-2\alpha}.
$$

## M-estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/M-estimator)

An M-estimator minimizes an empirical objective $\sum_i\rho(x_i,\theta)$ or, when differentiable, solves an estimating equation $\sum_i\psi(x_i,\theta)=0$.

### Sandwich variance of an M-estimator

↑ **Parent:** [M-estimator](#m-estimator)

For an estimating equation with population root $\theta=T(F)$, let $A=\mathbb E_F\partial_\theta\psi(X,\theta)$ be nonsingular and $B=\mathbb E_F[\psi\psi^T]$. Differentiating the contaminated population equation gives [influence function](#influence-function) $-A^{-1}\psi(x,\theta)$. A consistent sample root with differentiable local expansion satisfies $\sqrt n(\widehat\theta-\theta)=-A^{-1}n^{-1/2}\sum_i\psi(X_i,\theta)+o_p(1)$, so the [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) gives the displayed [covariance](variance.md#covariance). In the scalar case this is $\mathbb E\psi^2/A^2$.

### Argmin consistency under uniform convergence in probability

↑ **Parent:** [M-estimator](#m-estimator)

On a compact parameter set, a continuous deterministic objective with a unique minimum has a positive separation gap outside each neighbourhood of its [minimizer](analysis.md#global-minimizer). [Uniform convergence in probability](convergence-of-random-variables.md#uniform-convergence-in-probability) of the random objectives bounds the deterministic objective difference at any attained random [minimizer](analysis.md#global-minimizer) by twice the supremum discrepancy. This proves [statistical consistency](statistical-inference.md#consistency-statistics) of each measurable minimizing selection.

#### Global argmin may escape a compact convergence set

↑ **Parent:** [Argmin consistency under uniform convergence in probability](#argmin-consistency-under-uniform-convergence-in-probability)

[Uniform convergence in probability](convergence-of-random-variables.md#uniform-convergence-in-probability) of empirical criteria on a compact set proves consistency for minimizers in that set; it does not confine a minimizer over a larger domain. A bounded identifiable regression function can approach its true value again at infinity. For median regression, $a(\theta)=\theta^2/(1+\theta^4)$ has unique zero at zero, but a small positive fitted [sample median](probability-distribution.md#sample-median) $c$ has a second solution $\theta^2=(1+\sqrt{1-4c^2})/(2c)$. This solution diverges as $c\downarrow0$, although uniform convergence on any fixed compact interval holds. Constraining the estimator, or proving suitable global separation and localization, repairs the argument.

### Scale M-estimator

↑ **Parent:** [M-estimator](#m-estimator)

A scale M-estimator solves an equation of the form

$$
\sum_{i=1}^n\psi(x_i/t)=0
$$

for a positive scale $t$.

## Catoni mean estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)

A Catoni mean estimator replaces each scaled observation by a nondecreasing influence function whose exponential envelope is controlled by a quadratic. This yields sub-Gaussian deviation bounds assuming only a finite variance.

## B-robust estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)

A B-robust estimator has bounded [influence function](#influence-function), equivalently finite [gross-error sensitivity](#gross-error-sensitivity), at the reference distribution.

## Contamination (statistics)

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Contamination_(statistics))

Statistical contamination replaces part of an ideal distribution or sample by arbitrary observations.

### Kolmogorov neighborhood of a distribution

↑ **Parent:** [Contamination (statistics)](#contamination-statistics)

The Kolmogorov $\varepsilon$-neighborhood of a cumulative distribution function $F$ consists of all distribution functions $G$ satisfying

$$
\sup_t|G(t)-F(t)|\leq\varepsilon.
$$

### Epsilon-contamination neighborhood

↑ **Parent:** [Contamination (statistics)](#contamination-statistics)

The epsilon-contamination neighborhood of $P$ is the class $\{(1-\epsilon)P+\epsilon Q:Q\text{ is a probability distribution}\}$.

#### Huber contamination

↑ **Parent:** [Epsilon-contamination neighborhood](#epsilon-contamination-neighborhood)

Huber contamination is the epsilon-contamination model in which an arbitrary distribution contributes an unknown fraction of the observations.

## Influence function

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Influence_function)

An [influence function](#influence-function) asks how much a population answer moves when an infinitesimal fraction of its [probability distribution](probability-distribution.md) is relocated to a specified point. It distinguishes the unbounded response of the [mean](expected-value.md) from the bounded response of the [median](probability-distribution.md#median) and the [Huber location estimator](#huber-location-estimator). The [normal-location influence curves](#normal-location-influence-curves) and [finite contamination bias of normal location](#finite-contamination-bias-of-normal-location) below make that difference quantitative.

Let $T$ be a real-valued [statistical functional](statistical-inference.md#statistical-functional), $F$ a reference [probability measure](probability-space.md#probability-measure), and $\delta_x$ the [Dirac measure](measure.md#dirac-measure) concentrated at $x$. Along the [epsilon-contamination neighborhood](#epsilon-contamination-neighborhood) path $F_{\varepsilon,x}=(1-\varepsilon)F+\varepsilon\delta_x$, define the right [derivative](calculus.md#derivative)

$$
\operatorname{IF}(x;T,F)=\lim_{\varepsilon\downarrow0}\frac{T(F_{\varepsilon,x})-T(F)}{\varepsilon},\qquad
T(F_{\varepsilon,x})=T(F)+\varepsilon\operatorname{IF}(x;T,F)+o(\varepsilon).
$$

The name [influence curve](#influence-function) refers to the same object. The [derivative](calculus.md#derivative) is in the signed direction $\delta_x-F$, so the calculation removes baseline mass as well as adding a [Dirac measure](measure.md#dirac-measure). The definition is a [limit](calculus.md#limit-of-a-function) for each fixed $x$; it does not automatically give a remainder uniform over arbitrarily distant $x$.[Frank R. Hampel, The Influence Curve and Its Role in Robust Estimation, p. 383, §2: pointwise right-limit definition along mixtures with a point mass](mathematics-bibliography.md#the-influence-curve-and-its-role-in-robust-estimation-by-frank-r-hampel)

The [statistical functional](statistical-inference.md#statistical-functional) must be defined on these contaminated [probability measures](probability-space.md#probability-measure), and the right [derivative](calculus.md#derivative) must exist and be finite. For a [mean](expected-value.md), a finite first absolute [moment](expected-value.md#moment) suffices. For a [median](probability-distribution.md#median), require a unique baseline [median](probability-distribution.md#median) and a [probability density function](continuous-probability-distribution.md#probability-density-function) continuous and strictly positive there. For a smooth [M-estimator](#m-estimator), require an isolated population root, justified differentiation of its [expected value](expected-value.md), and a nonzero derivative with respect to the fitted parameter. These are specific conditions for the formulas below. Existence of the pointwise [influence function](#influence-function) alone proves neither an [asymptotic linear representation](#asymptotic-linear-representation) nor [pathwise differentiability of a statistical functional](statistical-inference.md#pathwise-differentiability-of-a-statistical-functional); each needs control of its own remainder and admissible [statistical paths](statistical-model.md#statistical-path).

### Influence function of the mean

↑ **Parent:** [Influence function](#influence-function)

For the [statistical functional](statistical-inference.md#statistical-functional) $T(F)=\mu=\mathbb E_F X$, assuming $\mathbb E_F|X|<\infty$, the contaminated [mean](expected-value.md) is exactly

$$
T(F_{\varepsilon,x})=(1-\varepsilon)\mu+\varepsilon x.
$$

Thus the [influence function of the mean](#influence-function-of-the-mean) is $x-\mu$, and its [gross-error sensitivity](#gross-error-sensitivity) is infinite on an unbounded sample space. The [linear approximation](calculus.md#linear-approximation) is exact here: any fixed positive contamination fraction allows an arbitrarily large change by moving $x$ far enough. No finite second [moment](expected-value.md#moment) is needed for this [derivative](calculus.md#derivative), although a finite [variance](variance.md) is needed for the usual [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) for the [sample mean](variance.md#sample-mean).

For comparison, the [influence function of the sample median](#influence-function-of-the-sample-median) is

$$
\operatorname{IF}(x;\operatorname{Med},F)=\frac{\operatorname{sgn}(x-m)}{2f(m)},\qquad x\ne m,
$$

when the [median](probability-distribution.md#median) $m$ is unique and the [probability density function](continuous-probability-distribution.md#probability-density-function) $f$ is positive and continuous at $m$. The [sign function](foundations-of-mathematics.md#sign-function) records which side of $m$ receives the contaminating mass. The [influence function of a quantile](#influence-function-of-a-quantile) supplies the short derivation. With the generalized-inverse [quantile](probability-distribution.md#quantile-function) convention, contamination exactly at $x=m$ leaves the [median](probability-distribution.md#median) at $m$, giving derivative zero there. If $f(m)$ is very small, this bounded [influence function](#influence-function) can still be large; if $f(m)=0$, the displayed formula is unavailable.

### Influence function of a Huber location estimator

↑ **Parent:** [Influence function](#influence-function)

Fix a scale $s>0$ and cutoff $k>0$. Define the population [Huber location estimator](#huber-location-estimator) by the root

$$
\mathbb E_F\psi_k\!\left(\frac{X-\theta}{s}\right)=0,\qquad \theta=T(F),\qquad
A=\mathbb E_F\psi_k'\!\left(\frac{X-\theta}{s}\right)>0.
$$

Here $\psi_k$ is the [Huber score](#huber-score). It has [Lipschitz continuity](real-analysis.md#lipschitz-continuity), so [dominated convergence](measure-theory.md#dominated-convergence-theorem) justifies differentiation when $F$ puts no mass at $\theta\pm ks$. Then $A=\mathbb P_F(|X-\theta|<ks)$, and the nonzero derivative identifies the local population root. The [implicit function theorem](multivariable-calculus.md#implicit-function-theorem) applies away from the contaminating score's kinks; its [Lipschitz continuity](real-analysis.md#lipschitz-continuity) also gives the first-order expansion at those kinks. Differentiating its contaminated equation yields

$$
0=-\frac A s\operatorname{IF}(x;T,F)+\psi_k\!\left(\frac{x-\theta}{s}\right),\qquad
\operatorname{IF}(x;T,F)=\frac{s\psi_k((x-\theta)/s)}{A}.
$$

The normalization matters: the [Huber score](#huber-score) alone is not the [influence function](#influence-function). The [gross-error sensitivity](#gross-error-sensitivity) is $sk/A$, while the [rejection point of an influence function](#rejection-point-of-an-influence-function) is infinite because the clipped tails stay nonzero. The original clipped estimating criterion and its derivative normalization also appear in the population analysis of [M-estimators](#m-estimator).[Peter J. Huber, Robust Estimation of a Location Parameter, §3, p. 78: derivative normalization; §4(iii), p. 79: clipped location criterion and central-mass denominator](mathematics-bibliography.md#robust-estimation-of-a-location-parameter-by-peter-j-huber)

Scale sets what counts as a large residual. For a [normal distribution](probability-distribution.md#normal-distribution) $N(\mu,\sigma^2)$ with fixed $s=\sigma$, [symmetry](physics.md#symmetry-physics) gives $\theta=\mu$ and $A=2\Phi(k)-1$, where $\Phi$ is the [standard normal distribution function](probability-distribution.md#standard-normal-distribution-function). If the scale is instead a [statistical functional](statistical-inference.md#statistical-functional) $S(F)$, differentiation of the joint equation adds the scale contribution:

$$
\operatorname{IF}(x;T,F)=\frac{s\psi_k(r_x)-B\operatorname{IF}(x;S,F)}{A},\qquad
r_x=\frac{x-\theta}{s},\quad B=\mathbb E_F\left[r_X\psi_k'(r_X)\right].
$$

Under a symmetric baseline and an odd [Huber score](#huber-score), $B=0$, so scale estimation drops out at first order. This cancellation needs regularity of $S$ and does not protect finite [contamination](#contamination-statistics) changes: an inflated [standard deviation](variance.md#standard-deviation) enlarges the physical cutoff $ks$. A robust choice, such as a suitable [Scale M-estimator](#scale-m-estimator), needs its own [influence function](#influence-function) and [breakdown point](#breakdown-point) checked. Fixing a numeric cutoff in raw units also sacrifices scale [equivariance](group-action.md#equivariant-map) when units change.[Peter J. Huber, Robust Estimation of a Location Parameter, §11, pp. 95-96: estimating location when normal-component scale and contamination fraction are unknown](mathematics-bibliography.md#robust-estimation-of-a-location-parameter-by-peter-j-huber)

### Normal-location influence curves

↑ **Parent:** [Influence function](#influence-function)

For $F=N(\mu,\sigma^2)$, put $z=(x-\mu)/\sigma$. The [influence function of the mean](#influence-function-of-the-mean), [influence function of the sample median](#influence-function-of-the-sample-median), and [influence function of a Huber location estimator](#influence-function-of-a-huber-location-estimator) with fixed $s=\sigma$ are respectively

$$
\sigma z,\qquad \sigma\sqrt{\frac\pi2}\operatorname{sgn}(z),\qquad
\frac{\sigma\psi_k(z)}{2\Phi(k)-1}.
$$

The first grows without bound, the second jumps at the [median](probability-distribution.md#median), and the third clips continuously. For $k=1.345$, $2\Phi(k)-1\simeq0.821375$ and the normalized Huber tail is about $1.63750\sigma$. This illustrates the [optimal bounded influence function for normal location](#optimal-bounded-influence-function-for-normal-location) without asserting that this cutoff is optimal for every contamination model.

<a id="image-mean-median-and-normalized-huber-influence-curves-for-two-normal-location-scale-models"></a>
![](normal-location-influence-curves.png)

**[Figure 1](#image-mean-median-and-normalized-huber-influence-curves-for-two-normal-location-scale-models). Mean, median, and normalized Huber influence curves for two normal location-scale models**.

Both panels are theoretical [normal distributions](probability-distribution.md#normal-distribution), with no sampled or observed data. Doubling $\sigma$ doubles the vertical [influence function](#influence-function) scale and the horizontal clipping distance. Changing $\mu$ translates the curves. The isolated dot marks the actual [median](probability-distribution.md#median) derivative at the center; connecting its two tails by a vertical segment would misrepresent that value. Bounded influence does not mean every small residual has less effect than on the [mean](expected-value.md): the central Huber slope is $1/(2\Phi(k)-1)>1$, a price paid for reducing sensitivity in the tails.

### Finite contamination bias of normal location

↑ **Parent:** [Influence function](#influence-function)

Consider the population [statistical model](statistical-model.md) $F_{\varepsilon,x}=(1-\varepsilon)N(0,1)+\varepsilon\delta_x$. The following are deterministic [statistical functional](statistical-inference.md#statistical-functional) calculations, not observed contamination experiments. Compare the actual location bias with the [linear approximation](calculus.md#linear-approximation) $\varepsilon\operatorname{IF}(x;T,F)$. The [mean](expected-value.md) bias is exactly $\varepsilon x$. For positive $x$ exceeding the shifted [median](probability-distribution.md#median) and $0\le\varepsilon<1/2$, the generalized-inverse [median](probability-distribution.md#median) bias is exactly

$$
b_{\operatorname{Med}}(\varepsilon,x)=\Phi^{-1}\!\left(\frac{1}{2(1-\varepsilon)}\right).
$$

This formula applies to both $x=1$ and $x=8$ throughout the plotted interval $0\le\varepsilon\le0.1$. If the contaminating atom lies inside the [quantile](probability-distribution.md#quantile-function) jump containing probability $1/2$, the generalized-inverse [median](probability-distribution.md#median) instead equals that atom.

For the [Huber location estimator](#huber-location-estimator) with $s=1$ and $k=1.345$, solve its actual population equation, rather than substituting the [influence function](#influence-function):

$$
(1-\varepsilon)g_k(t)+\varepsilon\psi_k(x-t)=0,\qquad g_k(t)=\mathbb E\psi_k(Z-t),\quad Z\sim N(0,1).
$$

Writing $a=t-k$ and $b=t+k$, integration of the [normal distribution](probability-distribution.md#normal-distribution) gives

$$
g_k(t)=\phi(a)-\phi(b)-t\bigl[\Phi(b)-\Phi(a)\bigr]+k\bigl[1-\Phi(b)-\Phi(a)\bigr],
$$

where $\phi$ is the [probability density function](continuous-probability-distribution.md#probability-density-function) of $N(0,1)$. Its [derivative](calculus.md#derivative) is $-[\Phi(t+k)-\Phi(t-k)]<0$, so the mixture score is strictly decreasing for $\varepsilon<1$. For $\varepsilon<1/2$, its limits at negative and positive infinity have opposite signs even with arbitrary distant point contamination. The displayed examples use the unique root, evaluated by the [bisection method](numerical-analysis.md#bisection-method) to numerical precision.

<a id="image-exact-population-contamination-biases-and-first-order-influence-predictions-for-normal-location-at-contaminating-points-1-and-8"></a>
![](normal-location-contamination-bias.png)

**[Figure 2](#image-exact-population-contamination-biases-and-first-order-influence-predictions-for-normal-location-at-contaminating-points-1-and-8). Exact population contamination biases and first-order influence predictions for normal location at contaminating points 1 and 8**.

At $x=8$ and $\varepsilon=0.01$, the exact [mean](expected-value.md), [median](probability-distribution.md#median), and [Huber location estimator](#huber-location-estimator) biases are $0.080000$, $0.012660$, and $0.016541$; the [influence function](#influence-function) predictions are $0.080000$, $0.012533$, and $0.016375$. At $\varepsilon=0.05$, they become $0.400000$, $0.066012$, and $0.086241$, versus predictions $0.400000$, $0.062666$, and $0.081875$. The bounded alternatives control the effect of the distant atom, but their actual response curves bend away from the tangent.

The nearby atom $x=1$ gives a useful comparison: at $\varepsilon=0.05$, the [Huber location estimator](#huber-location-estimator) bias is $0.060237$, slightly below its [linear approximation](calculus.md#linear-approximation) $0.060874$, whereas the [median](probability-distribution.md#median) bias is still $0.066012$. The direction and size of approximation error depend on the contaminating location. Even accurate local influence calculations must specify $F$, the scale, the cutoff, and the actual contamination fraction.

### Local influence versus replacement breakdown

↑ **Parent:** [Influence function](#influence-function)

The [influence function](#influence-function) describes an infinitesimal change at a specified reference [probability distribution](probability-distribution.md). The [replacement breakdown point](#replacement-breakdown-point) asks how many observations in a particular finite sample can be replaced before an [estimator](statistical-modelling.md#estimator) becomes unbounded. The [finite-sample maximum bias](#finite-sample-maximum-bias) records the intervening changes. These are different questions: a bounded [influence function](#influence-function) at one baseline is not a general bound over all [epsilon-contamination neighborhoods](#epsilon-contamination-neighborhood), nor a proof of a positive [replacement breakdown point](#replacement-breakdown-point).[Frank R. Hampel, The Influence Curve and Its Role in Robust Estimation, §4, p. 386: exact asymptotic curve supplemented by behavior at other distributions, especially empirical ones](mathematics-bibliography.md#the-influence-curve-and-its-role-in-robust-estimation-by-frank-r-hampel)

The [mean](expected-value.md) illustrates agreement between local and global fragility: its [gross-error sensitivity](#gross-error-sensitivity) is infinite and one replacement can send the [sample mean](variance.md#sample-mean) arbitrarily far. The [median](probability-distribution.md#median) has finite [gross-error sensitivity](#gross-error-sensitivity) under the stated positive-density assumptions, while its [sample median](probability-distribution.md#sample-median) withstands fewer than about half the observations being replaced under ordinary tie conventions. Its population contamination bias above still diverges as $\varepsilon\uparrow1/2$ when the atom remains beyond the shifted [median](probability-distribution.md#median). Here $x$ must also move outward; taking that limit with a fixed finite atom would invalidate the displayed [quantile](probability-distribution.md#quantile-function) formula.

For scalar location with a fixed positive scale, the [Huber score](#huber-score) has a direct global argument: if strictly more than half of the sample stays fixed, then beyond every retained observation by more than $ks$, their saturated scores outweigh all possible replaced scores. Every root therefore stays in a bounded interval. This is a separate finite-replacement argument; estimating scale changes its premises. A smooth bounded [influence function](#influence-function) is valuable local protection, but global robustness also depends on the full estimating rule, scale choice, and root selection.

### Rejection point of an influence function

↑ **Parent:** [Influence function](#influence-function)

For observations expressed in centered, standardized coordinates, the rejection point is

$$
\rho^*(T,F)=\inf\{r\ge0:\operatorname{IF}(x;T,F)=0\text{ whenever }|x|>r\},
$$

with value $\infty$ if the set is empty. A finite rejection point means sufficiently distant contamination has zero first-order effect. Boundedness of the [influence function](#influence-function) does not imply a finite rejection point: the [influence function of a quantile](#influence-function-of-a-quantile) has nonzero constant tails. Nor does tending to zero at infinity guarantee a finite rejection point unless those tails become identically zero.

### Local-shift sensitivity

↑ **Parent:** [Influence function](#influence-function)

The local-shift sensitivity of a scalar [statistical functional](statistical-inference.md#statistical-functional) is

$$
\lambda^*(T,F)=\sup_{x\ne y}\frac{|\operatorname{IF}(x;T,F)-\operatorname{IF}(y;T,F)|}{|x-y|}.
$$

It measures the sensitivity of the first-order contamination effect to moving the contaminating observation. If the [influence function](#influence-function) is continuously differentiable with bounded derivative, the [mean value theorem](calculus.md#mean-value-theorem) gives $\lambda^*\le\sup_x|\operatorname{IF}'(x)|$, and taking $y\to x$ proves equality. A jump in the [influence function](#influence-function) makes $\lambda^*$ infinite, even when [gross-error sensitivity](#gross-error-sensitivity) is finite.

### Influence function of a quantile

↑ **Parent:** [Influence function](#influence-function)

Let $q$ be the unique $p$th [quantile](probability-distribution.md#quantile-function), with $0<p<1$, and suppose the [density](fluid-mechanics.md#density) $f$ is continuous and positive at $q$. Define quantiles of contaminated distributions using the generalized inverse. For $z\ne q$, differentiating $(1-\varepsilon)F(q_\varepsilon)+\varepsilon\mathbf1_{z\le q_\varepsilon}=p$ gives

$$
\operatorname{IF}(z;q_p,F)=\frac{p-\mathbf1_{z\le q}}{f(q)}.
$$

At $z=q$, the generalized-inverse quantile stays exactly $q$ under this contamination, so its derivative is zero. The step formula thus holds $F$-almost everywhere and determines the [asymptotic variance](statistical-modelling.md#asymptotic-variance) $p(1-p)/(nf(q)^2)$. Its [gross-error sensitivity](#gross-error-sensitivity) is $\max(p,1-p)/f(q)$, but its [local-shift sensitivity](#local-shift-sensitivity) is infinite because of the jump.

### Empirical influence function

↑ **Parent:** [Influence function](#influence-function)

This plugs the [empirical distribution](information-theory.md#type-information-theory) into the population [influence function](#influence-function). For an [M-estimator](#m-estimator) it is $-[n^{-1}\sum_i\partial_\theta\psi(y_i,T(F_n))]^{-1}\psi(z,T(F_n))$, when this denominator is well-defined and nonzero. For functionals involving a density at a quantile, an unsmoothed empirical measure may not permit this derivative, so smoothing or an actual [sensitivity curve](#sensitivity-curve) is required.

### Sensitivity curve

↑ **Parent:** [Influence function](#influence-function)

Add one observation $z$ to the empirical sample, so $F_{n+1,z}=\frac n{n+1}F_n+\frac1{n+1}\delta_z$. The displayed finite difference is a finite-sample counterpart of the [influence function](#influence-function). Its supremum magnitude measures worst-case one-observation sensitivity; unlike an infinitesimal derivative it records the actual response at contamination fraction $1/(n+1)$.

### One-step estimator

↑ **Parent:** [Influence function](#influence-function)

A one-step estimator starts from a plug-in estimate and adds the empirical mean of an estimated influence function. Under suitable nuisance-estimation and remainder conditions, this correction removes the plug-in estimator's first-order bias and produces an asymptotically linear estimator.

### Asymptotic linear representation

↑ **Parent:** [Influence function](#influence-function)

An estimator has an asymptotic linear representation with influence function $\psi$ when

$$
\sqrt n(\widehat\theta-\theta)
=\frac1{\sqrt n}\sum_{i=1}^n\psi(X_i)+o_p(1).
$$

### Gross-error sensitivity

↑ **Parent:** [Influence function](#influence-function)

Gross-error sensitivity is the supremum of the absolute influence function over contamination points.

### Influence function of the sample median

↑ **Parent:** [Influence function](#influence-function)

At a distribution with positive density $f$ at its median $m$, the median influence function is $\operatorname{sgn}(x-m)/(2f(m))$ away from $m$.

## Breakdown point

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Breakdown_point)

A breakdown point is the smallest contamination fraction capable of making an estimator arbitrarily unreliable.

### Finite-sample maximum bias

↑ **Parent:** [Breakdown point](#breakdown-point)

Here $d_H$ counts the observations replaced. This curve measures the largest change after at most $m$ arbitrary replacements. Under the first-unbounded convention, the [replacement breakdown point](#replacement-breakdown-point) is $n^{-1}\min\{m:b_n(m;y)=\infty\}$. The largest fraction still guaranteed bounded is one grid step smaller; those conventions must not be confused. A [sample mean](variance.md#sample-mean) breaks after one replacement, while a scalar [sample median](probability-distribution.md#sample-median) with a fixed ordinary tie convention needs about half the sample replaced.

### Replacement breakdown point

↑ **Parent:** [Breakdown point](#breakdown-point)

The finite-sample replacement breakdown point is the largest replacement fraction under which an estimator remains bounded over arbitrary replacement values.

## Huber location estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)

The Huber location estimator solves $\sum_i\psi_k(x_i-\theta)=0$, where $\psi_k$ clips its argument to $[-k,k]$.

More generally, fix a known scale $s>0$ and a dimensionless threshold $k>0$ before fitting. For observations $x_1,\ldots,x_n$, a [Huber location estimator](#huber-location-estimator) is a [minimizer](analysis.md#global-minimizer) of the summed [Huber loss](#huber-loss), equivalently a root of its [estimating equation](statistical-inference.md#estimating-equation):

$$
Q_{k,s}(\theta)=\sum_{i=1}^n\rho_k\!\left(\frac{x_i-\theta}{s}\right),\qquad
\widehat\theta_{k,s}\in\operatorname*{argmin}_{\theta\in\mathbb R}Q_{k,s}(\theta),\qquad
\sum_{i=1}^n\psi_k\!\left(\frac{x_i-\widehat\theta_{k,s}}s\right)=0.
$$

Here $\rho_k$ is the [Huber loss](#huber-loss) and $\psi_k$ the [Huber score](#huber-score). The physical clipping distance is $ks$, in the observations' units; the initial formula uses $s=1$. A large observation keeps contributing a bounded signed score rather than being discarded. The original clipped location criterion appears in [Peter J. Huber](mathematics-author.md#peter-j-huber)'s 1964 paper.[§4(iii), printed p. 79: quadratic-central, linear-tail criterion and clipping around the fitted location](mathematics-bibliography.md#robust-estimation-of-a-location-parameter-by-peter-j-huber)

For the original data $(0,1,2,3,4,40)$, take $s=1$ and $k=2$. At $\theta=2.5$, the standardized differences and their [Huber scores](#huber-score) are

$$
(x_i-2.5)_{i=1}^6=(-2.5,-1.5,-0.5,0.5,1.5,37.5),\qquad
(\psi_2(x_i-2.5))_{i=1}^6=(-2,-1.5,-0.5,0.5,1.5,2).
$$

Their sum is zero, so the [Huber location estimator](#huber-location-estimator) is $2.5$. Four scores remain in the central linear region, making the root unique. By comparison, the [sample mean](variance.md#sample-mean) is $50/6\simeq8.3333$, and the [sample median](probability-distribution.md#sample-median), using the midpoint of the two middle observations, is $(2+3)/2=2.5$. Agreement with the [sample median](probability-distribution.md#sample-median) is a feature of these data, rather than an identity between the two [estimators](statistical-modelling.md#estimator).

The geometry explains both existence and possible nonuniqueness. The [Huber loss](#huber-loss) is a [convex function](real-analysis.md#convex-function), so $Q_{k,s}$ is a [convex function](real-analysis.md#convex-function) of $\theta$ and its [derivative](calculus.md#derivative) is $-s^{-1}\sum_i\psi_k((x_i-\theta)/s)$. For $n\geq1$, $Q_{k,s}(\theta)$ tends to infinity as $|\theta|$ grows, hence attains a [minimum](set.md#minimum-of-a-subset-of-a-total-order); its zero [derivative](calculus.md#derivative) characterizes every [minimizer](analysis.md#global-minimizer). Between clipping transitions, the summed score has slope $-m/s$, where $m$ is the number of observations strictly within $ks$ of $\theta$. A root with $m>0$ is unique. If $m=0$, a flat interval is possible: for data $(0,10)$ with $s=1,k=2$, every $\theta\in[2,8]$ is a [minimizer](analysis.md#global-minimizer). A complete single-valued [estimator](statistical-modelling.md#estimator) then needs a selection rule, such as the interval's midpoint.

A bounded [Huber score](#huber-score) limits one observation's contribution to the [estimating equation](statistical-inference.md#estimating-equation). The [influence function of a Huber location estimator](#influence-function-of-a-huber-location-estimator) additionally divides by the population's central mass, so the size of its bound depends on the reference [probability distribution](probability-distribution.md). Clipping does not by itself make the [bias of an estimator](statistical-modelling.md#bias-of-an-estimator) zero or prove a universal [breakdown point](#breakdown-point); the separate [local influence versus replacement breakdown](#local-influence-versus-replacement-breakdown) argument specifies what fixed scale permits. Estimating $s$ from the same data changes the procedure and requires separate analysis.

### Huber location response to one outlier

↑ **Parent:** [Huber location estimator](#huber-location-estimator)

Hold $(0,1,2,3,4)$ fixed and move only the sixth observation $M$. For $M\geq5$, the [sample mean](variance.md#sample-mean) is $(10+M)/6$, the [sample median](probability-distribution.md#sample-median) is $2.5$, and the [Huber location estimator](#huber-location-estimator) with fixed $s=1,k=2$ stays at $2.5$. Once $M-2.5\geq2$, its [Huber score](#huber-score) is already $2$; moving it farther changes the [Huber loss](#huber-loss) but leaves the root unchanged.

For a closer view of the transition, the exact [Huber location estimator](#huber-location-estimator) over $0\leq M\leq40$ is

$$
T(M)=\begin{cases}(8+M)/5,&0\leq M\leq4.5,\\2.5,&4.5\leq M\leq40.\end{cases}
$$

To verify the first branch, when $0\leq M\leq2$ the score of $4$ is saturated and the other five scores sum with it to $8+M-5\theta$. When $2\leq M\leq4.5$, the score of $0$ is saturated instead, giving the same expression. At $M=4.5$, the moving observation saturates too, and the equation becomes $10-4\theta=0$. The piecewise formula is continuous at the transition.

<a id="image-one-moving-observation-sample-mean-sample-median-and-fixed-scale-huber-location-estimator"></a>
![](huber-location-outlier-response.png)

**[Figure 3](#image-one-moving-observation-sample-mean-sample-median-and-fixed-scale-huber-location-estimator). One moving observation: sample mean, sample median, and fixed-scale Huber location estimator**. Original deterministic data $(0,1,2,3,4,M)$ with $s=1,k=2$. The inset resolves the region $0\leq M\leq6$, where the three [estimators](statistical-modelling.md#estimator) differ; the [Huber location estimator](#huber-location-estimator) saturates at $M=4.5$. For $5\leq M\leq40$, it coincides with the [sample median](probability-distribution.md#sample-median), while the [sample mean](variance.md#sample-mean) continues to rise.

The rising [sample mean](variance.md#sample-mean) comes from an unbounded linear score, the flat distant-outlier response from a bounded [Huber score](#huber-score). This is a finite-data response curve with a specified scale and threshold, rather than a population [influence function](#influence-function) or a general claim about arbitrary numbers of [outliers](statistical-modelling.md#outlier).

### Huber score

↑ **Parent:** [Huber location estimator](#huber-location-estimator)

The Huber score clips a residual at a fixed threshold:

$$
\psi_k(u)=\max(-k,\min(u,k)).
$$

For $k>0$, the [Huber score](#huber-score) is the [derivative](calculus.md#derivative) of the [Huber loss](#huber-loss):

$$
\psi_k(u)=\rho_k'(u)=\begin{cases}-k,&u<-k,\\u,&-k\leq u\leq k,\\k,&u>k.\end{cases}
$$

It is a continuous [odd function](calculus.md#odd-function) and a [monotone function](calculus.md#monotonic-function), with [Lipschitz continuity](real-analysis.md#lipschitz-continuity) and $|\psi_k(u)|\leq k$. In a [Huber location estimator](#huber-location-estimator), its argument is the standardized difference $u=(x-\theta)/s$. Its [derivative](calculus.md#derivative) is $1$ inside the clipping interval and $0$ outside; that [derivative](calculus.md#derivative) is undefined at the two endpoints. The score itself remains continuous there. This estimating score need not be the [score function](statistical-modelling.md#informant-function) of a separately specified [statistical model](statistical-model.md), nor is it already a normalized [influence function](#influence-function).

#### Optimal bounded influence function for normal location

↑ **Parent:** [Huber score](#huber-score)

For standard [normal distribution](probability-distribution.md#normal-distribution) location estimation, an [influence function](#influence-function) $h$ obeys $\mathbb E[Zh(Z)]=1$. Under $|h|\le C$, minimize $\mathbb E h^2$ by projecting $ax$ onto $[-C,C]$, choosing $a$ to meet that identity. For $C>\sqrt{\pi/2}$ this gives the displayed [Huber score](#huber-score) normalized by $2\Phi(K)-1$, with $C=K/(2\Phi(K)-1)$. Pointwise minimality of $h^2-2axh$ proves global optimality after integration. At $C=\sqrt{\pi/2}$ the only feasible normalized function is $C\operatorname{sgn}(x)$ almost everywhere, the [influence function of the sample median](#influence-function-of-the-sample-median). The endpoint is a limit of rescaled clipped scores, not the identically zero score obtained by substituting $K=0$ literally.

### Huber loss

↑ **Parent:** [Huber location estimator](#huber-location-estimator)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Huber_loss)

The Huber loss is quadratic near zero and linear beyond a fixed cutoff; its derivative is the clipped Huber score.

For threshold $k>0$, the [Huber loss](#huber-loss) is the [loss function](foundations-of-mathematics.md#loss-function)

$$
\rho_k(u)=\begin{cases}\tfrac12u^2,&|u|\leq k,\\k|u|-\tfrac12k^2,&|u|>k.\end{cases}
$$

The subtraction $k^2/2$ makes the values meet at $|u|=k$; the slopes also meet, so the [Huber loss](#huber-loss) is continuously [differentiable](analysis.md#differentiable-function) with [Huber score](#huber-score) as its [derivative](calculus.md#derivative). It is a [convex function](real-analysis.md#convex-function), since that [derivative](calculus.md#derivative) is a [monotone function](calculus.md#monotonic-function). These quadratic and linear pieces define the original clipped location criterion.[§1, printed p. 75: piecewise criterion; §4(iii), printed p. 79: corresponding location estimator](mathematics-bibliography.md#robust-estimation-of-a-location-parameter-by-peter-j-huber)

<a id="image-huber-loss-and-huber-score-for-threshold-k-2"></a>
![](huber-loss-and-score.png)

**[Figure 4](#image-huber-loss-and-huber-score-for-threshold-k-2). Huber loss and Huber score for threshold $k=2$**. Original curves compare the [Huber loss](#huber-loss) with $u^2/2$ and $2|u|$, then compare the [Huber score](#huber-score) with the linear score $u$ and $2\operatorname{sgn}(u)$. The dashed vertical lines mark $u=\pm2$.

For $k=2$, $\rho_2(1)=1/2$, $\rho_2(2)=2$, and $\rho_2(5)=8$, whereas the squared criterion $u^2/2$ at $u=5$ is $12.5$. Increasing a standardized difference from $5$ to $6$ raises the [Huber loss](#huber-loss) by $2$, but raises the squared criterion by $5.5$. The compromise preserves quadratic sensitivity to small differences while limiting the slope for large ones. This makes the [Huber loss](#huber-loss) useful when ordinary observations should retain their detailed distances yet isolated [outliers](statistical-modelling.md#outlier) should exert limited pull.

For a fixed finite dataset and scale, taking $k$ large enough that every difference from the [sample mean](variance.md#sample-mean) lies within $ks$ recovers that [sample mean](variance.md#sample-mean). Toward the other extreme, for each fixed $u$, $\rho_k(u)/k\to|u|$ as $k\downarrow0$, connecting the criterion to [median minimizes expected absolute loss](probability-distribution.md#median-minimizes-expected-absolute-loss). The normalization is essential: putting $k=0$ into the unscaled [Huber loss](#huber-loss) gives zero everywhere, not a usable [median](probability-distribution.md#median) criterion.

#### Huber gradient regularizer

↑ **Parent:** [Huber loss](#huber-loss)

A [Huber loss](#huber-loss) applied to a discrete gradient combines quadratic penalization of small slopes with linear penalization of large slopes. This interpolates between squared-gradient smoothing and [total variation denoising](inverse-problem.md#total-variation-denoising), allowing smooth regions while retaining an edge-preserving large-gradient regime. The threshold should be chosen consistently with the signal's units and discretization. It can reduce [staircasing in total variation denoising](inverse-problem.md#staircasing-in-total-variation-denoising) without guaranteeing its elimination.

## Median-of-means estimator

↑ **Parent:** [Robust statistics](robust-statistics.md)

The median-of-means estimator partitions a sample, computes each group mean, and returns the median of those means.

## Tukey median

↑ **Parent:** [Robust statistics](robust-statistics.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tukey_median)

The Tukey median maximizes halfspace depth, the smallest probability mass or empirical fraction in any closed halfspace containing the candidate point.

## Asymptotic distribution of a sample median

↑ **Parent:** [Robust statistics](robust-statistics.md)

For an odd sample size $n$ from a distribution with positive continuous density $f$ at its median $m$,

$$
\sqrt n(\widehat m-m)\Longrightarrow N\left(0,\frac1{4f(m)^2}\right).
$$

## ↑ Ancestors (5)

1. [Statistical inference](statistical-inference.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Laplace location and scale maximum likelihood](continuous-probability-distribution.md#laplace-location-and-scale-maximum-likelihood)
