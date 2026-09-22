# Paper 34

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper34.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper34.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
  - [i](#1/i)
    - [Solution](#1/i/solution)
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
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [Solution](#5/solution)

## 1

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [odds ratio](../../../statistical-modelling.md#odds-ratio) compares event odds, not event probabilities. Let group 1 denote the elective group and group 0 the reference group. Their fitted event [probabilities](../../../probability-theory.md#probability) are $\widehat p_1=9/1515\simeq0.00594$ and $\widehat p_0=1215/75057\simeq0.01619$. Thus

$$
\boxed{\widehat{\mathrm{OR}}_{\rm crude}
=\frac{9/(1515-9)}{1215/(75057-1215)}
=\frac{9\cdot73842}{1506\cdot1215}\simeq0.363.}
$$

The [risk ratio](../../../statistical-modelling.md#risk-ratio) is similarly about $0.367$. **The unadjusted observations show a lower adverse-event frequency in the elective group**, rather than an increase. This is an association, not evidence that choosing the procedure prevents adverse outcomes. The direction is opposite to the reported adjusted [odds ratio](../../../statistical-modelling.md#odds-ratio) above one; the two analyses compare different populations or different conditional risks.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Zero observed events do not mean that the underlying event [probability](../../../probability-theory.md#probability) cannot be estimated. For independent observations having a common [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution), the [binomial likelihood](../../../discrete-probability-distribution.md#binomial-likelihood) with no events is $(1-p)^{1515}$, maximized at $\widehat p=0$. A [zero-event binomial upper confidence bound](../../../discrete-probability-distribution.md#zero-event-binomial-upper-confidence-bound) shows the remaining uncertainty: the one-sided 95% upper bound solves $(1-p_U)^{1515}=0.05$, giving

$$
\boxed{p_U=1-0.05^{1/1515}\simeq0.00198.}
$$

Thus the point estimate is zero, but a nonzero mortality risk is compatible with the observations. This bound is an illustration under independent equal-risk sampling; [clustered data](../../../statistical-modelling.md#clustered-data) or unequal risks require their own uncertainty calculation.

The empirical unadjusted [odds ratio](../../../statistical-modelling.md#odds-ratio) is also defined:

$$
\boxed{\widehat{\mathrm{OR}}=\frac{0/1515}{53/75004}=0.}
$$

Its [log odds ratio](../../../statistical-modelling.md#log-odds-ratio) is $-\infty$, so the ordinary [normal approximation](../../../convergence-of-random-variables.md#normal-approximation) for a log-odds [confidence interval](../../../statistical-inference.md#confidence-interval) is unavailable. Exact likelihood-based limits can still describe uncertainty; a specified continuity correction would instead yield a finite, method-dependent point estimate.

In an unpenalized [logistic regression](../../../statistical-modelling.md#logistic-regression) with a separate coefficient for elective exposure, every exposed death outcome is zero. Decreasing that coefficient toward $-\infty$ increases the exposed observations' likelihood contributions and leaves the reference observations unchanged. This is [quasi-complete separation](../../../statistical-modelling.md#quasi-complete-separation): there is no finite ordinary [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) of the exposure coefficient, even after adding background predictors. It is reasonable to say that the usual finite adjusted coefficient could not be fitted; it is too strong to say that no risk estimate or statistical information is possible. A specified penalized likelihood or [Bayesian inference](../../../statistical-inference.md#bayesian-statistics) with proper coefficient priors can provide a finite adjusted estimate, whose dependence on the regularization must be reported.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write the [logistic regression](../../../statistical-modelling.md#logistic-regression) as

$$
\operatorname{logit}\{p(A,x)\}=\alpha+\beta A+\gamma^Tx,
$$

where $A=1$ denotes elective exposure and $x$ contains the measured background predictors. At fixed $x$, changing $A$ from zero to one changes the [log odds](../../../statistical-modelling.md#log-odds) by $\beta$, so the adjusted [odds ratio](../../../statistical-modelling.md#odds-ratio) is $e^\beta$. If $\widehat V$ is the estimated coefficient [covariance matrix](../../../variance.md#covariance-matrix), then

$$
\boxed{\widehat{\mathrm{OR}}_{\rm adjusted}=e^{\widehat\beta},\qquad
\mathrm{CI}_{95\%}=\left[e^{\widehat\beta-1.96\sqrt{\widehat V_{\beta\beta}}},\ e^{\widehat\beta+1.96\sqrt{\widehat V_{\beta\beta}}}\right].}
$$

Use the clinic-cluster [sandwich covariance matrix](../../../statistical-inference.md#sandwich-covariance-matrix) if that is how within-clinic dependence is allowed for. The interval is first calculated on the coefficient scale and then exponentiated; one does not add and subtract a standard error directly from the [odds ratio](../../../statistical-modelling.md#odds-ratio). This is a large-sample [Wald confidence interval](../../../statistical-inference.md#wald-confidence-interval); profile-likelihood limits are another option when the likelihood shape warrants them. If exposure interacts with background variables, there is no single common conditional [odds ratio](../../../statistical-modelling.md#odds-ratio): its logarithm includes the corresponding interaction terms.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

There is an apparent reversal, but not a mathematical contradiction. The crude [odds ratio](../../../statistical-modelling.md#odds-ratio) averages over the actual background distribution in each group, whereas the adjusted [logistic regression](../../../statistical-modelling.md#logistic-regression) compares groups at the same fitted background values. Strong [confounding](../../../causal-inference.md#confounding) could make those distributions very different: for example, elective patients might disproportionately come from low-risk backgrounds or clinics, while the reference patients come from higher-risk backgrounds. The [Simpson paradox](../../../causal-inference.md#simpson-s-paradox) can then reverse the marginal comparison even when every conditional comparison favours the same direction.

The [noncollapsibility of the odds ratio](../../../statistical-modelling.md#noncollapsibility-of-the-odds-ratio) can also make marginal and conditional odds ratios differ in magnitude. It does not, by itself, explain a sign reversal if both groups have the same covariate distribution and the common conditional effect has one sign: if $p(1,x)>p(0,x)$ for every $x$, averaging over the same distribution of $x$ still gives a larger exposed risk. A genuine reversal therefore requires differing background distributions, heterogeneous effects or another change in what is being compared. The observed reversal is a reason to investigate these issues, not proof of a programming error.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Using the reference event rate as the background-risk benchmark gives

$$
\boxed{1515\frac{1215}{75057}\simeq24.5,\quad\text{about 25 events}.}
$$

This is the expected count if the elective group had the reference group's baseline risk and the procedure added no effect. It is substantially above the observed count, illustrating the importance of the background-risk comparison.

Similarity of background factors alone does not fix the elective group's event risk if the procedure itself changes it. If one additionally retained the reported common adjusted [odds ratio](../../../statistical-modelling.md#odds-ratio) $R=2.7$ and used $p_0=1215/75057$ as the common baseline risk, then conversion from odds to [probability](../../../probability-theory.md#probability) would give

$$
p_1=\frac{Rp_0}{1-p_0+Rp_0},\qquad1515p_1\simeq64.4.
$$

These are different assumptions: **about 25 is the baseline/no-effect benchmark; about 64 includes an odds multiplier of 2.7**.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

As a rough rare-event calculation, divide the observed elective-group event count by the reported adjusted [odds ratio](../../../statistical-modelling.md#odds-ratio):

$$
\boxed{9/2.7\simeq3.3\text{ events}.}
$$

For a homogeneous illustrative risk, the exact odds conversion starts from $p_1=9/1515$ and gives

$$
p_0=\frac{p_1}{2.7(1-p_1)+p_1},\qquad1515p_0\simeq3.35.
$$

The corresponding baseline risk is about $0.22\%$, compared with $1.62\%$ in the observed reference group, roughly seven times lower. Thus **taking the adjusted result literally implies exceptionally low background risk among the elective patients**.

This is a diagnostic approximation, not an identified mean of [potential outcomes](../../../causal-inference.md#potential-outcome) obtainable from the aggregate table. A conditional [odds ratio](../../../statistical-modelling.md#odds-ratio) cannot generally be inverted at an aggregate mean: individual background risks are needed for [outcome standardization](../../../causal-inference.md#outcome-standardization). Interpreting the calculation causally also requires [conditional exchangeability](../../../causal-inference.md#conditional-exchangeability), the [positivity assumption](../../../causal-inference.md#positivity-assumption) and a correctly specified outcome model. At very small risks the rare-event approximation makes the estimate of roughly three events useful for checking the plausibility of the adjustment.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The groups were not formed by [randomization](../../../causal-inference.md#randomization). Their background health, access to care, clinic, country and reasons for selecting a delivery method can predict both the method and the outcome, creating [confounding](../../../causal-inference.md#confounding) and [selection bias](../../../causal-inference.md#selection-bias). Moreover, the label describing the reference delivery may be determined after labour: patients whose attempted nonoperative delivery develops a complication can move into an operative category, leaving a selected uncomplicated reference group. Comparing intended strategies would avoid treating this post-baseline classification as a baseline assignment.

A useful comparison would therefore align eligibility and follow-up time, compare intended delivery strategies among patients genuinely eligible for both, and account for sufficient pretreatment predictors. [Logistic regression](../../../statistical-modelling.md#logistic-regression) cannot create comparable patients where the [positivity assumption](../../../causal-inference.md#positivity-assumption) fails or remove unmeasured [confounding](../../../causal-inference.md#confounding).

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

**The displayed information does not establish increased maternal mortality caused by elective exposure.** There are no observed deaths in that group, and the reported adjusted estimate concerns a composite adverse outcome, not death alone. A composite can show an association driven by nonfatal components without identifying a mortality effect.

If the [logistic regression](../../../statistical-modelling.md#logistic-regression) and its adjustment are correct, its [confidence interval](../../../statistical-inference.md#confidence-interval) supports an adjusted association with the composite outcome. Calling that association a causal increase in risk additionally requires a defensible comparison group, adequate control of [confounding](../../../causal-inference.md#confounding), valid outcome classification and a well-defined intervention. The crude result is in the opposite direction, and the implied very low counterfactual baseline risk deserves examination. Conversely, zero deaths does not prove absence of harm. The justified conclusion is an association conditional on model and study assumptions, with mortality and morbidity distinguished.

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

A reversal this large calls for an audit, but the aggregate table cannot identify a particular error. Check the outcome and exposure coding, the reference category, the subset used in each analysis, missing-data exclusions, denominators, weights, and whether the reported coefficient actually corresponds to the intended comparison. Reversing an exposure contrast or exponentiating the wrong fitted coefficient would change the reported [odds ratio](../../../statistical-modelling.md#odds-ratio). Conditioning on variables affected by delivery, or including inappropriate interactions, could also change the [causal inference](../../../causal-inference.md) rather than merely improve precision.

Start by reproducing the crude [odds ratio](../../../statistical-modelling.md#odds-ratio) from an independent two-by-two calculation. Then fit progressively adjusted [logistic regressions](../../../statistical-modelling.md#logistic-regression), recording how the coefficient and analysis population change; inspect within-clinic comparisons, sparse cells and [separation](../../../statistical-modelling.md#separation-statistics). For an ordinary likelihood fit, check the fitted expected event count against the observed count and verify that changing only to cluster-robust standard errors leaves the fitted coefficients unchanged. A [sandwich covariance matrix](../../../statistical-inference.md#sandwich-covariance-matrix) corrects uncertainty for [clustered data](../../../statistical-modelling.md#clustered-data); it does not by itself turn a crude odds ratio below one into an adjusted odds ratio above one. Adding clinic effects, using weights or changing the model can change the point estimate and must be distinguished from that variance correction.

**Programming or reporting error is a possibility to check, not a conclusion proved by the reversal**. Strong legitimate [confounding](../../../causal-inference.md#confounding) remains another explanation.

## 2

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use a concurrent comparison: test the same specimens for both [cocaine](../../../biology.md#cocaine) and [mephedrone](../../../biology.md#mephedrone), rather than treating the historical cocaine percentage as an exactly known 2010 parameter. Assume representative sampling of privates, effectively independent specimens, stable underlying rates during the sampling period, and sufficiently accurate assays. I use a two-sided 5% test of equal positive-test [probabilities](../../../probability-theory.md#probability), with 80% [statistical power](../../../probability-and-statistics.md#statistical-power) at $p_C=0.010$ and $p_M=0.005$. This is a design to distinguish the rates at a twofold alternative; a significance test does not prove that their ratio is exactly two.

The paired design needs the joint positive-test distribution. For specimen $i$, write $C_i,M_i\in\{0,1\}$ and $D_i=C_i-M_i$. Put $q_{11}=P(C_i=M_i=1)$ and

$$
\delta=p_C-p_M=0.005,\qquad q=P(D_i\ne0)=p_C+p_M-2q_{11}.
$$

Then $\mathbb ED_i=\delta$ and $\operatorname{Var}(D_i)=q-\delta^2$. Under equal marginal rates, the two discordant outcomes have equal probabilities; conditional on the total number of discordant specimens, their split is a fair [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution). This gives the [McNemar test](../../../statistical-modelling.md#mcnemar-s-test). Its large-sample version rejects for a sufficiently large absolute difference between the discordant counts, divided by their estimated standard deviation.

For planning, suppose simultaneous positives are negligible, so $q\simeq0.015$. Under the alternative the difference in positive counts has mean $n\delta$ and standard deviation $\sqrt{n(q-\delta^2)}$; the approximate upper null rejection boundary is $z_{0.975}\sqrt{nq}$. Requiring 80% upper-tail rejection probability gives the [paired binary sample size calculation](../../../statistical-modelling.md#paired-binary-sample-size-calculation)

$$
\boxed{n\simeq\frac{\left[1.96\sqrt{0.015}+0.8416\sqrt{0.015-0.005^2}\right]^2}{0.005^2}\simeq4707.}
$$

**Add the mephedrone assay to about 5,000 existing tests, roughly ten weeks at 500 per week.** An exact conditional-power calculation under the negligible-overlap model gives about $77.6\%$ at 4,707 specimens and $80.2\%$ at 5,000, so the rounding also compensates for the conservative discrete test. If positivity for the two drugs were independent within a specimen, $q_{11}=0.00005$, giving a very similar requirement of about 4,676. For the stated marginal rates, $q\leq0.015$, so negligible overlap is a conservative variance choice within this approximation. Substantial co-use reduces the discordant proportion and changes the necessary size. Repeated tests on the same person, unit-level [clustered data](../../../statistical-modelling.md#clustered-data) or inaccurate assays can instead reduce effective information and require more specimens.

A pre-specified one-sided 5% comparison would use $1.645$ in place of $1.96$ and require about 3,708 specimens before allowing for discreteness under the negligible-overlap assumption. These are different testing conventions. Treating the historical 1% as fixed would give a one-sample calculation, but would ignore uncertainty or changes in the actual 2010 cocaine rate.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Model deaths in disjoint equal-duration periods as independent observations with [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) with comparable population exposure and ascertainment. The expected before and after counts are $\mu_0=400$ and $\mu_1=320$. Their difference has

$$
\mathbb E(D_0-D_1)=80,\qquad\operatorname{Var}(D_0-D_1)=400+320=720.
$$

The expected signal relative to its standard deviation is therefore

$$
\boxed{80/\sqrt{720}\simeq2.98.}
$$

Under the null of equal rates, condition on $N=D_0+D_1$: the first-period count has a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $N$ and $1/2$. At a total near 720, the two-sided 5% rejection boundary for $D_0-D_1$ is approximately $1.96\sqrt{720}$. Under the proposed alternative, conditional on that total, its mean is $N/9$ and its variance is $80N/81$. Thus at $N=720$ the [normal approximation](../../../convergence-of-random-variables.md#normal-approximation) gives power approximately

$$
\boxed{\Phi\left(\frac{80-1.96\sqrt{720}}{\sqrt{720\cdot80/81}}\right)\simeq0.85.}
$$

The lower-tail rejection probability is negligible at this alternative; allowing the Poisson total to fluctuate and using discrete rejection cutoffs changes the approximation slightly: an exact two-sided conditional test has about $83.8\%$ power under these Poisson means. **Two years on each side should have adequate power for a 20% reduction under this model**, though a particular realization can still fail to detect it.

This conclusion needs stable recording of drug-related deaths, comparable exposure denominators and no substantial [overdispersion](../../../exponential-family.md#overdispersion) or temporal dependence. A change in population size, certification practice or other drug use can affect the comparison. Detecting a decline does not establish that [mephedrone](../../../biology.md#mephedrone) caused it: attributing displacement requires a credible comparison of [potential outcomes](../../../causal-inference.md#potential-outcome), using an otherwise expected trend or other controls for changes occurring at the same time.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Expected death counts are the number of users multiplied by the death risk per user, with matching time windows and definitions. Relative to the [MDMA](../../../biology.md#mdma) benchmark, the proposed use prevalence contributes a multiplier of $0.6$ and the per-user fatality risk contributes a multiplier of $0.5$. Hence

$$
\boxed{30\times0.6\times0.5=9\text{ mephedrone-only deaths}.}
$$

This assumes comparable user exposure durations and recording of single-drug deaths. Population death counts alone would not identify a per-user [risk ratio](../../../statistical-modelling.md#risk-ratio) without the prevalence denominator.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

On the stipulated figures, a 20% decline from 200 [cocaine](../../../biology.md#cocaine)-related deaths means about 40 fewer deaths, against about 10 attributed to [mephedrone](../../../biology.md#mephedrone):

$$
\boxed{40-10\simeq30\text{ fewer deaths per year in this restricted comparison}.}
$$

That bookkeeping is relevant to a population-harm assessment only if the avoided deaths really result from substitution, the new deaths are counted comparably, and overlapping drug attributions are not counted twice. A change in the legality of one drug is an intervention affecting behaviour; the before-and-after association alone does not identify its [causal effect](../../../causal-inference.md#causal-effect).

Distinguish per-user danger from total population harm. More use can raise total deaths even for a less dangerous drug, and an increase can involve new users who would otherwise use no drug. Conversely, restricting a substitute may move users back to more dangerous alternatives. The relative fatality risks do not mechanically determine legal classification: nonfatal harm, dependence, dosage and purity, co-use, the composition of users, enforcement and supply effects, and uncertainty in the estimates all matter. Any policy assessment should compare plausible behavioural responses to the alternatives, including displacement of both [cocaine](../../../biology.md#cocaine) and [MDMA](../../../biology.md#mdma), rather than extrapolate from ten deaths alone.

**The hypothetical net reduction is a reason to examine harm reduction and substitution carefully, not sufficient evidence for a categorical legal recommendation.**

## 3

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Assume independent individuals and [independent censoring](../../../survival-analysis.md#independent-censoring), with the censoring law not involving the event-rate parameters. If $T_j$ is the [survival time](../../../survival-analysis.md#survival-time) and $C_j$ its censoring time, we observe $x_j=\min(T_j,C_j)$ and $v_j=\mathbf1_{\{T_j\leq C_j\}}$. The [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) gives

$$
f_j(x)=\theta_j e^{-\theta_jx},\qquad S_j(x)=e^{-\theta_jx}.
$$

An observed event contributes $f_j(x_j)$, while a [right-censored](../../../survival-analysis.md#right-censoring) observation contributes $S_j(x_j)$, because it only says the event has not occurred by $x_j$. Multiplying these [survival likelihood](../../../survival-analysis.md#survival-likelihood) contributions and omitting censoring factors independent of the parameters gives

$$
L(\theta_1,\ldots,\theta_n)\propto\prod_{j=1}^n\theta_j^{v_j}e^{-\theta_jx_j},
\qquad
\boxed{\ell(\theta)=\sum_{j=1}^n\{v_j\log\theta_j-\theta_jx_j\}+\text{constant}.}
$$

Without [independent censoring](../../../survival-analysis.md#independent-censoring) the censoring factors cannot generally be discarded in this way.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $D_k=\sum_{j:g_j=k}v_j$ be the observed event count and $T_k=\sum_{j:g_j=k}x_j$ the total [person-time](../../../survival-analysis.md#person-time) in group $k$. Both groups are present; suppose each has $T_k>0$. The grouped [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(\beta^{(0)},\beta^{(1)})=\sum_{k=0}^1\{D_k\log\beta^{(k)}-T_k\beta^{(k)}\}+\text{constant}.
$$

When $D_k>0$, its derivative is $D_k/\beta^{(k)}-T_k$ and its second derivative is $-D_k/(\beta^{(k)})^2<0$. Therefore the [maximum-likelihood estimates](../../../statistical-modelling.md#maximum-likelihood-estimator) are

$$
\boxed{\widehat\beta^{(k)}=D_k/T_k,\qquad k=0,1.}
$$

Both events and censored observations contribute to $T_k$. If $D_k=0$, the likelihood decreases with the positive rate: its supremum is at the boundary $\beta^{(k)}\downarrow0$, rather than at a finite strictly positive estimate. Writing $D_k/T_k=0$ then describes the closure estimate.

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) of a common rate, the same maximization gives

$$
\boxed{\widetilde\beta=\frac{D_0+D_1}{T_0+T_1}.}
$$

Let $D=D_0+D_1$ and $T=T_0+T_1$. The maximized linear terms cancel, since $T_k\widehat\beta^{(k)}=D_k$ and $T\widetilde\beta=D$. Thus the [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test) uses

$$
\boxed{W=-2\log\Lambda
=2\left[\sum_{k=0}^1D_k\log\frac{D_k}{T_k}-D\log\frac DT\right]
=2\sum_{k=0}^1D_k\log\frac{D_kT}{DT_k}.}
$$

Interpret a zero-event summand by continuity as zero. If $D=0$, both likelihood suprema are equal and $W=0$: no rate comparison is informed by observed events.

Under positive common hazard, [independent censoring](../../../survival-analysis.md#independent-censoring) and the usual increasing-information conditions in both groups, [Wilks theorem](../../../statistical-inference.md#wilks-theorem) gives $W\Rightarrow\chi_1^2$, because the unrestricted model has two rate parameters and the null has one. Reject for large $W$; at 5%, the usual cutoff is approximately $3.84$. The chi-squared calibration is asymptotic and can be poor with sparse event counts or boundary estimates.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Set $\alpha=\log\{\beta^{(1)}/\beta^{(0)}\}$ and absorb the common multiplier into $h_0(t)=m(t)\beta^{(0)}$. The model becomes

$$
h_j(t)=h_0(t)e^{\alpha g_j}.
$$

It is a [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model); the unknown baseline does not need a parametric form. The equality hypothesis is precisely $\alpha=0$. The absolute multipliers and $m$ have a scale ambiguity, but their [hazard ratio](../../../survival-analysis.md#hazard-ratio) $e^\alpha$ is identifiable when both groups supply information.

For an untied event at $a_k$, let $R_k$ be the [risk set](../../../survival-analysis.md#risk-set) just before the event, and let $i_k$ be the subject who fails. The conditional event [probability](../../../probability-theory.md#probability) is proportional to that subject's hazard, so the common baseline cancels:

$$
P_\alpha(i_k\mid R_k,\text{one event})
=\frac{e^{\alpha g_{i_k}}}{\sum_{i\in R_k}e^{\alpha g_i}}.
$$

Multiply these factors to form the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood). One can maximize it and compare its maximum with its value at $\alpha=0$ using a [partial likelihood-ratio test](../../../survival-analysis.md#partial-likelihood-ratio-test), or use the corresponding [score test](../../../statistical-modelling.md#score-test).

Explicitly, with group risk-set sizes $r_{k0},r_{k1}$ and observed event indicator $d_{k1}$ for group 1, the score at zero and its information are

$$
U=\sum_k\left(d_{k1}-\frac{r_{k1}}{r_{k0}+r_{k1}}\right),\qquad
V=\sum_k\frac{r_{k0}r_{k1}}{(r_{k0}+r_{k1})^2}.
$$

Under the null the event label has exactly this [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) conditional on its current [risk set](../../../survival-analysis.md#risk-set). Hence **$U^2/V$ is the usual one-degree-of-freedom log-rank test statistic**, with an asymptotic [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) when $V>0$ and enough informative events are observed. Censoring can differ between groups, provided it is independent of event time within the conditioning model. If there are recorded ties, use the appropriate tied-risk-set version: for $d_k$ events the null variance contribution is $d_k(r_k-d_k)r_{k0}r_{k1}/[r_k^2(r_k-1)]$.

## 4

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For individual $i$, let $N_i(t)$ count its observed event by time $t$ and let $Y_i(t)$ indicate membership of the [risk set](../../../survival-analysis.md#risk-set) immediately before $t$. Set $N=\sum_iN_i$ and $Y=\sum_iY_i$. Under a common [hazard function](../../../survival-analysis.md#hazard-function) $h(t)$ and [independent censoring](../../../survival-analysis.md#independent-censoring), a currently at-risk subject has event probability $h(t)dt+o(dt)$ in the next short interval. Summing over the current [risk set](../../../survival-analysis.md#risk-set) gives the conditional intensity

$$
\mathbb E[dN(t)\mid\mathcal F_{t-}]=Y(t)h(t)dt=Y(t)dH(t).
$$

Equivalently, the event count decomposes as

$$
N(t)=\int_0^tY(u)dH(u)+M(t),
$$

where $M$ is the mean-zero [counting-process martingale](../../../stochastic-process.md#counting-process-martingale) obtained by subtracting its conditional compensator. Estimating the unknown hazard increment by the observed event increment divided by the [risk set](../../../survival-analysis.md#risk-set) size gives the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dN(u)
=\sum_{a_j\leq t}\frac1{r_j}.}
$$

Here $a_j$ are the distinct observed event times and $r_j=Y(a_j)$ includes the subject who is about to fail. A censored observation affects subsequent [risk sets](../../../survival-analysis.md#risk-set), but causes no event jump. This is the requested no-ties estimator; tied event counts would produce $d_j/r_j$.

The derivation also identifies the estimation error:

$$
\widehat H(t)-\int_0^t\mathbf1_{\{Y(u)>0\}}\,dH(u)
=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dM(u).
$$

Thus it estimates $H(t)$ on the time range where individuals remain at risk. It is not exactly unbiased for the entire cumulative hazard after the last risk set disappears. Its usual [Nelson–Aalen variance estimator](../../../survival-analysis.md#nelson-aalen-variance-estimator) is $\sum_{a_j\leq t}r_j^{-2}$, since the compensator variance increment of the no-ties event process is $Y\,dH$.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Keep the [counting process](../../../stochastic-process.md#counting-process) and [at-risk process](../../../survival-analysis.md#at-risk-process) notation from the introductory derivation. Because the individual hazards add, the aggregate conditional intensity is

$$
\lambda(t)=\sum_iY_i(t)h_{0i}(t)+Y(t)h_1(t).
$$

The known individual contributions must be averaged over the current [risk set](../../../survival-analysis.md#risk-set), rather than over the original cohort. Define

$$
\overline h_0(t)=\frac{\sum_iY_i(t)h_{0i}(t)}{Y(t)}\qquad(Y(t)>0).
$$

Then $dN(t)/Y(t)$ estimates $\{\overline h_0(t)+h_1(t)\}dt$. Subtract the known average contribution to obtain the [offset-adjusted cumulative hazard estimator](../../../survival-analysis.md#offset-adjusted-cumulative-hazard-estimator)

$$
\boxed{\widehat H_1(t)
=\sum_{a_j\leq t}\frac1{r_j}
-\int_0^t\mathbf1_{\{Y(u)>0\}}\frac{\sum_iY_i(u)h_{0i}(u)}{Y(u)}\,du.}
$$

Take the quotient to be zero when $Y=0$. If $M(t)=N(t)-\int_0^t\lambda(u)du$, direct substitution gives

$$
\widehat H_1(t)
=\int_0^t\mathbf1_{\{Y(u)>0\}}h_1(u)du
+\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dM(u).
$$

This establishes the target and the mean-zero estimation noise, under the usual integrability conditions. It estimates $H_1(t)$ while there is a nonempty [risk set](../../../survival-analysis.md#risk-set); no data identify its continuation after follow-up has ended. With common known $h_{0i}=h_0$ and individuals at risk throughout $[0,t]$, it reduces to $\widehat H_1(t)=\widehat H(t)-H_0(t)$.

The estimate may decrease between events because the known offset is subtracted continuously. That is not an algebraic error: it is an unconstrained estimating-equation estimator, not automatically a nonnegative monotone cumulative hazard estimate. If such shape constraints are imposed, the fitting procedure must explicitly account for them. The working hazard model itself must satisfy $h_{0i}+h_1\geq0$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) of equal [survival distributions](../../../survival-analysis.md#survival-distribution), the two groups have the same event hazard. Conditional on the current [risk set](../../../survival-analysis.md#risk-set) and one event, the event is in A with probability $r_j^A/(r_j^A+r_j^B)$ and in B with probability $r_j^B/(r_j^A+r_j^B)$. Consequently, whenever both groups are represented,

$$
\mathbb E_0\left[\frac{d_j^A}{r_j^A}-\frac{d_j^B}{r_j^B}\,\middle|\,\mathcal F_{a_j-},\text{one event}\right]
=\frac1{r_j^A+r_j^B}-\frac1{r_j^A+r_j^B}=0.
$$

Thus a weighted sum of differences in estimated hazard increments is centered under the null. Its sign reflects which group has more events relative to its numbers at risk. The weights may depend on event time and the preceding [risk sets](../../../survival-analysis.md#risk-set), but must not be chosen after seeing which group failed; otherwise this conditional-centering argument fails. Positive weights emphasize selected time regions without reversing an increment's direction. Such tests can have weak power against crossing hazards whose positive and negative contributions cancel.

Let $I_j=d_j^A$, so $d_j^B=1-I_j$. Its conditional null [variance](../../../variance.md) is $r_j^Ar_j^B/(r_j^A+r_j^B)^2$. Since the unweighted hazard difference is $I_j(1/r_j^A+1/r_j^B)-1/r_j^B$, the conditional variance of its weighted contribution is $\omega_j^2/(r_j^Ar_j^B)$. Successive centered contributions form martingale differences. Their variance contributions add, providing a variance standardization for the test.

With the specified [log-rank weight](../../../survival-analysis.md#log-rank-weight), put $r_j=r_j^A+r_j^B$. Then

$$
\frac{r_j^Ar_j^B}{r_j}\left(\frac{d_j^A}{r_j^A}-\frac{d_j^B}{r_j^B}\right)
=\frac{r_j^Bd_j^A-r_j^Ad_j^B}{r_j}
=d_j^A-\frac{r_j^A}{r_j}.
$$

Therefore the displayed sum is exactly the unstandardized [log-rank statistic](../../../survival-analysis.md#log-rank-statistic)

$$
\boxed{U=\sum_j\left(d_j^A-\frac{r_j^A}{r_j}\right),\qquad
V=\sum_j\frac{r_j^Ar_j^B}{r_j^2}.}
$$

Its two-sided large-sample [log-rank test](../../../survival-analysis.md#log-rank-test) uses $U^2/V\Rightarrow\chi_1^2$ when $V>0$ and information is sufficient. If one group has no remaining subjects at some event time, its event contributes zero information. Use the final observed-minus-expected expression to define the contribution as zero; the original divided expression has an undefined $0/0$ and the log-rank weight becomes zero there. Thus strict positivity of the proposed weights implicitly restricts the comparison to event times when both groups are at risk. [Independent censoring](../../../survival-analysis.md#independent-censoring) and a valid conditional common-hazard model are required throughout.

## 5

↑ **Parent:** [Paper 34](paper-34.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $R(t^*)$ be the [risk set](../../../survival-analysis.md#risk-set) immediately before $t^*$, conditional on the preceding history. Only its members can experience the next event. In a short interval $[t^*,t^*+dt)$, the conditional probability that subject $j$ fails is $h_0(t^*)e^{\beta z_j}dt+o(dt)$, whereas the probability of one event from the [risk set](../../../survival-analysis.md#risk-set) is $h_0(t^*)\sum_{i\in R(t^*)}e^{\beta z_i}dt+o(dt)$. Dividing and taking the small-interval limit gives

$$
\boxed{P_\beta\{\pi(t^*)=j\mid\mathcal F_{t^*-},\text{one event}\}
=\frac{e^{\beta z_j}}{\sum_{i\in R(t^*)}e^{\beta z_i}},\qquad j\in R(t^*).}
$$

It is zero outside the [risk set](../../../survival-analysis.md#risk-set). The common [baseline hazard](../../../survival-analysis.md#baseline-hazard) cancels. This is the conditional event-label probability underlying the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood). Conditioning at an exact continuous event time is understood by this limiting conditional-intensity argument, rather than as division by the zero unconditional probability of an event at a fixed time. We use the standard simple event process with no simultaneous events and [independent censoring](../../../survival-analysis.md#independent-censoring).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Average the covariate over its possible event subjects using the conditional [probabilities](../../../probability-theory.md#probability) from part (a). Define the risk-weighted sums

$$
S_r(t,\beta)=\sum_{i\in R(t)}z_i^r e^{\beta z_i},\qquad r=0,1,2,
$$

with $z_i^0=1$. Then

$$
\boxed{\overline z(t^*,\beta)=\frac{S_1(t^*,\beta)}{S_0(t^*,\beta)}
=\frac{\sum_{i\in R(t^*)}z_i e^{\beta z_i}}{\sum_{i\in R(t^*)}e^{\beta z_i}}.}
$$

This is the mean covariate of the next event subject, conditional on the current [risk set](../../../survival-analysis.md#risk-set) and an event. It is generally not the unweighted average over the original sample. For $\beta=0$ it reduces to the unweighted current risk-set mean.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The difference $s(t^*,\beta)$ is the observed event subject's covariate minus its conditional expected value under the working coefficient. It is the [Schoenfeld function](../../../survival-analysis.md#schoenfeld-function); at a fitted coefficient it becomes a [Schoenfeld residual](../../../survival-analysis.md#schoenfeld-residual). If the conditional event-label distribution is generated by coefficient $\beta$, part (b) gives

$$
\boxed{\mathbb E_\beta[s(t^*,\beta)\mid\mathcal F_{t^*-},\text{one event}]
=\mathbb E_\beta[z_{\pi(t^*)}\mid\cdots]-\overline z(t^*,\beta)=0.}
$$

Hence its unconditional expectation is zero whenever it is integrable. Centering is at the true coefficient: data generated under $\beta_0$ do not generally make $s(t^*,\beta)$ mean zero at an arbitrary trial value $\beta\ne\beta_0$.

The same quantity is the [score function](../../../statistical-modelling.md#informant-function) of one conditional event factor, since

$$
\frac{\partial}{\partial\beta}\log\frac{e^{\beta z_{\pi(t^*)}}}{S_0(t^*,\beta)}
=z_{\pi(t^*)}-\frac{S_1(t^*,\beta)}{S_0(t^*,\beta)}.
$$

This connects its conditional centering to the usual zero-mean likelihood-score identity.

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For the distinct observed event times $a_k$, let $i_k=\pi(a_k)$ and let $R_k$ be the [risk set](../../../survival-analysis.md#risk-set) immediately before that event. The [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) is

$$
L_p(\beta)=\prod_{k=1}^d\frac{e^{\beta z_{i_k}}}{\sum_{i\in R_k}e^{\beta z_i}},\qquad
\ell_p(\beta)=\sum_{k=1}^d\left\{\beta z_{i_k}-\log S_0(a_k,\beta)\right\}.
$$

The different risk sets already incorporate each event and any intervening censoring. Differentiating this [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives

$$
U(\beta)=\ell_p'(\beta)=\sum_{k=1}^d\left[z_{i_k}-\frac{S_1(a_k,\beta)}{S_0(a_k,\beta)}\right]
=\sum_{k=1}^d s(a_k,\beta).
$$

Therefore a finite interior [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) from the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) satisfies the first-order condition

$$
\boxed{\sum_{k=1}^d s(a_k,\widehat\beta)=0.}
$$

Moreover

$$
-\ell_p''(\beta)=\sum_{k=1}^d\left[\frac{S_2(a_k,\beta)}{S_0(a_k,\beta)}-\left(\frac{S_1(a_k,\beta)}{S_0(a_k,\beta)}\right)^2\right]\geq0.
$$

Each summand is the conditional event-covariate [variance](../../../variance.md), so the [partial likelihood](../../../survival-analysis.md#partial-likelihood) is log-concave. If some informative risk set has unequal covariates, the curvature is strictly negative and an existing finite root is the unique maximizer.

The finite-interior qualification is necessary. With two at-risk subjects having covariates zero and one, suppose the subject with covariate one is the sole observed event and the other is subsequently censored. Then $L_p(\beta)=e^\beta/(1+e^\beta)$ increases strictly and has its supremum only as $\beta\to+\infty$; the score $1/(1+e^\beta)$ has no finite zero. If every event risk set has identical covariates, the coefficient is instead unidentifiable and the score is identically zero. The displayed fitted-score equation applies to the regular case in which the proportional-hazards estimate is finite.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
