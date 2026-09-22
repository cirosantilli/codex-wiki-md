# Paper 32

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_32.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_32.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [Solution](#4/solution)
- [5](#5)
  - [Solution](#5/solution)
- [6](#6)
  - [Solution](#6/solution)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
- [7](#7)
  - [Solution](#7/solution)
  - [a](#7/a)
    - [Solution](#7/a/solution)
  - [b](#7/b)
    - [Solution](#7/b/solution)

## 1

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

For a one-sided [Wald test](../../../statistical-modelling.md#wald-test) use the [signed normal Wald statistic](../../../statistical-modelling.md#signed-normal-wald-statistic), rather than its square. The [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is the [sample mean](../../../variance.md#sample-mean) $\bar Y_n$, with exact [variance](../../../variance.md) $\sigma^2/n$, so

$$
\boxed{W_n=\frac{\bar Y_n}{\sigma/\sqrt n}=\frac{\sum_{i=1}^nY_i}{\sigma\sqrt n}.}
$$

A sum of independent [normal random variables](../../../probability-theory.md#gaussian-random-variable) is normal, giving $\bar Y_n\sim N(\delta,\sigma^2/n)$ and hence $W_n\sim N(\sqrt n\delta/\sigma,1)$. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) its mean is zero:

$$
\boxed{W_n\mid\delta=0\sim N(0,1).}
$$

Thus its null distribution is exactly the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), without an asymptotic approximation. If the squared [Wald statistic](../../../statistical-modelling.md#wald-test) convention is used, $W_n^2$ has a [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with one degree of freedom; the signed form is needed to distinguish the two directions.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

The same affine transformation of the [normal distribution](../../../probability-theory.md#normal-distribution) gives

$$
\boxed{W_n\mid\delta=\delta^*\sim N\left(\frac{\sqrt n\delta^*}{\sigma},1\right).}
$$

Its [variance](../../../variance.md) stays one while its mean moves positively. This is the exact alternative distribution used to calculate [statistical power](../../../probability-and-statistics.md#statistical-power). The square, if used instead, has a [noncentral chi-squared distribution](../../../probability-theory.md#noncentral-chi-squared-distribution) with one degree of freedom and noncentrality $n(\delta^*)^2/\sigma^2$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $z_p=\Phi^{-1}(p)$ denote a [quantile](../../../probability-theory.md#quantile-function) of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution). Reject when $W_n>z_{1-\alpha}$. The [statistical power](../../../probability-and-statistics.md#statistical-power) at the specified positive effect is

$$
P_{\delta^*}(W_n>z_{1-\alpha})=1-\Phi\left(z_{1-\alpha}-\frac{\sqrt n\delta^*}{\sigma}\right).
$$

Equating this to $1-\beta$ and using $z_\beta=-z_{1-\beta}$ gives $\sqrt n\delta^*/\sigma=z_{1-\alpha}+z_{1-\beta}$. Thus, for the usual target $1-\beta>\alpha$,

$$
\boxed{n=\left\lceil\frac{\sigma^2}{(\delta^*)^2}\left(z_{1-\alpha}+z_{1-\beta}\right)^2\right\rceil.}
$$

Rounding up ensures at least the target [statistical power](../../../probability-and-statistics.md#statistical-power). This [normal-mean sample size calculation](../../../probability-and-statistics.md#normal-mean-sample-size-calculation) assumes a positive integer [sample size](../../../probability-and-statistics.md#sample-size); if a requested power is at most $\alpha$, every positive [sample size](../../../probability-and-statistics.md#sample-size) already exceeds that target for $\delta^*>0$, and one should not square a negative [quantile](../../../probability-theory.md#quantile-function) sum to impose an unnecessary lower bound.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Write $s=\sigma/\sqrt n$, $\mu=\delta/s$, and let $Z_1,Z_2$ be independent [standard normal random variables](../../../probability-theory.md#standard-normal-random-variable) obtained by centering and scaling the separate stage means. Then

$$
W_1=\mu+Z_1,\qquad W_2=\sqrt2\mu+\frac{Z_1+Z_2}{\sqrt2}.
$$

The second statistic uses all patients, so the statistics are correlated even though the stages' new observations are independent. Their [covariance](../../../variance.md#covariance) is $1/\sqrt2$ and each [variance](../../../variance.md) is one. This gives the exact [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution)

$$
\boxed{\begin{pmatrix}W_1\\W_2\end{pmatrix}\sim N_2\left[\begin{pmatrix}\mu\\\sqrt2\mu\end{pmatrix},\begin{pmatrix}1&1/\sqrt2\\1/\sqrt2&1\end{pmatrix}\right].}
$$

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) both means are zero. At $\delta=\delta^*$ replace $\mu$ by $\sqrt n\delta^*/\sigma$; the mean vector is $(\sqrt n\delta^*/\sigma,\sqrt{2n}\delta^*/\sigma)^T$. In this [group sequential design](../../../probability-and-statistics.md#group-sequential-design) the full-sample statistic may be viewed as a potential statistic from the underlying sequence of outcomes, even on paths where recruitment stops.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Set $z=z_{1-\alpha}$. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) rejection requires both $W_1\ge f$ and $W_2>z$. Since $W_2$ has the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution),

$$
P_0(\text{reject})=\alpha-P_0(W_1<f,\ W_2>z).
$$

The [bivariate normal distribution](../../../probability-and-statistics.md#bivariate-normal-distribution) in the preceding calculation has a nonsingular [covariance matrix](../../../variance.md#covariance-matrix) and strictly positive [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function) everywhere. For every finite [futility boundary](../../../probability-and-statistics.md#futility-boundary) $f$ and $0<\alpha<1$, the open rectangle $\{W_1<f,W_2>z\}$ has positive [probability](../../../probability-theory.md#probability). Therefore

$$
\boxed{0<P_0(\text{reject})<\alpha.}
$$

For an explicit expression, conditional on $W_1=w$ the full-sample statistic is $N(w/\sqrt2,1/2)$ under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), yielding

$$
P_0(\text{reject})=\int_f^\infty\phi(w)\left[1-\Phi(\sqrt2z-w)\right]dw.
$$

The [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) is reduced because some otherwise rejecting paths stop for futility. Equality is approached as $f\to-\infty$, but does not hold at a finite [futility boundary](../../../probability-and-statistics.md#futility-boundary).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Let $X$ and $Y$ denote the first- and second-stage [sample means](../../../variance.md#sample-mean), let $s=\sigma/\sqrt n$, and write $S=(X+Y)/2$. Continuation is the selection event $\mathcal C=\{X\ge sf\}$. The second-stage [sample mean](../../../variance.md#sample-mean) stays independent of $\mathcal C$, so $E(Y\mid\mathcal C)=\delta$. The first-stage [sample mean](../../../variance.md#sample-mean) has a [truncated normal distribution](../../../probability-theory.md#truncated-normal-distribution). With $a=f-\delta/s$ and the upper-tail [Inverse Mills ratio](../../../probability-theory.md#inverse-mills-ratio) $\lambda(a)=\phi(a)/(1-\Phi(a))$,

$$
E(X\mid\mathcal C)=\delta+s\lambda(a),\qquad
\boxed{E(S\mid\mathcal C)-\delta=\frac{s}{2}\lambda\left(f-\frac{\delta}{s}\right)>0.}
$$

The positive [conditional selection bias after futility continuation](../../../probability-and-statistics.md#conditional-selection-bias-after-futility-continuation) comes from selecting unusually large first-stage outcomes. The unconditional [sample mean](../../../variance.md#sample-mean) of a fixed $2n$ observations would be unbiased; that is a different sampling distribution from the one restricted to continued trials.

As $\delta\to\infty$, $a\to-\infty$, $\phi(a)\to0$ and $1-\Phi(a)\to1$, so the [estimator bias](../../../statistical-modelling.md#bias-of-an-estimator) tends to zero. It decreases with $\delta$: differentiating gives $\lambda'(a)=\lambda(a)(\lambda(a)-a)>0$, because $\lambda(a)=E(Z\mid Z>a)>a$ for a [standard normal random variable](../../../probability-theory.md#standard-normal-random-variable). Thus

$$
\boxed{\text{the bias is upward, decreases as the effect increases, and tends to }0.}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

**Use a [Rao-Blackwell estimator after interim selection](../../../probability-and-statistics.md#rao-blackwell-estimator-after-interim-selection), which is exactly conditionally unbiased.** The second-stage [sample mean](../../../variance.md#sample-mean) $Y$ alone is unbiased conditional on continuation, but discards the earlier observations. Apply the [Rao-Blackwell theorem](../../../probability-and-statistics.md#rao-blackwell-theorem) by averaging $Y$ conditional on the combined [sample mean](../../../variance.md#sample-mean) $S$ and the fact of continuation.

Set $c=sf$ and $v=s/\sqrt2=\sigma/\sqrt{2n}$. Before truncation, $X\mid S$ is $N(S,v^2)$, a distribution whose mean no longer involves the unknown $\delta$. After imposing $X\ge c$, its mean is $S+v\lambda((c-S)/v)$. Since $Y=2S-X$, the resulting estimator is

$$
\boxed{\widetilde\delta=E(Y\mid S,\mathcal C)=S-v\lambda\left(\frac{c-S}{v}\right).}
$$

It uses the outcomes from both stages through their combined [sample mean](../../../variance.md#sample-mean). By iterated [expectation](../../../probability-theory.md#expected-value), $E(\widetilde\delta\mid\mathcal C)=E(Y\mid\mathcal C)=\delta$, so its conditional [estimator bias](../../../statistical-modelling.md#bias-of-an-estimator) is zero, compared with the strictly positive [estimator bias](../../../statistical-modelling.md#bias-of-an-estimator) above. Its conditional [variance](../../../variance.md) is no larger than that of the second-stage-only estimate. This does not assert a smaller [mean squared error](../../../statistical-modelling.md#mean-squared-error) than every biased estimator.

## 2

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

**There are three free [transition intensities](../../../survival-analysis.md#transition-intensity): progression, death from the initial state, and death from the advanced state.** In the three-state [illness-death model](../../../survival-analysis.md#illness-death-model), state 3 is an [absorbing state](../../../markov-process.md#absorbing-state), and there is no recovery transition.

<a id="2/a/image-irreversible-three-state-progression-model-with-mild-severe-and-absorbing-death-states"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-32-multistate.png)

**[Figure 1](#2/a/image-irreversible-three-state-progression-model-with-mild-severe-and-absorbing-death-states). Irreversible three-state progression model with mild, severe and absorbing death states**.

Writing $a=q_{12}$, $b=q_{13}$ and $c=q_{23}$, with all three nonnegative, the [transition intensity matrix](../../../markov-process.md#transition-intensity-matrix) is

$$
\boxed{Q=\begin{pmatrix}-(a+b)&a&b\\0&-c&c\\0&0&0\end{pmatrix}.}
$$

Each diagonal entry is minus the sum of the row's outgoing [transition intensities](../../../survival-analysis.md#transition-intensity), rather than an additional unknown parameter. A [continuous-time multi-state model](../../../survival-analysis.md#continuous-time-multi-state-model) with these rates describes the severity labels in the observations; an explicit cured state would require a richer state space.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

In a time-homogeneous [continuous-time Markov chain](../../../markov-process.md#continuous-time-markov-chain), a state's [holding time](../../../markov-process.md#holding-time) is exponential with rate equal to its total outgoing [transition intensity](../../../survival-analysis.md#transition-intensity). Converting the specified times to months gives

$$
a+b=\frac1{96},\qquad \frac a{a+b}=\frac12,\qquad c=\frac1{36}.
$$

The exit-type [probability](../../../probability-theory.md#probability) follows by dividing its [transition intensity](../../../survival-analysis.md#transition-intensity) by the total exit rate. Therefore

$$
\boxed{a=b=\frac1{192},\quad c=\frac1{36},\quad Q=\begin{pmatrix}-1/96&1/192&1/192\\0&-1/36&1/36\\0&0&0\end{pmatrix}\ \text{month}^{-1}.}
$$

These are starting values for numerical estimation, rather than further observations or constraints on the final fitted rates.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Let $p_{rs}(t)=P(X(u+t)=s\mid X(u)=r)$ and $P(t)=e^{Qt}$, where time homogeneity removes dependence on $u$. A recorded state at the next clinic visit contributes a [transition probability](../../../markov-process.md#transition-probability); an exactly observed death contributes a [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function), not the [probability](../../../probability-theory.md#probability) of being dead at that time. If the last recorded living state is $r$, the [mixed panel and exact-death likelihood](../../../survival-analysis.md#mixed-panel-and-exact-death-likelihood) factor after an interval $t$ is

$$
g_{r3}(t)=\sum_{j=1}^2p_{rj}(t)q_{j3}=\frac{d}{dt}p_{r3}(t).
$$

This sums over the unobserved living state immediately before death.

Conditioning on the recorded initial states, the contribution of the three displayed patient histories is

$$
\boxed{L(Q)=p_{11}(8.5)\,p_{11}(26.3)\,p_{22}(12.6)\left[p_{21}(34.6)q_{13}+p_{22}(34.6)q_{23}\right].}
$$

In this irreversible [illness-death model](../../../survival-analysis.md#illness-death-model), $p_{21}=0$, $p_{11}(t)=e^{-(a+b)t}$ and $p_{22}(t)=e^{-ct}$, simplifying it to

$$
\boxed{L(Q)=c\exp\{-34.8(a+b)-47.2c\}.}
$$

The factor $c$ is essential: the death time is known exactly. Replacing the final [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function) by $p_{23}(34.6)$ would instead model interval observation of death and give a different [likelihood](../../../statistical-modelling.md#likelihood-function).

The assumptions are independent patient histories with common rates; the Markov property; constant rates over calendar/follow-up time in this model; the stated absence of recovery and absorption at death; accurate state labels and death times; and an observation/follow-up mechanism that is noninformative for the latent process given the observed history. Clinic dates are conditioned on. The displayed living endpoints contribute only the shown observations, with noninformative [right censoring](../../../survival-analysis.md#right-censoring) if they are follow-up endpoints. Initial state [probabilities](../../../probability-theory.md#probability) are omitted by conditioning on them. Progression between visits can be unobserved, which is precisely why [panel-observed multi-state likelihood](../../../survival-analysis.md#panel-observed-multi-state-likelihood) uses the [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) rather than assuming a transition occurs at a visit.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The [mean holding time from a transition intensity matrix](../../../markov-process.md#mean-holding-time-from-a-transition-intensity-matrix) is $-1/q_{rr}$. Apply this to the fitted exit rates and use monotonic inversion for each [confidence interval](../../../statistical-inference.md#confidence-interval):

$$
\begin{aligned}
\text{mild: }&\frac1{0.0115}=86.96\text{ months},&\quad95\%\text{ CI }&=\left[\frac1{0.0130},\frac1{0.0102}\right]=[76.92,98.04],\\
\text{severe: }&\frac1{0.0318}=31.45\text{ months},&95\%\text{ CI }&=\left[\frac1{0.0352},\frac1{0.0287}\right]=[28.41,34.84].
\end{aligned}
$$

Thus the expected state durations are **86.96 months** and **31.45 months**, respectively. A [confidence interval for a reciprocal rate](../../../statistical-inference.md#confidence-interval-for-a-reciprocal-rate) reverses the endpoint order; the negative diagonal rates must first be converted to positive exit rates.

For the [expected absorption time in an illness-death model](../../../survival-analysis.md#expected-absorption-time-in-an-illness-death-model), the time spent initially in the mild state is followed by an additional severe-state duration only if progression occurs before death. That [probability](../../../probability-theory.md#probability) is $0.0072/0.0115$. Therefore

$$
\boxed{E_1(T_{\mathrm{death}})=\frac1{0.0115}+\frac{0.0072}{0.0115}\frac1{0.0318}=106.64\text{ months}\approx8.89\text{ years}.}
$$

This is an unconditional mean including both possible paths to death, not a mean conditional on progression.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

In the [log-linear transition intensity model](../../../survival-analysis.md#log-linear-transition-intensity-model), each [hazard ratio](../../../survival-analysis.md#hazard-ratio) multiplies a specific off-diagonal [transition intensity](../../../survival-analysis.md#transition-intensity), comparing its post-transplant period with the pre-transplant period while holding the modeled origin state fixed. Diagonal entries must then be recalculated from row sums.

For mild-to-severe progression, the early [hazard ratio](../../../survival-analysis.md#hazard-ratio) $0.52$ suggests a 48% decrease, but its interval $(0.11,2.4)$ includes no effect. The later [hazard ratio](../../../survival-analysis.md#hazard-ratio) $0.02$, with interval wholly below one, suggests a 98% decrease. These findings are compatible with suppression of progression by [hematopoietic stem cell transplantation](../../../biology.md#hematopoietic-stem-cell-transplantation) among those remaining in the mild state.

For mild-to-death, the early [hazard ratio](../../../survival-analysis.md#hazard-ratio) $43.92$ indicates a very large relative increase, and the later ratio $3.54$ still indicates an increase; both intervals are above one. For severe-to-death, the early ratio $2.37$ indicates increased mortality, whereas the later ratio $0.57$ indicates a 43% decrease; these intervals also exclude one. Early treatment toxicity and infection are plausible explanations for an immediate mortality increase. Later control of the underlying [myelodysplastic syndrome](../../../biology.md#myelodysplastic-syndrome) is a plausible explanation for reduced advanced-state mortality and progression.

Relative increases must be interpreted alongside baseline rates. The early mild-state death rate is approximately $0.0016\times43.92=0.0703$ per month, whereas the early severe-state death rate is $0.0380\times2.37=0.0901$ per month. Thus the far larger mild-state [hazard ratio](../../../survival-analysis.md#hazard-ratio) partly reflects its much smaller starting mortality, rather than greater absolute mortality after transplantation. The later corresponding rates are $0.00566$ and $0.02166$ per month.

Within the question's model, **delaying transplantation while the disease is mild can avoid a large immediate mortality cost, whereas the high baseline mortality in the severe state makes the later survival benefit more valuable.** This provides a qualitative rationale for the stated policy. The estimates do not establish an optimal timing rule: treatment selection, changing health status, selection of survivors into the later period and the use of the previous visit's covariate value can affect the comparison. They are associations from the fitted cohort model, not automatically causal [hazard ratios](../../../survival-analysis.md#hazard-ratio).

## 3

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $Y$ denote the full data and $R$ the pattern of indicators, with $R_j=1$ for an observed component and $R_j=0$ for a missing one. For each fixed pattern $r$, split the data as $y=(y_{\mathrm{obs}}(r),y_{\mathrm{mis}}(r))$. The [missing at random](../../../probability-and-statistics.md#missing-at-random) condition is

$$
\boxed{P_\psi(R=r\mid Y=y)=P_\psi\bigl(R=r\mid Y_{\mathrm{obs}}(r)=y_{\mathrm{obs}}(r)\bigr).}
$$

Here $\psi$ parameterizes the missingness mechanism. Equivalently its [conditional probability](../../../probability-theory.md#conditional-probability), with the observed data fixed, is constant over all possible completions of the missing data. The restriction is pattern-specific because the observed components depend on $r$. [Missing at random](../../../probability-and-statistics.md#missing-at-random) allows missingness to depend on observed values; [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random) imposes independence from all the data.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Ask the doctor whether, **among patients with the same first-year drug-use status, patients who dropped out would be more or less likely to have used the drug in the second year than those who remained**. The comparison is within the observed first-year categories, not just between all dropouts and all completers.

If there is no remaining relationship with second-year drug use after conditioning on first-year use, [missing at random](../../../probability-and-statistics.md#missing-at-random) is plausible for these recorded variables. If treatment-related difficulties, new medication or deterioration lead to dropout in a way not accounted for by the recorded first-year status, [missing at random](../../../probability-and-statistics.md#missing-at-random) may fail. A different response rate in the two first-year categories is allowed under [missing at random](../../../probability-and-statistics.md#missing-at-random). The unobserved second-year outcomes mean that the observed table alone cannot establish this assumption; clinical knowledge or additional follow-up information is needed.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Apply [MAR standardization over a fully observed covariate](../../../probability-and-statistics.md#mar-standardization-over-a-fully-observed-covariate). All first-year statuses are known, so the estimated [probabilities](../../../probability-theory.md#probability) of no use and use in year one are $58/102$ and $44/102$. Within those categories, [missing at random](../../../probability-and-statistics.md#missing-at-random) lets the observed second-year [probabilities](../../../probability-theory.md#probability) represent the corresponding dropout outcomes as well. They are estimated by $7/37$ and $18/28$.

The [law of total probability](../../../probability-theory.md#law-of-total-probability) then gives

$$
\boxed{\widehat P(Y_2=1)=\frac{58}{102}\frac7{37}+\frac{44}{102}\frac{18}{28}=0.384889\approx38.49\%.}
$$

Equivalently, impute expected drug-use counts $21(7/37)$ and $16(18/28)$ for the two dropout groups, add these to the 25 observed second-year users, and divide by 102. This uses both the complete records and the fully observed first-year information.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

Under [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random), the observed second-year outcomes form a random subsample, so the direct pooled [complete-case analysis](../../../probability-and-statistics.md#complete-case-analysis) estimate is

$$
\boxed{\widehat P_{\mathrm{CC}}(Y_2=1)=\frac{25}{65}=\frac5{13}\approx0.384615=38.46\%.}
$$

It is valid under [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random) because dropout no longer changes the marginal distribution of second-year use. Pooling is simpler than reporting separate [conditional probabilities](../../../probability-theory.md#conditional-probability), but **MCAR alone does not make this estimate more efficient than the estimate in the previous part**. The fully observed first-year variable carries useful outcome information and can improve precision even when dropout is completely random.

To make the qualification explicit, write $X=Y_1$, $m(X)=P(Y_2=1\mid X)$, $\theta=E\{m(X)\}$ and $\rho=P(R=1)$ for the constant response [probability](../../../probability-theory.md#probability). For $N$ patients the leading [variance](../../../variance.md) of the pooled estimator is $\operatorname{Var}(Y_2)/(N\rho)$. The standardization estimator in the preceding part has leading [variance](../../../variance.md)

$$
V_{\mathrm{std}}=\frac1N\left[\operatorname{Var}\{m(X)\}+\frac{E\{m(X)(1-m(X))\}}{\rho}\right].
$$

Indeed its first-order centered contribution is $m(X)-\theta+R\{Y_2-m(X)\}/\rho$: the two terms have zero [covariance](../../../variance.md#covariance), and their [variances](../../../variance.md) give that expression. The [law of total variance](../../../probability-theory.md#law-of-total-variance) therefore yields

$$
\boxed{V_{\mathrm{CC}}-V_{\mathrm{std}}=\frac{1-\rho}{N\rho}\operatorname{Var}\{m(X)\}\ge0.}
$$

The inequality is strict when there is dropout and first-year use predicts second-year use, as the distinct conditional rates suggest here. Thus the requested universal efficiency claim needs qualification. In the unrestricted joint binary-outcome model, maximizing the [observed-data likelihood](../../../statistical-modelling.md#observed-data-likelihood) under either [missing at random](../../../probability-and-statistics.md#missing-at-random) or [missing completely at random](../../../probability-and-statistics.md#missing-completely-at-random) gives the same standardization estimate $0.384889$: the all-patient first-year proportion and the two observed conditional second-year proportions maximize its factored outcome [likelihood](../../../statistical-modelling.md#likelihood-function). Restricting the distinct missingness parameters to a common response [probability](../../../probability-theory.md#probability) affects their factor, not this estimate. **The pooled value is the simple valid MCAR answer; retaining the first-year information gives the efficient MCAR answer and does not require replacing the previous estimate.**

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

An [ignorable missingness mechanism](../../../probability-and-statistics.md#ignorable-missingness-mechanism) need not be absent from the data-generating process. It means that [likelihood](../../../statistical-modelling.md#likelihood-function) inference about the data-model parameters can omit the missingness factor, while still integrating over missing values.

Write the complete joint data [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function) as $f_\theta(y,x)$ and the conditional missingness [probability](../../../probability-theory.md#probability) as $g_\psi(r\mid y,x)$. All $y$ values and only $x_{\mathrm{obs}}$ are observed. Under [missing at random](../../../probability-and-statistics.md#missing-at-random), $g_\psi(r\mid y,x)$ is constant as $x_{\mathrm{mis}}$ varies with $(y,x_{\mathrm{obs}})$ fixed. The actual [observed-data likelihood](../../../statistical-modelling.md#observed-data-likelihood) is therefore

$$
\begin{aligned}
L(\theta,\psi;y,x_{\mathrm{obs}},r)
 &=\int f_\theta(y,x_{\mathrm{obs}},x_{\mathrm{mis}})g_\psi(r\mid y,x_{\mathrm{obs}},x_{\mathrm{mis}})\,dx_{\mathrm{mis}}\\
 &=g_\psi(r\mid y,x_{\mathrm{obs}})\underbrace{\int f_\theta(y,x_{\mathrm{obs}},x_{\mathrm{mis}})\,dx_{\mathrm{mis}}}_{L_{\mathrm{obs}}(\theta;y,x_{\mathrm{obs}})}.
\end{aligned}
$$

The assumed distinctness is understood as independent variation of $\theta$ and $\psi$. Maximizing over $\psi$ multiplies $L_{\mathrm{obs}}$ by a factor independent of $\theta$; [likelihood ratios](../../../statistical-modelling.md#likelihood-ratio), scores and [likelihood](../../../statistical-modelling.md#likelihood-function) curvature for $\theta$ are therefore unchanged by omitting $g_\psi$. This proves [likelihood](../../../statistical-modelling.md#likelihood-function) ignorability.

For implementation of the [observed-data likelihood with a missing covariate](../../../probability-and-statistics.md#observed-data-likelihood-with-a-missing-covariate), a [linear regression](../../../linear-regression.md) model for $Y\mid X$ must be accompanied by an appropriate model for the distribution of $X$. For independent individuals, write $f_{\beta}(y\mid x)$ for the regression [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function) and $g_\eta(x)$ for the age [statistical probability density](../../../continuous-probability-distribution.md#probability-density-function). Up to the ignorable factor,

$$
\boxed{L_{\mathrm{obs}}(\beta,\eta)=\prod_{i:R_i=1}f_\beta(y_i\mid x_i)g_\eta(x_i)\ \prod_{i:R_i=0}\int f_\beta(y_i\mid x)g_\eta(x)\,dx.}
$$

Ignorability does not authorize discarding missing-age cases or assuming their ages have the distribution seen in the complete cases. It removes the need to model the observation mechanism for [likelihood](../../../statistical-modelling.md#likelihood-function) inference under the stated conditions, not the need to handle the missing covariates.

## 4

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

For a [counting process](../../../stochastic-process.md#counting-process) $N(t)$ adapted to its observed history $\mathcal F_t$, a predictable [counting-process intensity](../../../stochastic-process.md#counting-process-intensity) $\lambda(t)$ specifies

$$
E\{dN(t)\mid\mathcal F_{t-}\}=\lambda(t)\,dt,
$$

or more generally $N(t)-\int_0^t\lambda(u)\,du$ is a [local martingale](../../../martingale.md#local-martingale). In [survival analysis](../../../survival-analysis.md), let $N_i(t)=\mathbf1\{x_i\le t,v_i=1\}$ record failures and $Y_i(t)=\mathbf1\{x_i\ge t\}$ record the [risk set](../../../survival-analysis.md#risk-set), including subjects at their own observation time. Under independent [right censoring](../../../survival-analysis.md#right-censoring) and a common [hazard function](../../../survival-analysis.md#hazard-function) $h$, the aggregate intensity is $Y(t)h(t)$, where $N=\sum_iN_i$ and $Y=\sum_iY_i$.

Writing $H(t)=\int_0^th(u)\,du$, the conditional increment equation is $E(dN\mid\mathcal F_{t-})=Y\,dH$. Replacing $dH$ by the observed increment $dN/Y$ gives the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator)

$$
\boxed{\widehat H(t)=\int_0^t\frac{\mathbf1\{Y(u)>0\}}{Y(u)}\,dN(u)=\sum_{t_j\le t}\frac1{Y(t_j)},}
$$

where $t_j$ ranges over the distinct observed event times. Censored observations remove subjects from subsequent [risk sets](../../../survival-analysis.md#risk-set) but do not produce hazard jumps.

For these data the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) gives

$$
\begin{array}{c|rrrrrr}
\text{observation time}&3&4&5&6&9&13\\\hline
\text{risk count just before}&6&5&4&3&2&1\\
\text{hazard increment}&1/6&0&0&1/3&1/2&1\\
\widehat H(\text{observation time})&1/6&1/6&1/6&1/2&1&2
\end{array}
$$

Thus the six fitted [cumulative hazards](../../../survival-analysis.md#cumulative-hazard-function) sum to $3(1/6)+1/2+1+2=4$, the number of observed failures.

The [event-count identity for Nelson–Aalen cumulative hazards](../../../survival-analysis.md#event-count-identity-for-nelson-aalen-cumulative-hazards) follows by exchanging the finite sums. With everyone entering at time zero,

$$
\boxed{\sum_{i=1}^n\widehat H(x_i)=\sum_{j:\text{event}}\frac{\sum_i\mathbf1\{x_i\ge t_j\}}{Y(t_j)}=\sum_{j:\text{event}}1=d.}
$$

This includes each failure subject in its own [risk set](../../../survival-analysis.md#risk-set). A delayed-entry dataset requires a different risk indicator and is not covered by this particular identity.

Under a [constant hazard survival model](../../../survival-analysis.md#constant-hazard-survival-model), $\widehat H(x_i)=\widehat\theta x_i$. Imposing the same identity gives the [events divided by exposure estimator](../../../survival-analysis.md#events-divided-by-exposure-estimator)

$$
\boxed{\widehat\theta=\frac d{\sum_i x_i}=\frac4{40}=0.1\ \text{per time unit}.}
$$

Its fitted [cumulative hazards](../../../survival-analysis.md#cumulative-hazard-function) at the six times are $0.3,0.4,0.5,0.6,0.9,1.3$, again summing to four. It is also the [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) under independent [right censoring](../../../survival-analysis.md#right-censoring), since the parameter-dependent [likelihood](../../../statistical-modelling.md#likelihood-function) is $\theta^d e^{-\theta\sum_i x_i}$. This is a sensible estimate if the exponential survival model is appropriate, but four failures give little precision. The event-count identity by itself does not validate constant hazard; the large final jump in the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) also reflects a [risk set](../../../survival-analysis.md#risk-set) of one, rather than by itself proving an increasing hazard.

## 5

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="5/solution">Solution</h3>

↑ **Parent:** [5](#5)

For a proper continuous event time, the [survival function](../../../survival-analysis.md#survival-function) is $S(t)=e^{-H(t)}$. The assumed invertibility of the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) gives, for $u\ge0$,

$$
P\{H(T)>u\}=P\{T>H^{-1}(u)\}=e^{-H(H^{-1}(u))}=e^{-u}.
$$

Therefore

$$
\boxed{U=H(T)\sim\operatorname{Exp}(1).}
$$

This is the [cumulative hazard probability transformation](../../../survival-analysis.md#cumulative-hazard-probability-transformation); it applies also conditionally on a subject's covariates, using that subject's correctly specified [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function).

The fitted transformed times are [Cox–Snell residuals](../../../survival-analysis.md#cox-snell-residual). They retain their event/[right censoring](../../../survival-analysis.md#right-censoring) indicators, so a [right-censored](../../../survival-analysis.md#right-censoring) residual represents an exponential observation known only to exceed its displayed value. Under the fitted model and independent [right censoring](../../../survival-analysis.md#right-censoring), calculate the [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) of residual survival and compare it with $e^{-y}$, or calculate the residual [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) and compare its [cumulative hazard](../../../survival-analysis.md#cumulative-hazard-function) with the diagonal $H(y)=y$. Systematic departures reveal model inadequacy; sparse extreme residual [risk sets](../../../survival-analysis.md#risk-set) and parameter estimation require caution. Treating all censored residuals as observed event times would invalidate this diagnostic.

Without [right censoring](../../../survival-analysis.md#right-censoring), the residual mean should be approximately one. With [right censoring](../../../survival-analysis.md#right-censoring), use the [modified Cox–Snell residual](../../../survival-analysis.md#modified-cox-snell-residual)

$$
\boxed{y_i^*=y_i+(1-v_i).}
$$

For a true unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution), the [memoryless property](../../../continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) gives $E(U\mid U>c)=c+1$. Thus an event keeps its known transformed time, while a censored observation is replaced by the conditional expected event time. Under independent [right censoring](../../../survival-analysis.md#right-censoring), iterated [expectation](../../../probability-theory.md#expected-value) makes the mean of these adjusted values one when the true hazards are used, and approximately one when fitted hazards are used. These mean-imputed values do not themselves have an exponential distribution, so the survival-curve diagnostic should still use the original censored residual dataset. Moreover fitting equations can force the adjusted sample mean to one, making its mean alone a weak diagnostic.

For the proposed mixture of a finite [right censoring](../../../survival-analysis.md#right-censoring) time $c\ge0$ and no [right censoring](../../../survival-analysis.md#right-censoring), $P(C<U)=\pi e^{-c}$ and

$$
E\{\min(U,C)\}=(1-\pi)E(U)+\pi\int_0^cP(U>u)\,du=1-\pi e^{-c}.
$$

Consequently

$$
\boxed{E(U^*)=1+(k-1)\pi e^{-c},\qquad k=1.}
$$

When [right censoring](../../../survival-analysis.md#right-censoring) has positive [probability](../../../probability-theory.md#probability) this choice is unique; if $\pi e^{-c}=0$, no correction is needed and any $k$ has the same effect. Its independence from $c$ is the content of exponential memorylessness: the expected extra lifetime after any [right censoring](../../../survival-analysis.md#right-censoring) time is one. Conditioning on an arbitrary independent [right censoring](../../../survival-analysis.md#right-censoring) time proves the same correction beyond this special two-point mixture.

## 6

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

For an event at $t_j$ from subject $i_j$, with covariate vector $z_i$, define the [Schoenfeld function](../../../survival-analysis.md#schoenfeld-function)

$$
\boxed{s_j(\beta)=z_{i_j}-\bar z(\beta,t_j),\qquad \bar z(\beta,t_j)=\frac{\sum_{i\in R_j}z_i e^{\beta^Tz_i}}{\sum_{i\in R_j}e^{\beta^Tz_i}}.}
$$

The second term is the hazard-weighted mean covariate in the [risk set](../../../survival-analysis.md#risk-set) just before the event. The [Schoenfeld residual](../../../survival-analysis.md#schoenfeld-residual) is this function evaluated at the fitted coefficient, $r_j=s_j(\widehat\beta)$. Calculate one residual vector per event, using every at-risk subject, including those who will subsequently be censored. There is no ordinary event residual assigned at a [right censoring](../../../survival-analysis.md#right-censoring) time.

The [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) [score function](../../../statistical-modelling.md#informant-function) is $\sum_j s_j(\beta)$. At the true constant coefficient in a [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model), the conditional event subject is selected with weights proportional to $e^{\beta^Tz_i}$, so each [Schoenfeld function](../../../survival-analysis.md#schoenfeld-function) has conditional mean zero. If the coefficient varies with time, that centering changes. Plot residuals against event time or a transformation of it, smooth them, and investigate departures from zero. [Scaled Schoenfeld residuals](../../../survival-analysis.md#scaled-schoenfeld-residual) account for the risk-set covariate [variance](../../../variance.md) and can display departures in coefficient units; [score function](../../../statistical-modelling.md#informant-function) tests based on residual-time association provide a formal check. Risk-set composition affects unscaled residual [variance](../../../variance.md), and the total residual [score function](../../../statistical-modelling.md#informant-function) can be zero by fitting even when a time trend is present.

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

Conditional on an event and the immediately preceding history, [probabilities](../../../probability-theory.md#probability) are proportional to the three instantaneous hazards. Put $w=e^{\beta_0}$. The two zero-covariate subjects each have weight one, and the one-covariate subject has weight $w$. The common [baseline hazard](../../../survival-analysis.md#baseline-hazard) cancels. Thus

$$
\boxed{P(z_{\mathrm{event}}=0\mid\text{event, history})=\frac2{2+w},\qquad P(z_{\mathrm{event}}=1\mid\text{event, history})=\frac w{2+w}.}
$$

Each individual with zero covariate has [probability](../../../probability-theory.md#probability) $1/(2+w)$; the first boxed [probability](../../../probability-theory.md#probability) is their combined [probability](../../../probability-theory.md#probability). Conditioning on an event at a specified continuous time can be understood by the limiting conditional event [probabilities](../../../probability-theory.md#probability) in a short interval.

The hazard-weighted covariate mean is $w/(2+w)$, so the [Schoenfeld function](../../../survival-analysis.md#schoenfeld-function) at the true coefficient is

$$
s(\beta_0)=\begin{cases}-w/(2+w),&z_{\mathrm{event}}=0,\\2/(2+w),&z_{\mathrm{event}}=1.\end{cases}
$$

Multiplying by the two [conditional probabilities](../../../probability-theory.md#conditional-probability) gives

$$
\boxed{E\{s(\beta_0)\mid\text{event, history}\}=\frac2{2+w}\frac{-w}{2+w}+\frac w{2+w}\frac2{2+w}=0.}
$$

This verifies the score-centering property directly for this [risk set](../../../survival-analysis.md#risk-set).

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

When the event comes from the one-covariate subject, the [Schoenfeld function for a three-person binary risk set](../../../survival-analysis.md#schoenfeld-function-for-a-three-person-binary-risk-set) is

$$
\boxed{s(\beta)=1-\frac{e^\beta}{2+e^\beta}=\frac2{2+e^\beta}.}
$$

Hence

$$
\boxed{s(-\infty)=1,\qquad s(0)=\frac23,\qquad s(\infty)=0.}
$$

These are limits where necessary. At a very negative coefficient the model assigns almost no event [probability](../../../probability-theory.md#probability) to the observed one-covariate subject, producing the largest positive discrepancy. At zero coefficient all three subjects have equal [hazard functions](../../../survival-analysis.md#hazard-function), so the expected event covariate is $1/3$ and the discrepancy is $2/3$. At a very positive coefficient the observed subject is predicted to have the event almost surely, so the discrepancy tends to zero. The function decreases strictly and stays positive at every finite coefficient: this one event alone favors increasing $\beta$, while the other events in the complete [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) determine its overall estimate.

## 7

↑ **Parent:** [Paper 32](paper-32.md)

<h3 id="7/solution">Solution</h3>

↑ **Parent:** [7](#7)

For mutually exclusive event types, let $T$ be the first event time and $J$ its type. The [cause-specific hazard](../../../survival-analysis.md#cause-specific-hazard) for cause $j$ is

$$
h_j(t)=\lim_{\Delta\downarrow0}\frac{P(t\le T<t+\Delta,J=j\mid T\ge t)}{\Delta}.
$$

It is a rate conditional on having had no event of any cause. The [cumulative incidence function](../../../survival-analysis.md#cumulative-incidence-function), also called the [cumulative risk function](../../../survival-analysis.md#cumulative-incidence-function), is the actual [probability](../../../probability-theory.md#probability) $F_j(t)=P(T\le t,J=j)$.

The total [hazard function](../../../survival-analysis.md#hazard-function) is $h(t)=\sum_kh_k(t)$, giving $S(t)=\exp\{-\int_0^t\sum_kh_k(u)\,du\}$. Surviving every cause to time $u$ and then experiencing cause $j$ gives

$$
\boxed{F_j(t)=\int_0^tS(u)h_j(u)\,du=\int_0^t\exp\left\{-\int_0^u\sum_kh_k(v)\,dv\right\}h_j(u)\,du.}
$$

In [competing risks](../../../survival-analysis.md#competing-risks), $F_j$ is generally not $1-e^{-\int_0^th_j}$, because competing events remove individuals before they can experience cause $j$. This formula does not require assuming independent latent failure times for the different causes.

<h3 id="7/a">a</h3>

↑ **Parent:** [7](#7)

<h4 id="7/a/solution">Solution</h4>

↑ **Parent:** [A](#7/a)

Write $r=\theta_A+\theta_B$, with $\theta_A\ge0$, $\theta_B>0$ and a finite $\tau\ge0$. The [competing risks model with transient surgical mortality](../../../survival-analysis.md#competing-risks-model-with-transient-surgical-mortality) has [survival function](../../../survival-analysis.md#survival-function)

$$
S(t)=\exp\{-\theta_Bt-\theta_A\min(t,\tau)\}.
$$

Integrating the disease [cause-specific hazard](../../../survival-analysis.md#cause-specific-hazard) against this [survival function](../../../survival-analysis.md#survival-function) gives

$$
\boxed{F_B(t)=\begin{cases}\dfrac{\theta_B}{r}(1-e^{-rt}),&0\le t\le\tau,\\[4pt]\dfrac{\theta_B}{r}(1-e^{-r\tau})+e^{-r\tau}\bigl(1-e^{-\theta_B(t-\tau)}\bigr),&t>\tau.\end{cases}}
$$

The first term accounts for disease deaths while both causes act; the second includes survivors of that period who then face only disease mortality. The [probability](../../../probability-theory.md#probability) of eventually dying from surgery is

$$
\boxed{P(J=A)=F_A(\infty)=\int_0^\tau\theta_Ae^{-ru}\,du=\frac{\theta_A}{r}(1-e^{-r\tau}).}
$$

Taking the limit in $F_B$ gives $F_B(\infty)=\theta_B(1-e^{-r\tau})/r+e^{-r\tau}$, and therefore

$$
\boxed{F_A(\infty)+F_B(\infty)=1,\qquad S(\infty)=0.}
$$

The ultimate-death conclusion uses the positive continuing disease hazard. If $\theta_B=0$, the surviving fraction $e^{-\theta_A\tau}$ would instead live indefinitely in this model; the asserted conclusion is not valid in that boundary case.

<h3 id="7/b">b</h3>

↑ **Parent:** [7](#7)

<h4 id="7/b/solution">Solution</h4>

↑ **Parent:** [B](#7/b)

Use the [Aalen–Johansen estimator](../../../survival-analysis.md#aalen-johansen-estimator) of the [cumulative incidence function](../../../survival-analysis.md#cumulative-incidence-function), updating the overall [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) for either event:

$$
\Delta\widehat F_B(t)=\widehat S(t-)\frac{d_B(t)}{Y(t)},\qquad \widehat S(t)=\widehat S(t-)\left[1-\frac{d_A(t)+d_B(t)}{Y(t)}\right].
$$

[Right censoring](../../../survival-analysis.md#right-censoring) changes subsequent [risk sets](../../../survival-analysis.md#risk-set), not the [survival function](../../../survival-analysis.md#survival-function) by itself. Starting with the given estimates at $a_k$, the complete calculation is

$$
\begin{array}{c|c|c|c|c|c}
\text{event time}&Y(t)&\widehat S(t-)&\Delta\widehat F_B(t)&\widehat F_B(t)&\widehat S(t)\\\hline
a_{k+1}&10&0.40&0.40/10=0.04&0.34&0.36\\
a_{k+2}&9&0.36&0&0.34&0.32\\
a_{k+3}&8&0.32&0.32/8=0.04&0.38&0.28
\end{array}
$$

The middle event is of the competing type: it decreases overall survival while leaving the disease [cumulative incidence function](../../../survival-analysis.md#cumulative-incidence-function) unchanged at that instant. The event-free intervals leave every estimate and [risk set](../../../survival-analysis.md#risk-set) unchanged.

At the final time, both the event subject and the subject censored at that time are in the just-before [risk set](../../../survival-analysis.md#risk-set), so its denominator is eight. This is the usual event-before-censoring convention for recorded ties. After the event and [right censoring](../../../survival-analysis.md#right-censoring), six subjects remain at risk. Consequently

$$
\boxed{\widehat F_B(a_{k+3})=0.30+0.04+0.04=0.38.}
$$

The nine numbered source items are the inputs to this single calculation, not nine further questions.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
