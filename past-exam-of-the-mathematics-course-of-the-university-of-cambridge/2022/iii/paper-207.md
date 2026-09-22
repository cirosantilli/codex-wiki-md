# Paper 207

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_207.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_207.pdf)

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
      - [Solution](#1/1/5/solution)
    - [6](#1/1/6)
      - [Solution](#1/1/6/solution)
- [2](#2)
  - [1](#2/1)
    - [Solution](#2/1/solution)
  - [2](#2/2)
    - [Solution](#2/2/solution)
    - [3](#2/2/3)
      - [Solution](#2/2/3/solution)
    - [4](#2/2/4)
      - [Solution](#2/2/4/solution)
    - [5](#2/2/5)
      - [Solution](#2/2/5/solution)
    - [6](#2/2/6)
      - [Solution](#2/2/6/solution)
    - [7](#2/2/7)
      - [a](#2/2/7/a)
        - [Solution](#2/2/7/a/solution)
      - [b](#2/2/7/b)
        - [Solution](#2/2/7/b/solution)
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
  - [f](#3/f)
    - [Solution](#3/f/solution)
  - [g](#3/g)
    - [Solution](#3/g/solution)
  - [h](#3/h)
    - [Solution](#3/h/solution)
- [4](#4)
  - [Solution](#4/solution)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [i](#5/b/i)
      - [Solution](#5/b/i/solution)
    - [ii](#5/b/ii)
      - [Solution](#5/b/ii/solution)
  - [c](#5/c)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [Solution](#6/solution)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="1/1">1</h3>

↑ **Parent:** [1](#1)

<h4 id="1/1/solution">Solution</h4>

↑ **Parent:** [1](#1/1)

Vitamin D is a causal determinant of mortality risk if an [intervention](../../../causal-inference.md#treatment) that changes vitamin-D status changes the distribution of the corresponding [potential outcome](../../../causal-inference.md#potential-outcome) for mortality. This is a claim about a [causal effect](../../../causal-inference.md#causal-effect), rather than merely an observed [association](../../../causal-inference.md#statistical-association).

<h4 id="1/1/2">2</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/2/solution">Solution</h5>

↑ **Parent:** [2](#1/1/2)

First, an [observational study](../../../causal-inference.md#observational-study) can suffer from [confounding](../../../causal-inference.md#confounding) or [reverse causality](../../../causal-inference.md#reverse-causality). Ill health may both lower circulating vitamin D and raise mortality, while lifestyle, socioeconomic status, and comorbidity may affect both variables. [Randomization](../../../causal-inference.md#randomization) breaks these baseline associations in expectation.

Second, the interventions answer different questions. Supplementation may be too small, too late, too short, or poorly adhered to, and an average effect can be nearly zero when benefit is confined to people with severe deficiency. Such [heterogeneous treatment effects](../../../causal-inference.md#heterogeneous-treatment-effect) can coexist with a strong observational gradient.

<h4 id="1/1/3">3</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/3/solution">Solution</h5>

↑ **Parent:** [3](#1/1/3)

The plots test the plausibility of the [instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence) and [exclusion restriction](../../../causal-inference.md#exclusion-restriction) assumptions. Both candidate instruments are strongly associated with 25(OH)D, supporting [instrument relevance](../../../causal-inference.md#instrument-relevance). The focused instrument has estimates near zero for the other measured traits. The polygenic instrument is strongly associated with LDL cholesterol and triglycerides, suggesting [horizontal pleiotropy](../../../causal-inference.md#horizontal-pleiotropy): it may influence mortality through lipid pathways that do not pass through vitamin D.

I would therefore prefer the focused instrument. Its use of fewer biologically understood variants may reduce precision, but its cleaner associations make the causal assumptions more credible.

<h4 id="1/1/4">4</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/4/solution">Solution</h5>

↑ **Parent:** [4](#1/1/4)

Let $G$ be the genetic instrument, $X$ vitamin-D concentration, $U$ an unmeasured cause of vitamin D and mortality, and $Y$ mortality. The [causal directed acyclic graph](../../../causal-inference.md#causal-directed-acyclic-graph) contains

$$
G\longrightarrow X\longleftarrow U\longrightarrow Y.
$$

Although $G$ and $U$ are marginally independent, $X$ is a [collider](../../../combinatorics.md#collider). Conditioning on $X$ opens the path $G\leftrightarrow U\to Y$, violating [instrumental-variable independence](../../../causal-inference.md#instrumental-variable-independence) within the resulting strata. [Residual exposure stratification](../../../causal-inference.md#residual-exposure-stratification) instead removes the component of $X$ predicted by $G$ before stratification; under the additive first-stage model, the stratifying variable is no longer caused by $G$.

<h4 id="1/1/5">5</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/5/solution">Solution</h5>

↑ **Parent:** [5](#1/1/5)

The overall [odds ratio](../../../statistical-modelling.md#odds-ratio) is $0.99$ with 95% interval $(0.95,1.02)$, so there is little evidence for an average effect. The estimate changes sharply across residual-vitamin-D strata: it is $0.69$ $(0.59,0.80)$ in the deficient group, $0.94$ $(0.89,0.99)$ in the insufficient group, and close to one in the two higher groups. The pattern is consistent with [effect modification](../../../causal-inference.md#effect-modifier): raising vitamin D may reduce mortality among deficient people but offer little benefit once concentration is adequate. The claim still depends on the [Mendelian randomization](../../../causal-inference.md#mendelian-randomization) assumptions and should account for the fact that several subgroup estimates were examined.

<h4 id="1/1/6">6</h4>

↑ **Parent:** [1](#1/1)

<h5 id="1/1/6/solution">Solution</h5>

↑ **Parent:** [6](#1/1/6)

One check is to use measured risk factors as [negative control outcomes](../../../causal-inference.md#negative-control-outcome). A valid instrument should not predict traits that cannot plausibly be downstream consequences of vitamin D; persistent associations would expose [horizontal pleiotropy](../../../causal-inference.md#horizontal-pleiotropy) or population structure.

A second check is to repeat the analysis with separate biologically motivated variants or gene-region scores and compare their ratio estimates. Agreement across instruments with distinct biological pathways supports the common vitamin-D mechanism, whereas excess between-instrument heterogeneity suggests direct effects. The same data can also support sensitivity analyses that adjust for measured pleiotropic pathways.

<h2 id="2">2</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="2/1">1</h3>

↑ **Parent:** [2](#2)

<h4 id="2/1/solution">Solution</h4>

↑ **Parent:** [1](#2/1)

Ignoring factors that do not depend on the parameters, the product of the two [binomial likelihoods](../../../discrete-probability-distribution.md#binomial-likelihood) is

$$
L(\phi_0,\phi_1)
=\phi_0^{120}(1-\phi_0)^{80}
 \phi_1^{110}(1-\phi_1)^{110}.
$$

Including the sampling constants multiplies this by ${200\choose120}{220\choose110}$.

<h3 id="2/2">2</h3>

↑ **Parent:** [2](#2)

<h4 id="2/2/solution">Solution</h4>

↑ **Parent:** [2](#2/2)

The [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator) are the success proportions

$$
\widehat\phi_0=\frac{120}{200}=\frac35,
\qquad
\widehat\phi_1=\frac{110}{220}=\frac12.
$$

The [invariance property of maximum likelihood estimation](../../../statistical-modelling.md#invariance-property-of-maximum-likelihood-estimation) therefore gives

$$
\boxed{\widehat\alpha=\widehat\phi_1-\widehat\phi_0
=\frac12-\frac35=-\frac1{10}.}
$$

<h4 id="2/2/3">3</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/3/solution">Solution</h5>

↑ **Parent:** [3](#2/2/3)

A [complete-case analysis](../../../probability-and-statistics.md#complete-case-analysis) estimates each success probability among clinic attenders. If attendance depends on the unobserved outcome even after conditioning on treatment, the observed success proportions differ systematically from those in the randomized groups. This outcome-dependent dropout causes [selection bias](../../../causal-inference.md#selection-bias) and can bias their difference.

<h4 id="2/2/4">4</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/4/solution">Solution</h5>

↑ **Parent:** [4](#2/2/4)

For a patient whose $Y$ is missing, summing the Bernoulli likelihood contribution over its two possible values gives

$$
\phi_z+(1-\phi_z)=1.
$$

Consequently the observed-data likelihood for all 490 patients is

$$
L_{\rm obs}(\phi_0,\phi_1)
=\phi_0^{120}(1-\phi_0)^{80}
 \phi_1^{110}(1-\phi_1)^{110},
$$

up to constants. The 70 missing outcomes contribute no information about $\phi_0$ or $\phi_1$ in this marginal model, so the estimators and $\widehat\alpha=-1/10$ are unchanged. This likelihood calculation alone does not make an outcome-dependent missingness mechanism ignorable.

<h4 id="2/2/5">5</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/5/solution">Solution</h5>

↑ **Parent:** [5](#2/2/5)

The data have a [monotone missing-data pattern](../../../probability-and-statistics.md#monotone-missing-data-pattern): $Z$ is always observed; a missing $Y$ always entails a missing later $W$; and $W$ may be missing after an observed $Y$.

<h4 id="2/2/6">6</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/6/solution">Solution</h5>

↑ **Parent:** [6](#2/2/6)

Under [missing at random](../../../probability-and-statistics.md#missing-at-random), dropout before the one-month visit may depend on observed treatment $Z$ but, conditional on $Z$, not on the unseen $Y$ or $W$. Dropout between the one- and six-month visits may depend on the observed history $(Z,Y)$ but, conditional on that history, not on the unseen $W$.

<h4 id="2/2/7">7</h4>

↑ **Parent:** [2](#2/2)

<h5 id="2/2/7/a">a</h5>

↑ **Parent:** [7](#2/2/7)

<h6 id="2/2/7/a/solution">Solution</h6>

↑ **Parent:** [A](#2/2/7/a)

The saturated first imputation model reproduces the observed conditional proportions. Thus

$$
\boxed{\widehat\phi_0\longrightarrow\frac{120}{200}=\frac35,
\qquad
\widehat\alpha\longrightarrow\frac12-\frac35=-\frac1{10}.}
$$

<h5 id="2/2/7/b">b</h5>

↑ **Parent:** [7](#2/2/7)

<h6 id="2/2/7/b/solution">Solution</h6>

↑ **Parent:** [B](#2/2/7/b)

For $Z=0$, the fitted conditional success probabilities for $W$ are

$$
\mathbb P(W=1\mid Z=0,Y=0)=\frac{20}{40}=\frac12,
\qquad
\mathbb P(W=1\mid Z=0,Y=1)=\frac{75}{90}=\frac56.
$$

Among all 250 subjects with $Z=0$, [multiple imputation](../../../probability-and-statistics.md#multiple-imputation) asymptotically assigns $100$ to $Y=0$ and $150$ to $Y=1$. Hence

$$
\widehat\psi_0\longrightarrow
\frac{100(1/2)+150(5/6)}{250}
=\frac7{10}.
$$

Using the supplied limit for $\widehat\psi_1$ gives

$$
\boxed{\widehat\beta\longrightarrow
\frac{25}{48}-\frac7{10}=-\frac{43}{240}.}
$$

<h2 id="3">3</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The [SI model](../../../mathematical-biology.md#si-model) has two compartments and one transition,

$$
S\xrightarrow{\,\beta SI/N\,}I,
$$

where $S$ and $I$ are the numbers susceptible and infectious and $\beta>0$ is the per-infective transmission-rate parameter under frequency-dependent homogeneous mixing.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The [ordinary differential equations](../../../differential-equation.md#ordinary-differential-equation) are

$$
\dot S=-\beta SI/N,
\qquad
\dot I=\beta SI/N,
\qquad
\beta>0,\qquad S,I\geq0.
$$

The [conservation of population](../../../mathematical-biology.md#conservation-of-population) identity $S+I=N$ follows by adding the equations.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Using $S=N-I$ reduces the system to the [logistic differential equation](../../../differential-equation.md#logistic-differential-equation)

$$
\dot I=\beta I(1-I/N).
$$

Separation of variables and the initial values give

$$
\log\frac{I}{N-I}=\beta t-\log\theta,
\qquad
I(t)=\frac{N}{1+\theta e^{-\beta t}}.
$$

Differentiation yields the incidence

$$
\boxed{\Lambda(t)=\dot I(t)
=\frac{\theta N\beta e^{-\beta t}}
{(1+\theta e^{-\beta t})^2}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Writing $x=\theta e^{-\beta t}$ gives $\Lambda=N\beta x/(1+x)^2$. Its maximum occurs at $x=1$, or

$$
t_*=\frac{\log\theta}{\beta},
\qquad
\Lambda(t_*)=\frac{N\beta}{4}.
$$

If time is restricted to $t\geq0$ and $\theta<1$, the unconstrained maximizer precedes the initial time, so the maximum on the observed interval is instead at $t=0$.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Set $\tau=t-t_*$. The [Logistic solution of the SI model](../../../mathematical-biology.md#logistic-solution-of-the-si-model) becomes

$$
\Lambda(\tau)=\frac{N\beta e^{-\beta\tau}}
{(1+e^{-\beta\tau})^2}
=\frac{N\beta}{4\cosh^2(\beta\tau/2)}.
$$

It is a symmetric, unimodal bell-shaped curve about the incidence peak $\tau=0$.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

The removal rate is $\dot R=\gamma I$. Because $\gamma$ is constant, its interior peak occurs when $I$ is maximal. At such a point,

$$
0=\dot I=I(\beta S-\gamma),
$$

and $I>0$, so

$$
S=\frac\gamma\beta.
$$

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

Dividing the $I$ equation by the $S$ equation gives

$$
\frac{dI}{dS}=-1+\frac{\gamma}{\beta S}.
$$

Therefore

$$
I+S-\frac\gamma\beta\log S
=I(0)+S(0)-\frac\gamma\beta\log S(0)
$$

is a [first integral](../../../differential-equation.md#first-integral). Define the [basic reproduction number](../../../mathematical-biology.md#basic-reproduction-number) by $R_0=\beta S(0)/\gamma$. At the removal peak, $S=S(0)/R_0$, and hence

$$
R_{\rm peak}=\frac{S(0)}{R_0}\log R_0,
$$

and, using $S+I+R=N$,

$$
I_{\rm peak}=I(0)+S(0)
-\frac{S(0)}{R_0}{1+\log R_0}.
$$

<h3 id="3/h">h</h3>

↑ **Parent:** [3](#3)

<h4 id="3/h/solution">Solution</h4>

↑ **Parent:** [H](#3/h)

The same first integral, evaluated initially and after the epidemic when $I(\infty)=0$, gives

$$
\log\frac{S(0)}{S(\infty)}
=\frac\beta\gamma R(\infty).
$$

When $I(0)$ is negligible and $R(0)=0$, [conservation of population](../../../mathematical-biology.md#conservation-of-population) gives $S(\infty)\simeq S(0)-R(\infty)$. Since $\beta/\gamma=R_0/S(0)$, this is equivalent to the [final size relation for an epidemic](../../../mathematical-biology.md#final-size-relation-for-an-epidemic)

$$
\boxed{R(\infty)\simeq
\frac{S(0)}{R_0}
\log\frac{S(0)}{S(0)-R(\infty)}.}
$$

<h2 id="4">4</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

At event time $t_j$, let $n_{Aj},n_{Bj}$ be the two [risk set](../../../survival-analysis.md#risk-set) sizes, $n_j=n_{Aj}+n_{Bj}$, and let $d_{Aj},d_{Bj}$ be the event counts with $d_j=d_{Aj}+d_{Bj}$. Under the null hypothesis of equal hazards, conditioning on the risk set and total number of events gives a [hypergeometric distribution](../../../discrete-probability-distribution.md#hypergeometric-distribution), so

$$
e_{Aj}=\mathbb E(d_{Aj})=d_j\frac{n_{Aj}}{n_j},
$$

and

$$
v_{Aj}=\operatorname{Var}(d_{Aj})
=\frac{n_{Aj}n_{Bj}d_j(n_j-d_j)}
{n_j^2(n_j-1)}.
$$

The [log-rank statistic](../../../survival-analysis.md#log-rank-statistic) and its estimated null variance are

$$
U=\sum_j(d_{Aj}-e_{Aj}),
\qquad
V=\sum_jv_{Aj}.
$$

Under the null, $U/\sqrt V$ is asymptotically standard normal, or $U^2/V$ is asymptotically chi-squared with one degree of freedom.

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The expected Treatment A deaths are $1/2$ at month 1, $1/2$ at month 2, and $3(2/6)=1$ at the three tied deaths at month 5. Thus

$$
E_A=2,
\qquad O_A=3.
$$

This is not half of the five deaths because [right censoring](../../../survival-analysis.md#right-censoring) changes the treatment proportions in successive [risk sets](../../../survival-analysis.md#risk-set). For Treatment B, $O_B=2$ and $E_B=3$. One observed-to-expected relative-risk estimate is therefore

$$
\boxed{\frac{O_A/E_A}{O_B/E_B}
=\frac{3/2}{2/3}=\frac94.}
$$

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

In a [constant hazard survival model](../../../survival-analysis.md#constant-hazard-survival-model), the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is the number of observed events divided by total [person-time at risk](../../../survival-analysis.md#person-time-at-risk). Treatment A contributes $3$ deaths in $1+2+3+3+5=14$ months, while Treatment B contributes $2$ deaths in $1+5+5+7+10=28$ months. Hence

$$
\boxed{\widehat h_A=\frac3{14},
\qquad
\widehat h_B=\frac2{28}=\frac1{14},
\qquad
\widehat{\operatorname{HR}}=3.}
$$

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) is

$$
\widehat H(t)=\sum_{t_j\leq t}\frac{d_j}{r_j}.
$$

For tied events, $d_j/r_j$ uses the number of events sharing time $t_j$ and the risk-set size just before that time.

At month 5,

$$
\widehat H_A(5)=\frac15+\frac14+1=\frac{29}{20},
\qquad
\widehat H_B(5)=\frac24=\frac12.
$$

Their ratio is $29/10=2.9$.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The three estimates are $9/4=2.25$, $3$, and $2.9$. They use different weightings of follow-up time and event times, but all indicate a substantially greater mortality hazard under Treatment A; the exponential and Nelson–Aalen estimates are particularly close.

<h2 id="5">5</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Conditioning on $T_1=t$ and using [independent random variables](../../../random-variable.md#independent-random-variables) gives

$$
\mathbb P(T_1<T_2)
=\int_0^\infty
\mathbb P(T_2>t\mid T_1=t)f_1(t)\,dt
=\int_0^\infty f_1(t)F_2(t)\,dt,
$$

where the notation in the paper uses $F_2$ for the [survival function](../../../survival-analysis.md#survival-function).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

With common fixed censoring time $c$, the ordering is known exactly when the earlier event occurs by $c$; continuity makes ties have probability zero. Thus the informative event is $\{min(T_1,T_2)\leq c\}$ and

$$
\boxed{\mathbb P(T_1<T_2\mid\text{informative})
=\frac{\int_0^c f_1(t)F_2(t)\,dt}
{1-F_1(c)F_2(c)}.}
$$

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/i">i</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/i/solution">Solution</h5>

↑ **Parent:** [I](#5/b/i)

For independent [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution), the numerator from part a(ii) is

$$
\int_0^c\lambda_1e^{-(\lambda_1+\lambda_2)t}\,dt
=\frac{\lambda_1}{\lambda_1+\lambda_2}
\{1-e^{-(\lambda_1+\lambda_2)c}\},
$$

while the denominator is the expression in braces. Their ratio is

$$
\boxed{\frac{\lambda_1}{\lambda_1+\lambda_2}.}
$$

<h4 id="5/b/ii">ii</h4>

↑ **Parent:** [B](#5/b)

<h5 id="5/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/b/ii)

Condition on the independently generated random censoring information. For every realized common censoring horizon, part b(i) gives the same conditional probability $\lambda_1/(\lambda_1+\lambda_2)$. The [law of total probability](../../../probability-theory.md#law-of-total-probability) therefore gives that ratio after averaging over the censoring distribution as well.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

Since $T_i$ has [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) $\phi_iH_0(t)$,

$$
\mathbb P\{H_0(T_i)>u\}
=\mathbb P\{T_i>H_0^{-1}(u)\}
=e^{-\phi_i u}.
$$

**Thus the cumulative-hazard time change $U_i=H_0(T_i)$ has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) of rate $\phi_i$.**

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

The increasing time change $H_0$ preserves the ordering of event times and transforms each censoring time by the same rule. Applying part b to $U_1,U_2$ therefore gives

$$
\mathbb P(T_1<T_2\mid\text{informative})
=\frac{\phi_1}{\phi_1+\phi_2}.
$$

This is the pairwise race probability for a [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

In a [competing risks model](../../../survival-analysis.md#competing-risks-model), the latent times to different event types form such a race: only the smallest time and its cause are observed. With proportional cause-specific hazards $\phi_i h_0(t)$, the probability that cause $i$ wins is $\phi_i/\sum_j\phi_j$, independently of the baseline hazard and under independent censoring. This is the same cancellation derived above.

<h2 id="6">6</h2>

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="6/solution">Solution</h3>

↑ **Parent:** [6](#6)

A [proportional frailty model](../../../survival-analysis.md#proportional-frailty-model) specifies

$$
h(t\mid U=u)=u h_0(t),
\qquad
S(t\mid U=u)=e^{-uH_0(t)}.
$$

Its population [survival function](../../../survival-analysis.md#survival-function) is the [Laplace transform](../../../analysis.md#laplace-transform) of the frailty density,

$$
\overline S(t)=\int_0^\infty e^{-uH_0(t)}g(u)\,du.
$$

If $m=\mathbb EU<\infty$, replacing $U$ by $U/m$ and $h_0$ by $m h_0$ leaves their product, and hence the model, unchanged. The normalization $\mathbb EU=1$ identifies this otherwise arbitrary scale and makes $h_0(0)$ the initial population hazard when $H_0(0)=0$.

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

For $g(u)=e^{-u}$,

$$
\overline S(t)=\int_0^\infty e^{-u\{1+H_0(t)\}}\,du
=\frac1{1+H_0(t)}.
$$

Therefore the population [hazard function](../../../survival-analysis.md#hazard-function) is

$$
\boxed{\overline h(t)
=-\frac d{dt}\log\overline S(t)
=\frac{h_0(t)}{1+H_0(t)}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

By [Bayes' theorem](../../../probability-theory.md#bayes-theorem), the [frailty distribution among survivors](../../../survival-analysis.md#frailty-distribution-among-survivors) has density

$$
g(u,t)
=\frac{\mathbb P(T>t\mid U=u)g(u)}{\overline S(t)}
=\{1+H_0(t)\}e^{-u\{1+H_0(t)\}},
\qquad u\geq0.
$$

It is an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with rate $1+H_0(t)$.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

The conditional mean frailty among survivors is

$$
\mathbb E(U\mid T>t)=\frac1{1+H_0(t)}.
$$

Because the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function) is nondecreasing, this mean is nonincreasing: high-frailty individuals tend to experience the event earlier, leaving a progressively more robust surviving population.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

Conditionally on survival, average the individual hazard $Uh_0(t)$:

$$
\overline h(t)
=h_0(t)\mathbb E(U\mid T>t)
=\frac{h_0(t)}{1+H_0(t)},
$$

which agrees with part a.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
