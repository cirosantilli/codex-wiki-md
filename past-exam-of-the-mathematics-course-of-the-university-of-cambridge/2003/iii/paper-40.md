# Paper 40

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper40.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2003/Paper40.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
    - [v](#1/b/v)
      - [Solution](#1/b/v/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
  - [v](#2/v)
    - [Solution](#2/v/solution)
- [3](#3)
  - [i](#3/i)
    - [Solution](#3/i/solution)
    - [1](#3/i/1)
      - [Solution](#3/i/1/solution)
    - [2](#3/i/2)
      - [Solution](#3/i/2/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
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
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)
    - [iii](#6/b/iii)
      - [Solution](#6/b/iii/solution)
    - [iv](#6/b/iv)
      - [Solution](#6/b/iv/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For $t\ge0$ and $\theta>0$, the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) has [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $f(t)=\theta e^{-\theta t}$. Integrating the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) gives the [survivor function](../../../survival-analysis.md#survival-function) $S(t)=P(T>t)=e^{-\theta t}$. The [hazard function](../../../survival-analysis.md#hazard-function) divides instantaneous failure density by the [probability](../../../probability-theory.md#probability) of having survived, and the [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function) accumulates this rate. Thus

$$
\boxed{f(t)=\theta e^{-\theta t},\quad S(t)=e^{-\theta t},\quad h(t)=f(t)/S(t)=\theta,\quad H(t)=\int_0^t h(u)\,du=\theta t=-\log S(t).}
$$

The [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is zero for $t<0$, and the [survivor function](../../../survival-analysis.md#survival-function) is one there.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Write $X=\min(T,c)$ and $\Delta=\mathbf1_{\{T\le c\}}$ for the [right-censored](../../../survival-analysis.md#right-censoring) [survival time](../../../survival-analysis.md#survival-time) and observed-failure indicator. Since the [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) is continuous, including or excluding equality at $c$ makes no difference. Using the tail-integral expression for an [expectation](../../../probability-theory.md#expected-value),

$$
E[X]=\int_0^cP(T>u)\,du=\int_0^c e^{-\theta u}\,du=\frac{1-e^{-\theta c}}{\theta}.
$$

Consequently the expected [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function) at the observed endpoint satisfies

$$
\boxed{E[H(X)]=\theta E[X]=1-e^{-\theta c}=P(T\le c)=E[\Delta].}
$$

[Administrative censoring](../../../survival-analysis.md#administrative-censoring) therefore stops both the accumulated exposure and the opportunity to record a failure.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

For individual $i$, let $X_i=\min(T_i,c_i)$ and $\Delta_i=\mathbf1_{\{T_i\le c_i\}}$. The preceding [expectation](../../../probability-theory.md#expected-value) calculation applies separately at each fixed [censoring](../../../survival-analysis.md#censoring-statistics) time:

$$
E[H(X_i)]=\theta E[X_i]=1-e^{-\theta c_i}=E[\Delta_i].
$$

Summing and using linearity of [expectation](../../../probability-theory.md#expected-value), with $D=\sum_i\Delta_i$ the failure count, gives

$$
\boxed{\sum_{i=1}^nE[H(X_i)]=\theta\sum_{i=1}^nE[X_i]=E[D].}
$$

This identity needs the stated marginal [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution), but not independence between individuals; independence will be needed for the product [likelihood](../../../statistical-modelling.md#likelihood-function).

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

Replace the expected total [person-time](../../../survival-analysis.md#person-time) and failure count in the preceding identity by their observed values, $E=\sum_i x_i$ and $d$. The resulting estimating equation is $\theta E=d$, so

$$
\boxed{\widetilde\theta=\frac{d}{\sum_i x_i}.}
$$

This [events divided by exposure estimator](../../../survival-analysis.md#events-divided-by-exposure-estimator) is failures per unit observed [person-time](../../../survival-analysis.md#person-time). We assume positive total exposure; if $d=0$, it gives the boundary estimate zero.

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

For independent individuals under fixed [administrative censoring](../../../survival-analysis.md#administrative-censoring), an observed failure contributes the [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $\theta e^{-\theta x_i}$, while a censored observation contributes the [survivor function](../../../survival-analysis.md#survival-function) $e^{-\theta x_i}$. Hence the [survival likelihood](../../../survival-analysis.md#survival-likelihood) and [log-likelihood](../../../statistical-modelling.md#log-likelihood) are

$$
L(\theta)=\prod_i[\theta e^{-\theta x_i}]^{\Delta_i}[e^{-\theta x_i}]^{1-\Delta_i}=\theta^d e^{-\theta E},\qquad \ell(\theta)=d\log\theta-\theta E.
$$

For $d>0$, the [score function](../../../statistical-modelling.md#informant-function) $\ell'(\theta)=d/\theta-E$ vanishes at $d/E$, and $\ell''(\theta)=-d/\theta^2<0$. This is the unique maximum over $\theta>0$:

$$
\boxed{\widehat\theta=d/E=\widetilde\theta.}
$$

Thus [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) agrees with the observed-exposure estimating equation. If there are no failures, the [likelihood](../../../statistical-modelling.md#likelihood-function) decreases with $\theta$: its supremum is approached as $\theta\downarrow0$, or attained at zero if that boundary is admitted.

<h4 id="1/b/v">v</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/v/solution">Solution</h5>

↑ **Parent:** [V](#1/b/v)

Differentiate the [log-likelihood](../../../statistical-modelling.md#log-likelihood) again. For $d>0$, the positive interior [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) gives

$$
\boxed{\ell''(\widehat\theta)=-\frac{d}{\widehat\theta^2}.}
$$

The [observed information](../../../statistical-modelling.md#observed-fisher-information) is $-\ell''(\widehat\theta)=d/\widehat\theta^2$, giving the usual local [standard error](../../../statistical-inference.md#standard-error) approximation $\widehat\theta/\sqrt d$. For $d=0$ there is no positive interior maximum, so the displayed substitution and this [standard error](../../../statistical-inference.md#standard-error) approximation do not apply; at every positive $\theta$ the second derivative is zero.

## 2

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Let $N(t)$ count observed failures and let $Y(t)$ be the [at-risk process](../../../survival-analysis.md#at-risk-process), counting subjects under observation and still alive immediately before $t$. Under [independent censoring](../../../survival-analysis.md#independent-censoring), a short interval of length $dt$ has conditional expected failure count $Y(t)h(t)\,dt=Y(t)\,dH(t)$. The estimating equation obtained by replacing the count expectation by its observation is $d\widehat H(t)=dN(t)/Y(t)$. Each distinct failure gives $\Delta N(a_m)=1$ and $Y(a_m)=r_m$, so the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) is

$$
\boxed{\widehat H_{\rm NA}(t)=\sum_{a_m\le t}\frac1{r_m}.}
$$

The same increment maximizes the local working [likelihood](../../../statistical-modelling.md#likelihood-function) for a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $r_m\Delta H_m$: differentiating $\Delta N_m\log(\Delta H_m)-r_m\Delta H_m$ gives $\Delta H_m=\Delta N_m/r_m$. The counting-process derivation explains why the [risk set](../../../survival-analysis.md#risk-set), rather than the initial sample size, supplies the denominator.

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Collect distinct observed failure times as $a_m$, with $d_m$ failures and $r_m$ individuals in the [risk set](../../../survival-analysis.md#risk-set) just before $a_m$. The grouped [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) is

$$
\boxed{\widehat H_{\rm NA}(t)=\sum_{a_m\le t}\frac{d_m}{r_m}.}
$$

All failures recorded at one time use the same pre-event [risk set](../../../survival-analysis.md#risk-set). When failures and [censoring](../../../survival-analysis.md#censoring-statistics) share a recorded time, the usual convention includes those censored at that time in the [risk set](../../../survival-analysis.md#risk-set) and processes failures before removing censored individuals. A known different ordering should instead be honored. If ties arise solely through rounding of a continuous-time process, an alternative is to resolve the unobserved ordering: $d_m$ successive failures without intervening [censoring](../../../survival-analysis.md#censoring-statistics) would contribute $\sum_{s=0}^{d_m-1}(r_m-s)^{-1}$. That is not the grouped jump $d_m/r_m$; the difference represents a choice about what the recorded ties mean.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

At a distinct event time $a_m$, estimate the conditional [probability](../../../probability-theory.md#probability) of surviving that time by $1-d_m/r_m$. Multiplication of these conditional [survival probabilities](../../../markov-process.md#survival-probability) gives the [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator), and taking minus its logarithm gives an [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function) estimate:

$$
\boxed{\widehat S_{\rm KM}(t)=\prod_{a_m\le t}\left(1-\frac{d_m}{r_m}\right),\qquad \widehat H_{\rm KM}(t)=-\log\widehat S_{\rm KM}(t)=\sum_{a_m\le t}-\log\left(1-\frac{d_m}{r_m}\right).}
$$

The conditional failure count has a [binomial likelihood](../../../discrete-probability-distribution.md#binomial-likelihood) whose maximizing event fraction is $d_m/r_m$. Tied failures therefore enter directly as one count. Even ordering $d_m$ failures arbitrarily, with no intervening [censoring](../../../survival-analysis.md#censoring-statistics), produces the same [survivor function](../../../survival-analysis.md#survival-function) factor because

$$
\prod_{s=0}^{d_m-1}\left(1-\frac1{r_m-s}\right)=\frac{r_m-d_m}{r_m}=1-\frac{d_m}{r_m}.
$$

The failure-versus-[censoring](../../../survival-analysis.md#censoring-statistics) ordering convention still matters when both have the same recorded time. If $d_m=r_m$, the [survivor function](../../../survival-analysis.md#survival-function) becomes zero and the logarithmic [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function) is infinite.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Put $u_m=d_m/r_m$. The [Taylor series](../../../calculus.md#taylor-series) of the logarithm gives the [small-jump comparison of cumulative hazard estimators](../../../survival-analysis.md#small-jump-comparison-of-cumulative-hazard-estimators):

$$
-\log(1-u_m)=u_m+\frac{u_m^2}{2}+\frac{u_m^3}{3}+\cdots.
$$

Consequently, if $\max_m u_m\le\varepsilon<1$, the two [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function) estimates obey

$$
0\le\widehat H_{\rm KM}-\widehat H_{\rm NA}\le\frac1{2(1-\varepsilon)}\sum_m u_m^2\le\frac{\varepsilon}{2(1-\varepsilon)}\widehat H_{\rm NA}.
$$

**They are close when every event fraction is small.** In particular, with distinct single failures and large [risk sets](../../../survival-analysis.md#risk-set), $u_m=1/r_m$ is small. With tied data, large [risk sets](../../../survival-analysis.md#risk-set) alone are insufficient if a substantial fraction of the [risk set](../../../survival-analysis.md#risk-set) fails together.

<h3 id="2/v">v</h3>

↑ **Parent:** [2](#2)

<h4 id="2/v/solution">Solution</h4>

↑ **Parent:** [V](#2/v)

At the last observed failure time $a_*$, any individual still in the [risk set](../../../survival-analysis.md#risk-set) must either fail there or be censored there or later. If there are no such censored observations, every remaining individual fails, so $d_*=r_*$. Thus the final [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) factor is zero, while the final [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) jump is one:

$$
\boxed{\widehat H_{\rm KM}(a_*)=+\infty,\qquad \widehat H_{\rm NA}(a_*)=\sum_{a_m\le a_*}\frac{d_m}{r_m}<\infty.}
$$

There is no small-jump approximation at this endpoint. Without ties the final [risk set](../../../survival-analysis.md#risk-set) has size one, so the same discrepancy follows from its last single failure.

## 3

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Use the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) for independent outcomes in each nonoverlapping batch, and let the [CUSUM](../../../statistical-inference.md#cusum) accumulate the [log-likelihood ratio](../../../statistical-modelling.md#log-likelihood-ratio) favoring a specified change. The two numbered calculations below treat the batch score and the initial-response design separately.

<h4 id="3/i/1">1</h4>

↑ **Parent:** [I](#3/i)

<h5 id="3/i/1/solution">Solution</h5>

↑ **Parent:** [1](#3/i/1)

Let $p_1$ be the alternative death [probability](../../../probability-theory.md#probability). The [odds ratio](../../../statistical-modelling.md#odds-ratio) specifies

$$
\frac{p_1}{1-p_1}=k\frac{p_0}{1-p_0},\qquad p_1=\frac{kp_0}{1-p_0+kp_0},\qquad 1-p_1=\frac{1-p_0}{1-p_0+kp_0}.
$$

Assume $0<p_0<1$ and $k>0$. For observed batch count $y_t$, the common combinatorial factor in the two [binomial likelihoods](../../../discrete-probability-distribution.md#binomial-likelihood) cancels, giving the [CUSUM](../../../statistical-inference.md#cusum) increment

$$
\begin{aligned}
W_t&=\log\frac{\binom n{y_t}p_1^{y_t}(1-p_1)^{n-y_t}}{\binom n{y_t}p_0^{y_t}(1-p_0)^{n-y_t}}\\
&=y_t\log(p_1/p_0)+(n-y_t)\log[(1-p_1)/(1-p_0)].
\end{aligned}
$$

Therefore

$$
\boxed{W_t=y_t\log k-n\log\{1+(k-1)p_0\}.}
$$

For $k>1$ large death counts add positive evidence of deterioration; for $k<1$ unusually small death counts add evidence for improvement. The score has nonpositive [expectation](../../../probability-theory.md#expected-value) under the null and nonnegative [expectation](../../../probability-theory.md#expected-value) under the specified alternative, as follows from the nonnegativity of [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence). Independent, nonoverlapping batches avoid counting the same patient's outcome repeatedly.

<h4 id="3/i/2">2</h4>

↑ **Parent:** [I](#3/i)

<h5 id="3/i/2/solution">Solution</h5>

↑ **Parent:** [2](#3/i/2)

A classical [sequential probability ratio test](../../../statistical-modelling.md#sequential-probability-ratio-test) addresses a fixed-start choice between two simple [statistical hypotheses](../../../statistical-modelling.md#statistical-hypothesis). It sums [log-likelihood ratio](../../../statistical-modelling.md#log-likelihood-ratio) increments until an upper boundary accepts the alternative or a lower boundary accepts the null; it then terminates that test. A [CUSUM](../../../statistical-inference.md#cusum) instead monitors indefinitely for a change at an unknown time. Its reset at zero discards sustained evidence from a previously satisfactory period, so a late change need not first undo all earlier negative scores. An upper boundary $h$ signals when the accumulated change evidence is sufficiently large.

A [fast initial response CUSUM](../../../statistical-inference.md#fast-initial-response-cusum) takes $0<X_0<h$, often $X_0=h/2$, in place of a zero start. Until its first reset or signal, it acts like a fixed-start [sequential probability ratio test](../../../statistical-modelling.md#sequential-probability-ratio-test) with a lower boundary at $-X_0$ and an upper boundary at $h-X_0$ for the subsequent cumulative increments. Upon reaching the lower boundary it resets and continues as an ordinary [CUSUM](../../../statistical-inference.md#cusum). **The head start gives faster detection if a change is already present when monitoring begins or restarts.** It is useful after an intervention, a shutdown or a previous alarm when immediate renewed surveillance is desired. Its initial false-alarm behavior differs from the zero-start scheme, so the head start and signalling boundary must be calibrated together; the preceding numerical choice is a design convention, not a universal optimum.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Four distinct objections, each with a corresponding improvement, are as follows.

- **Different patients imply different baseline risks.** Raw death rates confound performance with [case mix](../../../causal-inference.md#case-mix), including urgency, disease severity and comorbidity. Use a prespecified, validated [risk-adjusted provider comparison](../../../causal-inference.md#risk-adjusted-provider-comparison), standardizing to comparable patients or comparing observed deaths with $\sum_i\widehat p_i$. Check overlap and model calibration rather than assuming adjustment removes all [confounding](../../../causal-inference.md#confounding).
- **Small annual volumes produce unstable rankings.** A few deaths can move a surgeon far up or down a league table; zero deaths need not indicate zero risk. Display counts and suitably calibrated [confidence intervals](../../../statistical-inference.md#confidence-interval) for [binomial proportions](../../../discrete-probability-distribution.md#binomial-proportion), preferably in [funnel plots](../../../statistical-inference.md#funnel-plot) against volume. Pool suitable periods or use a [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model) to stabilize estimates, while allowing genuine time changes.
- **Many simultaneous comparisons generate chance outliers.** With $m$ independent null comparisons, the [probability](../../../probability-theory.md#probability) of at least one false positive is $1-0.95^m$, and ranks amplify selection of extremes. Use [multiple testing](../../../statistical-modelling.md#multiple-hypothesis-testing) adjustments or simultaneous control limits and seek confirmation before interpreting an apparent outlier. Dependence through the national comparator must also be accounted for.
- **The endpoint and unit of attribution can mislead.** In-hospital death depends on discharge and transfer policy, and care is delivered by a team; follow-up after discharge is omitted. Use an independently audited fixed-horizon endpoint, such as a prespecified 30-day mortality outcome, linked across hospitals and to death registrations, and report an appropriate team or institutional comparison alongside any surgeon-level estimate. Reliable attribution and consistent inclusion criteria reduce incentives to manipulate coding or case selection.

**A confidence interval containing the national rate does not demonstrate equivalence**, and a raw ranking does not establish a causal performance difference. The improved presentation should convey precision and uncertainty as well as the estimated outcome.

## 4

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Use individual [stratified randomization](../../../causal-inference.md#stratified-randomization) within each prison, with concealed centrally generated [permuted-block randomization](../../../causal-inference.md#permuted-block-randomization) and varying block sizes. Prison can affect both baseline risk and intervention delivery, so balancing assignments within prison protects against imbalance in that important [covariate](../../../statistical-model.md#covariate). Varying block sizes and [allocation concealment](../../../causal-inference.md#allocation-concealment) prevent staff from predicting the next allocation and selecting participants accordingly. Prespecify how incomplete final blocks are treated. To enforce the overall 4000:4000 allocation exactly, coordinate the stratum totals centrally, allocating odd final places through a concealed random rule; exact half allocation within every prison is impossible if some prison totals are odd.

**Individual randomization stratified by prison is preferable to randomizing only twenty whole prisons for this design.** A [cluster-randomized trial](../../../causal-inference.md#cluster-randomized-trial) would have few independent units and could lose substantial precision through [intraclass correlation](../../../variance.md#intraclass-correlation-coefficient). Sharing or selling the intervention can cause [treatment contamination](../../../causal-inference.md#treatment-contamination), so record it and retain an [intention-to-treat analysis](../../../causal-inference.md#intention-to-treat-analysis); substantial spillover might justify a separately powered cluster design rather than being ignored.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Use a conventional [two-sided test](../../../statistical-modelling.md#two-sided-hypothesis-test) at [significance level](../../../statistical-modelling.md#significance-level) $0.05$. Let $n=4000$ per arm, $p_C=0.005$, $p_T=0.0025$ and $\Delta=p_C-p_T=0.0025$. Under the specified alternative, the [normal approximation](../../../convergence-of-random-variables.md#normal-approximation) to the difference of independent [binomial proportions](../../../discrete-probability-distribution.md#binomial-proportion) has [standard deviation](../../../variance.md#standard-deviation)

$$
\sigma_1=\sqrt{\frac{p_C(1-p_C)+p_T(1-p_T)}n}=0.00136646.
$$

For planning the pooled null [standard error](../../../statistical-inference.md#standard-error), use $\bar p=(p_C+p_T)/2=0.00375$, giving $\sigma_0=\sqrt{2\bar p(1-\bar p)/n}=0.00136674$. The rejection threshold is approximately $1.96\sigma_0=0.00267880$, exceeding the mean alternative difference. With $\Phi$ the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function), the approximate [statistical power](../../../probability-and-statistics.md#statistical-power) is

$$
1-\Phi\left(\frac{1.96\sigma_0-\Delta}{\sigma_1}\right)+\Phi\left(\frac{-1.96\sigma_0-\Delta}{\sigma_1}\right)\simeq0.448.
$$

**No: the usual two-sided 5% calculation gives about 45% power, below 50%.** The expected death counts are only 20 and 10, so an exact discrete design calculation could refine this approximation.

The question does not specify the tail convention. If a beneficial direction is prespecified and a [one-sided test](../../../statistical-modelling.md#one-sided-hypothesis-test) at 5% is justified, replace $1.96$ by approximately $1.645$; the resulting [statistical power](../../../probability-and-statistics.md#statistical-power) is about $0.573$, and the answer is then yes. This change of testing convention must be declared.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Assume individuals who immediately sell the intervention retain the untreated risk $0.005$, while those who keep it have the posited halved risk $0.0025$. The law of total [expectation](../../../probability-theory.md#expected-value) gives the expected count per thousand assigned to treatment:

$$
\boxed{200(0.005)+800(0.0025)=1+2=3.}
$$

The assignment risk is therefore $0.003$. This is an [intention-to-treat](../../../causal-inference.md#intention-to-treat-analysis) mixture under the stated adherence-specific risks, not an assertion that receipt or sale is randomized. It also assumes that selling does not itself change the seller's baseline risk and that effects on recipients outside this group do not alter this calculation.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

For equal allocation, let $n$ be the required [sample size](../../../probability-and-statistics.md#sample-size) per arm, $p_C=0.0045$, $p_T=0.003$ and $\Delta=0.0015$. In the standard [sample size for comparing two proportions](../../../probability-and-statistics.md#sample-size-for-comparing-two-proportions) calculation, a [two-sided test](../../../statistical-modelling.md#two-sided-hypothesis-test) at 5% with 80% [statistical power](../../../probability-and-statistics.md#statistical-power) requires

$$
\Delta\sqrt n\simeq z_{0.975}\sqrt{2\bar p(1-\bar p)}+z_{0.8}\sqrt{p_C(1-p_C)+p_T(1-p_T)},\qquad \bar p=0.00375.
$$

Using $z_{0.975}=1.95996$ and $z_{0.8}=0.84162$ gives $n\simeq26063.64$, which is rounded upward for actual recruitment. Thus

$$
\boxed{N_{\rm total}\simeq52128,\quad\text{about }52.1\text{ thousand participants, or about }53\text{ thousand when planning in whole thousands}.}
$$

Since the risks are small, dropping the $(1-p)$ corrections and using $1.96+0.84$ gives $N_{\rm total}\simeq2(2.8)^2(0.0075)/(0.0015)^2=52266.7$, conventionally about 52.3 thousand. These are slightly different approximations to the same planning requirement. Add an allowance if outcome ascertainment is incomplete or the allocation is clustered. A prespecified [one-sided test](../../../statistical-modelling.md#one-sided-hypothesis-test) would need a different, smaller [sample size](../../../probability-and-statistics.md#sample-size); the calculation here uses the conventional two-sided interpretation consistently with part (b).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Two useful questions separate intervention retention from actual opportunities to use it.

- **What happened to the intervention after release?** Ask when it was obtained, whether it was carried during the first two weeks, and whether it was sold, lost, given away or replaced. This measures adherence and possible [treatment contamination](../../../causal-inference.md#treatment-contamination).
- **Was it used during an overdose, and for whom?** Ask whether an overdose was witnessed or experienced, whether the intervention was available and administered, who administered it, whether it was used on the respondent or someone else, and the recorded outcome. This distinguishes nonuse despite availability from lack of an opportunity, and detects spillover to other individuals.

Responses can explain implementation, but cannot replace the randomized [intention-to-treat analysis](../../../causal-inference.md#intention-to-treat-analysis). Reincarcerated survivors are a selected subgroup, and recall errors and missing follow-up may affect their reports.

## 5

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

[Genetic linkage](../../../biology.md#genetic-linkage) analysis asks whether a [genetic marker](../../../biology.md#genetic-marker) and a disease [genetic locus](../../../biology.md#genetic-locus) cosegregate within families more often than would be expected under [independent assortment](../../../biology.md#independent-assortment). It uses [pedigrees](../../../biology.md#pedigree) and [Mendelian segregation](../../../biology.md#mendelian-segregation) to estimate the [recombination fraction](../../../biology.md#recombination-fraction) $\theta$, with evidence for linkage arising when the data favor $\theta<1/2$. Even when founders are in linkage equilibrium, linked loci can show familial cosegregation.

[Genetic association](../../../biology.md#genetic-association) analysis instead asks whether observed [allele](../../../biology.md#allele) or [genotype](../../../biology.md#genotype) frequencies differ with disease status in a sampled population, often comparing cases with controls. It can detect a causal variant or a correlated [genetic marker](../../../biology.md#genetic-marker) through [linkage disequilibrium](../../../biology.md#linkage-disequilibrium); population structure and selection can also create association. **Linkage is about familial transmission; association is about population dependence.** Neither an association alone nor a low family recombination estimate establishes that the marker itself causes disease.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Distinguish the disease [alleles](../../../biology.md#allele) $D$ (normal) and $d$ (recessive disease) from the marker [alleles](../../../biology.md#allele) $A,a$. The affected mother and two affected children are $dd$. The unaffected father must be $Dd$, since he has affected children; the unaffected child is $Dd$, since the mother always transmits $d$. The mother is $AA$ at the marker, so the marker [genotypes](../../../biology.md#genotype) identify the father's transmissions to the three children as $a,A,A$. Their disease transmissions from the father are $d,d,D$.

The father's unphased double [heterozygosity](../../../biology.md#heterozygosity) has two possible pairs of [haplotypes](../../../biology.md#haplotype):

$$
s_1:AD/ad,\qquad s_2:Ad/aD.
$$

Under $s_1$, the three paternal transmissions $(ad,Ad,AD)$ are respectively nonrecombinant, recombinant and nonrecombinant. Under $s_2$, they are recombinant, nonrecombinant and recombinant. Each particular gamete has [probability](../../../probability-theory.md#probability) $(1-\theta)/2$ or $\theta/2$, giving the conditional [pedigree likelihoods](../../../biology.md#pedigree-likelihood)

$$
L_1(\theta)=\frac{\theta(1-\theta)^2}{8},\qquad L_2(\theta)=\frac{\theta^2(1-\theta)}8.
$$

Assuming linkage equilibrium among founder [haplotypes](../../../biology.md#haplotype), the two phases have equal prior weights conditional on the observed paternal [genotype](../../../biology.md#genotype). [Phase averaging in a linkage likelihood](../../../biology.md#phase-averaging-in-a-linkage-likelihood) therefore gives

$$
\boxed{L(\theta)=\tfrac12L_1(\theta)+\tfrac12L_2(\theta)=\frac{\theta(1-\theta)}{16},\qquad0\le\theta\le\tfrac12.}
$$

Any factors for the parental [genotypes](../../../biology.md#genotype) omitted by this conditioning are constant in $\theta$. The derivative is $(1-2\theta)/16$, so **the maximum likelihood estimate is $\widehat\theta=1/2$ and there is no evidence for linkage**: the maximum [LOD score](../../../biology.md#lod-score) is zero. Choosing the best phase after observing the offspring would give a different and inappropriate calculation; the unknown phase must be averaged. The linkage-equilibrium assumption is modified explicitly in part (v).

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Arrange rows by marker [genotype](../../../biology.md#genotype), with cases and controls as the two columns. Both column totals are 100, and the three row totals are 100, 60 and 40. Under the null of no [genetic association](../../../biology.md#genetic-association), estimate each common row [probability](../../../probability-theory.md#probability) from its pooled proportion. The expected count is row total times column total divided by the grand total. Thus the expected [contingency table](../../../statistical-modelling.md#contingency-table) is

$$
\boxed{\begin{array}{c|rr}
&\text{cases}&\text{controls}\\\hline
aa&50&50\\Aa&30&30\\AA&20&20
\end{array}.}
$$

The [Pearson chi-squared test of independence](../../../statistical-modelling.md#pearson-chi-squared-test-of-independence) uses

$$
X^2=\sum_{r,c}\frac{(O_{rc}-E_{rc})^2}{E_{rc}}=2\left(\frac{34^2}{50}+\frac{18^2}{30}+\frac{16^2}{20}\right)=93.44.
$$

Under independent sampled individuals and the no-association null, its reference [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) has $(3-1)(2-1)=2$ [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom). All expected cells are well above five. **The null is overwhelmingly rejected**: the approximate [p-value](../../../statistical-modelling.md#p-value) is $e^{-93.44/2}\simeq5.13\times10^{-21}$. This establishes association in the sampling model, not by itself a causal role for the marker.

<h3 id="5/iv">iv</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#5/iv)

Each diploid individual contributes two marker [alleles](../../../biology.md#allele). Count $A$ copies as twice the $AA$ count plus the $Aa$ count, and count $a$ copies analogously. The observed chromosome-level [contingency table](../../../statistical-modelling.md#contingency-table), followed by its null expected table, is

$$
\boxed{\begin{array}{c|rr}
O&\text{cases}&\text{controls}\\\hline
A&20&120\\a&180&80
\end{array}\qquad
\begin{array}{c|rr}
E&\text{cases}&\text{controls}\\\hline
A&70&70\\a&130&130
\end{array}.}
$$

There are 200 [chromosomes](../../../biology.md#chromosome) in each group; pooled totals are 140 $A$ and 260 $a$. The usual allelic [Pearson chi-squared test of independence](../../../statistical-modelling.md#pearson-chi-squared-test-of-independence) gives

$$
X^2=2\left(\frac{50^2}{70}+\frac{50^2}{130}\right)=\frac{10000}{91}\simeq109.89.
$$

With the ordinary independent-chromosome null model, use one [degree of freedom](../../../classical-mechanics.md#degree-of-freedom); its [p-value](../../../statistical-modelling.md#p-value) is about $1.04\times10^{-25}$, providing very strong evidence of [genetic association](../../../biology.md#genetic-association).

The two [alleles](../../../biology.md#allele) from the same person are not automatically two independent observations. The usual one-degree-of-freedom calibration is justified, for example, for unrelated individuals with [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) under the null. If that assumption is not suitable, retain individuals as the sampling units and test their allele dosages using an appropriate variance or permutation of case-control labels, or use the genotype-level test from part (iii). No [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) assumption was needed for that genotype-level test.

<h3 id="5/v">v</h3>

↑ **Parent:** [5](#5)

<h4 id="5/v/solution">Solution</h4>

↑ **Parent:** [V](#5/v)

Using cases as disease [haplotypes](../../../biology.md#haplotype) and controls as control [haplotypes](../../../biology.md#haplotype) in the model requested here, the chromosome counts estimate

$$
P(A\mid d)=20/200=0.10,\quad P(a\mid d)=0.90,\quad P(A\mid D)=120/200=0.60,\quad P(a\mid D)=0.40.
$$

These are conditional marker [allele](../../../biology.md#allele) frequencies, not the reverse [conditional probabilities](../../../probability-theory.md#conditional-probability) $P(d\mid A)$. Under independent founder [chromosomes](../../../biology.md#chromosome), conditional on the father's $Dd,Aa$ [genotype](../../../biology.md#genotype), the phase $AD/ad$ has weight proportional to $0.60\cdot0.90=0.54$, and $Ad/aD$ has weight proportional to $0.10\cdot0.40=0.04$. Their normalized weights are $27/29$ and $2/29$. This conditions on the model's observed parental genotypes; the omitted disease-allele frequencies cancel in the phase-weight ratio.

Using the two phase-specific [pedigree likelihoods](../../../biology.md#pedigree-likelihood) already derived,

$$
\begin{aligned}
L_{\rm LD}(\theta)&=\frac{0.54L_1(\theta)+0.04L_2(\theta)}{0.58}\\
&=\frac{\theta(1-\theta)}{8(0.58)}\{0.54(1-\theta)+0.04\theta\}\\
&=\frac{\theta(1-\theta)(0.54-0.50\theta)}{4.64}.
\end{aligned}
$$

The normalizing factor is independent of $\theta$, so maximize $g(\theta)=0.54\theta-1.04\theta^2+0.50\theta^3$. Its derivative gives exactly

$$
\boxed{1.5\widehat\theta^2-2.08\widehat\theta+0.54=0.}
$$

Only the smaller root lies in $[0,1/2]$:

$$
\boxed{\widehat\theta=\frac{2.08-\sqrt{2.08^2-4(1.5)(0.54)}}3\simeq0.34590.}
$$

On this interval $g''(\theta)=-2.08+3\theta<0$, so this stationary point is the unique maximum. The maximum [LOD score](../../../biology.md#lod-score), retaining the same [linkage disequilibrium](../../../biology.md#linkage-disequilibrium) frequencies in numerator and denominator, is

$$
\boxed{Z_{\max}=\log_{10}\frac{\widehat\theta(1-\widehat\theta)(0.54-0.50\widehat\theta)}{(1/2)(1/2)(0.54-0.25)}\simeq0.05898.}
$$

This is only a [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) of about $1.145$ against $\theta=1/2$, hence very weak evidence. The population frequencies are treated as fixed plug-in estimates, as requested; uncertainty in those estimates and possible disease-model differences between controls and normal-allele chromosomes would matter in a fuller analysis.

## 6

↑ **Parent:** [Paper 40](paper-40.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

The [kinship coefficient](../../../biology.md#kinship-coefficient) $\phi_{XY}$ is the [probability](../../../probability-theory.md#probability) that one [allele](../../../biology.md#allele) copy sampled uniformly from each of individuals $X,Y$, independently conditional on their copies, is [identical by descent](../../../biology.md#identity-by-descent). The [inbreeding coefficient](../../../biology.md#inbreeding-coefficient) $F_X$ is the [probability](../../../probability-theory.md#probability) that the two homologous [allele](../../../biology.md#allele) copies within $X$ are [identical by descent](../../../biology.md#identity-by-descent). For distinct offspring and older individual, [Mendelian segregation](../../../biology.md#mendelian-segregation) gives

$$
\phi_{XY}=\tfrac12(\phi_{P_XY}+\phi_{M_XY}),\qquad F_X=\phi_{P_XM_X},\qquad \phi_{XX}=\tfrac12(1+F_X).
$$

For the last identity, two independent selections choose the same copy with [probability](../../../probability-theory.md#probability) $1/2$, and choose distinct copies with [probability](../../../probability-theory.md#probability) $1/2$, in which case identity has [probability](../../../probability-theory.md#probability) $F_X$. **An unrelated, noninbred founder has $F=0$ and self-kinship $1/2$**, while distinct such founders have zero mutual [kinship coefficient](../../../biology.md#kinship-coefficient). The source's statement of zero founder kinship must be read as zero kinship between distinct founders; zero self-kinship would contradict the definition.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

To identify the unlabelled individuals in the original [pedigree](../../../biology.md#pedigree), call the three children of $A,B$ from left to right $U,V,W$. Then $G$ has parents $C,U$, $D$ has parents $V,W$, and $E,F$ have parents $G,D$. The three [full siblings](../../../biology.md#full-sibling) $U,V,W$ are noninbred because $A,B$ are unrelated noninbred [founders in a pedigree](../../../biology.md#founder-in-a-pedigree). Their pairwise [kinship coefficients](../../../biology.md#kinship-coefficient) are

$$
\phi_{UV}=\phi_{UW}=\phi_{VW}=\frac{\phi_{AA}+\phi_{BB}}4=\frac14.
$$

Since $D$ is the child of the sibling pair $V,W$, its [inbreeding coefficient](../../../biology.md#inbreeding-coefficient) is

$$
\boxed{F_D=\phi_{VW}=\frac14.}
$$

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

The founder $C$ is unrelated to the descendants of $A,B$, while the [kinship coefficient](../../../biology.md#kinship-coefficient) between $D$ and its parents' sibling $U$ is

$$
\phi_{DU}=\tfrac12(\phi_{VU}+\phi_{WU})=\frac14.
$$

As $G$ has parents $C,U$, the [kinship coefficient](../../../biology.md#kinship-coefficient) between $D,G$ is

$$
\phi_{DG}=\tfrac12(\phi_{DC}+\phi_{DU})=\tfrac12(0+\tfrac14)=\frac18.
$$

The parents of $E$ are $D,G$, so

$$
\boxed{F_E=\phi_{DG}=\frac18.}
$$

The same calculation gives $F_F=1/8$.

<h4 id="6/b/iii">iii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/b/iii)

The self-[kinship coefficient](../../../biology.md#kinship-coefficient) of the inbred individual $D$ is $\phi_{DD}=(1+F_D)/2=5/8$. Since $E$ receives a uniformly chosen parental [allele](../../../biology.md#allele) from each of $D,G$,

$$
\boxed{\phi_{DE}=\tfrac12(\phi_{DD}+\phi_{DG})=\tfrac12(\tfrac58+\tfrac18)=\frac38.}
$$

The $\phi_{DD}$ term is essential: self-[kinship coefficient](../../../biology.md#kinship-coefficient) is not zero, even for a noninbred individual.

<h4 id="6/b/iv">iv</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/b/iv)

The [full siblings](../../../biology.md#full-sibling) $E,F$ have parents $G,D$. Since $G$ is noninbred, $\phi_{GG}=1/2$, whereas $\phi_{DD}=5/8$ and $\phi_{GD}=1/8$. Applying the parental [kinship coefficient](../../../biology.md#kinship-coefficient) recursion to both siblings gives

$$
\boxed{\phi_{EF}=\frac{\phi_{GG}+2\phi_{GD}+\phi_{DD}}4=\frac{1/2+2(1/8)+5/8}{4}=\frac{11}{32}.}
$$

The familiar outbred-sibling value $1/4$ does not apply to this inbred [pedigree](../../../biology.md#pedigree).

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

For the usual no-linkage reference model with unrelated, noninbred parents, define $J$ as the number of homologous [allele](../../../biology.md#allele) copies shared [identical by descent](../../../biology.md#identity-by-descent) by two [full siblings](../../../biology.md#full-sibling) at the marker. The two siblings receive the same paternal copy with [probability](../../../probability-theory.md#probability) $1/2$, and independently receive the same maternal copy with [probability](../../../probability-theory.md#probability) $1/2$. Therefore [Mendelian IBD sharing of full siblings](../../../biology.md#mendelian-ibd-sharing-of-full-siblings) gives

$$
P(J=0)=\frac14,\quad P(J=1)=\frac12,\quad P(J=2)=\frac14,\qquad J\sim\operatorname{Bin}(2,1/2).
$$

Hence

$$
\boxed{E[J]=1,\qquad \operatorname{Var}(J)=\frac12.}
$$

For affected siblings, absence of [genetic linkage](../../../biology.md#genetic-linkage) makes the marker transmissions independent of selection by disease, so these are the relevant null moments. This is a fresh outbred reference calculation, not an application of these sharing probabilities to the inbred siblings $E,F$ in part (b). Without the outbred-parent assumption the three ordinary sharing probabilities require modification.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Use the prespecified excess-sharing alternative: affected [full siblings](../../../biology.md#full-sibling) linked to a disease [genetic locus](../../../biology.md#genetic-locus) are expected to share more marker copies [identical by descent](../../../biology.md#identity-by-descent). The total sharing count is $0(42)+1(98)+2(60)=218$, so $\bar J=218/200=1.09$. Under the no-linkage null, independent sibling pairs have $E[J]=1$ and $\operatorname{Var}(J)=1/2$, giving the [mean allele-sharing test for affected siblings](../../../biology.md#mean-allele-sharing-test-for-affected-siblings)

$$
\boxed{Z=\frac{1.09-1}{\sqrt{(1/2)/200}}=1.8.}
$$

The upper 5% [standard normal](../../../probability-theory.md#standard-normal-distribution) critical value is approximately $1.64$, so **there is evidence of excess sharing, and hence linkage, at the one-sided 5% level**. The [normal approximation](../../../convergence-of-random-variables.md#normal-approximation) gives upper-tail [p-value](../../../statistical-modelling.md#p-value) $1-\Phi(1.8)\simeq0.0359$.

The conclusion depends on the intended directional test. A [two-sided test](../../../statistical-modelling.md#two-sided-hypothesis-test) of the sharing mean uses $1.96$, so it would not reject at 5%. An omnibus [Pearson chi-squared goodness-of-fit test](../../../statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test) of the three counts against $(50,100,50)$ gives $64/50+4/100+100/50=3.32$ with two [degrees of freedom](../../../classical-mechanics.md#degree-of-freedom) and also would not reject. The directional mean-sharing test targets the scientifically specified excess-sharing alternative; these different tests should not be selected after seeing which rejects. Independence of the 200 pairs is assumed: if pairs overlap within families, the [standard error](../../../statistical-inference.md#standard-error) needs adjustment.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2003](../../2003.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
