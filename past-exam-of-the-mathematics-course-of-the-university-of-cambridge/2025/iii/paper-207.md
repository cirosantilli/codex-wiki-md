# Paper 207

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_207.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_207.pdf)

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
    - [i](#1/e/i)
      - [Solution](#1/e/i/solution)
    - [ii](#1/e/ii)
      - [Solution](#1/e/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [i](#2/d/i)
      - [Solution](#2/d/i/solution)
    - [ii](#2/d/ii)
      - [Solution](#2/d/ii/solution)
    - [iii](#2/d/iii)
      - [Solution](#2/d/iii/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [Principles of the log-rank test](#4/principles-of-the-log-rank-test)
    - [Solution](#4/principles-of-the-log-rank-test/solution)
  - [Fixed assessment times](#4/fixed-assessment-times)
    - [Solution](#4/fixed-assessment-times/solution)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
    - [iii](#4/a/iii)
      - [Solution](#4/a/iii/solution)
    - [iv](#4/a/iv)
      - [Solution](#4/a/iv/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
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
  - [Unconditional hazard in a frailty model](#6/unconditional-hazard-in-a-frailty-model)
    - [Solution](#6/unconditional-hazard-in-a-frailty-model/solution)
  - [a](#6/a)
    - [i](#6/a/i)
      - [Solution](#6/a/i/solution)
    - [ii](#6/a/ii)
      - [Solution](#6/a/ii/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)

## 1

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let $Z=1$ denote gestation under unrestricted sugar and $Z=0$ gestation under rationing, and let $Y_i(z)$ be person $i$'s [potential outcome](../../../causal-inference.md#potential-outcome) for later Type 2 diabetes under exposure $z$. A sharp [causal null hypothesis](../../../causal-inference.md#causal-null-hypothesis) is

$$
H_0:Y_i(1)=Y_i(0)\quad\text{for every }i,
$$

against the alternative that the two potential outcomes differ for at least one person. An average-effect formulation instead tests $H_0:\mathbb E[Y(1)-Y(0)]=0$ against a nonzero, or scientifically directed positive, average effect.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The birth-period comparison requires [consistency](../../../causal-inference.md#consistency-in-causal-inference), no interference between individuals, and a real discontinuity in sugar exposure at the end of rationing. Near the cutoff, potential diabetes outcomes must otherwise vary continuously with birth date: no simultaneous policy, nutritional, diagnostic, seasonal, or demographic discontinuity may affect them. Birth dates must not be manipulable around the cutoff, and survival and UK Biobank participation must not create differential [selection bias](../../../causal-inference.md#selection-bias). These assumptions make cutoff assignment locally exchangeable and give a [regression discontinuity design](../../../causal-inference.md#regression-discontinuity-design) an exclusion restriction in which birth period affects diabetes through sugar exposure.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

First, age and smooth birth-cohort trends affect diabetes risk. Restricting analysis to a narrow bandwidth around September 1953 and fitting flexible trends on both sides reduces this bias. Second, quarter of birth may affect later health through season, maternal infection, or food availability. Compare the same calendar quarters in adjacent years, include season effects, and examine placebo cutoffs. Third, other post-rationing changes in diet, income, healthcare, or early-life conditions may coincide with sugar availability. Measure and adjust those changes where possible, use outcomes they should affect as [negative control outcomes](../../../causal-inference.md#negative-control-outcome), and compare with countries or groups lacking the sugar change. Differential survival or Biobank recruitment is another concern and should be examined with participation data, inverse-probability weighting, and sensitivity analysis.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Cultural abstainers form a [negative control group](../../../causal-inference.md#negative-control-group): ending rationing should not materially change their sugar intake. A diabetes discontinuity at the cutoff among consumers but not abstainers supports the proposed sugar pathway, whereas a similar discontinuity in both groups points to cohort confounding. The interaction between cutoff exposure and consumer status, or a [difference-in-differences](../../../causal-inference.md#difference-in-differences) contrast, formalizes this comparison, provided abstention itself is not differentially selected across cohorts.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/i">i</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/i/solution">Solution</h5>

↑ **Parent:** [I](#1/e/i)

Nonrepresentativeness does not automatically destroy [internal validity](../../../causal-inference.md#internal-validity): a causal contrast can remain valid among Biobank participants if selection is independent of the joint exposure-outcome process after conditioning on analysis variables. It does create bias if health or affluence affects participation and is also related to birth cohort or diabetes, especially when conditioning on participation opens a [collider bias](../../../causal-inference.md#collider-bias) path.

<h4 id="1/e/ii">ii</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/e/ii)

[External validity](../../../causal-inference.md#external-validity) is weaker because affluent, healthy volunteers need not have the same baseline risk or sugar effect as the UK target population. Generalization requires either negligible [effect modification](../../../causal-inference.md#effect-modifier) by selection-related characteristics or standardization and inverse-probability weighting to the target population using variables measured in both sources. The unweighted estimate should otherwise be described as an effect for Biobank-like participants.

## 2

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Use a two-state [continuous-time Markov chain](../../../markov-process.md#continuous-time-markov-chain) with uninfected state $S$ and infected state $I$:

$$
S\xrightarrow{a}I,
\qquad
I\xrightarrow{b}S.
$$

The generator is $Q=\begin{pmatrix}-a&a\\b&-b\end{pmatrix}$. Exponential holding times give expected time from recovery to the next infection $1/a$ and expected infection duration $1/b$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The hypotheses imply $a=1/5=0.2$ and $b=1/1.25=0.8$, so $a+b=1$. Conditional on the negative result at month 1, the likelihood is the probability of remaining in $S$ at month 2 and moving to $I$ by month 3. The supplied [matrix exponential](../../../linear-operator-theory.md#matrix-exponential) gives

$$
P_{SS}(1)=0.8+0.2e^{-1},
\qquad
P_{SI}(1)=0.2(1-e^{-1}).
$$

The [Markov property](../../../markov-process.md#markov-property) therefore gives

$$
\boxed{P_{SS}(1)P_{SI}(1)
=(0.8+0.2e^{-1})0.2(1-e^{-1})
=0.16-0.12e^{-1}-0.04e^{-2}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Acquired immunity means that the reinfection rate is no longer the common constant $a$: it should depend on infection history, usually decreasing immediately after recovery and perhaps rising as immunity wanes. The two observed states are then not Markov unless the state is enlarged to record time since infection, number of prior infections, or latent immune class. Monthly binary tests identify infection status only at visits, so infection and recovery times are [interval-censored](../../../survival-analysis.md#interval-censoring) and past short episodes may be missed. The sparse histories contain little information for estimating several history-dependent transition intensities.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/i">i</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/i/solution">Solution</h5>

↑ **Parent:** [I](#2/d/i)

The [SIR model](../../../mathematical-biology.md#sir-model) is

$$
S\xrightarrow{\lambda(t)}I\xrightarrow{\gamma}R.
$$

The expected infectious duration is $d=1/\gamma$.

<h4 id="2/d/ii">ii</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/d/ii)

The [SEIR model](../../../mathematical-biology.md#seir-model) inserts a latent exposed state:

$$
S\xrightarrow{\lambda(t)}E\xrightarrow{\sigma}I\xrightarrow{\gamma}R.
$$

The expected time from infection through the end of infectiousness is $d=1/\sigma+1/\gamma$; the duration during which transmission occurs is $1/\gamma$.

<h4 id="2/d/iii">iii</h4>

↑ **Parent:** [D](#2/d)

<h5 id="2/d/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/d/iii)

The [SIRS model](../../../mathematical-biology.md#sir-model-with-waning-immunity) has waning immunity:

$$
S\xrightarrow{\lambda(t)}I\xrightarrow{\gamma}R\xrightarrow{\omega}S.
$$

An infection lasts $d=1/\gamma$, while immunity lasts $1/\omega$ on average.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Under frequency-dependent [mass-action kinetics](../../../mathematical-biology.md#law-of-mass-action), if $I(t)$ of the $N(t)$ individuals are infectious, the force of infection is

$$
\lambda(t)=\beta\frac{I(t)}{N(t)}.
$$

One newly infectious person in an otherwise susceptible population transmits at total rate approximately $\beta$ for mean infectious duration $1/\gamma$. Hence the [basic reproduction number](../../../mathematical-biology.md#basic-reproduction-number) is

$$
R_0=\frac\beta\gamma=\beta d_I,
$$

where $d_I$ is the infectious, rather than latent-plus-infectious, duration.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Hospital admissions are a delayed thinning of infections. If $f(s)$ is the delay density and $\lambda(t)$ denotes the population infection incidence rate, then the [convolution](../../../fourier-analysis.md#convolution)

$$
\mu(t)=p\int_0^t\lambda(t-s)f(s)\,ds
=p\int_0^tf(t-s)\lambda(s)\,ds
$$

is the admission incidence rate, with an additional term for infections before time zero if the observation window starts during an epidemic.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

For $f(s)=\sigma e^{-\sigma s}$,

$$
\mu(t)=p\sigma\int_0^te^{-\sigma(t-s)}\lambda(s)ds.
$$

Differentiating the convolution, equivalently integrating by parts, gives

$$
\mu'(t)=p\sigma\lambda(t)-p\sigma^2
\int_0^te^{-\sigma(t-s)}\lambda(s)ds
=\sigma\{p\lambda(t)-\mu(t)\}.
$$

**Thus admissions follow a first-order lag: they move toward $p$ times current infection incidence at adjustment rate $\sigma$.**

## 3

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The pooled [Wald test](../../../statistical-modelling.md#wald-test) statistic is

$$
T=\frac{p_1-p_0}
{\sqrt{\bar p(1-\bar p)(1/n_1+1/n_0)}}.
$$

In asymptotic calculations one replaces $\bar p$ by its probability limit $\bar\pi=(n_1\pi_1+n_0\pi_0)/(n_1+n_0)$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

At the boundary null $\pi_1=\pi_0=\pi$, $\bar\pi=\pi$. Independence of the binomial proportions gives

$$
\mathbb ET=0,
\qquad
\operatorname{Var}T=1,
$$

asymptotically, so $T\Rightarrow N(0,1)$. For the composite null $\delta<0$, the mean moves to the nonrejection side, making the boundary the least favorable case.

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Under $\delta=\delta_A$,

$$
\mathbb ET\simeq
\frac{\delta_A}{\sqrt{\bar\pi(1-\bar\pi)(1/n_1+1/n_0)}},
$$

and

$$
\operatorname{Var}T\simeq
\frac{\pi_1(1-\pi_1)/n_1+\pi_0(1-\pi_0)/n_0}
{\bar\pi(1-\bar\pi)(1/n_1+1/n_0)}.
$$

The [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) therefore gives an asymptotic normal distribution with this mean and variance.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $n$ be the sample size in each arm, $\pi_{1A}=\pi_0+\delta_A$, and $\bar\pi_A=(\pi_{1A}+\pi_0)/2$. Solving the normal-approximation power equation gives

$$
n=\frac{
\left[z_{1-\alpha}\sqrt{2\bar\pi_A(1-\bar\pi_A)}
+z_{1-\beta}\sqrt{\pi_{1A}(1-\pi_{1A})+\pi_0(1-\pi_0)}\right]^2
}{\delta_A^2},
$$

rounded upward. The total sample size is $2n$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\pi$ be the new-treatment response probability in the trial's target population and let the fixed historical standard-of-care rate be $\pi_0$. The one-sided hypotheses are

$$
H_0:\pi\leq\pi_0,
\qquad
H_1:\pi>\pi_0.
$$

The boundary $\pi=\pi_0$ determines the type-I error because rejection probability increases with $\pi$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $X_1\sim\operatorname{Binomial}(22,\pi_0)$ be interim responses and independently $X_2\sim\operatorname{Binomial}(32,\pi_0)$ be second-stage responses. The design rejects immediately when $X_1\geq e_1=10$, continues when $r_1<X_1<e_1$, and after continuation rejects when $X_1+X_2\geq r=20$. Hence at $\pi_0=0.3$,

$$
\alpha=
\sum_{x=10}^{22}b(22,0.3,x)
+\sum_{x=8}^{9}b(22,0.3,x)
\sum_{y=20-x}^{32}b(32,0.3,y).
$$

This is the type-I error of the specified [two-stage clinical trial design](../../../probability-and-statistics.md#two-stage-clinical-trial-design).

## 4

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="4/principles-of-the-log-rank-test">Principles of the log-rank test</h3>

↑ **Parent:** [4](#4)

<h4 id="4/principles-of-the-log-rank-test/solution">Solution</h4>

↑ **Parent:** [Principles of the log-rank test](#4/principles-of-the-log-rank-test)

The [log-rank test](../../../survival-analysis.md#log-rank-test) compares observed failures in each group with the numbers expected under equal hazards, conditioning at every event time on the risk set and total failures. Its score sums $O_{1j}-Y_{1j}d_j/Y_j$ and is standardized by its null hypergeometric variance. It is most powerful for approximately [proportional hazards](../../../survival-analysis.md#proportional-hazards-model). Strongly crossing survival curves can produce large positive and negative contributions that cancel, so very different distributions may yield a weak log-rank statistic.

<h3 id="4/fixed-assessment-times">Fixed assessment times</h3>

↑ **Parent:** [4](#4)

<h4 id="4/fixed-assessment-times/solution">Solution</h4>

↑ **Parent:** [Fixed assessment times](#4/fixed-assessment-times)

Monthly assessment gives [interval censoring](../../../survival-analysis.md#interval-censoring), although recording failure at the visit treats it as exact. It also creates many tied times. Ordinary continuous-time log-rank calculations then require a tie convention or grouped-time method, and unequal or missed visits can induce informative observation.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

At times 1 and 2, the risk sets immediately before failure contain respectively $(5,5)$ and $(4,4)$ low- and high-dose patients, with one failure each. The low-dose expected counts are $1/2$ and $1/2$. Immediately before time 5, one low-dose and four high-dose patients remain; three tied failures give low-dose expectation $3(1/5)=3/5$. Thus

$$
\boxed{E_A=\frac12+\frac12+\frac35=1.6.}
$$

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

**No.** The high-dose expectation is

$$
E_B=\frac12+\frac12+3\frac45=3.4.
$$

Although both groups start with five patients, censoring removes two low-dose patients at month 3 and one high-dose patient at month 1. Their later risk sets therefore differ; only the sum $E_A+E_B=5$ must equal the total observed failures.

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The unstandardized low-dose log-rank statistic is

$$
U_A=O_A-E_A=3-1.6=1.4.
$$

Its positive sign means more low-dose failures than expected under equal survival, indicating a higher low-dose treatment-failure hazard and favoring the high dose.

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

An observed-to-expected estimate of the low-versus-high relative failure risk is

$$
\frac{O_A/E_A}{O_B/E_B}
=\frac{3/1.6}{2/3.4}
=3.1875.
$$

**Thus the low-dose failure hazard is estimated to be roughly $3.2$ times the high-dose hazard, with great uncertainty in this tiny dataset.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

A baseline-group log-rank test is inappropriate. Receiving surgery is determined at month 3, so classifying patients by that future decision gives the surgery group guaranteed survival without treatment failure to the decision time, creating [immortal time bias](../../../survival-analysis.md#immortal-time-bias). Fitness also strongly confounds surgery and prognosis. One can perform a month-3 [landmark analysis](../../../survival-analysis.md#landmark-analysis) among patients still at risk, or model surgery as a [time-dependent covariate](../../../survival-analysis.md#time-dependent-covariate), while adjusting for the clinical variables driving the decision.

## 5

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

Under independent [right censoring](../../../survival-analysis.md#right-censoring), observation $(x_i,d_i)$ contributes

$$
f(x_i;\eta)^{d_i}S(x_i;\eta)^{1-d_i}
=h(x_i;\eta)^{d_i}S(x_i;\eta),
$$

where $d_i$ indicates an event. Multiply these contributions, take the [log-likelihood](../../../statistical-modelling.md#log-likelihood), and maximize it over the parametric survival-model parameter $\eta$, numerically if the score equations have no closed form.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

For constant hazard $h_i(t)=\lambda$, $S_i(t)=e^{-\lambda t}$. With $D=\sum_i d_i$ and total person-time $T=\sum_i x_i$,

$$
\ell(\lambda)=D\log\lambda-\lambda T,
\qquad
\widehat\lambda=\frac DT.
$$

**Thus the maximum-likelihood estimate is events divided by [person-time at risk](../../../survival-analysis.md#person-time-at-risk).**

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $D_k=\sum_{i:z_i=k}d_i$ and $T_k=\sum_{i:z_i=k}x_i$. Since the cumulative hazard is $\theta e^{z_i\beta}x_i$,

$$
\ell(\theta,\beta)
=(D_0+D_1)\log\theta+D_1\beta
-\theta(T_0+e^\beta T_1).
$$

The score equations imply $D_1=\theta e^\beta T_1$ and $D_0=\theta T_0$. Therefore

$$
\widehat\theta=\frac{D_0}{T_0},
\qquad
\widehat\beta=log\frac{D_1/T_1}{D_0/T_0},
$$

when both event counts are positive, with the usual infinite boundary estimates otherwise.

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

The group hazards are $\lambda_0=\theta$ and $\lambda_1=\theta e^\beta$. Separate constant-hazard likelihoods give

$$
\widehat\lambda_0=\frac{D_0}{T_0},
\qquad
\widehat\lambda_1=\frac{D_1}{T_1}.
$$

Part (c) then verifies exactly that $\widehat\lambda_0=\widehat\theta$ and $\widehat\lambda_1=\widehat\theta e^{\widehat\beta}$.

## 6

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="6/unconditional-hazard-in-a-frailty-model">Unconditional hazard in a frailty model</h3>

↑ **Parent:** [6](#6)

<h4 id="6/unconditional-hazard-in-a-frailty-model/solution">Solution</h4>

↑ **Parent:** [Unconditional hazard in a frailty model](#6/unconditional-hazard-in-a-frailty-model)

A [frailty model](../../../survival-analysis.md#frailty-model) introduces an unobserved positive random effect $U$ that multiplies an individual's hazard. With $H_0(t)=\int_0^th_0(s)ds$, marginal survival is

$$
\bar S(t)=\int_0^\infty e^{-uH_0(t)}g(u)du.
$$

Differentiation gives

$$
\bar h(t)=h_0(t)
\frac{\int_0^\infty u e^{-uH_0(t)}g(u)du}
{\int_0^\infty e^{-uH_0(t)}g(u)du}
=h_0(t)\mathbb E[U\mid T\geq t].
$$

**Consequently $\bar h(0)=h_0(0)$ exactly when $\mathbb EU=1$.**

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

For equal point masses at $1/2$ and $3/2$ with $h_0=\theta$,

$$
\bar h(t)=\frac\theta2
\frac{e^{-\theta t/2}+3e^{-3\theta t/2}}
{e^{-\theta t/2}+e^{-3\theta t/2}}.
$$

Its initial value is $\theta$ because $\mathbb EU=1$, while $\bar h(t)\to\theta/2$ as the more frail survivors are progressively depleted.

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

For $U\sim\operatorname{Exponential}(1)$,

$$
\bar S(t)=\int_0^\infty e^{-u\theta t}e^{-u}du
=\frac1{1+\theta t},
\qquad
\bar h(t)=\frac\theta{1+\theta t}.
$$

Again $\bar h(0)=\theta$ because $\mathbb EU=1$, but now $\bar h(t)\to0$ as $t\to\infty$.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

Survival preferentially selects smaller frailties, so $\mathbb E[U\mid T\geq t]$ generally decreases with $t$. For the two-point distribution,

$$
\gamma(u,t)=
\frac{e^{-u\theta t}
[\delta(u-1/2)+\delta(u-3/2)]/2}
{[e^{-\theta t/2}+e^{-3\theta t/2}]/2}.
$$

At $t=0$ this equals $g(u)$, and

$$
\mathbb E[U\mid T\geq t]
=\frac{\tfrac12e^{-\theta t/2}+\tfrac32e^{-3\theta t/2}}
{e^{-\theta t/2}+e^{-3\theta t/2}}.
$$

It decreases from $1$ to $1/2$, demonstrating survivor selection toward the less frail class.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Frailty makes a population hazard ratio mix the conditional treatment effect with changing survivor composition. Suppose

$$
h(t\mid U=u,Z=z)=u\theta e^{\beta z}
$$

and $U\sim\operatorname{Exponential}(1)$. Part (a)(ii), with $\theta$ replaced by $\theta e^{\beta z}$, gives

$$
\bar h_z(t)=\frac{\theta e^{\beta z}}
{1+\theta e^{\beta z}t}.
$$

Although conditional hazards are proportional with ratio $e^\beta$, the marginal ratio is

$$
\frac{\bar h_1(t)}{\bar h_0(t)}
=e^\beta\frac{1+\theta t}{1+\theta e^\beta t},
$$

which varies with time and tends to one. Thus an ordinary marginal [proportional hazards](../../../survival-analysis.md#proportional-hazards-model) interpretation can be misleading in the presence of unobserved heterogeneity.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
