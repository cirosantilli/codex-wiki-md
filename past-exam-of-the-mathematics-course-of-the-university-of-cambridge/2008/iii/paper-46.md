# Paper 46

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper46.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2008/Paper46.pdf)

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
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [mean](../../../probability-theory.md#expected-value) ratio is $R=(\lambda e^\beta)/\lambda=e^\beta$, so its logarithm is exactly $\beta$; the baseline coefficient $\alpha$ cancels. Under the stated asymptotic [normal approximation](../../../convergence-of-random-variables.md#normal-approximation), the [Wald confidence interval](../../../statistical-inference.md#wald-confidence-interval) for $\beta$ is $0.69\pm1.96(0.15)=(0.396,0.984)$. Exponentiation is monotone and therefore preserves the interval's coverage event. Hence

$$
\boxed{\widehat R=e^{0.69}\simeq1.99,\qquad
R\text{ has approximate }95\%\text{ CI }(1.49,2.68).}
$$

The [standard error](../../../statistical-inference.md#standard-error) of $\alpha$ is not needed for this [confidence interval](../../../statistical-inference.md#confidence-interval): the [Poisson regression](../../../statistical-modelling.md#poisson-regression) already supplies the [standard error](../../../statistical-inference.md#standard-error) of the contrast $\beta$. It would be incorrect to combine the two reported [standard errors](../../../statistical-inference.md#standard-error) as if the [mean](../../../probability-theory.md#expected-value) ratio depended on both coefficients independently.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $Y_0$ and $Y_1$ be the aggregate counts in the control and treated groups. Assuming independent physicians, their [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) have [means](../../../probability-theory.md#expected-value) $12\lambda$ and $12\lambda e^\beta$. Condition on $E=\{Y_0+Y_1=m\}$. By [independent Poisson conditioning](../../../statistical-modelling.md#independent-poisson-conditioning),

$$
Y_1\mid E\sim\operatorname{Bin}\left(m,p\right),\qquad
p=\frac{12\lambda e^\beta}{12\lambda+12\lambda e^\beta}
=\frac{e^\beta}{1+e^\beta}.
$$

The PDF's full table gives $Y_0=67$, $Y_1=133$ and $m=200$. Thus the [Two-group Poisson ratio conditional likelihood](../../../statistical-modelling.md#two-group-poisson-ratio-conditional-likelihood) is

$$
\boxed{L_c(p)=\binom{200}{133}p^{133}(1-p)^{67},\qquad0<p<1.}
$$

Conditioning the individual observations instead gives a multinomial distribution with cell probabilities $(1-p)/12$ in the first group and $p/12$ in the second; its parameter-dependent [likelihood](../../../statistical-modelling.md#likelihood-function) is the same. No factor involves $\lambda$. The conditional estimates are $\widehat p=133/200$ and $\widehat\beta=\log(133/67)\simeq0.6857$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The solid [Poisson regression](../../../statistical-modelling.md#poisson-regression) profile and dashed [negative binomial regression](../../../statistical-modelling.md#negative-binomial-regression) profile peak at essentially the same $\beta\simeq0.69$. The dashed profile is slightly wider and has heavier shoulders: it gives larger relative [likelihood](../../../statistical-modelling.md#likelihood-function) to values farther from the common maximizer. Thus **the estimated [mean](../../../probability-theory.md#expected-value) ratio is stable, while the negative binomial model expresses slightly greater uncertainty**.

The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) constrains [variance](../../../variance.md) to equal the [mean](../../../probability-theory.md#expected-value). A common negative binomial parametrization instead has $\operatorname{Var}(Y)=\mu+\mu^2/k$, with additional shape $k>0$; it permits [overdispersion](../../../exponential-family.md#overdispersion) due, for example, to unexplained between-physician heterogeneity. Profiling this extra parameter lets the data support greater count variability and usually reduces information about the [mean](../../../probability-theory.md#expected-value) contrast. In this two-group model, the fitted group [means](../../../probability-theory.md#expected-value) remain the [sample means](../../../variance.md#sample-mean) for fixed $k$, which explains the nearly identical maximizers. The small separation of the profiles indicates a modest effect here, not overwhelming evidence for strong [overdispersion](../../../exponential-family.md#overdispersion). The comparison concerns the original PDF figure; no figure is reproduced.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For pair $i$, use conditionally independent counts $Y_{i0}\sim\operatorname{Pois}(\lambda_i)$ and $Y_{i1}\sim\operatorname{Pois}(\lambda_i e^\beta)$, with a common effect $\beta$ and a separate positive baseline rate for each physician. Equivalently the linear predictor is $\alpha_i+\beta x$, with $\alpha_i=\log\lambda_i$. This [Poisson regression](../../../statistical-modelling.md#poisson-regression) controls each physician's stable baseline propensity.

Condition on all twelve pair totals $N_i=Y_{i0}+Y_{i1}$. The [paired Poisson conditional likelihood](../../../statistical-modelling.md#paired-poisson-conditional-likelihood) has independent factors

$$
Y_{i1}\mid N_i\sim\operatorname{Bin}\left(N_i,\frac{e^\beta}{1+e^\beta}\right),\qquad
\boxed{L_c(\beta)\propto
\frac{e^{\beta\sum_iY_{i1}}}{(1+e^\beta)^{\sum_iN_i}}.}
$$

This eliminates every $\lambda_i$ exactly. It is more useful as a nuisance-elimination device than the unpaired calculation, which removes only one common baseline: many pair-specific rates are otherwise estimated from just two measurements each.

A possible concern is loss of information through conditioning on totals that are not ancillary for $\beta$, especially with sparse pairs; a zero-total pair contributes no conditional information. There is an important qualification in this exact fixed-baseline Poisson model. Maximizing over $\lambda_i$ gives $\widehat\lambda_i=N_i/(1+e^\beta)$, and substitution leaves precisely the same $\beta$-dependent factor as the [conditional likelihood](../../../statistical-modelling.md#conditional-likelihood). Hence **there is no extra loss relative to ordinary profiling in this particular model**; one should not automatically assert an incidental-parameter bias in its estimate of $\beta$.

Additional baseline observations, a calibrated distribution of baseline rates, or informative hierarchical constraints can retain information in the pair totals. A [Gamma–Poisson hierarchical model](../../../statistical-inference.md#gamma-poisson-hierarchical-model) is one possible structured model, but merely giving it a completely free common [mean](../../../probability-theory.md#expected-value) does not automatically create extra information about $\beta$: that [mean](../../../probability-theory.md#expected-value) can absorb the factor $1+e^\beta$ in the totals. Such remedies trade exact nuisance elimination for additional data or assumptions. Finally, paired sampling alone does not establish conditional Poisson independence or equidispersion: remaining within-physician dependence or [overdispersion](../../../exponential-family.md#overdispersion) should be checked, and an appropriate joint count model or physician-level robust [variance](../../../variance.md) used if needed. The common multiplicative-effect assumption is also part of the analysis.

## 2

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Treat the two retrieved sets of positive tests as independent binomial samples, each of size 500, and use a two-sided test at significance level $0.05$. The normal-approximation [sample size for comparing two proportions](../../../probability-and-statistics.md#sample-size-for-comparing-two-proportions), with equal numbers $n$ in each group, is

$$
n\simeq\frac{\left[z_{0.975}\sqrt{2\bar p(1-\bar p)}+
z_{0.8}\sqrt{p_0(1-p_0)+p_1(1-p_1)}\right]^2}{(p_0-p_1)^2},
\qquad\bar p=\frac{p_0+p_1}{2}.
$$

For $p_0=0.4$, $p_1=0.3$, this gives $n\simeq355.94$, or 356 per group. Thus **500 positives in each period are sufficient for 80% power under these assumptions**.

More explicitly, a pooled two-proportion test rejects when

$$
\left|\frac{\widehat p_0-\widehat p_1}
{\sqrt{\widehat p(1-\widehat p)(1/500+1/500)}}\right|>1.96,
$$

where $\widehat p$ pools the maximum-readout successes. At the proposed alternative, the difference has [mean](../../../probability-theory.md#expected-value) $0.10$ and [standard deviation](../../../variance.md#standard-deviation) $\sqrt{0.45/500}=0.03$. The planning null critical difference is $1.96\sqrt{0.455/500}\simeq0.0591$, giving approximate power

$$
\Phi\left(\frac{0.10-0.0591}{0.03}\right)
+\Phi\left(\frac{-0.10-0.0591}{0.03}\right)
\simeq0.913.
$$

This compares the readout percentage among positive tests. It assumes comparable measurement rules and independent observations; a change in that percentage alone does not identify its causal explanation or the prevalence of drug use in the full tested population.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Use equal individual allocation, a two-sided 5% test as in part (a), 80% power, complete four-week ascertainment and the supplied fatal-overdose endpoint. Then $p_0=1/200=0.005$, $p_1=0.7p_0=0.0035$, and $\bar p=0.00425$. Substituting into the [sample size for comparing two proportions](../../../probability-and-statistics.md#sample-size-for-comparing-two-proportions) gives

$$
n\simeq
\frac{\left[1.959964\sqrt{2(0.00425)(0.99575)}+
0.841621\sqrt{(0.005)(0.995)+(0.0035)(0.9965)}\right]^2}
{(0.0015)^2}
\simeq29524.1.
$$

Rounding upward for equal allocation gives

$$
\boxed{29525\text{ consented eligible prisoners per arm},\qquad
59050\text{ in total, approximately }59000.}
$$

The corresponding expected endpoint counts are about 148 in the control arm and 103 in the active arm. The one-third eligibility proportion affects how many prisoners must be screened, not the number of eligible participants randomized; at full consent and eligibility ascertainment, roughly three times this randomized total would need screening. Loss to follow-up, nonadherence or a changed baseline mortality risk would require a separate design adjustment.

The wording needs an endpoint qualification. The supplied risk is death from overdose, and the proposed effect concerns preventing those deaths. It does not give the incidence of all overdoses. Thus the calculation above sizes **fatal overdoses**, the intended endpoint supported by the data. For a literal 30% reduction in all overdoses, the unknown baseline incidence $q$ must replace $0.005$ in the formula, with $p_1=0.7q$. This is the [endpoint-specific rare-event sample size](../../../probability-and-statistics.md#endpoint-specific-rare-event-sample-size) issue: the same fatal risk can coexist with many nonfatal rates. For example $q=0.005$ gives about 29525 per arm, whereas $q=0.05$ gives about 2838; knowing only the fatal rate cannot determine that latter [sample size](../../../probability-and-statistics.md#sample-size).

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Use individual [stratified randomization](../../../causal-inference.md#stratified-randomization) within each joint combination of prison and the three prespecified addiction-management categories. Within every joint stratum, use [permuted-block randomization](../../../causal-inference.md#permuted-block-randomization) with equal numbers of active and control assignments in each completed block. This directly balances allocations within prison and within management category, rather than hoping that simple independent allocation will achieve both.

Run the allocation sequentially, since the availability and frequency of management categories change during recruitment. Completed blocks balance contemporaneously, so the expanding category is not assigned predominantly to one trial arm. Use varying block sizes and centrally protected [allocation concealment](../../../causal-inference.md#allocation-concealment) to prevent prediction of future assignments. Incomplete final blocks allow a small residual imbalance, and an odd stratum total cannot be split exactly equally. If many joint strata are very sparse, a prespecified [randomized minimization in clinical trials](../../../causal-inference.md#randomized-minimization-in-clinical-trials) scheme can instead target the prison and management margins, retaining a random component. The analysis should account for the important design strata.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

An ethical objection concerns the proposed saving of control-prison staff costs: the trial is explicitly based on individual [informed consent](../../../biology.md#informed-consent), and institutional allocation does not justify omitting control participants' information, consent or appropriate outcome follow-up. These responsibilities remain in both arms. A [cluster-randomized trial](../../../causal-inference.md#cluster-randomized-trial) can sometimes be ethically defensible, but changing the randomized unit alone does not make those participant protections unnecessary.

The statistical objection is loss of independent information and potential prison-level imbalance. Outcomes within a prison may share baseline risks, management practices and release conditions, yielding positive [intraclass correlation](../../../variance.md#intraclass-correlation-coefficient). For equal cluster size $m$, the usual exchangeable approximation gives [design effect](../../../statistical-inference.md#design-effect) $1+(m-1)\rho$, so the individual-randomization calculation understates the sample required when $\rho>0$. There are also fewer independent randomized units, and prison-specific adoption of management practices can be unbalanced across arms. Thus **randomizing prisons generally loses precision for this individually deliverable intervention, unless compensating design features and additional clusters are supplied**.

## 3

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a continuous [survival distribution](../../../survival-analysis.md#survival-distribution), $S(t)=e^{-H(t)}$, $h(t)=H'(t)$ and $f(t)=h(t)S(t)$. Applying these identities gives the [Weibull distribution](../../../probability-theory.md#weibull-distribution)

$$
\boxed{S(t)=e^{-(\lambda t)^p},\qquad
h(t)=p\lambda^pt^{p-1},\qquad
f(t)=p\lambda^pt^{p-1}e^{-(\lambda t)^p},\quad t>0.}
$$

The [survivor function](../../../survival-analysis.md#survival-function) has value one at zero; the [hazard](../../../survival-analysis.md#hazard-function) may diverge there when $p<1$, which does not invalidate the distribution.

For common shape $p$, the [hazard ratio](../../../survival-analysis.md#hazard-ratio) is $h_2(t)/h_1(t)=(\lambda_2/\lambda_1)^p$, independent of time. Thus the two distributions lie in the same [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family). They also satisfy

$$
S_2(t)=S_1\left(\frac{\lambda_2}{\lambda_1}t\right),\qquad
T_2\overset d=\frac{\lambda_1}{\lambda_2}T_1.
$$

Hence **the time multiplier is $\lambda_1/\lambda_2$ and the [hazard](../../../survival-analysis.md#hazard-function) multiplier is $(\lambda_2/\lambda_1)^p$**, establishing the common [accelerated life family](../../../survival-analysis.md#accelerated-life-family) as well. Here $\lambda$ is reciprocal scale, not the ordinary time-scale parameter.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Under [independent censoring](../../../survival-analysis.md#independent-censoring) conditional on the modelled [covariates](../../../statistical-model.md#covariate), an observed event contributes $f_i(x_i)=h_i(x_i)e^{-H_i(x_i)}$, and a right-censored observation contributes $S_i(x_i)=e^{-H_i(x_i)}$. Factors from the censoring distribution may be omitted when they contain no survival-model parameters. The [survival likelihood](../../../survival-analysis.md#survival-likelihood) and [log-likelihood](../../../statistical-modelling.md#log-likelihood) are therefore

$$
\boxed{L=\prod_i h_i(x_i)^{v_i}e^{-H_i(x_i)},\qquad
\ell=\sum_i v_i\log h_i(x_i)-\sum_iH_i(x_i).}
$$

Censored individuals still contribute their observed exposure through $H_i(x_i)$; they are not deleted from the analysis.

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Put $d=\sum_i v_i$. With common [Weibull distribution](../../../probability-theory.md#weibull-distribution) parameters and the [hazard](../../../survival-analysis.md#hazard-function) from part (a), substitution into the general [log-likelihood](../../../statistical-modelling.md#log-likelihood) gives

$$
\boxed{\ell(\lambda,p)=d\log p+pd\log\lambda
+(p-1)\sum_i v_i\log x_i-\lambda^p\sum_i x_i^p.}
$$

This is up to censoring-mechanism terms independent of $\lambda,p$. For $d>0$ and fixed $p$, its maximizing rate is $(d/\sum_i x_i^p)^{1/p}$; the shape still requires separate estimation if it is unknown.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Write $X=\sum_i x_i>0$ and $d=\sum_i v_i$. The exponential [survival likelihood](../../../survival-analysis.md#survival-likelihood) has $\ell(\lambda)=d\log\lambda-\lambda X$. Its score is $d/\lambda-X$, and for $d>0$ its second derivative is $-d/\lambda^2<0$. Thus the [exponential-rate estimation from censored exposure](../../../survival-analysis.md#exponential-rate-estimation-from-censored-exposure) gives

$$
\boxed{\widehat\lambda=\frac dX.}
$$

All observation times, including censoring times, belong in $X$. If $d=0$, the [likelihood](../../../statistical-modelling.md#likelihood-function) decreases with positive $\lambda$ and has its supremum as $\lambda\downarrow0$; under the stated strict positivity constraint there is no interior maximum.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Set $g_i=G_i'(x_i)$, $X=\sum_i x_i$, $d=\sum_i v_i$ and $A=\sum_i v_i g_i$. Then $h_i(x_i)=\lambda+g_i$ and

$$
\ell(\lambda)=\sum_i v_i\log(\lambda+g_i)-\lambda X-\sum_iG_i(x_i),\qquad
U(\lambda)=\sum_i\frac{v_i}{\lambda+g_i}-X.
$$

The integrated offsets are known and enter only as constants in estimation of $\lambda$. Let $\lambda_0=d/X$ and assume $d>0$ and every $g_i$ at an event is small compared with $\lambda_0$. Expanding the score gives

$$
U(\lambda)=\frac d\lambda-\frac A{\lambda^2}-X
+O\left(\frac{\sum_i v_i g_i^2}{\lambda^3}\right).
$$

Now write $\lambda=\lambda_0+\delta$ and retain first-order terms in $g_i,\delta$. Since $d/\lambda_0=X$, the equation becomes $-d\delta/\lambda_0^2-A/\lambda_0^2=0$. Therefore the [exponential rate with a small known additive hazard](../../../survival-analysis.md#exponential-rate-with-a-small-known-additive-hazard) estimate is

$$
\boxed{\widehat\lambda\simeq\frac dX-\frac1d\sum_i v_iG_i'(x_i).}
$$

The correction is negative: some event risk is already supplied by the known additive [hazards](../../../survival-analysis.md#hazard-function). As a check, if every $g_i=g$, the score equation gives the exact positive interior estimate $d/X-g$. The approximation is intended for small offsets and a positive interior solution; a negative approximation or no observed events requires handling the boundary rather than reporting a negative rate.

## 4

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Let $t_j$ be the distinct observed event times, with $r_j$ individuals at risk just before $t_j$ and $d_j$ events there. Parameterize the event-time distribution by the conditional failure probabilities $q_j=\mathbb P(T=t_j\mid T\geq t_j)$. Under [independent censoring](../../../survival-analysis.md#independent-censoring), the survival part of the nonparametric [likelihood](../../../statistical-modelling.md#likelihood-function) groups into factors

$$
L(q)\propto\prod_j q_j^{d_j}(1-q_j)^{r_j-d_j}.
$$

An individual still under observation at $t_j$ contributes either a failure factor or a survival factor; later-censored individuals contribute the latter factors until censoring. Maximizing each factor independently gives $\widehat q_j=d_j/r_j$, including the boundary solutions when $d_j=0$ or $d_j=r_j$. Multiplying the conditional survival probabilities yields the [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator)

$$
\boxed{\widehat F(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

The notation $F$ here denotes the [survivor function](../../../survival-analysis.md#survival-function), as in the question. The estimator is constant between event times. Under the usual simultaneous-event convention, individuals censored at $t_j$ remain in its [risk set](../../../survival-analysis.md#risk-set) while events are processed, and are then removed.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $r$ be the number at risk just after $a$, and suppose the $d$ events are grouped into tie sizes $d_1,\ldots,d_m$ at ordered times in $(a,b]$. With no intervening censoring or entry, their risk counts are $r$, $r-d_1$, $r-d_1-d_2$, and so on. Hence the [Kaplan–Meier telescoping across a censor-free interval](../../../survival-analysis.md#kaplan-meier-telescoping-across-a-censor-free-interval) gives

$$
\frac{\widehat F(b)}{\widehat F(a)}
=\prod_{j=1}^m
\frac{r-\sum_{k\leq j}d_k}{r-\sum_{k<j}d_k}
=\frac{r-d}{r},
\qquad
\boxed{\widehat F(b)=\widehat F(a)\frac{r-d}{r}.}
$$

Only the total $d$ appears. Consequently **the order of the events and their grouping into ties do not affect the estimate at $b$**. Censoring exactly at $b$ does not change this conclusion when it is processed after the events at that time, as in the standard convention. The calculation assumes $r>0$; no estimator beyond an exhausted [risk set](../../../survival-analysis.md#risk-set) is being inferred from unobserved follow-up.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

Use time since enrolment, and assume the cohorts share a common [survival distribution](../../../survival-analysis.md#survival-distribution) with independent [administrative censoring](../../../survival-analysis.md#administrative-censoring). The PDF starts cohort A in 2006, not the corrupted 2000 date in the TeX aid. During the first follow-up year the pooled sample begins with 200 subjects and has $28+31=59$ deaths, with no earlier censoring. By part (a),

$$
\boxed{\widehat F(1)=\frac{200-59}{200}=0.705.}
$$

At one year, the 69 remaining cohort-B subjects are administratively censored. Cohort A supplies 72 subjects at risk for the second follow-up year, with 24 deaths and 48 survivors. Therefore

$$
\boxed{\widehat F(2)=\frac{141}{200}\frac{48}{72}=0.470.}
$$

The given grouped totals suffice because there is no censoring inside either follow-up interval; no assumption about the ordering or ties of its deaths is needed.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

Cohort A alone would give $\widehat F_A(2)=48/100=0.48$. But two-year survival is the product of first-year survival and conditional survival through the second year. Cohort B contributes a full year's information to the first factor even though it has no second-year follow-up. Omitting it discards useful early deaths and survivors. The pooled estimate $0.47$ combines the first-year information from both cohorts with the conditional second-year information from cohort A.

Thus **lack of two-year follow-up is handled by censoring, not by removing the entire short-follow-up cohort**. This is [cohort pooling under administrative censoring](../../../survival-analysis.md#cohort-pooling-under-administrative-censoring). The criticism assumes comparable time-since-entry [survival distributions](../../../survival-analysis.md#survival-distribution): if enrolment cohort or calendar period genuinely changes the [hazard](../../../survival-analysis.md#hazard-function), naive pooling is not justified. One should model or stratify that effect, and an estimand specifically restricted to cohort A may appropriately use its own [survival distribution](../../../survival-analysis.md#survival-distribution).

## 5

↑ **Parent:** [Paper 46](paper-46.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

The [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model) specifies

$$
\boxed{h_i(t)=h_0(t)\exp(\beta^Tz_i),}
$$

where $h_0(t)$ is an unspecified common baseline [hazard](../../../survival-analysis.md#hazard-function) and $z_i$ is the individual's [covariate](../../../statistical-model.md#covariate) vector. The [hazard ratio](../../../survival-analysis.md#hazard-ratio) for two fixed [covariate](../../../statistical-model.md#covariate) vectors is $\exp[\beta^T(z_i-z_k)]$, constant in time. Assume independent subjects and [independent censoring](../../../survival-analysis.md#independent-censoring) conditional on their [covariates](../../../statistical-model.md#covariate), and use the question's absence of tied events.

Let $t_j$ be an event time, $i_j$ its failing subject, and $R_j$ the [risk set](../../../survival-analysis.md#risk-set) immediately before that time. In a short interval of length $dt$, the conditional probability that subject $i$ fails, given one failure among those at risk, is

$$
\frac{h_i(t_j)dt+o(dt)}{\sum_{k\in R_j}h_k(t_j)dt+o(dt)}
\longrightarrow\frac{e^{\beta^Tz_i}}{\sum_{k\in R_j}e^{\beta^Tz_k}}.
$$

The baseline [hazard](../../../survival-analysis.md#hazard-function) cancels. Multiplying the successive conditional event-identity factors gives the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) for $\beta$:

$$
\boxed{L_p(\beta)=\prod_j
\frac{e^{\beta^Tz_{i_j}}}{\sum_{k\in R_j}e^{\beta^Tz_k}},\qquad
\ell_p(\beta)=\sum_j\left[\beta^Tz_{i_j}-\log\sum_{k\in R_j}e^{\beta^Tz_k}\right].}
$$

This is a partial [likelihood](../../../statistical-modelling.md#likelihood-function), not the full survival [likelihood](../../../statistical-modelling.md#likelihood-function) for the unspecified $h_0$. [Risk sets](../../../survival-analysis.md#risk-set) evolve with the observed history; the derivation uses their successive conditional [hazards](../../../survival-analysis.md#hazard-function), rather than assuming the [risk sets](../../../survival-analysis.md#risk-set) themselves are independent.

Define $w_{jk}(\beta)=e^{\beta^Tz_k}/\sum_{\ell\in R_j}e^{\beta^Tz_\ell}$ and $\bar z_j(\beta)=\sum_{k\in R_j}w_{jk}(\beta)z_k$. For component $r$,

$$
\boxed{\frac{\partial\ell_p}{\partial\beta_r}
=\sum_j\left[z_{i_j,r}-\sum_{k\in R_j}w_{jk}(\beta)z_{k,r}\right].}
$$

Differentiating again gives

$$
\frac{\partial^2\ell_p}{\partial\beta_r\partial\beta_s}
=-\sum_j\left[\sum_{k\in R_j}w_{jk}z_{k,r}z_{k,s}
-\bar z_{j,r}\bar z_{j,s}\right].
$$

Thus the [score and information of Cox partial likelihood](../../../survival-analysis.md#score-and-information-of-cox-partial-likelihood) are the sum of event-minus-risk-mean contrasts and the sum of risk-weighted covariance matrices, respectively. The Hessian is negative semidefinite; the [likelihood](../../../statistical-modelling.md#likelihood-function) is concave, with strict identifiability requiring variation in the relevant risk-set [covariates](../../../statistical-model.md#covariate).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

At event time $t_j$, the vector [Schoenfeld residual](../../../survival-analysis.md#schoenfeld-residual) is

$$
\boxed{r_j=z_{i_j}-\bar z_j(\widehat\beta),}
$$

where $\widehat\beta$ is the fitted partial-likelihood coefficient. It compares the [covariate](../../../statistical-model.md#covariate) of the person who actually failed with the [covariate](../../../statistical-model.md#covariate) [mean](../../../probability-theory.md#expected-value) predicted for the failing person, using the fitted [hazard](../../../survival-analysis.md#hazard-function) weights over the [risk set](../../../survival-analysis.md#risk-set). Under the model at the true coefficient, the conditional expected failing [covariate](../../../statistical-model.md#covariate) is precisely that weighted [mean](../../../probability-theory.md#expected-value), so the corresponding [Schoenfeld function](../../../survival-analysis.md#schoenfeld-function) is conditionally centered at zero. Residuals are defined at observed events, not at censoring times.

The score equation from part (a) is exactly

$$
U(\beta)=\sum_j[z_{i_j}-\bar z_j(\beta)].
$$

At a finite interior unpenalized maximum, $U(\widehat\beta)=0$, so

$$
\boxed{\sum_j r_j=0.}
$$

This is the intended fitted-residual identity. For an arbitrary trial coefficient it is a score, not generally zero; a single event with [covariates](../../../statistical-model.md#covariate) zero and one in its [risk set](../../../survival-analysis.md#risk-set) can have Schoenfeld function $1/2$ at $\beta=0$. Penalized estimates or a boundary maximum also need their own score conditions rather than this unqualified zero-sum assertion.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Under [proportional hazards](../../../survival-analysis.md#proportional-hazards-model), each coefficient is constant over event time. Examine the [Schoenfeld residuals](../../../survival-analysis.md#schoenfeld-residual), preferably [scaled Schoenfeld residuals](../../../survival-analysis.md#scaled-schoenfeld-residual), against time or a prespecified transformation such as log time, ranks or a fitted survival-time transformation. Plot a smooth trend and its uncertainty for each [covariate](../../../statistical-model.md#covariate). Under the working model there should be no systematic residual-time association; a persistent trend suggests a time-varying coefficient. In a coefficient-scale plot that adds $\widehat\beta$ to the scaled residuals, the null trend is horizontal at the fitted coefficient.

A formal [proportional hazards assumption test](../../../survival-analysis.md#proportional-hazards-assumption-test) can add a time interaction, for example $\beta_r(t)=\beta_r+\theta_r g(t)$, and test $\theta_r=0$ using a score test with information adjusted for the fitted constant coefficients. The score contributions involve the Schoenfeld functions weighted by $g(t_j)$. One can test each [covariate](../../../statistical-model.md#covariate) and use a joint global test for a vector of time-interaction coefficients. Such an association would be possible despite the unweighted residual sum being zero, so that fitted identity does not establish [proportional hazards](../../../survival-analysis.md#proportional-hazards-model).

**A systematic nonhorizontal coefficient trend or significant residual-time association is evidence against a constant [hazard ratio](../../../survival-analysis.md#hazard-ratio).** Failure to reject is compatible with the assumption, not proof of it. These diagnostics target the proportionality restriction; they do not by themselves verify [covariate](../../../statistical-model.md#covariate) functional form or independence of the censoring mechanism.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2008](../../2008.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
