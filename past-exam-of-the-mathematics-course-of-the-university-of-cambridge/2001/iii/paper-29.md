# Paper 29

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper29.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper29.pdf)

The area for the [pedigrees](../../../biology.md#pedigree) on page 7 is blank in the official Part III PDF and [PostScript edition](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2001/Paper29.ps), and in the corresponding [MPhil PDF](https://www.maths.cam.ac.uk/postgrad/mphil/files/stats/2001/Paper29.pdf) and [MPhil PostScript edition](https://www.maths.cam.ac.uk/postgrad/mphil/files/stats/2001/Paper29.ps). All four copies have been checked visually. The family-specific calculations in Question 6 remain dependent on those unavailable drawings.

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
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
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
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
  - [vi](#6/vi)
    - [Solution](#6/vi/solution)

## 1

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Write $S(t)=\mathbb P(T>t)$ for the [survival function](../../../survival-analysis.md#survival-function); this is the function denoted $F_T$ in the survival notation. For a proper continuous event-time distribution with [hazard function](../../../survival-analysis.md#hazard-function) $h$, its [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) is $H(t)=\int_0^th(s)ds=-\log S(t)$. The [probability integral transform](../../../probability-theory.md#probability-integral-transform) makes $S(T)$ uniform on $(0,1)$, including when $S$ has flat intervals: those intervals have zero event [probability](../../../probability-theory.md#probability). Consequently

$$
\mathbb P(H(T)>u)=\mathbb P(S(T)<e^{-u})=e^{-u},\qquad u\geq0.
$$

Thus the [cumulative hazard probability transformation](../../../survival-analysis.md#cumulative-hazard-probability-transformation) gives $\boxed{H(T)\sim\operatorname{Exponential}(1)}$. No strict monotonicity of $H$ is needed on intervals that carry no event mass. The usual proper continuous survival law is essential; an atom of subjects who never fail would instead require separate treatment of the mass at infinity.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Under [independent censoring](../../../survival-analysis.md#independent-censoring), order the distinct observed failure times as $t_1<\cdots<t_m$. Let $r_j=\#\{i:x_i\geq t_j\}$ be the size of the [risk set](../../../survival-analysis.md#risk-set) just before $t_j$, and let $d_j=\#\{i:x_i=t_j,v_i=1\}$ be the number of failures there. The estimated [conditional probability](../../../probability-theory.md#conditional-probability) of surviving that event time is $1-d_j/r_j$. Multiplying these conditional survival [probabilities](../../../probability-theory.md#probability) gives the [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator)

$$
\boxed{\widehat S(t)=\prod_{t_j\leq t}\left(1-\frac{d_j}{r_j}\right).}
$$

A censored observation leaves the [risk set](../../../survival-analysis.md#risk-set) after its [censoring](../../../survival-analysis.md#censoring-statistics) time but does not create a downward survival jump. With tied failure and [censoring](../../../survival-analysis.md#censoring-statistics) times, the displayed risk-set convention includes those censored at the time while processing failures, then removes them.

Since $H=-\log S$, the [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) of the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) is

$$
\boxed{\widehat H_{\mathrm{KM}}(t)=-\log\widehat S(t)=\sum_{t_j\leq t}-\log\left(1-\frac{d_j}{r_j}\right).}
$$

This is not exactly the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) $\sum_{t_j\leq t}d_j/r_j$, although the two are close when the individual fractions are small. If a jump exhausts the [risk set](../../../survival-analysis.md#risk-set), $\widehat S$ becomes zero and $\widehat H_{\mathrm{KM}}$ becomes infinite; transformed residuals beyond that point require a finite-tail modelling convention or restriction of follow-up.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The transformed values are [Cox–Snell residuals](../../../survival-analysis.md#cox-snell-residual). Under a correct common [survival function](../../../survival-analysis.md#survival-function) and a good fitted [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function), the complete transformed failure times should have unit [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). Transform the observed times and retain their original [censoring](../../../survival-analysis.md#censoring-statistics) indicators, then estimate residual survival with a [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator). Its target is

$$
\boxed{S_u(u)=e^{-u},\qquad u\geq0,}
$$

so a plot of its logarithm against $u$ should lie approximately on a line of slope $-1$. Censored residuals must not be treated as fully observed failure times.

There is a useful caution for this particular common nonparametric fit. The [shared-fit Cox–Snell residuals reproduce the fitted survival curve](../../../survival-analysis.md#shared-fit-cox-snell-residuals-reproduce-the-fitted-survival-curve) property means that the pooled residual plot is largely built into the transformation. With event ordering and compatible tie processing preserved, at a transformed failure time $u_j=\widehat H(t_j)$ its residual [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) equals $\widehat S(t_j)=e^{-u_j}$. Finite steps, coalesced [censoring](../../../survival-analysis.md#censoring-statistics) times and estimation uncertainty still matter, and an infinite final residual arises if the fitted survivor becomes zero. Separate group plots are more informative about a common-distribution assumption than this pooled fit alone.

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

If both groups share the same [survival function](../../../survival-analysis.md#survival-function) and the common fit is adequate, their complete [Cox–Snell residuals](../../../survival-analysis.md#cox-snell-residual) have the same unit [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution). Under [independent censoring](../../../survival-analysis.md#independent-censoring) in each group, both groupwise [Kaplan–Meier estimators](../../../survival-analysis.md#kaplan-meier-estimator) should therefore be close to $e^{-u}$ and to each other, subject to ordinary sampling variation and the number of subjects still at risk. Different [censoring](../../../survival-analysis.md#censoring-statistics) patterns can change precision without changing the residual survival target.

**Both group curves should approximately follow the same unit-exponential survival curve.**

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Let $S_A,S_B$ be the distinct group [survival functions](../../../survival-analysis.md#survival-function), and let $H_*$ denote the common pooled [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) used for the residuals. At a point where its inverse is defined, residual survival in group $g$ is

$$
S_{u,g}(u)=S_g(H_*^{-1}(u)).
$$

Thus the group residual curves generally differ. On intervals where $S_A(t)>S_B(t)$, the same common increasing transformation gives $S_{u,A}(u)>S_{u,B}(u)$: the better-surviving group has more large residual failure times. If the original survival curves cross, the residual curves can also cross, so no fixed ordering or [proportional hazards](../../../survival-analysis.md#proportional-hazards-model) assumption is implied.

**Distinct group distributions generally produce distinct residual survival curves, even when the pooled residual curve looks exponential.** Separate correctly fitted group hazards would restore the unit-exponential target within each group, but that is a different transformation from the common fit under discussion.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For the population identity, write $X=\min(T,C)$, $V=\mathbf1_{\{T\leq C\}}$, and $G(t)=\mathbb P(C\geq t)$. Assume [independent censoring](../../../survival-analysis.md#independent-censoring), with $f_T(t)=h(t)S(t)$. Then

$$
\mathbb EV=\int_0^\infty f_T(t)G(t)dt,
$$

while the [Tonelli theorem](../../../measure-theory.md#tonelli-theorem) and the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) give

$$
\mathbb EH(X)=\mathbb E\int_0^\infty h(t)\mathbf1_{\{X\geq t\}}dt
=\int_0^\infty h(t)S(t)G(t)dt=\mathbb EV.
$$

This is [mean accumulated hazard under independent censoring](../../../survival-analysis.md#mean-accumulated-hazard-under-independent-censoring), proving $\mathbb E[V-H(X)]=0$. For the fitted [martingale residual](../../../survival-analysis.md#martingale-residual) $Y=V-\widehat H(X)$,

$$
\boxed{\mathbb EY=-\mathbb E[\widehat H(X)-H(X)],\qquad
|\mathbb EY|\leq\mathbb E|\widehat H(X)-H(X)|.}
$$

Hence its [expectation](../../../probability-theory.md#expected-value) is approximately zero when the fitted hazard error at the observed time is small in mean. This spells out the required sense of a good estimate; pointwise consistency alone does not control a divergent tail. In particular, a [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator) with zero final survival gives infinite transformed times there and cannot supply finite residuals without a tail restriction. Neither exact finite-sample zero mean nor validity under [informative censoring](../../../survival-analysis.md#informative-censoring) is being assumed.

To check an omitted explanatory variable $Z$, plot the [martingale residuals](../../../survival-analysis.md#martingale-residual) against $Z$ or compare groupwise mean residuals, using a smooth trend or appropriate uncertainty intervals. Under a correct conditional survival model and conditionally [independent censoring](../../../survival-analysis.md#independent-censoring), $\mathbb E[Y\mid Z]$ should be approximately zero. A systematic positive trend indicates more observed failures than the fitted accumulated hazard predicts; a negative trend indicates fewer. Such patterns suggest adding $Z$, a nonlinear term or an interaction and reassessing the fit. The bounded-above, often long negative tail of [martingale residuals](../../../survival-analysis.md#martingale-residual) means that the diagnostic is a mean-pattern check, not a requirement for symmetric Gaussian residuals.

## 2

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For a continuous nonnegative event time with [hazard function](../../../survival-analysis.md#hazard-function) $h$, the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) is

$$
\boxed{H(t)=\int_0^t h(s)\,ds,\qquad H(0)=0.}
$$

Its derivative is the instantaneous hazard wherever the derivative exists.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Writing $F$ for the [survival function](../../../survival-analysis.md#survival-function) here, the relation $F'(t)=-h(t)F(t)$ with $F(0)=1$ gives

$$
\boxed{F(t)=e^{-H(t)}.}
$$

This notation uses $F$ for survival rather than for the cumulative distribution function.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

The continuous failure-time [probability density function](../../../continuous-probability-distribution.md#probability-density-function) is the negative derivative of the [survival function](../../../survival-analysis.md#survival-function):

$$
\boxed{f(t)=-F'(t)=h(t)F(t)=h(t)e^{-H(t)}.}
$$

The minus sign is essential because survivor [probability](../../../probability-theory.md#probability) decreases with time.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Assume independent individuals and [independent censoring](../../../survival-analysis.md#independent-censoring) conditional on their explanatory variables, with the [censoring](../../../survival-analysis.md#censoring-statistics) mechanism carrying no parameter $\theta$. A failure contributes its failure-time [probability density function](../../../continuous-probability-distribution.md#probability-density-function) $f_i(x_i;\theta)$, while a censored observation contributes the [survival function](../../../survival-analysis.md#survival-function) $F_i(x_i;\theta)$ because its failure time exceeds $x_i$. Terms from the [censoring](../../../survival-analysis.md#censoring-statistics) distribution then factor out of the survival-parameter [likelihood](../../../statistical-modelling.md#likelihood-function). Thus the [survival likelihood](../../../survival-analysis.md#survival-likelihood) and its logarithm are

$$
L(\theta)\propto\prod_{i=1}^n f_i(x_i;\theta)^{v_i}F_i(x_i;\theta)^{1-v_i},
$$



$$
\boxed{\ell(\theta)=\sum_{i=1}^n\{v_i\log f_i(x_i;\theta)+(1-v_i)\log F_i(x_i;\theta)\}+\text{constant}.}
$$

The individual subscripts allow the same parameter vector to act through different [covariate](../../../statistical-model.md#covariate) values.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

Insert $f_i=h_iF_i$ and $F_i=e^{-H_i}$ into the [survival likelihood](../../../survival-analysis.md#survival-likelihood). Each individual's log contribution simplifies to

$$
v_i\log h_i(x_i;\theta)+\log F_i(x_i;\theta).
$$

Therefore

$$
\boxed{\ell(\theta)=\sum_{i=1}^n\{v_i\log h_i(x_i;\theta)-H_i(x_i;\theta)\}+\text{constant}.}
$$

Failures contribute a log [hazard function](../../../survival-analysis.md#hazard-function) term as well as exposure, whereas both failures and censored subjects contribute the negative [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) over their observed follow-up.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For individual $i$, let $\pi_i=\pi_i(\psi)$, $q_i(t)$ be the known baseline [hazard function](../../../survival-analysis.md#hazard-function), and $r_i(t;\phi)$ the extra hazard. Put

$$
Q_i(t)=\int_0^tq_i(s)ds,\qquad R_i(t;\phi)=\int_0^tr_i(s;\phi)ds.
$$

The class-specific [survival functions](../../../survival-analysis.md#survival-function) are $e^{-Q_i(t)}$ and $e^{-Q_i(t)-R_i(t)}$. Consequently the unconditional survivor and failure density are

$$
F_i(t)=e^{-Q_i(t)}[\pi_i+(1-\pi_i)e^{-R_i(t)}],
$$



$$
f_i(t)=e^{-Q_i(t)}[\pi_iq_i(t)+(1-\pi_i)(q_i(t)+r_i(t))e^{-R_i(t)}].
$$

Mixture [probabilities](../../../probability-theory.md#probability) must be summed before taking a logarithm; a weighted average of class log-likelihoods would be a different, complete-data calculation. Substitution into the right-censored [survival likelihood](../../../survival-analysis.md#survival-likelihood) gives

$$
\boxed{\begin{aligned}
\ell(\phi,\psi)=\sum_i\bigl[&-Q_i(x_i)
+v_i\log\{\pi_iq_i(x_i)+(1-\pi_i)[q_i(x_i)+r_i(x_i;\phi)]e^{-R_i(x_i;\phi)}\}\\
&+(1-v_i)\log\{\pi_i+(1-\pi_i)e^{-R_i(x_i;\phi)}\}\bigr]+\text{constant}.
\end{aligned}}
$$

Equivalently, this [additive excess-hazard mixture likelihood](../../../survival-analysis.md#additive-excess-hazard-mixture-likelihood) has contribution

$$
L_i=e^{-Q_i(x_i)}\{\pi_iq_i(x_i)^{v_i}+(1-\pi_i)[q_i(x_i)+r_i(x_i)]^{v_i}e^{-R_i(x_i)}\}.
$$

Here $q_i$ and $q_i+r_i$ must be nonnegative hazards. The factor $-Q_i(x_i)$ can be dropped when maximizing over $\phi,\psi$ because $q_i$ is known. Factoring out [censoring](../../../survival-analysis.md#censoring-statistics) presumes a common parameter-free [censoring](../../../survival-analysis.md#censoring-statistics) mechanism independent of failure and latent class, conditional on the observed [covariates](../../../statistical-model.md#covariate); unmodelled class-specific [censoring](../../../survival-analysis.md#censoring-statistics) would change these mixture contributions.

## 3

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

Treat each release as an independent Bernoulli observation with a two-week event [probability](../../../probability-theory.md#probability), giving two independent [binomial distributions](../../../discrete-probability-distribution.md#binomial-distribution). Under the specified effect, the [probabilities](../../../probability-theory.md#probability) are $p_0=0.0016$ and $p_1=0.0008$ with $n=15000$ in each period. The expected event counts are therefore 24 and 12. For a conventional two-sided 5% comparison of proportions, let $D=\widehat p_0-\widehat p_1$, $\delta=p_0-p_1=0.0008$ and $\bar p=(p_0+p_1)/2=0.0012$. Use

$$
s_0=\sqrt{\frac{2\bar p(1-\bar p)}n}=0.00039976,\qquad
s_1=\sqrt{\frac{p_0(1-p_0)+p_1(1-p_1)}n}=0.00039973.
$$

The approximate null rejection region is $|D|>1.96s_0$, and under the alternative $D$ is approximately $N(\delta,s_1^2)$. Thus the [power of a two-sample rare-event comparison](../../../probability-and-statistics.md#power-of-a-two-sample-rare-event-comparison) is

$$
\begin{aligned}
\operatorname{Power}
&\approx1-\Phi\left(\frac{1.96s_0-\delta}{s_1}\right)
+\Phi\left(\frac{-1.96s_0-\delta}{s_1}\right)\\
&\approx0.5165.
\end{aligned}
$$

Here $\Phi$ is the [standard normal distribution function](../../../probability-theory.md#standard-normal-distribution-function). Hence the normal approximation gives $\boxed{\text{two-sided power approximately }52\%}$: detecting the proposed halving is far from assured.

For the small counts, a discrete calculation is also appropriate. Approximate the two counts by independent [Poisson distributions](../../../discrete-probability-distribution.md#poisson-distribution) with means 24 and 12. Conditional on their total $K$, the pre-intervention count is $\operatorname{Binomial}(K,1/2)$ under equal rates and $\operatorname{Binomial}(K,2/3)$ under the halving alternative; $K\sim\operatorname{Poisson}(36)$ under that alternative. If $\mathcal R_k$ is the rejection set of the symmetric exact two-sided 5% binomial test, its power is

$$
\sum_{k=0}^{\infty}e^{-36}\frac{36^k}{k!}
\sum_{j\in\mathcal R_k}\binom kj(2/3)^j(1/3)^{k-j}\approx0.454.
$$

This conservative discrete test has about 45% power, lower than the normal approximation because its achieved level can be below 5%. If a decrease-only one-sided 5% test had been specified in advance, replace 1.96 by 1.645; the normal-approximation power is about 64%. The tail convention and the chosen test must accompany any quoted [statistical power](../../../probability-and-statistics.md#statistical-power).

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

**Use a concurrent randomized comparison of the new leaflet with the existing release information.** Random allocation makes the groups comparable in [expectation](../../../probability-theory.md#expected-value) and avoids attributing a secular change in drug supply, release populations or post-release services to the leaflet. Both arms should use the same outcome ascertainment and two-week follow-up. This improves the causal interpretation over a historical before-and-after comparison; adequate sample size remains necessary given the low [statistical power](../../../probability-and-statistics.md#statistical-power) calculated above. If contamination prevents individual allocation, a carefully designed cluster [randomized controlled trial](../../../causal-inference.md#randomized-controlled-trial) is an alternative, with its sample-size calculation allowing for within-cluster dependence.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

The one-day slaughter-inspection yield is

$$
\widehat p_{\mathrm{inspection}}=\frac{15}{30000}=0.0005,
$$

or 500 detections per million inspected adult cattle. The routine field detections correspond, using a stable herd size of five million, to

$$
\widehat r_{\mathrm{field}}=\frac{14600}{5\times10^6\times365}=8.0\times10^{-6}
$$

per adult-cattle day, or 8 detections per million adult-cattle days. Therefore the numerical one-day comparison is

$$
\boxed{\frac{0.0005}{8.0\times10^{-6}}=62.5.}
$$

The annual field rate is $14600/(5\times10^6)=0.00292$ per cattle-year; comparing the inspection [probability](../../../probability-theory.md#probability) directly with this annual proportion would mix observation periods. Applying the random inspection-sample proportion to all 150000 slaughtered adults would predict about 75 detected cases in that slaughter cohort. These arithmetic comparisons describe detection yields, not a 62.5-fold biological disease-risk difference: a cross-sectional inspection estimates a [prevalence](../../../mathematical-biology.md#prevalence) yield, whereas daily field reporting is an ascertainment rate over animal-time.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Two reasons are [selection bias](../../../causal-inference.md#selection-bias) and unequal ascertainment.

- The slaughter cohort need not be representative of the adult dairy herd. Culling can select animals with poor health, while its age distribution may also differ. Eligibility from 24 months includes many cattle below the usual age at clinical onset, and cases before 30 months are rare; differing age composition can strongly alter the underlying risk. These effects can work in different directions, so age and reason for slaughter should be examined rather than assuming a direction.
- A focused veterinary examination at slaughter and repeated routine observations by farmers have different opportunities to detect subtle clinical signs. Early disease can remain unreported in the field, while inspection can reveal previously accumulated undetected cases. Thus one is a single-time screen for existing disease and the other a stream of newly recognized cases; even after converting denominators to comparable time units, [prevalence](../../../mathematical-biology.md#prevalence), [incidence](../../../mathematical-biology.md#incidence-epidemiology) and detection sensitivity are not identical quantities.

**Standardize the sampled population and the ascertainment process before interpreting the numerical detection-rate ratio causally.**

## 4

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

A [Beta distribution](../../../probability-theory.md#beta-distribution) is a convenient prior for a [probability](../../../probability-theory.md#probability) $p\in(0,1)$ and is conjugate to the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) of the death count. Match its mean $m=0.05$ and [variance](../../../variance.md) $v=0.02^2=0.0004$. For $p\sim\operatorname{Beta}(\alpha,\beta)$,

$$
\frac{\alpha}{\alpha+\beta}=m,\qquad
\frac{m(1-m)}{\alpha+\beta+1}=v.
$$

The [moment matching for a beta prior](../../../probability-theory.md#moment-matching-for-a-beta-prior) formula gives

$$
\kappa=\alpha+\beta=\frac{0.05(0.95)}{0.0004}-1=117.75,
\qquad\boxed{\alpha=5.8875,\quad\beta=111.8625.}
$$

Conditional on $p$, use $D\sim\operatorname{Binomial}(90,p)$ and the observed count $D=9$. Multiplying its [likelihood](../../../statistical-modelling.md#likelihood-function) $p^9(1-p)^{81}$ by the prior density gives the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) through [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy):

$$
\boxed{p\mid D=9\sim\operatorname{Beta}(14.8875,192.8625).}
$$

Under [squared-error loss](../../../statistical-inference.md#squared-error-loss), take its [posterior mean](../../../statistical-inference.md#posterior-mean) as the point estimate. A 95% equal-tail [credible interval](../../../statistical-inference.md#credible-interval) is given by its 0.025 and 0.975 quantiles. Numerically,

$$
\boxed{\widehat p_{\mathrm B}=0.07166,\qquad\operatorname{CI}_{0.95}=[0.04076,0.11035].}
$$

Matching two moments does not uniquely determine a prior distribution; the beta family is a justified convenient choice, not a conclusion forced by those moments. Its transfer to this hospital presumes that the historical between-hospital distribution is relevant to the present risk and [case mix](../../../causal-inference.md#case-mix).

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

The [posterior mean](../../../statistical-inference.md#posterior-mean) is a weighted average of the sample proportion and prior mean:

$$
\frac{9+\alpha}{90+\kappa}
=\frac{90}{207.75}(0.10)+\frac{117.75}{207.75}(0.05).
$$

Thus it is pulled from 10% toward the prior's 5%, giving about 7.17%. This is an [affine shrinkage estimator for a binomial proportion](../../../statistical-modelling.md#affine-shrinkage-estimator-for-a-binomial-proportion). The prior carries substantial concentration relative to the 90 observations, so the posterior is also more precise under this model: its standard deviation is about $0.01785$, compared with the binomial plug-in standard error $\sqrt{0.1(0.9)/90}=0.03162$. The posterior 95% [credible interval](../../../statistical-inference.md#credible-interval) $[0.04076,0.11035]$ is narrower and shifted down compared with the simple Wald interval $[0.03802,0.16198]$ based on $9/90$ alone.

**The point estimate shrinks toward the historical mean, and the interval is narrower under the informative prior.** A [credible interval](../../../statistical-inference.md#credible-interval) and a frequentist [confidence interval](../../../statistical-inference.md#confidence-interval) have different [probability](../../../probability-theory.md#probability) interpretations; the comparison does not make the prior's relevance automatic.

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

For any prior density $\pi(p)$, the Bayes estimate under [squared-error loss](../../../statistical-inference.md#squared-error-loss) is the [posterior mean](../../../statistical-inference.md#posterior-mean):

$$
\widehat p_{\mathrm B}
=\frac{\int_0^1 p\,p^9(1-p)^{81}\pi(p)\,dp}{\int_0^1p^9(1-p)^{81}\pi(p)\,dp}.
$$

For the matched [Beta distribution](../../../probability-theory.md#beta-distribution), the integrals are beta integrals and their ratio is

$$
\boxed{\widehat p_{\mathrm B}=\frac{B(\alpha+10,\beta+81)}{B(\alpha+9,\beta+81)}
=\frac{\alpha+9}{\alpha+\beta+90}=0.07166065.}
$$

The posterior mean minimizes posterior expected squared error because $\mathbb E[(p-a)^2\mid D]=\operatorname{Var}(p\mid D)+(a-\mathbb E[p\mid D])^2$. The phrase Bayes point estimate depends on the loss: under [absolute-error loss](../../../statistical-inference.md#absolute-error-loss) it would be a posterior median, while the posterior mode is a different summary and here equals $(14.8875-1)/(207.75-2)\approx0.06750$.

<h3 id="4/iv">iv</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#4/iv)

[Exchangeability](../../../probability-theory.md#exchangeable-random-variables) means that the joint prior law of the hospital risks is unchanged by relabelling hospitals; it permits different realized $p_j$. We should not assume unconditional [exchangeability](../../../probability-theory.md#exchangeable-random-variables) when known hospital characteristics predict systematic risk differences. Examples include severity and age of patients, elective versus emergency operations, procedure mix, specialist referral status, or a relationship between surgical volume and risk. Mixing such groups in one unconditional prior confounds these differences with unexplained hospital variation.

Use [covariates](../../../statistical-model.md#covariate) or clinically comparable strata first; only remaining hospital effects might reasonably be [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables). This is [conditional exchangeability of hospital risks](../../../statistical-inference.md#conditional-exchangeability-of-hospital-risks). Different sample sizes alone do not refute [exchangeability](../../../probability-theory.md#exchangeable-random-variables) of the underlying risks, although a known association between size and risk would matter. Nor does variation in the observed death proportions refute [exchangeability](../../../probability-theory.md#exchangeable-random-variables): sampling variability and genuine random heterogeneity are both allowed.

**Do not pool hospitals as exchangeable risks when their known [case mix](../../../causal-inference.md#case-mix), procedures or other relevant characteristics distinguish their expected risk distributions.**

<h3 id="4/v">v</h3>

↑ **Parent:** [4](#4)

<h4 id="4/v/solution">Solution</h4>

↑ **Parent:** [V](#4/v)

Use a [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model) with binomial observation errors and a common distribution for the underlying risks:

$$
D_j\mid p_j,n_j\sim\operatorname{Binomial}(n_j,p_j),\qquad
p_j\mid\alpha,\beta\ \overset{\mathrm{ind}}\sim\operatorname{Beta}(\alpha,\beta),\qquad j=1,\ldots,n.
$$

Give $(\alpha,\beta)$ a shared hyperprior, or parameterize them by mean $m=\alpha/(\alpha+\beta)$ and concentration $\kappa=\alpha+\beta$ and put priors on $m\in(0,1)$ and $\kappa>0$. Conditional on these hyperparameters, the risks are independent and identically distributed; after integrating them out they are [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables) with shared uncertainty. The data estimate the overall risk level and between-hospital variation. Conditional [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy) gives

$$
p_j\mid\alpha,\beta,D_j\sim\operatorname{Beta}(\alpha+D_j,\beta+n_j-D_j),
$$

and full Bayes point estimates under [squared-error loss](../../../statistical-inference.md#squared-error-loss) are

$$
\boxed{\mathbb E[p_j\mid\boldsymbol D]=\mathbb E\left[\frac{\alpha+D_j}{\alpha+\beta+n_j}\,\middle|\,\boldsymbol D\right].}
$$

An [Empirical Bayes method](../../../statistical-inference.md#empirical-bayes-method) instead estimates the hyperparameters from the marginal [beta-binomial distribution](../../../statistical-inference.md#beta-binomial-distribution) [likelihood](../../../statistical-modelling.md#likelihood-function)

$$
\prod_j\binom{n_j}{D_j}\frac{B(\alpha+D_j,\beta+n_j-D_j)}{B(\alpha,\beta)}
$$

and inserts their fitted values in the conditional posterior means. Both approaches provide partial pooling, stronger for smaller hospitals. Full Bayes also propagates hyperparameter uncertainty into the [credible intervals](../../../statistical-inference.md#credible-interval). If systematic [covariates](../../../statistical-model.md#covariate) are needed, one can place exchangeable residual effects in a [logistic regression](../../../statistical-modelling.md#logistic-regression) model rather than assuming a common unconditional risk distribution.

## 5

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Let $I,J$ denote the two ordered [alleles](../../../biology.md#allele) at the [genetic locus](../../../biology.md#genetic-locus). Under [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) they are independent with [probabilities](../../../probability-theory.md#probability) $\pi_i,\pi_j$. Write the multiplicative [penetrance](../../../biology.md#penetrance) as $\mathbb P(D\mid I=i,J=j)=k\psi_i\psi_j$, with parameters chosen so these are valid [probabilities](../../../probability-theory.md#probability), and set $Z=\sum_u\pi_u\psi_u$. Then

$$
\mathbb P(D)=k\sum_{i,j}\pi_i\pi_j\psi_i\psi_j=kZ^2.
$$

The [Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives

$$
\boxed{\mathbb P(I=i,J=j\mid D)
=\frac{k\pi_i\pi_j\psi_i\psi_j}{kZ^2}
=\pi_i^*\pi_j^*,\qquad \pi_i^*=\frac{\pi_i\psi_i}{Z}.}
$$

Thus [multiplicative penetrance preserves Hardy-Weinberg equilibrium](../../../biology.md#multiplicative-penetrance-preserves-hardy-weinberg-equilibrium): the affected subjects still have two independent [allele](../../../biology.md#allele) draws, with tilted [allele](../../../biology.md#allele) frequencies. The displayed product uses ordered [allele](../../../biology.md#allele) slots. For the usual unordered [genotypes](../../../biology.md#genotype), the corresponding [probabilities](../../../probability-theory.md#probability) are

$$
\boxed{\mathbb P(i/i\mid D)=(\pi_i^*)^2,\qquad
\mathbb P(i/j\mid D)=2\pi_i^*\pi_j^*\quad(i\ne j).}
$$

The factor of two is required for heterozygotes and must not be dropped when translating the ordered notation into [genotype](../../../biology.md#genotype) counts.

For [genetic association](../../../biology.md#genetic-association) analysis, the case [genotype](../../../biology.md#genotype) [probabilities](../../../probability-theory.md#probability) factor into [allele](../../../biology.md#allele) frequencies, so under this model an allelic comparison with representative population controls is appropriate; separate dominance departures are not required by the [penetrance](../../../biology.md#penetrance) model. The ratio of case [allele](../../../biology.md#allele) frequency to population [allele](../../../biology.md#allele) frequency is proportional to $\psi_i$, and relative risk multipliers satisfy $\psi_i/\psi_j=(\pi_i^*/\pi_i)/(\pi_j^*/\pi_j)$. Population controls are important to this exact statement. Among specifically unaffected controls,

$$
\mathbb P(I=i,J=j\mid D^c)=\frac{\pi_i\pi_j(1-k\psi_i\psi_j)}{1-kZ^2},
$$

which generally does not factor. For a rare disease it is close to the population [genotype](../../../biology.md#genotype) law, but no rare-disease assumption was needed for the case factorization itself. [Population stratification](../../../biology.md#population-stratification) and sampling dependence must also be addressed before using an ordinary allelic [chi-squared test](../../../statistical-inference.md#chi-squared-test).

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Label each parent's two [allele](../../../biology.md#allele) copies by its realized transmission: let $(A,B)$ be the transmitted and untransmitted [alleles](../../../biology.md#allele) of the first parent and $(C,D')$ those of the second. Under [random mating](../../../biology.md#panmixia) and [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle), the four parental [allele](../../../biology.md#allele) draws are independent with population frequencies $\pi$. Random [Mendelian segregation](../../../biology.md#mendelian-segregation) merely swaps the two independent copies within each parent, so the transmitted/untransmitted labelled pair still has [probability](../../../probability-theory.md#probability) $\pi_a\pi_b$; the second pair has [probability](../../../probability-theory.md#probability) $\pi_c\pi_d$.

The child receives $A,C$. If $\mathcal D$ is its disease event, its [penetrance](../../../biology.md#penetrance) is $k\psi_A\psi_C$ and its overall disease [probability](../../../probability-theory.md#probability) is $kZ^2$. Therefore

$$
\boxed{\begin{aligned}
&\mathbb P(A=a,B=b,C=c,D'=d\mid\mathcal D)\\
&\qquad=\frac{k\psi_a\psi_c\pi_a\pi_b\pi_c\pi_d}{kZ^2}
=\pi_a^*\pi_c^*\pi_b\pi_d.
\end{aligned}}
$$

This proves the [transmitted and untransmitted alleles under multiplicative penetrance](../../../biology.md#transmitted-and-untransmitted-alleles-under-multiplicative-penetrance) factorization. Under these assumptions, the transmitted pair $a/c$ has the affected-case distribution, while the complementary pair $b/d$ has the population distribution and is independent of the transmitted pair. It is the [family pseudo-control genotype](../../../biology.md#family-pseudo-control-genotype).

As in part (a), the formula records labelled transmissions. When observed [genotypes](../../../biology.md#genotype) are unordered, sum over every compatible parental-origin transmission. This includes multiplicities for overlapping parental [alleles](../../../biology.md#allele) or two heterozygous parents producing a heterozygous child; it avoids interpreting one product as the total [probability](../../../probability-theory.md#probability) of all observationally identical configurations. The homogeneous random-mating model is also essential to the unconditional independence: mixing ancestry strata can correlate the case and pseudo-control through their shared family background.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

The usual [transmission disequilibrium test](../../../biology.md#transmission-disequilibrium-test) conditions on the observed parental [genotypes](../../../biology.md#genotype), rather than modelling their population [probabilities](../../../probability-theory.md#probability). For a heterozygous parent carrying $i,j$, the two transmission outcomes are equally likely under no association. With multiplicative [penetrance](../../../biology.md#penetrance), ascertainment through an affected child weights them by $\psi_i,\psi_j$, so

$$
\mathbb P(\text{transmit }i\mid\text{parent }i/j,\text{affected child})=\frac{\psi_i}{\psi_i+\psi_j}.
$$

The other parent's [penetrance](../../../biology.md#penetrance) factor cancels. This is a special case of [disease-ascertained transmission probability](../../../biology.md#disease-ascertained-transmission-probability). Under the null $\psi_i=\psi_j$, the [conditional probability](../../../probability-theory.md#conditional-probability) is $1/2$. Count the discordant transmitted/untransmitted pairs from heterozygous parents and test their balance, using [McNemar's test](../../../statistical-modelling.md#mcnemar-s-test) or its exact conditional binomial form. Homozygous parental transmissions do not distinguish the alternatives.

This conditional analysis removes the nuisance population [allele](../../../biology.md#allele) frequencies and retains the family matching. It is therefore robust to [population stratification](../../../biology.md#population-stratification), which can otherwise make [allele](../../../biology.md#allele) frequencies differ between cases and controls without a within-family transmission effect. It does not require the unconditional [Hardy-Weinberg equilibrium](../../../biology.md#hardy-weinberg-principle) and random-mating assumptions used for the population pseudo-control factorization. Independence of suitably sampled families, valid [genotypes](../../../biology.md#genotype) and the Mendelian null transmission model still matter.

**Prefer the within-family conditional transmission test to an unconditional population case–control analysis when the population-frequency assumptions and ancestry comparability are not secure.**

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

A case chromosome is transmitted and a pseudo-control chromosome is untransmitted. Summing the paired table by columns for cases and by rows for controls gives

$$
\begin{array}{c|rr}
\text{Allele}&\text{Case}&\text{Pseudo-control}\\\hline
1&27&33\\
2&73&67\\\hline
\text{Total}&100&100
\end{array}.
$$

For the ordinary unpaired [chi-squared test](../../../statistical-inference.md#chi-squared-test) of independence, the expected cells are 30,30,70,70. Its uncorrected Pearson statistic is

$$
\boxed{X^2=\frac{(27-30)^2}{30}+\frac{(33-30)^2}{30}
+\frac{(73-70)^2}{70}+\frac{(67-70)^2}{70}
=\frac67\approx0.8571.}
$$

For the paired [McNemar's test](../../../statistical-modelling.md#mcnemar-s-test), only the discordant transmissions matter, with counts 24 and 18. Thus

$$
\boxed{X^2_{\mathrm{McN}}=\frac{(24-18)^2}{24+18}=\frac67\approx0.8571.}
$$

Both uncorrected statistics happen to coincide and have the same approximate one-degree-of-freedom [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) reference, giving $p\approx0.355$. The data do not show persuasive transmission imbalance at the conventional 5% level.

The equality is a numerical coincidence, not a justification for ignoring pairing. To see the [equality criterion for paired and unpaired allele tests](../../../statistical-modelling.md#equality-criterion-for-paired-and-unpaired-allele-tests), write the original matched cells as $a,b,c,d$ and $n=a+b+c+d$. The unpaired marginal-table statistic is

$$
\frac{2n(b-c)^2}{(2a+b+c)(2d+b+c)},
$$

whereas McNemar's is $(b-c)^2/(b+c)$. Here $n=100$, $b+c=42$, and $(2a+b+c)(2d+b+c)=60\times140=2n(b+c)$, giving equality. Changing concordant counts can change the unpaired statistic without changing McNemar's. The [transmission disequilibrium test](../../../biology.md#transmission-disequilibrium-test) should retain its conditional paired interpretation.

If a continuity correction is used, state it explicitly: McNemar's corrected statistic is $(|24-18|-1)^2/42=25/42\approx0.5952$; the corresponding Yates-corrected marginal statistic also coincides here. An exact conditional test uses $\operatorname{Binomial}(42,1/2)$ and gives the two-sided [probability](../../../probability-theory.md#probability) $2\mathbb P(K\leq18)\approx0.4408$.

## 6

↑ **Parent:** [Paper 29](paper-29.md)

<h3 id="6/i">i</h3>

↑ **Parent:** [6](#6)

<h4 id="6/i/solution">Solution</h4>

↑ **Parent:** [I](#6/i)

The [recombination fraction](../../../biology.md#recombination-fraction) is the [probability](../../../probability-theory.md#probability) that a transmitted gamete is recombinant between the two loci in the ordinary two-locus [genetic linkage](../../../biology.md#genetic-linkage) model. Its conventional range is

$$
\boxed{0\leq\theta\leq\tfrac12.}
$$

Zero corresponds to complete linkage and $1/2$ to independent assortment. Multiple physical crossovers can restore parental phase, so the recombination fraction is not the expected number of crossovers or an unrestricted crossover [probability](../../../probability-theory.md#probability).

<h3 id="6/ii">ii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#6/ii)

**The individuals' [haplotypes](../../../biology.md#haplotype) are not identifiable from the supplied source: the pedigree drawings are missing.** The original PDF has a blank figure area, and the accompanying TeX contains no family [genotypes](../../../biology.md#genotype). Even the two-locus [genotypes](../../../biology.md#genotype) of individuals 3 and 4 are not stated elsewhere, so numerical [allele](../../../biology.md#allele) pairs cannot be supplied honestly.

The method, once the drawings are available, is to use parental or grandparental [genotypes](../../../biology.md#genotype) to assign the [allele](../../../biology.md#allele) inherited at each locus on the same chromosome. A double heterozygote with [alleles](../../../biology.md#allele) $A_1,A_2$ and $B_1,B_2$ has the two candidate [haplotype](../../../biology.md#haplotype) pairs $A_1B_1/A_2B_2$ and $A_1B_2/A_2B_1$; ancestor and offspring transmissions determine or restrict its phase. These symbols describe the general phasing problem, not invented [genotypes](../../../biology.md#genotype) for the missing individuals. If pedigree transmissions leave more than one phase possible, retain all compatible phases rather than selecting one without evidence.

<h3 id="6/iii">iii</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#6/iii)

For known parental [haplotypes](../../../biology.md#haplotype), count $r_1$ recombinant transmissions among $m_1$ informative meioses. The conditional [pedigree likelihood](../../../biology.md#pedigree-likelihood) has the form

$$
L_1(\theta)=C_1\theta^{r_1}(1-\theta)^{m_1-r_1},
$$

where $C_1$ contains parameter-independent gamete and [genotype](../../../biology.md#genotype) factors. Differentiating its logarithm gives $r_1/\theta-(m_1-r_1)/(1-\theta)$, so the constrained [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is

$$
\boxed{\widehat\theta_1=\min\{r_1/m_1,\tfrac12\}\quad(m_1>0).}
$$

When $r_1=0$ the maximum is at zero; if no meiosis is informative, the [likelihood](../../../statistical-modelling.md#likelihood-function) is constant and the parameter is not estimable from that family. This formula presumes the family phase has been resolved; otherwise use [phase averaging in a linkage likelihood](../../../biology.md#phase-averaging-in-a-linkage-likelihood) first.

**The family-specific value cannot be calculated because its pedigree, phases and transmission counts are absent from the supplied PDF.** The missing data cannot be reconstructed from the requested estimate alone.

<h3 id="6/iv">iv</h3>

↑ **Parent:** [6](#6)

<h4 id="6/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#6/iv)

Let $s$ index compatible parental phases in family 2, with fixed prior conditional weights $\pi_s$. For a given phase, let $r_s$ be the recombinant count and $m_s$ the informative-transmission count, absorbing any fixed [genotype](../../../biology.md#genotype) factors into $C_s$. The appropriate [pedigree likelihood](../../../biology.md#pedigree-likelihood) is

$$
\boxed{L_2(\theta)=\sum_s\pi_s C_s\theta^{r_s}(1-\theta)^{m_s-r_s}.}
$$

This is [phase averaging in a linkage likelihood](../../../biology.md#phase-averaging-in-a-linkage-likelihood); maximizing over a phase after observing the offspring would not be the same [likelihood](../../../statistical-modelling.md#likelihood-function). In the common special case of two equally likely phases that exchange recombinant and nonrecombinant labels across $m_2$ transmissions, it reduces, up to a constant, to

$$
\tfrac12\{\theta^r(1-\theta)^{m_2-r}+\theta^{m_2-r}(1-\theta)^r\}.
$$

The constrained [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) compares all stationary points and endpoints on $[0,1/2]$.

**The actual phase set, weights, counts and numerical maximum for family 2 cannot be determined without its missing pedigree.** The special two-phase expression is a conditional example, not an assertion about this unidentified family.

<h3 id="6/v">v</h3>

↑ **Parent:** [6](#6)

<h4 id="6/v/solution">Solution</h4>

↑ **Parent:** [V](#6/v)

For independent families, multiply their [pedigree likelihoods](../../../biology.md#pedigree-likelihood). If family 1 has the known-phase counts above, the combined [log-likelihood](../../../statistical-modelling.md#log-likelihood) derivative at an interior point is

$$
\ell'(\theta)=\frac{r_1}{\theta}-\frac{m_1-r_1}{1-\theta}+\frac{L_2'(\theta)}{L_2(\theta)}.
$$

Thus the [score equation for a phase-averaged linkage likelihood](../../../biology.md#score-equation-for-a-phase-averaged-linkage-likelihood) is

$$
\boxed{[r_1-m_1\widehat\theta]L_2(\widehat\theta)
+\widehat\theta(1-\widehat\theta)L_2'(\widehat\theta)=0.}
$$

For the general phase sum, let $w_s(\theta)=\pi_sC_s\theta^{r_s}(1-\theta)^{m_s-r_s}/L_2(\theta)$. Since the weights sum to one, the equivalent interior equation is

$$
\widehat\theta=\frac{r_1+\sum_sw_s(\widehat\theta)r_s}{m_1+\sum_sw_s(\widehat\theta)m_s}.
$$

The finite [likelihood](../../../statistical-modelling.md#likelihood-function) sum is continuous on the compact parameter interval $[0,1/2]$, so a constrained maximum exists. This does not by itself prove an interior score root: complete nonrecombinant data, for example, maximize at zero. To show the requested root lies in the appropriate range for the two particular families, one must insert their transmission counts and evaluate the score or the resulting polynomial at the relevant endpoints.

**The source lacks those pedigree counts, so the data-specific equation and its asserted interior-root verification remain undetermined.** No universal interior-root claim is substituted for the missing calculation.

<h3 id="6/vi">vi</h3>

↑ **Parent:** [6](#6)

<h4 id="6/vi/solution">Solution</h4>

↑ **Parent:** [Vi](#6/vi)

The [LOD score](../../../biology.md#lod-score) is the base-ten log [likelihood](../../../statistical-modelling.md#likelihood-function) ratio against independent assortment. For the two families,

$$
\boxed{Z_{\max}=\log_{10}\frac{L_1(\widehat\theta)L_2(\widehat\theta)}{L_1(1/2)L_2(1/2)},\qquad0\leq\widehat\theta\leq\tfrac12.}
$$

For a known-phase first family this becomes

$$
Z_{\max}=r_1\log_{10}(2\widehat\theta)
+(m_1-r_1)\log_{10}(2(1-\widehat\theta))
+\log_{10}\frac{L_2(\widehat\theta)}{L_2(1/2)},
$$

with endpoint terms interpreted by limits, such as $0\log0=0$ when the corresponding count is zero. Positive values favour [genetic linkage](../../../biology.md#genetic-linkage), and the [likelihood](../../../statistical-modelling.md#likelihood-function) ratio is $10^{Z_{\max}}$. A conventional large positive threshold such as 3 represents a [likelihood](../../../statistical-modelling.md#likelihood-function) ratio of 1000, not automatically a posterior [probability](../../../probability-theory.md#probability) or a universal 5% test.

For a test calibrated to this study, use the distribution of the maximized statistic under $\theta=1/2$, for example by simulating transmissions conditional on the same parental [genotype](../../../biology.md#genotype) and ascertainment scheme. Reject for sufficiently large values with the chosen significance threshold; phase uncertainty and the boundary null prevent assuming an unqualified ordinary interior Wilks reference. The missing pedigrees prevent the numerical value or their explicit [likelihood](../../../statistical-modelling.md#likelihood-function) polynomial from being supplied, but the likelihood-ratio definition and testing procedure apply once those data are recovered.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2001](../../2001.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
