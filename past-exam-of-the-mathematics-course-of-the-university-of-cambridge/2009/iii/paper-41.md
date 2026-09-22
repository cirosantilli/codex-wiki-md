# Paper 41

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper41.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper41.pdf)

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
    - [iv](#2/b/iv)
      - [Solution](#2/b/iv/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)

## 1

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Use separate [randomization](../../../causal-inference.md#randomization) lists for women with and without a self-reported history of depression. Within each [stratum](../../../survival-analysis.md#stratum), the central service could assign intervention and control in a $1:1$ ratio using randomly permuted blocks, preferably with concealed and varying block sizes. This is [stratified randomization](../../../causal-inference.md#stratified-randomization); the internet service can retain [allocation concealment](../../../causal-inference.md#allocation-concealment) because the recruiting staff do not know the next assignment.

History is plausibly prognostic for the outcome. Keeping its distribution similar between arms reduces the risk of a chance imbalance in that important baseline factor and can improve precision. It also allows a comparison within each history [stratum](../../../survival-analysis.md#stratum). Stratification does not guarantee balance of every other [covariate](../../../statistical-model.md#covariate), and staff must not be allowed to choose assignments. The [regression model](../../../statistical-model.md#regression-model) can retain history as a [baseline covariate](../../../statistical-model.md#baseline-covariate), respecting the design.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Specify the expected control-group event probability at the chosen follow-up time, the intervention probability or smallest clinically important absolute reduction to detect, the primary test's [significance level](../../../statistical-modelling.md#significance-level) and whether it is one- or two-sided, the desired [statistical power](../../../probability-and-statistics.md#statistical-power), and the allocation ratio. [Statistical power](../../../probability-and-statistics.md#statistical-power) is the [probability](../../../probability-theory.md#probability) of rejecting the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) under that specified alternative; its complement is the [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) probability.

For two independent binary-outcome groups, these probabilities determine the response [variances](../../../variance.md) needed by the sample-size calculation. Also specify how much loss to follow-up is anticipated when converting the required evaluable sample into a recruitment target. Here the design is balanced and the stated primary [significance level](../../../statistical-modelling.md#significance-level) is $0.05$. A target [statistical power](../../../probability-and-statistics.md#statistical-power) such as $80\%$ or $90\%$ and the anticipated event [probabilities](../../../probability-theory.md#probability) cannot be recovered from the [sample size](../../../probability-and-statistics.md#sample-size) alone, so they should not be invented. The recruitment inflation allows for attrition rather than changing the target effect.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The primary outcome addresses the main prespecified question; the secondary outcomes involve several additional comparisons. Testing each at $0.05$ would increase the chance of at least one false positive across them. The smaller secondary [significance level](../../../statistical-modelling.md#significance-level) makes their individual tests more conservative, reducing [multiple testing](../../../statistical-modelling.md#multiple-hypothesis-testing) problems.

This is a design distinction between confirmatory and additional outcomes, not a claim that secondary outcomes are intrinsically less important. A level of $0.01$ per secondary test does not by itself establish a particular bound on the [familywise error rate](../../../statistical-modelling.md#familywise-error-rate) unless the whole testing plan and number of tests are specified. Likewise, having two primary measurements still needs a clear prespecified reporting and multiplicity strategy.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The research nurses should be unaware of each woman's randomized allocation. [Blinded outcome assessment](../../../causal-inference.md#blinded-outcome-assessment) reduces the possibility that knowledge of receiving peer support changes how questions are asked, how answers are interpreted, or how a clinical diagnosis is recorded. It is especially useful for interview-based and partly subjective outcomes.

The mothers and volunteers would generally know whether calls took place. A mother might mention her volunteer, or a nurse might infer allocation from the conversation or consult records revealing it. This can break assessor blinding even when the allocation list is hidden. Standardized outcome interviews, separate intervention records and asking participants not to disclose allocation can help. Outcome assessment blinding is distinct from [allocation concealment](../../../causal-inference.md#allocation-concealment) at recruitment, and does not prevent participants' own awareness from affecting reported symptoms.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Let $Y_i=1$ indicate a depressed outcome and $C_i=1$ indicate the control arm. A [logistic regression](../../../statistical-modelling.md#logistic-regression) could specify

$$
\log\frac{p_i}{1-p_i}=\beta_0+\beta_C C_i+\gamma^T x_i,
\qquad p_i=\Pr(Y_i=1\mid C_i,x_i),
$$

with $x_i$ containing prespecified baseline characteristics, including the stratification factor. Fit the coefficients by maximizing the [likelihood](../../../statistical-modelling.md#likelihood-function) for independent [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) $\prod_i p_i^{Y_i}(1-p_i)^{1-Y_i}$. For equal [covariate](../../../statistical-model.md#covariate) values the control-to-intervention [odds ratio](../../../statistical-modelling.md#odds-ratio) is $e^{\beta_C}$. Thus an estimate $\widehat\beta_C=\log(2.1)$ produces the quoted adjusted ratio. An ordinary [Wald confidence interval](../../../statistical-inference.md#wald-confidence-interval) is obtained by exponentiating the endpoints of the coefficient's [confidence interval](../../../statistical-inference.md#confidence-interval).

The raw control-to-intervention [odds ratio](../../../statistical-modelling.md#odds-ratio), using the actual counts, is

$$
\boxed{\frac{78/(316-78)}{40/(297-40)}
=\frac{78\cdot257}{238\cdot40}\simeq2.106.}
$$

Using only the quoted percentages gives about $2.05$, so both versions are approximately $2.1$. The printed $14\%$ is not the usual whole-percentage rounding of $40/297\simeq13.47\%$; using the counts avoids that small numerical inconsistency. The reversed intervention-to-control ratio is about $0.475$.

The apparent surprise is a coding issue: with depression as the adverse outcome and intervention relative to control, protection would give an [odds ratio](../../../statistical-modelling.md#odds-ratio) below one. A ratio above one is favourable if the comparison is control relative to intervention, as above, or if the outcome has been recoded as absence of depression and intervention is compared with control. Both comparison and outcome must be specified. The adjusted ratio need not equal the crude one, even in a randomized trial: [covariate](../../../statistical-model.md#covariate) adjustment and [noncollapsibility of the odds ratio](../../../statistical-modelling.md#noncollapsibility-of-the-odds-ratio) can change an [odds ratio](../../../statistical-modelling.md#odds-ratio). Their close numerical values here do not prove that the regression adjustment was unnecessary.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

There was no clear documentation of initiation for $349-328=21$ women, giving

$$
\boxed{100\frac{21}{349}\simeq6.0\%.}
$$

These women may not have received the intervention, although missing documentation is not proof that no contact occurred. Documentation of initiation also does not establish completion or full adherence.

Under [intention-to-treat analysis](../../../causal-inference.md#intention-to-treat-analysis), women retain their randomized arm regardless of actual uptake. Removing nonadherent women would condition on a post-randomization characteristic and could destroy the comparability created by [randomization](../../../causal-inference.md#randomization). The resulting estimand is the effect of offering the intervention under the trial's actual adherence pattern. Keeping nonadherent women in their arm does not itself solve missing-outcome problems: the reported 12-week denominators are smaller than the randomized totals, so the outcome analysis still needs an appropriate strategy and assumptions for losses to follow-up.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The [number needed to treat](../../../causal-inference.md#number-needed-to-treat) is the reciprocal of the absolute reduction in the 12-week adverse-outcome risk. Using the counts rather than rounding the percentages first gives

$$
\widehat\Delta=\frac{78}{316}-\frac{40}{297}\simeq0.11216,
\qquad\boxed{\mathrm{NNT}=\frac1{\widehat\Delta}\simeq8.92,\ \text{reported as }9.}
$$

This means about nine high-risk women would need to be offered the intervention to prevent one additional screen-defined case over that follow-up, under the trial's comparison. It is not a lifetime quantity or automatically an estimate for clinical-interview diagnoses. Calculating from the rounded difference $25\%-14\%$ gives approximately nine but need not give the same integer rounding; the exact counts explain the reported value.

For a [confidence interval](../../../statistical-inference.md#confidence-interval), first construct an interval for the difference between the two [independent](../../../random-variable.md#independent-random-variables) event proportions, allowing for [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) sampling uncertainty. If both risk-reduction endpoints are positive, take their reciprocals and reverse their order to obtain an NNT interval. A [bootstrap](../../../statistical-modelling.md#bootstrapping-statistics) can instead resample women within their [randomized controlled trial](../../../causal-inference.md#randomized-controlled-trial) arms and transform the resulting risk-difference distribution. If the difference interval includes zero, the NNT confidence set extends through infinity and can include harm as well as benefit; it is not an ordinary bounded interval. The raw-outcome interval also relies on the missing-outcome assumptions discussed above.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

The clinical interview produced far fewer events, so the trial may have had substantially less [statistical power](../../../probability-and-statistics.md#statistical-power) for that measurement than for the screening-scale threshold. Its intervention-versus-control difference is less striking: the crude event proportions are about $4.7\%$ and $7.3\%$, based on only 37 diagnoses altogether. A concise abstract may therefore have emphasized the more statistically convincing screening result. These are possible explanations, not evidence of the authors' motives.

Nevertheless, a prespecified primary measure should not disappear merely because its result is less favourable. [Selective outcome reporting](../../../causal-inference.md#selective-outcome-reporting) could make the evidence seem more consistent across primary measurements than it is. A reasonable abstract should at least acknowledge the clinical result and its uncertainty, while distinguishing a positive screen from a diagnosis. Limited space can justify brevity, but not a misleading implication that both primary measures provide the same evidence.

The unexpectedly low clinical prevalence also merits investigation, including the telephone interview's implementation, timing, recruitment and diagnostic definition. A [meta-analysis](../../../statistical-inference.md#meta-analysis) of different studies is not automatically a like-for-like reference population; its higher pooled percentage does not by itself establish measurement failure in this trial.

## 2

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Interpret each mechanism for a fixed missingness pattern $r$: the observed and missing response components are the coordinates selected by that pattern, and the [covariates](../../../statistical-model.md#covariate) $X$ are assumed fully recorded.

For [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random), missingness depends on neither response values nor [covariates](../../../statistical-model.md#covariate):

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r).}
$$

For [covariate-dependent missing completely at random](../../../probability-and-statistics.md#covariate-dependent-missing-completely-at-random), response observation may depend on $X$ but not on the response after conditioning on $X$:

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r\mid X).}
$$

This is [conditional independence](../../../random-variable.md#conditional-independence) $R\perp Y\mid X$ and can still produce a marginal association between response and missingness.

For [covariate-dependent missing at random](../../../probability-and-statistics.md#covariate-dependent-missing-at-random), the observation probability may use observed response components and [covariates](../../../statistical-model.md#covariate), but not the values missing under that pattern:

$$
\boxed{f(r\mid Y^o,Y^m,X)=f(r\mid Y^o,X).}
$$

For [missing not at random](../../../probability-and-statistics.md#missing-not-at-random), there remains dependence on $Y^m$ after conditioning on $Y^o,X$; the displayed simplification is not valid. For example, refusal could depend on the unreported response itself, even among individuals sharing all recorded [covariates](../../../statistical-model.md#covariate). These mechanisms concern the reason for nonobservation, not whether the incomplete records merely look irregular. Their distinction is not generally identifiable from the observed responses alone.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The observed positive counts are $200(0.18)=36$ and $400(0.08)=32$. Thus the responder-only estimate is

$$
\boxed{\widehat p_R=\frac{36+32}{600}=\frac{68}{600}\simeq11.33\%.}
$$

This estimates the proportion among the responders; it does not yet address either kind of nonresponse.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Assume that, conditional on the recorded embarrassment category, answering the item is independent of virginity status. Also assume that this category is assessed comparably for both groups and that both response strata have positive observation probabilities. This is [covariate-dependent missing completely at random](../../../probability-and-statistics.md#covariate-dependent-missing-completely-at-random) for the item response with embarrassment as the fully observed [covariate](../../../statistical-model.md#covariate); it supports [MAR standardization over a fully observed covariate](../../../probability-and-statistics.md#mar-standardization-over-a-fully-observed-covariate).

Use the responder probabilities $0.18$ and $0.08$ within strata, but the [stratum](../../../survival-analysis.md#stratum) sizes in the full group of responders plus item nonresponders: $300$ and $450$. This gives

$$
\boxed{\widehat p_{R+I}=\frac{300(0.18)+450(0.08)}{750}
=\frac{90}{750}=12\%.}
$$

Equivalently, the estimated missing positive counts are $100(0.18)=18$ and $50(0.08)=4$, adding 22 to the 68 observed positives. The marginal estimate changes because the full group contains a larger proportion judged embarrassed. Merely copying the unstratified responder percentage would ignore that difference. The [conditional independence](../../../random-variable.md#conditional-independence) assumption cannot be verified using the missing item responses.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

The [unit and item nonresponse](../../../probability-and-statistics.md#unit-and-item-nonresponse) distinction matters: embarrassment was not recorded for the 300 unit nonresponders. [Conditional independence](../../../random-variable.md#conditional-independence) of unit response and virginity given embarrassment is therefore not enough unless the embarrassment distribution among unit nonresponders is also supplied.

One sufficient set of additional assumptions is that unit response is independent of the pair consisting of embarrassment and virginity. Equivalently for this estimation purpose, assume that unit nonresponders have the same embarrassment mixture as the other 750 individuals, and the same virginity probabilities within those strata. The former gives an embarrassed fraction $300/750=0.4$, and the latter gives probabilities $0.18$ and $0.08$. Their estimated positive proportion is consequently $0.4(0.18)+0.6(0.08)=0.12$, or 36 of the 300. Combining the groups gives

$$
\boxed{\widehat p_{\mathrm{all}}=\frac{90+36}{1050}=12\%.}
$$

The item-response assumption from (ii) supplies the first 90; the added unit-response transport assumptions supply the final 36. A weaker sufficient assumption is simply that the unit nonresponders' marginal virginity proportion equals the estimated $12\%$ in the other group, but it is still untestable from these data.

Without any unit-response transport assumption, retain the item assumption and write the unidentified unit proportion as $p_U$. Then

$$
p_{\mathrm{all}}=\frac{90+300p_U}{1050},\qquad
\boxed{8.57\%\leq p_{\mathrm{all}}\leq37.14\%.}
$$

Thus the extrapolation is an assumption-dependent estimate, not a quantity determined by the observed table alone.

<h4 id="2/b/iv">iv</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/b/iv)

A [sensitivity analysis for unit and item nonresponse](../../../probability-and-statistics.md#sensitivity-analysis-for-unit-and-item-nonresponse) asks how much the population estimate and substantive conclusions change when the untestable response assumptions are weakened. Vary plausible virginity probabilities among the missing groups, and vary the unknown embarrassment mixture among unit nonresponders; identify combinations which materially alter the estimate or reverse a conclusion.

For example, let $a,b$ be the positive probabilities among embarrassed and nonembarrassed item nonresponders, let $q$ be the embarrassed fraction among unit nonresponders, and let $c,d$ be their corresponding positive probabilities. The sensitivity estimate is

$$
\boxed{p_{\mathrm{all}}(a,b,c,d,q)=\frac{68+100a+50b+300[qc+(1-q)d]}{1050}.}
$$

The nominal assumptions set $a=c=0.18$, $b=d=0.08$ and $q=0.4$, reproducing $12\%$. Different choices model outcome-dependent refusal or a changed mixture. Sampling [confidence intervals](../../../statistical-inference.md#confidence-interval) measure a different uncertainty and should also be reported where appropriate; they do not validate the missingness assumptions.

## 3

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

A [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family) has a common [baseline hazard](../../../survival-analysis.md#baseline-hazard) $h_0$ and positive constants $a_z$ such that $h_z(t)=a_z h_0(t)$. Thus its [hazard ratios](../../../survival-analysis.md#hazard-ratio) are constant in time, and its [survivor functions](../../../survival-analysis.md#survival-function) satisfy $S_z(t)=S_0(t)^{a_z}$. An [accelerated life family](../../../survival-analysis.md#accelerated-life-family) instead has positive constants $c_z$ such that $T_z$ has the distribution of $c_zT_0$. Equivalently, $S_z(t)=S_0(t/c_z)$: all time [quantiles](../../../probability-theory.md#quantile-function) are multiplied by the same factor. These two properties are generally different.

Integrating the printed [Weibull distribution](../../../probability-theory.md#weibull-distribution) density, or differentiating the following expression and checking its initial value, gives

$$
S_{p,\lambda}(t)=\exp[-(\lambda t)^p],\qquad
H_{p,\lambda}(t)=(\lambda t)^p,\qquad
h_{p,\lambda}(t)=p\lambda^p t^{p-1}.
$$

Here $\lambda$ is an inverse-time parameter: the coefficient of $t^p$ in the [cumulative hazard](../../../survival-analysis.md#cumulative-hazard-function) is $\lambda^p$, not $\lambda$. This matters when comparing different parameterizations of a [Weibull distribution](../../../probability-theory.md#weibull-distribution).

With common shape $p$, the [hazard ratio](../../../survival-analysis.md#hazard-ratio) is

$$
\boxed{\frac{h_{p,\lambda_1}(t)}{h_{p,\lambda_2}(t)}
=\left(\frac{\lambda_1}{\lambda_2}\right)^p.}
$$

It does not depend on $t$, proving membership in one [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family). For the other property,

$$
S_{p,\lambda_1}(t)=S_{p,\lambda_2}\left(\frac{\lambda_1}{\lambda_2}t\right),
\qquad
\boxed{T_1\ \overset{d}{=}\ \frac{\lambda_2}{\lambda_1}T_2.}
$$

Consequently they also belong to one [accelerated life family](../../../survival-analysis.md#accelerated-life-family). A larger inverse-time parameter gives shorter survival times and larger hazards, consistently in both descriptions. This is the common-shape case of [Weibull accelerated-life and proportional-hazards families](../../../survival-analysis.md#weibull-accelerated-life-and-proportional-hazards-families).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Write the [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model) as $h_i(t)=h_0(t)u_i$, where $u_i=\exp(\beta^Tz_i)$ is the [hazard multiplier](../../../survival-analysis.md#hazard-multiplier) and $h_0$ is the unspecified [baseline hazard](../../../survival-analysis.md#baseline-hazard). At an untied event time $t_j$, let $R_j$ be the [risk set](../../../survival-analysis.md#risk-set) immediately before the event and $i_j$ its failing individual. With [independent censoring](../../../survival-analysis.md#independent-censoring) conditional on the [covariates](../../../statistical-model.md#covariate), the [conditional probability](../../../probability-theory.md#conditional-probability) that individual $i$ supplies the next event, given an event at that time and the [risk set](../../../survival-analysis.md#risk-set), is obtained by dividing its instantaneous event rate by the aggregate rate:

$$
\Pr(i_j=i\mid\text{one event at }t_j,R_j)
=\frac{h_0(t_j)u_i}{\sum_{k\in R_j}h_0(t_j)u_k}
=\frac{u_i}{\sum_{k\in R_j}u_k}.
$$

More precisely this is the limit of the [conditional probability](../../../probability-theory.md#conditional-probability) for one event in a short interval; simultaneous events have smaller-order probability in the continuous model. Multiplication of these successive conditional contributions gives the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood)

$$
\boxed{L_P(\beta)=\prod_{j:\,\text{event}}\frac{\exp(\beta^Tz_{i_j})}{\sum_{k\in R_j}\exp(\beta^Tz_k)}.}
$$

Censored individuals remain in each [risk set](../../../survival-analysis.md#risk-set) until their [censoring](../../../survival-analysis.md#censoring-statistics) time but supply no numerator. Conditioning removes the [baseline hazard](../../../survival-analysis.md#baseline-hazard); this is a [partial likelihood](../../../survival-analysis.md#partial-likelihood) for $\beta$, rather than a complete [likelihood](../../../statistical-modelling.md#likelihood-function) for event and [censoring](../../../survival-analysis.md#censoring-statistics) times.

**Ties require an observation model or an approximation.** Suppose a recorded tie hides the order of $d$ continuous events, with no intervening entry or [censoring](../../../survival-analysis.md#censoring-statistics). Put $D$ for the tied event set and $S=\sum_{i\in R}u_i$. An exact marginal contribution for the coarsened ranks is the sum of the ordinary rank contributions over every possible order:

$$
L_{\mathrm{rank},D}=\sum_{\pi\in\operatorname{Perm}(D)}
\prod_{q=0}^{d-1}\frac{u_{\pi_{q+1}}}{S-\sum_{r=1}^{q}u_{\pi_r}}.
$$

For example, if $A,B$ fail together while $C$ remains at risk, the two possible orders give

$$
L_{\mathrm{rank},\{A,B\}}=
\frac{u_Au_B}{S}\left(\frac1{S-u_A}+\frac1{S-u_B}\right),
\qquad S=u_A+u_B+u_C.
$$

The [risk set](../../../survival-analysis.md#risk-set) is depleted after the first of the two events. This expression concerns the missing event order; it is not the full [likelihood](../../../statistical-modelling.md#likelihood-function) of an interval in which the events occurred.

Convenient alternatives are the [Breslow approximation for tied event times](../../../survival-analysis.md#breslow-approximation-for-tied-event-times) and the [Efron approximation for tied event times](../../../survival-analysis.md#efron-approximation-for-tied-event-times):

$$
L_{B,D}=\frac{\prod_{i\in D}u_i}{S^d},\qquad
L_{E,D}=\frac{\prod_{i\in D}u_i}{\prod_{q=0}^{d-1}[S-(q/d)\sum_{i\in D}u_i]}.
$$

The first keeps the initial denominator at every event; the second removes an average share of the tied-event multipliers successively. In the example their denominators are $S^2$ and $S[S-(u_A+u_B)/2]$. These conventional partial-likelihood factors omit multiplicities independent of $\beta$, which do not affect its estimate; they should not be mistaken for normalized probabilities of the unordered event set.

For genuinely discrete event times there is another exact construction. If individual event odds are proportional to $u_i$, conditioning on exactly $d$ events gives the [exact tied-set conditional likelihood](../../../survival-analysis.md#exact-tied-set-conditional-likelihood)

$$
L_{\mathrm{set},D}=\frac{\prod_{i\in D}u_i}{\sum_{A\subseteq R:\,|A|=d}\prod_{i\in A}u_i}.
$$

For the same three individuals this is $u_Au_B/(u_Au_B+u_Au_C+u_Bu_C)$. It is not generally equal to the continuous-time rank sum: the assumptions differ.

Large tie groups make naive summation over $d!$ orders or $\binom{|R|}{d}$ subsets impractical. Recursion helps with the subset denominator, and Breslow or Efron avoids exhaustive enumeration. However, extensive ties can also indicate that time is measured too coarsely for an exact continuous-time ordering to be a useful target.

For example, if patients are assessed only at annual visits, use one row per patient-year still at risk and model the probability $p_{ij}$ of an event in that interval. A [grouped proportional-hazards model](../../../survival-analysis.md#grouped-proportional-hazards-model) follows directly by integrating the hazard over the interval, with [covariates](../../../statistical-model.md#covariate) constant there:

$$
p_{ij}=1-\exp[-\Delta H_{0j}\exp(\beta^Tz_i)],
\qquad
\boxed{\log[-\log(1-p_{ij})]=\alpha_j+\beta^Tz_i,\quad
\alpha_j=\log\Delta H_{0j}.}
$$

Fit the resulting person-period [likelihood](../../../statistical-modelling.md#likelihood-function), with [Bernoulli distributions](../../../discrete-probability-distribution.md#bernoulli-distribution) for the interval event indicators and interval-specific intercepts. Many events in the same year are then ordinary observations rather than a combinatorial ordering problem. This requires a compatible interval-observation scheme and appropriate [independent censoring](../../../survival-analysis.md#independent-censoring); it avoids pretending that unobserved within-year event times are known.

## 4

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Let $N(t)$ count observed events and $Y(t)$ count individuals still in the [risk set](../../../survival-analysis.md#risk-set) just before $t$. Under a common [hazard function](../../../survival-analysis.md#hazard-function) $h(t)$ and [independent censoring](../../../survival-analysis.md#independent-censoring), the expected event count over a short interval, conditional on the observed past, is

$$
\operatorname E[dN(t)\mid\mathcal F_{t-}]=Y(t)h(t)\,dt=Y(t)\,dH(t).
$$

Here $H(t)=\int_0^t h(u)\,du$ is the [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function). Thus an estimating increment for $dH$ is $dN/Y$, on the range where the [risk set](../../../survival-analysis.md#risk-set) is nonempty. Accumulating these increments gives the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1_{\{Y(u)>0\}}}{Y(u)}\,dN(u)
=\sum_{t_j\leq t}\frac{\delta_j}{r_j}.}
$$

The observation times $t_j$ include both events and censorings, $r_j=Y(t_j)$, and $\delta_j$ is one for an event and zero for [censoring](../../../survival-analysis.md#censoring-statistics). Without ties each event adds $1/r_j$; [censoring](../../../survival-analysis.md#censoring-statistics) changes later [risk sets](../../../survival-analysis.md#risk-set) but adds nothing immediately. Equivalently, the local event fraction estimates the local hazard increment, and summing those estimates produces the [integrated hazard](../../../survival-analysis.md#cumulative-hazard-function). The [counting-process intensity in survival analysis](../../../stochastic-process.md#counting-process-intensity-in-survival-analysis) justifies this estimating equation; it does not imply exact finite-sample unbiasedness after the [risk set](../../../survival-analysis.md#risk-set) can become empty.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Assume the usual cohort setup: all individuals enter at time zero, each contributes one event or [censoring](../../../survival-analysis.md#censoring-statistics) time, and every such observation is included. Order these distinct observation times as $t_1<\cdots<t_m$. The [risk set](../../../survival-analysis.md#risk-set) size just before $t_k$ is then $r_k=m-k+1$. Write $\delta_k=1$ for an event and zero for [censoring](../../../survival-analysis.md#censoring-statistics). Including the jump at an event time, the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) is

$$
\widehat H_j=\sum_{k=1}^{j}\frac{\delta_k}{m-k+1}.
$$

Exchange the two finite sums:

$$
\sum_{j=1}^{m}\widehat H_j
=\sum_{k=1}^{m}\frac{\delta_k}{m-k+1}\sum_{j=k}^{m}1
=\sum_{k=1}^{m}\delta_k.
$$

Thus **the sum equals the number of observed events**. Each event increment appears once for each individual still at risk at that event, exactly cancelling its denominator. This is the [event-count identity for Nelson–Aalen cumulative hazards](../../../survival-analysis.md#event-count-identity-for-nelson-aalen-cumulative-hazards). The cohort and entry convention matter: delayed entry would invalidate the simple equation $r_k=m-k+1$ and require a modified identity.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

One method breaks a tied group into a sequence of distinct artificial times, by a specified or random ordering. Process tied events before tied censorings if their common recorded time means the censored individuals were still under observation when the events occurred. At each artificial event, add the reciprocal of the current [risk set](../../../survival-analysis.md#risk-set) size and then remove that individual. This applies the untied [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) to the resulting grid. For example, two tied failures among two individuals give successive increments $1/2$ and $1$.

On that expanded grid there is one observation time per individual. The cancellation argument in (b) is unchanged, so **breaking ties preserves the identity when the sum includes every artificially separated observation**. The chosen ordering can affect the estimated curve within a tied group and must not be presented as an observed event order.

A second method retains the recorded tied times. For a group with $d_j$ events and pre-time [risk set](../../../survival-analysis.md#risk-set) size $r_j$, the grouped [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) adds $d_j/r_j$ once. All events in the group use the same denominator; censorings in the group are removed afterwards. If two individuals fail at the same time and there are no other observations, the curve has one jump of $2/2=1$. Its sum over the one distinct time is $1$, whereas the event count is $2$. Hence **the unweighted distinct-time identity does not generally survive grouping ties**. On the artificially separated grid in the first method, the two post-observation values would instead be $1/2$ and $3/2$, whose sum is $2$.

There is nevertheless an exact weighted version for the grouped method. Let $n_j$ count all observations, event or [censoring](../../../survival-analysis.md#censoring-statistics), at distinct time $t_j$. With everyone entering at zero, $r_k=\sum_{j\geq k}n_j$. Therefore

$$
\boxed{\sum_j n_j\widehat H(t_j)
=\sum_k\frac{d_k}{r_k}\sum_{j\geq k}n_j
=\sum_kd_k.}
$$

This [grouped Nelson–Aalen event-count identity](../../../survival-analysis.md#grouped-nelson-aalen-event-count-identity) sums over individuals, with repeated values for tied times, rather than once per distinct time. Keeping that distinction resolves the apparent conflict between a valid grouped estimator and failure of the literal unweighted formula.

## 5

↑ **Parent:** [Paper 41](paper-41.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A standard setting is [relative survival](../../../survival-analysis.md#relative-survival) in cancer registries. Patients' all-cause mortality is compared with mortality expected from population life tables matched for factors such as attained age, sex and calendar year. These provide the known individual [background hazards](../../../survival-analysis.md#background-hazard) $h_B^{(i)}$; the remaining common [excess hazard](../../../survival-analysis.md#excess-hazard) $h_E$ describes mortality above that expected background.

This is useful when causes of death are incomplete or unreliable: all observed deaths can be used without deciding which were caused by the cancer. It also separates changes in background population mortality from excess mortality in the diseased cohort. The reference life tables must be appropriate, and a common [excess hazard](../../../survival-analysis.md#excess-hazard) is a modeling assumption, not automatic. A [relative survivor function](../../../survival-analysis.md#relative-survivor-function) can then describe the cohort's excess survival, but interpreting it as the effect of a causal elimination of the disease requires further assumptions.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Define the individual background [survivor function](../../../survival-analysis.md#survival-function) and common excess component by

$$
F_B^{(i)}(t)=\exp\left[-\int_0^t h_B^{(i)}(u)\,du\right],
\qquad
\boxed{F_E(t)=\exp\left[-\int_0^t h_E(u)\,du\right].}
$$

Integrating the additive [hazard function](../../../survival-analysis.md#hazard-function) decomposition gives

$$
F^{(i)}(t)=F_B^{(i)}(t)F_E(t),\qquad F_E(t)=\frac{F^{(i)}(t)}{F_B^{(i)}(t)}.
$$

The [relative survivor function](../../../survival-analysis.md#relative-survivor-function) therefore compares actual survival with the survival expected from background mortality, and is common across individuals under this model. If $h_E\geq0$, it is the [survivor function](../../../survival-analysis.md#survival-function) of a hypothetical process having only the [excess hazard](../../../survival-analysis.md#excess-hazard). If excess mortality can be negative, the ratio may exceed one and lacks an ordinary survival-probability interpretation.

To estimate it, let $Y_i(u)$ indicate that individual $i$ is in the [risk set](../../../survival-analysis.md#risk-set), let $Y(u)=\sum_iY_i(u)$, and let $N(u)$ count all observed deaths. Assume appropriate [independent censoring](../../../survival-analysis.md#independent-censoring). The aggregate event intensity is

$$
\sum_iY_i(u)h^{(i)}(u)
=Y(u)h_E(u)+\sum_iY_i(u)h_B^{(i)}(u).
$$

Consequently the background correction must use the current risk-set average

$$
\overline h_B(u)=\frac{\sum_iY_i(u)h_B^{(i)}(u)}{Y(u)},\qquad
B_R(t)=\int_0^t\overline h_B(u)\,du,
$$

only on the observed range where $Y>0$. Dividing the event count by $Y$ estimates the total hazard there. Subtracting the known average background gives the [offset-adjusted cumulative hazard estimator](../../../survival-analysis.md#offset-adjusted-cumulative-hazard-estimator)

$$
\boxed{\widehat H_E(t)=\sum_{t_j\leq t}\frac{d_j}{r_j}-B_R(t).}
$$

Here $d_j$ is the event count at $t_j$ and $r_j=Y(t_j)$; under an untied scheme $d_j=1$. One possible estimate is $\widehat F_{E,\exp}=\exp[-\widehat H_E]$.

A product-limit version retains the full event fraction, which is especially relevant when the excess mortality is not small. Estimate the relative-survival differential equation $dF_E/F_E=-dH_E$ by

$$
\frac{d\widehat F_E(t)}{\widehat F_E(t-)}=-\frac{dN(t)}{Y(t)}+\overline h_B(t)\,dt.
$$

At an event time it multiplies the curve by $1-d_j/r_j$. Between events it solves $\widehat F_E'=\overline h_B\widehat F_E$. Starting at one therefore gives the [risk-set-adjusted relative survivor estimator](../../../survival-analysis.md#risk-set-adjusted-relative-survivor-estimator)

$$
\boxed{\widehat F_E(t)=\exp[B_R(t)]\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right)
=\exp[B_R(t)]\widehat S_{\mathrm{KM}}(t).}
$$

The [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) factor accounts for observed all-cause mortality; the continuous multiplier corrects for known background mortality. The exponential cumulative-hazard version instead has event jumps $\exp(-d_j/r_j)$; it is close when event fractions are small but is not identical to this product-limit version.

Even if each [background hazard](../../../survival-analysis.md#background-hazard) is small, its accumulated contribution over long follow-up cannot simply be discarded. Nor should the excess contribution be linearized merely because the background is small. Using the known background integral inside the exponential avoids both errors. The average is over the evolving [risk set](../../../survival-analysis.md#risk-set): replacing it by an initial-cohort mean, or dividing by an arbitrary average of individual background [survivor functions](../../../survival-analysis.md#survival-function), is generally wrong when the [background hazards](../../../survival-analysis.md#background-hazard) differ. [Censoring](../../../survival-analysis.md#censoring-statistics) and deaths change which individuals contribute to the background correction.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Use the product-limit estimate in (b). Between consecutive event times there are no mortality jumps, so

$$
\frac{d\widehat F_E(t)}{dt}=\overline h_B(t)\widehat F_E(t).
$$

Thus **the estimated relative survivor curve rises between events** when background mortality is positive, and is constant if it is zero. [Censoring](../../../survival-analysis.md#censoring-statistics) changes the [risk set](../../../survival-analysis.md#risk-set) and can change the slope, but supplies no downward event jump. At the next event time the curve is multiplied by $1-d_k/r_k$.

Provided the curve is still positive, the ratio of the post-event estimates at the two consecutive event times is

$$
\frac{\widehat F_E(t_k)}{\widehat F_E(t_j)}
=\exp\left[\int_{t_j}^{t_k}\overline h_B(u)\,du\right]
\left(1-\frac{d_k}{r_k}\right).
$$

For $d_k<r_k$, the later value is larger precisely when

$$
\boxed{\int_{t_j}^{t_k}\overline h_B(u)\,du>
-\log\left(1-\frac{d_k}{r_k}\right).}
$$

For example, suppose there are 100 individuals in the [risk set](../../../survival-analysis.md#risk-set) after the earlier event, no intervening [censoring](../../../survival-analysis.md#censoring-statistics), a 20-day gap, and one death at its end. If every [background hazard](../../../survival-analysis.md#background-hazard) is $0.001$ per day, then the integrated background contribution is $0.02$ and

$$
\frac{\widehat F_E(t_k)}{\widehat F_E(t_j)}=e^{0.02}(1-1/100)\simeq1.010>1.
$$

The individual [background hazards](../../../survival-analysis.md#background-hazard) are small, but the interval contains less observed mortality than expected from that background. This can occur by chance in a small event sample or when the cohort is healthier than the life-table reference on other dimensions.

A nonnegative true [excess hazard](../../../survival-analysis.md#excess-hazard) makes $F_E$ nonincreasing, but this unconstrained [estimator](../../../statistical-modelling.md#estimator) need not inherit that restriction. An increase is therefore not proof of a clinical survival benefit. If the exponential cumulative-hazard version is chosen instead, its corresponding condition is $\int_{t_j}^{t_k}\overline h_B>d_k/r_k$; the qualitative explanation remains the same. If the [risk set](../../../survival-analysis.md#risk-set) is exhausted by deaths, the product-limit factor is zero and no later increase is possible.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
