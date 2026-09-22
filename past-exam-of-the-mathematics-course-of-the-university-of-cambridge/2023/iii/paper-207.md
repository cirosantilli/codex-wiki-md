# Paper 207

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_207.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2023/Paper_207.pdf)

**Table of contents**

- [1](#1)
  - [1](#1/1)
    - [Solution](#1/1/solution)
    - [2](#1/1/2)
      - [Solution](#1/1/2/solution)
    - [3](#1/1/3)
      - [Solution](#1/1/3/solution)
    - [4](#1/1/4)
      - [Solution](#1/1/4/solution)
    - [5](#1/1/5)
      - [i](#1/1/5/i)
        - [Solution](#1/1/5/i/solution)
      - [ii](#1/1/5/ii)
        - [Solution](#1/1/5/ii/solution)
      - [iii](#1/1/5/iii)
        - [Solution](#1/1/5/iii/solution)
      - [iv](#1/1/5/iv)
        - [Solution](#1/1/5/iv/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [i](#2/c/i)
      - [Solution](#2/c/i/solution)
    - [ii](#2/c/ii)
      - [Solution](#2/c/ii/solution)
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
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
  - [d](#4/d)
    - [i](#4/d/i)
      - [Solution](#4/d/i/solution)
    - [ii](#4/d/ii)
      - [Solution](#4/d/ii/solution)
    - [iii](#4/d/iii)
      - [Solution](#4/d/iii/solution)
    - [iv](#4/d/iv)
      - [Solution](#4/d/iv/solution)
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
  - [vii](#5/vii)
    - [Solution](#5/vii/solution)
  - [viii](#5/viii)
    - [Solution](#5/viii/solution)
  - [ix](#5/ix)
    - [Solution](#5/ix/solution)
  - [x](#5/x)
    - [Solution](#5/x/solution)
- [6](#6)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
    - [iii](#6/a/iii)
      - [Solution](#6/a/iii/solution)
    - [iv](#6/a/iv)
      - [Solution](#6/a/iv/solution)
    - [v](#6/a/v)
      - [Solution](#6/a/v/solution)
    - [vi](#6/a/vi)
      - [Solution](#6/a/vi/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
    - [iv](#6/b/iv)
      - [Solution](#6/b/iv/solution)
    - [v](#6/b/v)
      - [Solution](#6/b/v/solution)
    - [vi](#6/b/vi)
      - [Solution](#6/b/vi/solution)
    - [vii](#6/b/vii)
      - [Solution](#6/b/vii/solution)
    - [viii](#6/b/viii)
      - [Solution](#6/b/viii/solution)

## 1

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Let $Z$ indicate a recent birthday event, $A$ indicate a social gathering, and $Y$ denote subsequent household COVID-19 infection. The standard [instrumental variable](../../../causal-inference.md#instrumental-variable) conditions are:

- [Instrument relevance](../../../causal-inference.md#instrument-relevance): $Z$ changes the probability or intensity of $A$.
- [Instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence): conditional on chosen baseline covariates, birthday timing is independent of unmeasured causes of infection and of the relevant [potential outcomes](../../../causal-inference.md#potential-outcome).
- The [exclusion restriction](../../../causal-inference.md#exclusion-restriction): $Z$ affects $Y$ only through the social gathering $A$.
- For a [local average treatment effect](../../../causal-inference.md#local-average-treatment-effect), [instrumental-variable monotonicity](../../../causal-inference.md#instrumental-variable-monotonicity) excludes households that would hold a gathering without a birthday event but would suppress it because of one.

The usual [consistency in causal inference](../../../causal-inference.md#consistency-in-causal-inference), well-defined exposure, and absence of relevant [interference in causal inference](../../../causal-inference.md#interference-in-causal-inference) are also needed to interpret the result causally.

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

The assumptions are plausible only approximately. First, birthday timing can correlate with age, household composition, season, holidays, local epidemic phase, testing, or health-care use. Any such common cause of $Z$ and $Y$ violates [instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence). Second, a birthday may alter contacts, deliveries, travel, or testing even without the intended party exposure; those pathways violate the [exclusion restriction](../../../causal-inference.md#exclusion-restriction). The instrument may also be weak where restrictions or low local prevalence suppress gatherings.

Two useful assessments are:

- Check [covariate balance](../../../causal-inference.md#covariate-balance) across birthday-event groups, including age, household size, calendar time, local prevalence, and pre-event infection or testing. Repeat the analysis at placebo dates and for [negative control outcomes](../../../causal-inference.md#negative-control-outcome).
- Measure a first-stage proxy for gatherings, such as mobility, restaurant visits, or contact reports, and verify [instrument relevance](../../../causal-inference.md#instrument-relevance). An event-study around the birthday can test for pre-existing trends and for an effect concentrated after, rather than before, the birthday.

These checks cannot prove independence or exclusion, but failures directly falsify implications of those assumptions.

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/solution">Solution</h5>

↑ **Parent:** [3](#1/1/3)

Political environment may be an [effect modifier](../../../causal-inference.md#effect-modifier) of the first stage: if red-county households hold larger birthday gatherings or use fewer mitigations, a truly causal contact mechanism predicts a larger birthday-associated infection increase there than in otherwise comparable blue counties. The comparison is therefore a mechanism check for [heterogeneous treatment effects](../../../causal-inference.md#heterogeneous-treatment-effect).

Its interpretation requires comparable epidemic timing, baseline prevalence, demographics, urbanicity, testing, reporting, and public-health rules across the compared counties, or adequate adjustment for them. It also assumes political classification changes gathering behavior without creating a different direct birthday-to-testing or birthday-to-infection pathway. Because voting category is ecological rather than individual, interpreting the pattern as individual behavior additionally risks the [ecological fallacy](../../../causal-inference.md#ecological-fallacy).

<h4 id="1/1/4">4</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/4/solution">Solution</h5>

↑ **Parent:** [4](#1/1/4)

First, compare counties only after matching, weighting, or regression adjustment for baseline prevalence, calendar date, population density, age structure, household size, income, testing intensity, and public-health restrictions. Use county-clustered uncertainty to respect within-county dependence.

Second, replace the coarse red/blue split by continuous vote share and estimate a prespecified birthday-event-by-vote-share interaction. A continuous analysis retains information, permits a dose-response check, and avoids sensitivity to an arbitrary 50% cutoff. Reporting subgroup sample sizes and correcting for multiple subgroup searches would further reduce selective interpretation.

<h4 id="1/1/5">5</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/5/i">i</h5>

↑ **Parent:** [5](#1/1/5)

<h6 id="1/1/5/i/solution">Solution</h6>

↑ **Parent:** [I](#1/1/5/i)

A useful comparison divides counties into periods with strict and lenient limits on private gatherings. The split is worthwhile because the policy should alter the size or frequency of birthday gatherings, providing an independent check on the proposed first-stage mechanism.

<h5 id="1/1/5/ii">ii</h5>

↑ **Parent:** [5](#1/1/5)

<h6 id="1/1/5/ii/solution">Solution</h6>

↑ **Parent:** [Ii](#1/1/5/ii)

If gatherings causally raise infection risk and restrictions reduce birthday contacts, the birthday-event association should be smaller under strict restrictions and larger under lenient restrictions. A graded pattern across restriction intensity would be stronger evidence than a single binary contrast.

<h5 id="1/1/5/iii">iii</h5>

↑ **Parent:** [5](#1/1/5)

<h6 id="1/1/5/iii/solution">Solution</h6>

↑ **Parent:** [Iii](#1/1/5/iii)

The analysis assumes that restriction status is not merely a proxy for local epidemic severity, testing, voluntary caution, vaccination, or other determinants of infection, and that it does not change the direct effect of birthday timing on outcome ascertainment. It also assumes comparable compliance within each policy category and no differential migration or reporting.

<h5 id="1/1/5/iv">iv</h5>

↑ **Parent:** [5](#1/1/5)

<h6 id="1/1/5/iv/solution">Solution</h6>

↑ **Parent:** [Iv](#1/1/5/iv)

Assess these assumptions by balancing or adjusting for pre-policy prevalence, testing, vaccination, mobility, demographics, and calendar time; inspect infection and testing trends before policy changes; and use mobility or contact data to confirm that restrictions actually weaken the birthday-to-gathering first stage. Placebo outcomes and dates provide additional [negative control outcomes](../../../causal-inference.md#negative-control-outcome).

<h2 id="2">2</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

Put

$$
a=\frac{p_0}{1-p_0},
\qquad
b=\frac{p_1}{1-p_1}.
$$

At a fixed alternative $\theta$, the approximate power of the [Wald test](../../../statistical-modelling.md#wald-test) increases as its variance

$$
V(n_0,n_1)=\frac a{n_0}+\frac b{n_1}
$$

decreases. For fixed total sample size $n=n_0+n_1$, the allocation problem is therefore

$$
\min_{n_0,n_1>0}\left\{\frac a{n_0}+\frac b{n_1}:n_0+n_1=n\right\},
$$

with integer rounding applied after solving the continuous problem. The second-order condition is positivity of the second derivative at the stationary point.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Writing $R=n_0/n_1$ gives $n_0=nR/(1+R)$ and $n_1=n/(1+R)$, so apart from the positive factor $1/n$ the variance is

$$
f(R)=(1+R)\left(\frac aR+b\right).
$$

Hence

$$
f'(R)=-\frac a{R^2}+b,
\qquad
f''(R)=\frac{2a}{R^3}>0.
$$

The unique minimum is

$$
R^*=\sqrt{\frac ab}
=\sqrt{\frac{p_0(1-p_1)}{p_1(1-p_0)}}.
$$

This is the [Neyman allocation](../../../probability-and-statistics.md#neyman-allocation) for the log relative risk of failure.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The expected number of failures is

$$
F(n_0,n_1)=n_0(1-p_0)+n_1(1-p_1).
$$

Holding the alternative and test size fixed, constant power is equivalent to fixing $V(n_0,n_1)=C$. The ethical allocation problem is therefore

$$
\min_{n_0,n_1>0}F(n_0,n_1)
\quad\text{subject to}\quad
\frac a{n_0}+\frac b{n_1}=C.
$$

The [Lagrange multiplier](../../../mathematical-optimization.md#lagrange-multiplier) stationary equations determine the ratio; the second-order condition requires the constrained stationary point to be a local minimum.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

For

$$
\mathcal L=n_0(1-p_0)+n_1(1-p_1)
+\eta\left(\frac a{n_0}+\frac b{n_1}-C\right),
$$

the stationary equations are

$$
1-p_0=\frac{\eta a}{n_0^2},
\qquad
1-p_1=\frac{\eta b}{n_1^2}.
$$

Dividing them gives

$$
R^*=\frac{n_0}{n_1}
=\sqrt{\frac{a(1-p_1)}{b(1-p_0)}}
=\sqrt{\frac{p_0}{p_1}}\frac{1-p_1}{1-p_0}.
$$

The fixed-power constraint then determines the total sample size. Strict convexity after eliminating one variable supplies the second-order minimum condition.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/i">i</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/i/solution">Solution</h5>

↑ **Parent:** [I](#2/c/i)

For each substudy define the log-odds treatment effect

$$
d_j=\theta_{1j}
=\operatorname{logit}(p_{j1})-\operatorname{logit}(p_{j0}).
$$

The normal random-effects log-likelihood, up to an additive constant, is

$$
\ell(\mu,\sigma^2)
=-\frac J2\log\sigma^2
-\frac1{2\sigma^2}\sum_{j=1}^J(d_j-\mu)^2.
$$

Its [score equations](../../../statistical-modelling.md#score-equation) give

$$
\widehat\mu=\frac1J\sum_{j=1}^Jd_j,
\qquad
\widehat\sigma^2=\frac1J\sum_{j=1}^J(d_j-\widehat\mu)^2.
$$

These are the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator) rather than the unbiased sample-variance estimator. At an interior solution with $\widehat\sigma^2>0$, the Hessian in $(\mu,\sigma^2)$ is negative definite, which is the required second-order condition.

<h4 id="2/c/ii">ii</h4>

↑ **Parent:** [C](#2/c)

<h5 id="2/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/c/ii)

Given numerical values of $\mu$ and $\sigma^2$, maximize the joint log-likelihood over the response rates $0<p_{jk}<1$:

$$
\sum_{j,k}\left[
S_{jk}\log p_{jk}+(n_{jk}-S_{jk})\log(1-p_{jk})
\right]
-\frac1{2\sigma^2}\sum_j
\left\{
\operatorname{logit}(p_{j1})-\operatorname{logit}(p_{j0})-\mu
\right\}^2.
$$

This is a penalized [binomial regression](../../../statistical-modelling.md#binomial-regression) problem and can be solved by [Newton method](../../../mathematical-optimization.md#newton-s-method-in-optimization) or another numerical optimizer. One may alternate this maximization with the closed-form updates for $\mu$ and $\sigma^2$ from part i until convergence. The selected solution should have a negative-definite Hessian in the fitted log-odds parameters.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use a time-homogeneous [continuous-time multi-state model](../../../survival-analysis.md#continuous-time-multi-state-model) with states $H$ (healthy), $I$ (ill), and $D$ (dead), where $D$ is absorbing. For risk-factor indicator $z\in\{0,1\}$, let the transition intensities be

$$
H\xrightarrow{\lambda_z}I,
\qquad
I\xrightarrow{\gamma}H,
\qquad
I\xrightarrow{\delta}D,
\qquad
\lambda_z=\lambda_0e^{\beta z}.
$$

Here $\lambda_0$ is the infection rate without the risk factor, $e^\beta$ is the infection [hazard ratio](../../../survival-analysis.md#hazard-ratio), $\gamma$ is the recovery rate, and $\delta$ is the disease-death rate. The assumption that the risk factor affects only acquisition makes $\gamma$ and $\delta$ common to both groups. The [infinitesimal generator](../../../stochastic-process.md#infinitesimal-generator-stochastic-processes) is

$$
Q_z=
\begin{pmatrix}
-\lambda_z&\lambda_z&0\\
\gamma&-(\gamma+\delta)&\delta\\
0&0&0
\end{pmatrix}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $P_{rs}^{(z)}(t)=\mathbb P(X(t)=s\mid X(0)=r,z)$ denote the [transition semigroup of a continuous-time Markov chain](../../../markov-process.md#transition-semigroup-of-a-continuous-time-markov-chain). The first person is observed in $H$ at day zero, $I$ at day seven, and $H$ at day fourteen, so the contribution is

$$
L_1=P_{HI}^{(0)}(7)P_{IH}^{(0)}(7).
$$

For the second person, death is observed exactly at day six but the infection time is latent. The density of an $I\to D$ transition at day six is

$$
L_2=P_{HI}^{(1)}(6)\,\delta.
$$

Thus the combined contribution $L_1L_2$ is a function of $(\lambda_0,\beta,\gamma,\delta)$. This illustrates how panel observations contribute transition probabilities while an exactly observed transition contributes a state probability times its [transition intensity](../../../survival-analysis.md#transition-intensity).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

An illness episode ends at total rate $\gamma+\delta$, so its mean duration is

$$
\frac1{\gamma+\delta}=10\text{ days}.
$$

The probability that its terminating transition is fatal is $\delta/(\gamma+\delta)=0.1$. Therefore, in day units,

$$
\widehat\delta=0.01,
\qquad
\widehat\gamma=0.09.
$$

Starting healthy, the first infection time is exponential with rate $\lambda_z$. Hence

$$
1-e^{-30\lambda_1}=0.06,
\qquad
1-e^{-30\lambda_0}=0.01,
$$

and

$$
\widehat\lambda_1=-\frac{\log0.94}{30},
\qquad
\widehat\lambda_0=-\frac{\log0.99}{30},
\qquad
\widehat\beta=\log\frac{\widehat\lambda_1}{\widehat\lambda_0}.
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

For each $z$, integrate the probability of occupying the ill state:

$$
\mathbb E_H^{(z)}\!\left[\text{total future time in }I\right]
=\int_0^\infty P_{HI}^{(z)}(t)\,dt.
$$

Equivalently, this is the $(H,I)$ entry of the [fundamental matrix of an absorbing continuous-time Markov chain](../../../survival-analysis.md#fundamental-matrix-of-an-absorbing-continuous-time-markov-chain) $(-Q_{z,T})^{-1}$.

There is also a direct calculation. Each episode is fatal with probability $\delta/(\gamma+\delta)$, so the expected number of episodes before death is $(\gamma+\delta)/\delta$. Each lasts on average $1/(\gamma+\delta)$, giving

$$
\mathbb E_H^{(z)}[\text{total ill time}]=\frac1\delta=100\text{ days}.
$$

The acquisition rates change the waiting time between episodes but, under this model, not the total time eventually spent ill. Thus both risk groups have the same estimate.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

One analysis can treat a reported symptom-onset date as the exact $H\to I$ transition time. That adds an exactly observed infection-time density to the likelihood, but assumes symptoms begin immediately at infection, every relevant episode is symptomatic, and dates are recalled and reported without error.

A more realistic analysis treats true infection as a latent transition and symptom onset as a noisy observation. A reporting-delay distribution, and possibly probabilities of asymptomatic infection and non-reporting, can be added to a [Hidden Markov model](../../../markov-process.md#hidden-markov-model). Weekly tests then interval-censor the state transition while the symptom date refines its distribution. This approach uses more information but requires an identifiable and correctly specified symptom-delay and reporting model.

<h2 id="4">4</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The [risk set](../../../survival-analysis.md#risk-set) at $x_i$ contains every individual still under observation and event-free immediately before $x_i$. Since the observed times are strictly ordered increasingly, these are individuals $i,i+1,\ldots,n$, so its size is

$$
\boxed{Y(x_i)=n-i+1.}
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

At time $x_i$, the observed number of events is $v_i$ and the exposure to the common instantaneous hazard is the risk-set size $n-i+1$. The likelihood score for a hazard increment therefore equates observed and expected events:

$$
v_i=(n-i+1)\,d\widehat H(x_i).
$$

Thus the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) is

$$
\widehat H(t)
=\sum_{i:x_i\leq t}\frac{v_i}{n-i+1}.
$$

It estimates the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) by adding event count divided by current exposure at every observed event time.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A [martingale residual](../../../survival-analysis.md#martingale-residual) is observed minus model-expected event count:

$$
\widehat M_i=v_i-\widehat\Lambda_i(x_i),
$$

where $\widehat\Lambda_i$ is the fitted individual [cumulative hazard](../../../survival-analysis.md#cumulative-hazard-function). Under an adequate model it estimates the terminal value of a counting-process [martingale](../../../martingale.md).

Fit a model omitting the continuous explanatory variable $z$, plot $\widehat M_i$ against $z_i$, and add a flexible smooth curve. A curve fluctuating around zero without structure supports omission. A monotone or curved trend indicates that event incidence still depends on $z$, suggesting inclusion of $z$ or a nonlinear transformation of it. The residuals are highly skewed, so the smoothed trend is more informative than an assumption of Gaussian scatter.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

With a common hazard and the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) from part a,

$$
\widehat M_i
=v_i-\widehat H(x_i)
=v_i-\sum_{j=1}^i\frac{v_j}{n-j+1}.
$$

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

Interchanging the order of the finite sums gives

$$
\begin{aligned}
\sum_{i=1}^n\widehat M_i
&=\sum_{i=1}^nv_i
-\sum_{i=1}^n\sum_{j=1}^i\frac{v_j}{n-j+1}\\
&=\sum_{j=1}^nv_j
-\sum_{j=1}^n\frac{v_j}{n-j+1}
\sum_{i=j}^n1\\
&=\sum_{j=1}^nv_j-\sum_{j=1}^nv_j=0.
\end{aligned}
$$

Each hazard increment is counted once for every individual exposed to it, exactly reproducing its event count.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/i">i</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/i/solution">Solution</h5>

↑ **Parent:** [I](#4/d/i)

For the fitted [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model),

$$
\widehat M_i
=v_i-e^{\widehat\beta z_i}\widehat H_0(x_i),
$$

where $\widehat H_0$ is the fitted baseline cumulative hazard, usually obtained with the [Breslow estimator](../../../survival-analysis.md#breslow-estimator).

<h4 id="4/d/ii">ii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/d/ii)

A residual $0.99$ must correspond to an event and fitted cumulative event count $0.01$. The event occurred much earlier than the model expected for that individual.

A residual $-4$ means that the fitted expected event count by the observed follow-up time exceeded the observed count by four. It may be a censored individual with fitted cumulative hazard four, or an individual whose event occurred only after fitted cumulative hazard five. In either case the individual remained event-free substantially longer than predicted.

<h4 id="4/d/iii">iii</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/d/iii)

For an observed event,

$$
\widehat M_i=1-\widehat\Lambda_i(x_i)<1.
$$

Its supremum is one, approached when the fitted cumulative hazard is near zero, while there is no finite theoretical lower bound.

For a censored observation,

$$
\widehat M_i=-\widehat\Lambda_i(x_i)\leq0.
$$

Its supremum is zero and again there is no finite theoretical lower bound. In a finite fitted dataset the realized minima are of course finite.

<h4 id="4/d/iv">iv</h4>

↑ **Parent:** [D](#4/d)

<h5 id="4/d/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/d/iv)

The residual plot has two asymmetric clouds. Event residuals lie below the horizontal boundary $1$, while censored residuals lie at or below $0$. Because $\widehat\beta>0$, fitted cumulative hazard contains the rapidly increasing multiplier $e^{\widehat\beta z}$; individuals with large $z$ who remain event-free until censoring can therefore have very negative residuals. At small $z$, events tend to lie near $1$ and censored observations near $0$. The resulting scatter is wedge-shaped and increasingly spread toward negative values as $z$ grows, rather than homoscedastic or approximately normal.

<h2 id="5">5</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

At the month-48 analysis, the observed time from treatment start is:

$$
\begin{array}{c|cccccc}
\text{patient}&A&B&C&D&E&F\\ \hline
\text{time}&26&7&13&37&7&27\\
\text{status}&\text{death}&\text{death}&\text{death}&\text{censored}&\text{death}&\text{death}.
\end{array}
$$

For example, patient D contributes $48-12+1=37$ months. This is [right censoring](../../../survival-analysis.md#right-censoring) at a common calendar data cutoff but with staggered treatment entry.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

At duration seven there are six at risk and two deaths, at duration thirteen there are four at risk and one death, at duration twenty-six there are three at risk and one death, and at duration twenty-seven there are two at risk and one death. The [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) is therefore

$$
\widehat F_{48}(t)=
\begin{cases}
1,&0\leq t<7,\\
\dfrac23,&7\leq t<13,\\
\dfrac12,&13\leq t<26,\\
\dfrac13,&26\leq t<27,\\
\dfrac16,&t\geq27.
\end{cases}
$$

The censoring of D at duration thirty-seven causes no multiplicative drop.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

At month 24 the durations and statuses are

$$
A:24\text{ censored},\quad B:7\text{ death},\quad
C:13\text{ death},\quad D:13\text{ censored},\quad
E:7\text{ death},\quad F:9\text{ censored}.
$$

At duration seven, two of six patients die, giving $2/3$. Patient F is censored at duration nine. At duration thirteen, C dies while C, D, and A are at risk; treating an event before censoring at a tied time gives a factor $2/3$. Hence

$$
\widehat F_{24}(t)=
\begin{cases}
1,&0\leq t<7,\\
\dfrac23,&7\leq t<13,\\
\dfrac49,&t\geq13.
\end{cases}
$$

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

At month 36, patients F and D are censored at treatment durations 21 and 25, after which patient A is the sole remaining member of the [risk set](../../../survival-analysis.md#risk-set) and dies at duration 26. The corresponding Kaplan–Meier factor is $1-1/1=0$, so

$$
\widehat F_{36}(48)=0
$$

without needing the earlier factors.

At month 48, D remains at risk past duration 26 and is eventually censored at 37, so no event empties the risk set. Part ii gives

$$
\boxed{\widehat F_{48}(48)=\frac16>0.}
$$

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

At month 12, patients C and D are censored at durations 6 and 1, respectively. When B dies at duration 7, only A and B remain at risk, so

$$
\widehat F_{12}(12)=1-\frac12=\frac12.
$$

At month 36, all six patients have at least twelve months of potential follow-up unless they die earlier. The only deaths by duration twelve are B and E, tied at duration seven, so

$$
\boxed{\widehat F_{36}(12)=1-\frac26=\frac23.}
$$

<h3 id="5/vi">vi</h3>

↑ **Parent:** [5](#5)

<h4 id="5/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#5/vi)

In the final data, the only deaths by treatment duration twelve are B and E. Thus

$$
\widehat F_\infty(12)=\frac23.
$$

The month-24 estimate already has this numerical value, so month 24 is the first twelve-monthly analysis satisfying $\widehat F_M(12)=\widehat F_\infty(12)$.

Equality is not yet knowable at month 24 because patient F has only nine months of follow-up and could still die before duration twelve. Patient F reaches twelve complete months at the end of month 27, so month 36 is the earliest scheduled analysis at which the final value at duration twelve is evaluable.

<h3 id="5/vii">vii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/vii/solution">Solution</h4>

↑ **Parent:** [Vii](#5/vii)

Every patient must either have an observed death or at least 48 months of follow-up. The unresolved patient is D, who starts in month 12 and completes 48 months at the end of month 59. Therefore the month-60 analysis is the earliest twelve-monthly analysis at which $\widehat F_\infty(48)$ is evaluable.

<h3 id="5/viii">viii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/viii/solution">Solution</h4>

↑ **Parent:** [Viii](#5/viii)

The [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) requires [independent censoring](../../../survival-analysis.md#independent-censoring): conditional on modeled covariates, censoring must carry no information about the future event time. Censoring at a common administrative data cutoff satisfies this condition when calendar entry time is independent of prognosis. Under that assumption, the month-24 analysis has valid administrative censoring despite unequal follow-up caused by staggered entry.

<h3 id="5/ix">ix</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ix/solution">Solution</h4>

↑ **Parent:** [Ix](#5/ix)

The researcher should not selectively add A's post-cutoff death to an analysis explicitly defined by the month-24 data cutoff. Doing so gives extra follow-up to a patient precisely because an event became known, creating outcome-dependent ascertainment. The defensible choices are to retain the locked month-24 analysis or update every patient's record to one common later cutoff and label it as a new analysis.

<h3 id="5/x">x</h3>

↑ **Parent:** [5](#5)

<h4 id="5/x/solution">Solution</h4>

↑ **Parent:** [X](#5/x)

**Yes.** A selective update would invalidate the answer to part viii: A's censoring time would be extended because A died, while follow-up for other patients remained truncated at month 24. The resulting censoring mechanism is informative. A uniform update of every patient to the same later administrative cutoff would preserve independent censoring under the original entry-time assumption.

## 6

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

A [competing risks model](../../../survival-analysis.md#competing-risks-model) describes mutually exclusive first-event types. Once one event occurs, it prevents the other event types from being observed as that individual's first event.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

The [cause-specific hazard](../../../survival-analysis.md#cause-specific-hazard) for cause $k$ is

$$
h_k(t)=\lim_{\Delta t\downarrow0}
\frac{\mathbb P(t\leq T<t+\Delta t,\ J=k\mid T\geq t)}{\Delta t}.
$$

It is the instantaneous rate of cause $k$ among individuals still free of every competing event.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

The [cumulative incidence function](../../../survival-analysis.md#cumulative-incidence-function) for cause $k$ is

$$
F_k(t)=\mathbb P(T\leq t,J=k).
$$

Unlike one minus a cause-specific survivor function, it is the absolute probability of observing cause $k$ by time $t$ in the presence of all competing causes.

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

With cause-specific hazards $h_A$ and $h_B$, survival free of either event through time $u$ is

$$
S(u)=\exp\!\left[-\int_0^u\{h_A(s)+h_B(s)\}\,ds\right].
$$

The probability of remaining event-free to $u$ and then experiencing $A$ in $du$ is $S(u)h_A(u)du$. Therefore

$$
\boxed{F_A(t)=\int_0^t
\exp\!\left[-\int_0^u\{h_A(s)+h_B(s)\}\,ds\right]
h_A(u)\,du.}
$$

<h4 id="6/a/v">v</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/v/solution">Solution</h5>

↑ **Parent:** [V](#6/a/v)

For constant hazards $h_A=\theta$ and $h_B=\phi$,

$$
F_A(t)=\int_0^t\theta e^{-(\theta+\phi)u}\,du
=\frac{\theta}{\theta+\phi}
\left(1-e^{-(\theta+\phi)t}\right).
$$

Its limit $\theta/(\theta+\phi)$ is the probability that $A$ occurs before $B$.

<h4 id="6/a/vi">vi</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#6/a/vi)

The composite event has total constant hazard $\theta+\phi$, so its cumulative incidence is

$$
F_{A\cup B}(t)=1-e^{-(\theta+\phi)t}.
$$

It also equals $F_A(t)+F_B(t)$ because the two first-event types are mutually exclusive.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Without administrative stopping, the probability that one patient experiences $A$ before $B$ is $\theta/(\theta+\phi)$. For $n$ patients the expected event count is therefore

$$
\boxed{\mathbb E[v_+]=n\frac{\theta}{\theta+\phi}.}
$$

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Time to the first of $A$ and $B$ is exponential with rate $\theta+\phi$ and mean $1/(\theta+\phi)$. The expected total [person-time at risk](../../../survival-analysis.md#person-time-at-risk) is

$$
\boxed{\mathbb E[x_+]=\frac n{\theta+\phi}.}
$$

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

The ratio of expected event count to expected person-time is

$$
\frac{\mathbb E[v_+]}{\mathbb E[x_+]}=\theta.
$$

**Thus incidence per unit person-time recovers the cause-specific hazard of interest despite independent competing censoring.**

<h4 id="6/b/iv">iv</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/b/iv)

With administrative censoring at $c$, one patient is observed to experience $A$ with probability

$$
\int_0^c\theta e^{-(\theta+\phi)t}\,dt
=\frac{\theta}{\theta+\phi}
\left(1-e^{-(\theta+\phi)c}\right),
$$

so

$$
\mathbb E[v_+]
=n\frac{\theta}{\theta+\phi}
\left(1-e^{-(\theta+\phi)c}\right).
$$

The observed time is $\min(T_A,T_B,c)$, whose mean follows from the [tail-sum formula for expectation](../../../probability-theory.md#tail-sum-formula-for-expectation):

$$
\mathbb E[\min(T_A,T_B,c)]
=\int_0^ce^{-(\theta+\phi)t}\,dt
=\frac{1-e^{-(\theta+\phi)c}}{\theta+\phi}.
$$

Hence

$$
\boxed{\mathbb E[x_+]
=n\frac{1-e^{-(\theta+\phi)c}}{\theta+\phi},
\qquad
\frac{\mathbb E[v_+]}{\mathbb E[x_+]}=\theta.}
$$

<h4 id="6/b/v">v</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/v/solution">Solution</h5>

↑ **Parent:** [V](#6/b/v)

Ignoring factors that do not depend on $\theta$, each observed side-effect contributes $\theta e^{-\theta x_i}$ and each censored observation contributes $e^{-\theta x_i}$. Thus

$$
L(\theta)\propto\theta^{v_+}e^{-\theta x_+},
\qquad
\ell(\theta)=v_+\log\theta-\theta x_++\text{constant}.
$$

The [score equation](../../../statistical-modelling.md#score-equation) $v_+/\theta-x_+=0$ gives

$$
\widehat\theta=\frac{v_+}{x_+}.
$$

This event-count divided by person-time estimator is the sample analogue of the expectation ratio in part iv.

<h4 id="6/b/vi">vi</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#6/b/vi)

The second derivative is

$$
\ell''(\theta)=-\frac{v_+}{\theta^2}.
$$

It is negative when $v_+>0$, verifying a strict maximum. The [Observed Fisher information](../../../statistical-modelling.md#observed-fisher-information) is $v_+/\theta^2$: more observed side-effects sharpen the likelihood, while the curvature vanishes when no side-effect is observed and the maximum then lies at the boundary $\widehat\theta=0$.

<h4 id="6/b/vii">vii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/vii/solution">Solution</h5>

↑ **Parent:** [Vii](#6/b/vii)

At $\theta_0$, the expected Fisher information is

$$
\mathcal I(\theta_0)=\frac{\mathbb E_{\theta_0,\phi_0}[v_+]}{\theta_0^2}.
$$

Requiring it to exceed $I_0$ directly controls the large-sample variance of the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator), approximately $\mathcal I(\theta_0)^{-1}$. Choose $I_0$ from the desired standard error, confidence-interval width, or power for clinically relevant alternatives, allowing for any planned significance level.

<h4 id="6/b/viii">viii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/viii/solution">Solution</h5>

↑ **Parent:** [Viii](#6/b/viii)

Part iv gives

$$
\mathbb E[v_+\mid\theta_0,\phi_0]
=n\frac{\theta_0}{\theta_0+\phi_0}
\left(1-e^{-(\theta_0+\phi_0)c}\right).
$$

Therefore the information requirement is

$$
n\frac{1-e^{-(\theta_0+\phi_0)c}}
{\theta_0(\theta_0+\phi_0)}
\geq I_0.
$$

The required integer sample size is

$$
\boxed{n=
\left\lceil
\frac{I_0\theta_0(\theta_0+\phi_0)}
{1-e^{-(\theta_0+\phi_0)c}}
\right\rceil.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2023](../../2023.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
