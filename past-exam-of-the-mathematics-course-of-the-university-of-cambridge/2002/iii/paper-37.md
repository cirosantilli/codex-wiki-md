# Paper 37

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper37.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2002/Paper37.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
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
- [5](#5)
  - [i](#5/i)
    - [Solution](#5/i/solution)
  - [ii](#5/ii)
    - [Solution](#5/ii/solution)
  - [iii](#5/iii)
    - [Solution](#5/iii/solution)
- [6](#6)
  - [i](#6/i)
    - [Solution](#6/i/solution)
  - [ii](#6/ii)
    - [Solution](#6/ii/solution)
  - [iii](#6/iii)
    - [Solution](#6/iii/solution)
  - [iv](#6/iv)
    - [Solution](#6/iv/solution)
  - [v](#6/v)
    - [Solution](#6/v/solution)

## 1

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Let $T_i$ be an event time and $C_i$ a potential censoring time. Under [independent censoring](../../../survival-analysis.md#independent-censoring), observe $Y_i=\min(T_i,C_i)$ and $\delta_i=\mathbf1\{T_i\leq C_i\}$. For an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\theta$, an observed failure contributes $\theta e^{-\theta Y_i}$ to the [survival likelihood](../../../survival-analysis.md#survival-likelihood), whereas a [right-censored](../../../survival-analysis.md#right-censoring) observation contributes $e^{-\theta Y_i}$. The censoring-law factors may be discarded when they are independent of $\theta$. Thus, writing $d=\sum_i\delta_i$ and $V=\sum_iY_i$ for total observed [person-time](../../../survival-analysis.md#person-time),

$$
L(\theta)\propto\theta^d e^{-\theta V},\qquad
\ell'(\theta)=\frac d\theta-V,\qquad
\ell''(\theta)=-\frac d{\theta^2}.
$$

For $d,V>0$ the unique [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is

$$
\boxed{\widehat\theta=\frac dV.}
$$

Censored times belong in $V$: they record time during which failure was not observed. With $d=0$ and $V>0$, the [likelihood](../../../statistical-modelling.md#likelihood-function) decreases with $\theta$, so the supremum is at the boundary $\theta\downarrow0$; there is no positive interior estimate. This is [exponential-rate estimation from censored exposure](../../../survival-analysis.md#exponential-rate-estimation-from-censored-exposure).

[Uninformative censoring](../../../survival-analysis.md#independent-censoring) means that the potential censoring time supplies no information about the latent failure time after conditioning on the modeled variables. A study ending at a fixed follow-up duration independent of prognosis is an example of [administrative censoring](../../../survival-analysis.md#administrative-censoring). [Informative censoring](../../../survival-analysis.md#informative-censoring) occurs, for example, when a seriously deteriorating patient withdraws because of that deterioration and the prognostic information is omitted from the model. Under [informative censoring](../../../survival-analysis.md#informative-censoring), those remaining in the [risk set](../../../survival-analysis.md#risk-set) are selected by their future failure propensity, so the ordinary [survival likelihood](../../../survival-analysis.md#survival-likelihood) and its estimate need not target the true rate.

Using the reported durations and flags as though they were valid [right-censored](../../../survival-analysis.md#right-censoring) records gives

$$
\boxed{\widehat\theta_{\rm labelled}=\frac{500}{1031.6}\simeq0.48468.}
$$

Treating all durations as failures instead gives

$$
\boxed{\widehat\theta_{\rm complete}=\frac{1000}{1031.6}\simeq0.96937.}
$$

Relabelling has halved the event count without shortening any observed follow-up. The resulting estimate is therefore exactly half the complete-data estimate.

**This is not a simulation of uninformative ordinary right-censoring.** For a record declared censored at $Y_i$, ordinary [right censoring](../../../survival-analysis.md#right-censoring) requires $T_i>Y_i$; the construction instead took $Y_i$ to be the simulated failure time itself. Keeping a failure time and hiding only its flag does not produce the minimum of that time and an independent earlier censoring time. Even choosing labels at random does not fix this: independence of a flag from the recorded duration is different from [independent censoring](../../../survival-analysis.md#independent-censoring) of a latent event time. Indeed the labelled durations still have mean one while the failure fraction is one half, so their ordinary censored estimate converges to $1/2$, not the generating rate one. Thus it is not a valid uninformative censoring scheme for the intended failure distribution; strictly, it has not implemented ordinary right-censoring of those simulated failure times at all. One could reproduce the randomly labelled record distribution with independent latent event and censoring times both of rate $1/2$, but that would be a different failure model, not the claimed rate-one model. Calling the flags random is therefore insufficient to justify the target distribution or its censored likelihood. This is the [random relabelling is not independent right censoring](../../../survival-analysis.md#random-relabelling-is-not-independent-right-censoring) issue.

A valid simulation draws independently $T\sim\operatorname{Exp}(1)$ and $C\sim\operatorname{Exp}(1)$, and records $(\min(T,C),\mathbf1\{T\leq C\})$. Since

$$
\Pr(C<T)=\int_0^\infty e^{-c}e^{-c}\,dc=\frac12,
$$

it gives [independent censoring](../../../survival-analysis.md#independent-censoring) with the requested probability. Equivalently generate $T=-\log U$ and $C=-\log V$ from independent uniform random numbers. Another valid choice is fixed censoring at $\log2$, since $\Pr(T>\log2)=1/2$. These give a random censored fraction with expectation one half; they do not promise exactly 500 censored records. For the independent-exponential scheme, observed durations have rate two and mean one half, so $d/\sum Y_i$ correctly converges to one.

## 2

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

For the numerical [competing risks](../../../survival-analysis.md#competing-risks) update, the estimated probability of remaining event-free just before the tied time is

$$
\widehat S(7.8-)=1-0.285-0.241=0.474.
$$

There were no intervening events, so the [cumulative incidence functions](../../../survival-analysis.md#cumulative-incidence-function) did not jump between the two stated times. The [Aalen–Johansen estimator](../../../survival-analysis.md#aalen-johansen-estimator) uses the [risk set](../../../survival-analysis.md#risk-set) immediately before the event time, including the subject censored at that same time under the usual events-before-censoring tie convention. Therefore the cause-$A$ increment is $0.474(2/20)$, and

$$
\boxed{\widehat F_A(7.8)=0.285+0.474\frac2{20}=0.3324.}
$$

For a consistency check, $\widehat F_B(7.8)=0.241+0.474/20=0.2647$ and $\widehat S(7.8)=0.474(1-3/20)=0.4029$; these sum to one. The censoring does not create an incidence jump and leaves $16$ subjects for subsequent follow-up. Dividing by $19$ would instead assume that the censored subject had already left before the event time, contrary to the stated immediately preceding [risk set](../../../survival-analysis.md#risk-set). This is a [cumulative incidence update with tied censoring](../../../survival-analysis.md#cumulative-incidence-update-with-tied-censoring).

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Interpret $h_A,h_B$ as [cause-specific hazards](../../../survival-analysis.md#cause-specific-hazard): their conditioning population consists of individuals still free of both events. Write

$$
H_A(t)=\int_0^t h_A(u)\,du,\qquad H_B(t)=\int_0^t h_B(u)\,du.
$$

In a short interval, either event removes an individual from that population. Hence the [survivor function](../../../survival-analysis.md#survival-function) satisfies $S'(t)=-S(t)[h_A(t)+h_B(t)]$, with $S(0)=1$. Integrating gives

$$
\boxed{\Pr(T>t)=S(t)=\exp\{-H_A(t)-H_B(t)\}.}
$$

No independence assumption on hypothetical latent event times is needed: this follows directly from the specified [cause-specific hazards](../../../survival-analysis.md#cause-specific-hazard).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

The probability of a first event of type $A$ in $(u,u+du)$ is the probability $S(u)$ of still being at risk times $h_A(u)du$. Thus its [cumulative incidence function](../../../survival-analysis.md#cumulative-incidence-function) is

$$
\boxed{F_A(t)=\int_0^t h_A(u)\exp\{-H_A(u)-H_B(u)\}\,du.}
$$

Similarly $F_B(t)=\int_0^t h_B(u)S(u)\,du$. In general $F_A(t)\ne1-e^{-H_A(t)}$: that latter expression ignores the competing removal caused by $B$ and instead describes a [net survival](../../../survival-analysis.md#net-survival) complement.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

The two event types are mutually exclusive as observed first outcomes. Summing their [cumulative incidence functions](../../../survival-analysis.md#cumulative-incidence-function) and using the [survivor function](../../../survival-analysis.md#survival-function) gives

$$
F_A(t)+F_B(t)=1-S(t).
$$

Taking the increasing limit in time therefore yields

$$
\boxed{\Pr(\text{an event ever occurs})=1-\exp\{-H_A(\infty)-H_B(\infty)\}.}
$$

The expression is one when the sum of the two [cumulative hazards](../../../survival-analysis.md#cumulative-hazard-function) diverges, with $e^{-\infty}=0$. Finite total [cumulative hazard](../../../survival-analysis.md#cumulative-hazard-function) leaves a positive probability of never experiencing either event.

## 3

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

Under the proposed exposure-only model, suppose a unit of infectious exposure has the same probability of producing an ascertained onset in either cohort. Conditional on the total of $108$ onsets, the allocation is a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with younger-cohort probability

$$
\pi=\frac{85000}{85000+170000}=\frac13.
$$

Thus the expected cohort counts are $36$ and $72$, respectively, whereas the observed allocation is reversed. The [Pearson chi-squared goodness-of-fit test](../../../statistical-modelling.md#pearson-chi-squared-goodness-of-fit-test) gives

$$
X^2=\frac{(72-36)^2}{36}+\frac{(36-72)^2}{72}=54.
$$

With one degree of freedom its approximate [p-value](../../../statistical-modelling.md#p-value) is $2.0\times10^{-13}$; the exact upper [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) tail $\Pr\{\operatorname{Bin}(108,1/3)\geq72\}$ is approximately $1.56\times10^{-12}$. These are exceptionally incompatible with proportional allocation. Equivalently, the observed onset count per exposure unit is four times larger in the younger cohort:

$$
\frac{72/85000}{36/170000}=4.
$$

**Under the stated common-risk exposure model, the observed counts are not consistent with the early exposure period as their sole explanation.** This does not identify the source of the discrepancy, or prove a particular later exposure caused it. The inference also requires comparable ascertainment and a common fraction of exposure-derived cases manifesting by the observation date. Age-independent [incubation periods](../../../mathematical-biology.md#incubation-period) alone do not guarantee that fraction when the two cohorts' exposure profiles within the decade differ; decade totals omit that timing information. The reasoning concerns the hypothetical historical [BSE](../../../biology.md#bovine-spongiform-encephalopathy)/[vCJD](../../../biology.md#variant-creutzfeldt-jakob-disease) model, not an estimate of current disease risk.

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

Two distinct issues are:

- **Exposure measurement and comparability.** Infectious-dose estimates can have substantial error, and consumption categories may differ in infectivity or processing. If the assumed cohort exposure ratio is wrong, the expected allocation used in the [goodness-of-fit test](../../../statistical-modelling.md#goodness-of-fit-test) is wrong. The calendar distribution within the aggregated exposure period also matters for how many onsets have matured by the observation date.
- **Ascertainment of outcomes.** Clinical recognition, diagnostic testing, reporting and competing mortality may differ between cohorts. Unequal detection probabilities can alter the observed onset ratio even with equal biological susceptibility and [incubation periods](../../../mathematical-biology.md#incubation-period).

Thus the comparison must account for uncertainty in both its exposure denominator and its observed-disease numerator; a very small sampling [p-value](../../../statistical-modelling.md#p-value) does not remove those model uncertainties.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Using the upper stated [scrapie](../../../biology.md#scrapie)-test-positive fraction, its value among slaughtered sheep is $2000/4000000=0.0005$. The stipulated conditional [BSE](../../../biology.md#bovine-spongiform-encephalopathy) positivity then gives marginal test-positive probability

$$
q=\frac{2000}{4000000}\times0.02=10^{-5},
$$

because the other stratum contributes zero. If the sample consists of independently tested, representative animals, the count $D$ has a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $n,q$. Therefore

$$
\Pr(D=0)=(1-10^{-5})^n\simeq e^{-n10^{-5}}.
$$

The two results are

$$
\boxed{\Pr(D=0\mid n=50000)\simeq0.60653,\qquad
\Pr(D=0\mid n=500000)\simeq0.0067378.}
$$

The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) approximation uses mean counts $0.5$ and $5$, respectively. If fewer than 2000 animals belong to the test-positive stratum, these probabilities of finding nothing are higher; the calculation at 2000 is not a guaranteed detection probability.

There is also a sampling-design distinction. If exactly $K$ positive animals in a fixed annual population of $N$ are known and the sample is without replacement, use the [hypergeometric distribution](../../../discrete-probability-distribution.md#hypergeometric-distribution) instead:

$$
\Pr(D=0)=\frac{\binom{N-K}{n}}{\binom Nn}.
$$

The given expected prevalence does not assert an exactly fixed $K$, so the independent prevalence model is the natural interpretation of the requested calculation.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

Surveillance should be calibrated to the prevalence of concern, $q_*=1/200000=5\times10^{-6}$, rather than only to the higher rate used in the preceding calculation. With $50000$ representative independent tests,

$$
\Pr(\text{at least one positive}\mid q_*)=1-(1-q_*)^{50000}\simeq0.2212.
$$

Thus **50,000 tests give only about 22% detection probability at the concerning rate**; a negative survey is quite likely, with probability about $78\%$. It costs $50000\times\pounds40=\pounds2$ million. Even $500000$ tests, costing $\pounds20$ million, give about $91.8\%$ detection probability at $q_*$.

For a target $95\%$ detection probability, solve

$$
(1-q_*)^n\leq0.05,
\qquad
\boxed{n\geq\left\lceil\frac{\log0.05}{\log(1-q_*)}\right\rceil=599145.}
$$

The cost is about $\pounds24$ million. The [zero-event binomial upper confidence bound](../../../discrete-probability-distribution.md#zero-event-binomial-upper-confidence-bound) gives the same perspective: after zero positives in $50000$ tests, the one-sided $95\%$ upper bound is

$$
1-0.05^{1/50000}\simeq5.99\times10^{-5},
$$

roughly one in $16700$, well above the concerning rate. **A 50,000-animal survey is insufficient to rule out that prevalence with high confidence.** A practical design should specify its desired detection probability, diagnostic sensitivity, representativeness and dependence between sampled animals. Targeting the higher-risk [scrapie](../../../biology.md#scrapie)-positive stratum may improve efficiency if testing that stratum is feasible and its contribution to the slaughter population is estimated; its result then needs the appropriate population weighting. A cost alone does not establish adequate surveillance.

## 4

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

For a [CUSUM](../../../statistical-inference.md#cusum) threshold $h$, define the first signalling time

$$
\tau_h=\inf\{t\geq1:X_t\geq h\}.
$$

The [average run length](../../../statistical-inference.md#average-run-length) is $\mathbb E(\tau_h)$ under a specified distribution of the observations and specified initial state, here $X_0=0$. The in-control value $\operatorname{ARL}_0$ is computed under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis); a large value means false signals occur infrequently. The out-of-control value $\operatorname{ARL}_A$ is computed under a specified [alternative hypothesis](../../../statistical-modelling.md#alternative-hypothesis); a small value means rapid detection when that alternative holds from monitoring's start. If a change occurs later, its detection delay depends also on the chart state at change time, so the zero-state alternative [average run length](../../../statistical-inference.md#average-run-length) is not every possible delay.

A fixed-horizon [statistical hypothesis test](../../../statistical-modelling.md#statistical-hypothesis-test) is characterized by [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) probability under its null and [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) probability under a specified alternative. Continuous monitoring repeatedly offers opportunities to signal: over an indefinitely long run its probability of eventually signalling can be one even under the null. The [average run length](../../../statistical-inference.md#average-run-length) quantifies waiting time rather than that eventual probability. It replaces the single-test emphasis on a false-rejection probability with a false-signal timescale, and compares detection speed rather than only a fixed-horizon miss probability. However, a mean run length alone does not determine either finite-horizon error probability; those require the run-length distribution.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

For a specified change, **use the log-likelihood-ratio score**. A [log-likelihood ratio](../../../statistical-modelling.md#log-likelihood-ratio) accumulates comparable evidence for the [alternative hypothesis](../../../statistical-modelling.md#alternative-hypothesis) against the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), includes the changing expected number of deaths, and yields the standard [CUSUM](../../../statistical-inference.md#cusum) designed to detect that alternative. Under the null its expected increment is negative; under the target increase it is positive.

By contrast, raw $O-E$ has zero null drift and does not specify which increase is being sought. Its noise scale changes with expected exposure, since a [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) count with mean $E$ has variance $E$. A reset-at-zero chart with this zero-drift score can wander upwards through chance variation, and its threshold has no direct likelihood-evidence interpretation. An $O-E$ chart can be redesigned with an allowance and appropriately calibrated limits, but unadjusted $O-E$ is not the same as the [Poisson likelihood-ratio CUSUM](../../../statistical-inference.md#poisson-likelihood-ratio-cusum).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Let the annual count be $Y_t=y_t$, with null mean $\lambda_{0t}$ and alternative mean $\theta\lambda_{0t}$. Dividing the two [probability mass functions](../../../probability-theory.md#probability-mass-function) for the [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) cancels $y_t!$ and the common power of $\lambda_{0t}$:

$$
\frac{f_A(y_t)}{f_0(y_t)}
=e^{-(\theta-1)\lambda_{0t}}\theta^{y_t}.
$$

Consequently the score for the [Poisson likelihood-ratio CUSUM](../../../statistical-inference.md#poisson-likelihood-ratio-cusum) is

$$
\boxed{W_t=y_t\log\theta-(\theta-1)\lambda_{0t}.}
$$

At $\theta=2$, this becomes

$$
\boxed{W_t=O\log2-E.}
$$

Under the stated [Poisson](../../../discrete-probability-distribution.md#poisson-distribution) model this identity is exact, rather than an additional approximation. The approximation in a practical application concerns the mortality model and the use of an estimated expected count.

For $\theta>1$, the expected scores verify the direction of evidence:

$$
\mathbb E_0W_t=\lambda_{0t}[\log\theta-(\theta-1)]<0,
\qquad
\mathbb E_AW_t=\lambda_{0t}[\theta\log\theta-(\theta-1)]>0.
$$

The first inequality follows from $\log\theta<\theta-1$; the second bracket is zero at one and has positive derivative $\log\theta$ above one.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

Iterating the [CUSUM](../../../statistical-inference.md#cusum) recursion shows that

$$
X_t=\max\left(0,\max_{1\leq k\leq t}\sum_{s=k}^tW_s\right).
$$

Thus it searches all possible starting times for a recent stretch of evidence favoring an increase. If adding an increment makes the current sum negative, that accumulated evidence favors the null; retaining it would force a later real deterioration first to repay a deficit accumulated during healthy years. Starting a new candidate segment gives zero instead. **Resetting at zero makes detection responsive to a change with unknown onset.** Negative values would be permissible for a fixed-start signed [log-likelihood ratio](../../../statistical-modelling.md#log-likelihood-ratio), but that is a different statistic from this one-sided tabular [CUSUM](../../../statistical-inference.md#cusum).

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

The source plot's sharp rise in the final year crosses the chosen control boundary. **Trigger a prompt independent investigation of the mortality signal.** First verify records, deaths, follow-up and expected-count calculations, then review [case mix](../../../causal-inference.md#case-mix), changes in referral or recording, and plausible clinical explanations. The response should include appropriate clinical governance and safeguards while the cause is assessed; a statistical signal is not, by itself, proof of misconduct or a particular cause.

The stated null [average run length](../../../statistical-inference.md#average-run-length) of $111$ years makes a signal unusual under the calibrated null, while the alternative value of $5.2$ years indicates sensitivity to a sustained doubling under the specified model. Neither number gives the posterior probability that a doubling has occurred, and $1/111$ is not automatically the false-alarm probability for this particular ten-year history. Likewise the threshold is not a standalone fixed-test significance level.

The earlier value $X_{1993}=0$ says only that, at that point, no recent accumulated positive [log-likelihood ratio](../../../statistical-modelling.md#log-likelihood-ratio) survived the resets. It is **not evidence that the earlier death rate was certainly normal, and does not cancel the later signal**. The zero reset is deliberately part of the change-detection design; the 1994–1996 increments can independently justify an alarm. The full earlier clinical history remains relevant to investigation, even though a negative earlier accumulated score is not carried into the new [CUSUM](../../../statistical-inference.md#cusum) segment.

## 5

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="5/i">i</h3>

↑ **Parent:** [5](#5)

<h4 id="5/i/solution">Solution</h4>

↑ **Parent:** [I](#5/i)

Under [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle), the two parental [allele](../../../biology.md#allele) copies are sampled independently from the same pool. Multiplying their frequencies, and adding the two orderings for a heterozygote, gives

$$
\boxed{\Pr(a/a)=p^2,\qquad\Pr(a/b)=2p(1-p),\qquad\Pr(b/b)=(1-p)^2.}
$$

Their sum is $(p+(1-p))^2=1$. The [genotypes](../../../biology.md#genotype) are unordered even though the paternal and maternal transmissions may be distinguished in the calculation.

<h3 id="5/ii">ii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#5/ii)

Treat the two parents as unordered, so three possible [genotypes](../../../biology.md#genotype) give six mating types. A homozygous parent transmits its allele with probability one; a heterozygous parent transmits either [allele](../../../biology.md#allele) with probability one half by [Mendelian segregation](../../../biology.md#mendelian-segregation). Independent parental transmissions give the following complete offspring distributions:

$$
\begin{array}{c|ccc}
\text{parental genotypes}&\Pr(a/a)&\Pr(a/b)&\Pr(b/b)\\\hline
a/a\times a/a&1&0&0\\
a/a\times a/b&1/2&1/2&0\\
a/a\times b/b&0&1&0\\
a/b\times a/b&1/4&1/2&1/4\\
a/b\times b/b&0&1/2&1/2\\
b/b\times b/b&0&0&1
\end{array}
$$

Each row sums to one. In particular, heterozygote-by-heterozygote mating can produce all three offspring [genotypes](../../../biology.md#genotype), whereas the two opposite homozygotes produce only heterozygotes. These conditional offspring probabilities do not require [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) of the parents.

<h3 id="5/iii">iii</h3>

↑ **Parent:** [5](#5)

<h4 id="5/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#5/iii)

Let the initial [genotype](../../../biology.md#genotype) frequencies be arbitrary $u,v,w$ for $a/a,a/b,b/b$, with $u+v+w=1$. [Mendelian segregation](../../../biology.md#mendelian-segregation) makes the [allele](../../../biology.md#allele) frequency among gametes

$$
p=u+\frac v2,\qquad 1-p=w+\frac v2.
$$

In random mating, the two parents are selected independently. If $g(G)$ is a parent's transmission probability for allele $a$, then independence gives $\mathbb E[g(G_1)g(G_2)]=\mathbb E g(G_1)\mathbb E g(G_2)=p^2$. Thus the two independently united gametes have [allele](../../../biology.md#allele) probabilities $p,1-p$, even though the two alleles within an original parent need not have been independent. The offspring frequencies are therefore

$$
\boxed{p^2,\quad2p(1-p),\quad(1-p)^2.}
$$

No initial condition $v^2=4uw$ was used. This proves [one-generation random-mating equilibrium](../../../biology.md#one-generation-random-mating-equilibrium). The usual assumptions are a common allele pool in the two sexes, random union of gametes, ordinary [Mendelian segregation](../../../biology.md#mendelian-segregation), and no intervening mutation or genotype-dependent survival selection. Unequal male and female allele frequencies, for example, would instead give $p_m p_f$ for $a/a$, not generally the square of a single common frequency.

## 6

↑ **Parent:** [Paper 37](paper-37.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

Let $G$ count copies of allele $2$. Under [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle), $G$ has a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $2,\phi$, and the [penetrance](../../../biology.md#penetrance) is $q_G=p\theta^G$. Consequently

$$
\begin{aligned}
\Pr(Y=1)
&=p(1-\phi)^2+\theta p\,2\phi(1-\phi)+\theta^2p\phi^2\\
&=p[(1-\phi)+\phi\theta]^2
=p\alpha^2.
\end{aligned}
$$

Thus **the overall penetrance is**

$$
\boxed{K=p\alpha^2,\qquad\alpha=1+\phi(\theta-1).}
$$

The [multiplicative diallelic penetrance](../../../biology.md#multiplicative-diallelic-penetrance) model requires $0\leq\phi\leq1$, $p\geq0$, $\theta\geq0$, and each occupied genotype's value $p\theta^G$ to be at most one. These are probabilities, not unrestricted relative-risk scores.

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

Since the binary trait $Y$ has marginal [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) with probability $K=p\alpha^2$, its total [variance](../../../variance.md) is

$$
\boxed{\operatorname{Var}(Y)=p\alpha^2(1-p\alpha^2).}
$$

Within a specified [genotype](../../../biology.md#genotype) $G=g$, the [conditional variance](../../../variance.md#conditional-variance) is $q_g(1-q_g)$. The within-genotype contribution to total variance is its average over the population:

$$
V_W=\mathbb E[q_G(1-q_G)]
=\mathbb E(q_G)-\mathbb E(q_G^2).
$$

Another [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) average gives

$$
\mathbb E(q_G^2)
=p^2[(1-\phi)+\phi\theta^2]^2=p^2\beta^2,
\qquad\beta=1+\phi(\theta^2-1).
$$

Hence

$$
\boxed{V_W=p\alpha^2-p^2\beta^2.}
$$

By the [law of total variance](../../../probability-theory.md#law-of-total-variance), the remaining between-genotype component is the [genetic variance of penetrance](../../../biology.md#genetic-variance-of-penetrance), namely

$$
\boxed{V_G=\operatorname{Var}(q_G)
=\operatorname{Var}(Y)-V_W=p^2(\beta^2-\alpha^4).}
$$

It is nonnegative, as a [variance](../../../variance.md) must be. It also follows from $\beta-\alpha^2=\phi(1-\phi)(\theta-1)^2\geq0$. The single-genotype variance and its population average are different quantities; both have been specified.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

Use the usual genetic model in which disease outcomes are conditionally independent given the two individuals' [genotypes](../../../biology.md#genotype), and unshared founder [alleles](../../../biology.md#allele) are independently drawn from the same outbred population. Let $J$ denote their number of allele copies shared by [identity by descent](../../../biology.md#identity-by-descent). Conditional independence then gives

$$
\mathbb E(Y_1Y_2\mid G_1,G_2)=q_{G_1}q_{G_2}.
$$

When $J=2$, both individuals have the same genotype $G$. Its distribution remains the population genotype distribution under [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle), so their individual trait means are $K=p\alpha^2$ and

$$
\mathbb E(Y_1Y_2\mid J=2)=\mathbb E(q_G^2)=p^2\beta^2.
$$

Therefore

$$
\boxed{\operatorname{Cov}(Y_1,Y_2\mid J=2)
=p^2(\beta^2-\alpha^4)=V_G.}
$$

When $J=0$, all four unshared copies are independent, making $G_1,G_2$ independent population genotypes. Thus $\mathbb E(q_{G_1}q_{G_2})=(p\alpha^2)^2$ and

$$
\boxed{\operatorname{Cov}(Y_1,Y_2\mid J=0)=0.}
$$

**The residual-independence assumption is necessary.** Marginal penetrances alone do not determine joint disease probabilities. For example, with $\theta=1$, setting both traits equal to one shared [Bernoulli](../../../discrete-probability-distribution.md#bernoulli-distribution) variable of probability $p$ preserves every marginal penetrance, but gives covariance $p(1-p)$ even with no shared alleles. Shared environmental disease determinants or population structure therefore require an expanded model. The displayed answers are the intended locus-only covariance results, not a consequence of the penetrance table without that usual assumption.

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

For binary traits, $Y_1Y_2$ is the indicator that both individuals are affected. Hence the pair probability is its [expectation](../../../probability-theory.md#expected-value), or equivalently the [covariance](../../../variance.md#covariance) plus the product of individual means. Using the preceding results,

$$
\boxed{\Pr(Y_1=Y_2=1\mid J=2)=p^2\beta^2,\qquad
\Pr(Y_1=Y_2=1\mid J=0)=p^2\alpha^4.}
$$

These statements retain the same conditional-independence and common-population assumptions as the [multiplicative diallelic penetrance](../../../biology.md#multiplicative-diallelic-penetrance) covariance calculation.

<h3 id="6/v">v</h3>

↑ **Parent:** [6](#6)

<h4 id="6/v/solution">Solution</h4>

↑ **Parent:** [V](#6/v)

For [full siblings](../../../biology.md#full-sibling) in an [outbred pedigree](../../../biology.md#outbred-pedigree), [Mendelian IBD sharing of full siblings](../../../biology.md#mendelian-ibd-sharing-of-full-siblings) gives prior sharing probabilities $(1/4,1/2,1/4)$ for $J=0,1,2$. Let $A$ be the event that both siblings are affected. Bayes' rule weights those probabilities by the pair penetrances, giving immediately

$$
\boxed{\frac{\Pr(J=2\mid A)}{\Pr(J=0\mid A)}
=\frac{(1/4)p^2\beta^2}{(1/4)p^2\alpha^4}
=\frac{\beta^2}{\alpha^4}.}
$$

To obtain the one-shared-copy probability, assign each [allele](../../../biology.md#allele) a risk multiplier $R$, equal to $1$ with probability $1-\phi$ and $\theta$ with probability $\phi$. Then $\mathbb E R=\alpha$ and $\mathbb E R^2=\beta$. With $J=1$, write the siblings' penetrances as $pR_sR_1$ and $pR_sR_2$, where the shared multiplier $R_s$ and the two unshared multipliers are independent. Conditional independence of the disease outcomes gives

$$
\Pr(A\mid J=1)=p^2\mathbb E(R_s^2)\mathbb E(R_1)\mathbb E(R_2)
=p^2\beta\alpha^2.
$$

The total pair probability is therefore $p^2(\beta+\alpha^2)^2/4$, and the three ascertained sharing probabilities are

$$
\boxed{(z_0,z_1,z_2)
=\frac{(\alpha^4,\,2\alpha^2\beta,\,\beta^2)}{(\alpha^2+\beta)^2}.}
$$

In particular,

$$
\frac12-z_1
=\frac{(\beta-\alpha^2)^2}{2(\beta+\alpha^2)^2}\geq0.
$$

**The one-IBD proportion is below one half for a polymorphic locus with a genuine penetrance effect.** Equality holds when $\beta=\alpha^2$, namely when $\phi\in\{0,1\}$ or $\theta=1$; there is then no variation in the allele risk multiplier. The inequality follows from the different ascertainment weights for zero, one and two shared copies, rather than from applying the unascertained sibling probabilities to affected pairs. This is [sibling IBD ascertainment under multiplicative penetrance](../../../biology.md#sibling-ibd-ascertainment-under-multiplicative-penetrance). All affected-pair conditional probabilities presume $\Pr(A)>0$; if disease never occurs, conditioning on affected pairs is undefined.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2002](../../2002.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
