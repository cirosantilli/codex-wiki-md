# Paper 207

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_207.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_207.pdf)

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
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [i](#1/e/i)
      - [Solution](#1/e/i/solution)
    - [ii](#1/e/ii)
      - [Solution](#1/e/ii/solution)
  - [f](#1/f)
    - [i](#1/f/i)
      - [Solution](#1/f/i/solution)
    - [ii](#1/f/ii)
      - [Solution](#1/f/ii/solution)
  - [g](#1/g)
    - [Solution](#1/g/solution)
  - [h](#1/h)
    - [Solution](#1/h/solution)
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
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [i](#3/c/i)
      - [Solution](#3/c/i/solution)
    - [ii](#3/c/ii)
      - [Solution](#3/c/ii/solution)
    - [iii](#3/c/iii)
      - [Solution](#3/c/iii/solution)
    - [iv](#3/c/iv)
      - [Solution](#3/c/iv/solution)
- [4](#4)
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
  - [c](#4/c)
    - [i](#4/c/i)
      - [Solution](#4/c/i/solution)
    - [ii](#4/c/ii)
      - [Solution](#4/c/ii/solution)
    - [iii](#4/c/iii)
      - [Solution](#4/c/iii/solution)
    - [iv](#4/c/iv)
      - [Solution](#4/c/iv/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
    - [i](#5/a/i)
      - [Solution](#5/a/i/solution)
    - [ii](#5/a/ii)
      - [Solution](#5/a/ii/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
    - [i](#5/c/i)
      - [Solution](#5/c/i/solution)
    - [ii](#5/c/ii)
      - [Solution](#5/c/ii/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
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
    - [Solution](#6/b/solution)
    - [i](#6/b/i)
      - [Solution](#6/b/i/solution)
    - [ii](#6/b/ii)
      - [Solution](#6/b/ii/solution)

## 1

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The first subscript in $\beta_{t,\tau}$ is the [calendar time](../../../mathematical-biology.md#calendar-time) $t$, and the second is the [infection age](../../../mathematical-biology.md#infection-age) $\tau$, the time elapsed since the source individual became infected. Thus $\beta_{t,\tau}$ is the rate at which an individual of infection age $\tau$ generates infections at time $t$. The corresponding discrete [infectious disease renewal equation](../../../mathematical-biology.md#infectious-disease-renewal-equation) is

$$
\Delta_t=\sum_{\tau=1}^{t}\beta_{t,\tau}\Delta_{t-\tau},
$$

up to a separately modelled term for [imported infection](../../../mathematical-biology.md#imported-infection). The upper limit may instead be a fixed maximal infectious age, with unavailable terms set to zero.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [instantaneous reproduction number](../../../mathematical-biology.md#instantaneous-reproduction-number) at time $t$ is

$$
R_t^{\mathrm{inst}}=\sum_{\tau\geq1}\beta_{t,\tau}.
$$

It is the expected number of secondary infections that one infected individual would produce if the transmission conditions at time $t$ applied throughout that individual's infectious life. The [case reproduction number](../../../mathematical-biology.md#case-reproduction-number), also called the effective reproduction number in this question, is

$$
R_t^{\mathrm{case}}=\sum_{\tau\geq1}\beta_{t+\tau,\tau},
$$

the expected number actually produced by a person infected at $t$ as calendar-time conditions subsequently change. The instantaneous quantity is easier to estimate in real time because it depends on current and past [incidence](../../../mathematical-biology.md#incidence-epidemiology); the case quantity depends on future conditions.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Assume the [infectivity profile](../../../mathematical-biology.md#infectivity-profile) is separable:

$$
\beta_{t,\tau}=R_tg_\tau,
\qquad g_\tau\geq0,
\qquad \sum_{\tau\geq1}g_\tau=1.
$$

Then $g_\tau$ is the discretized [generation-interval distribution](../../../mathematical-biology.md#generation-interval-distribution), $R_t$ is the [instantaneous reproduction number](../../../mathematical-biology.md#instantaneous-reproduction-number), and the [infectious disease renewal equation](../../../mathematical-biology.md#infectious-disease-renewal-equation) becomes

$$
\Delta_t=R_t\Lambda_t,
\qquad
\Lambda_t=\sum_{\tau=1}^{t}g_\tau\Delta_{t-\tau}.
$$

**Hence $R_t=\Delta_t/\Lambda_t$ whenever the total infectiousness $\Lambda_t$ is positive.**

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

If [incidence](../../../mathematical-biology.md#incidence-epidemiology) grows exponentially, $\Delta_t=C e^{\rho t}$, substitution in the [infectious disease renewal equation](../../../mathematical-biology.md#infectious-disease-renewal-equation) gives the discrete [Euler-Lotka equation](../../../mathematical-biology.md#euler-lotka-equation)

$$
1=R_t\sum_{i=1}^{t}g_i e^{-\rho i},
\qquad
R_t=\left(\sum_{i=1}^{t}g_i e^{-\rho i}\right)^{-1}.
$$

For $X\sim\operatorname{Geometric}(p)$ on $\{0,1,\ldots\}$, $g_i=\mathbb P(X=i-1)=p(1-p)^{i-1}$. The [finite geometric series](../../../real-analysis.md#finite-geometric-series) therefore yields

$$
\sum_{i=1}^{t}g_i e^{-\rho i}
=pe^{-\rho}\frac{1-(1-p)^t e^{-\rho t}}{1-(1-p)e^{-\rho}},
$$

and consequently

$$
\boxed{R_t=
\frac{1-(1-p)e^{-\rho}}
{pe^{-\rho}\bigl(1-(1-p)^t e^{-\rho t}\bigr)}.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Treat the diagnosis counts as the observed [incidence](../../../mathematical-biology.md#incidence-epidemiology) series and define their total infectiousness by

$$
s_t=\sum_{\tau=1}^{t}g_\tau I_{t-\tau}.
$$

A conditionally independent [Poisson observation model](../../../discrete-probability-distribution.md#poisson-observation-model) for the renewal process is

$$
I_t\mid R_t,g,I_0,\ldots,I_{t-1}\sim\operatorname{Poisson}(R_ts_t),
\qquad
p(I_1,\ldots,I_T\mid R,g)=\prod_{t=1}^{T}
\frac{e^{-R_ts_t}(R_ts_t)^{I_t}}{I_t!}.
$$

Initial infections before the observation window can be included in the definition of $s_t$.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Use the shape-rate convention $R_k\sim\operatorname{Gamma}(\alpha_0,\beta_0)$. The factors involving $R_k$ in the [posterior density](../../../statistical-inference.md#posterior-density) are

$$
R_k^{I_k}e^{-s_kR_k}R_k^{\alpha_0-1}e^{-\beta_0R_k}
=R_k^{I_k+\alpha_0-1}e^{-(s_k+\beta_0)R_k}.
$$

By [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy),

$$
R_k\mid I_k,s_k\sim\operatorname{Gamma}(I_k+\alpha_0,s_k+\beta_0),
$$

so its [posterior mean](../../../statistical-inference.md#posterior-mean) is $(I_k+\alpha_0)/(s_k+\beta_0)$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Use a three-state [continuous-time multi-state model](../../../survival-analysis.md#continuous-time-multi-state-model) with transient infected state $I$ and absorbing recovered and dead states $R$ and $D$. If recovery and death have constant [transition intensities](../../../survival-analysis.md#transition-intensity) $\gamma$ and $\mu$, its [Q-matrix](../../../markov-process.md#transition-rate-matrix) is

$$
Q=
\begin{pmatrix}
-(\gamma+\mu)&\gamma&\mu\\
0&0&0\\
0&0&0
\end{pmatrix},
$$

with state order $(I,R,D)$. This is also a [competing risks model](../../../survival-analysis.md#competing-risks-model): recovery and death are the two mutually exclusive first events.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/i">i</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/i/solution">Solution</h5>

↑ **Parent:** [I](#1/e/i)

The two event clocks have independent [exponential distributions](../../../continuous-probability-distribution.md#exponential-distribution) with rates $\mu$ and $\gamma$. The [competing exponential clocks](../../../continuous-probability-distribution.md#competing-exponential-clocks) identity gives

$$
\boxed{\mathbb P_I(D\text{ before }R)=\frac{\mu}{\mu+\gamma}.}
$$

<h4 id="1/e/ii">ii</h4>

↑ **Parent:** [E](#1/e)

<h5 id="1/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/e/ii)

The minimum of the recovery and death clocks has an [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution) with rate $\mu+\gamma$. Its [expected value](../../../probability-theory.md#expected-value) is therefore

$$
\boxed{\mathbb E_I[T_{\{R,D\}}]=\frac1{\mu+\gamma}.}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/i">i</h4>

↑ **Parent:** [F](#1/f)

<h5 id="1/f/i/solution">Solution</h5>

↑ **Parent:** [I](#1/f/i)

The [transition probability matrix](../../../markov-process.md#transition-semigroup-of-a-continuous-time-markov-chain) has entries

$$
P_{rs}(u)=\mathbb P(X(t+u)=s\mid X(t)=r)
$$

under the [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property). For the finite-state model in part d, the [transition semigroup of a continuous-time Markov chain](../../../markov-process.md#transition-semigroup-of-a-continuous-time-markov-chain) is

$$
\boxed{P(u)=e^{uQ}.}
$$

<h4 id="1/f/ii">ii</h4>

↑ **Parent:** [F](#1/f)

<h5 id="1/f/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/f/ii)

Assume a negative test identifies the recovered state. Person 1 remains infected through day 7 and recovers during $(7,14]$, so their [interval-censored](../../../survival-analysis.md#interval-censoring) contribution is

$$
P_{II}(7)P_{IR}(7).
$$

Person 2 remains infected through day 7 and makes an exact $I\to D$ transition at day 10. A transition at an exact time contributes a transition probability density, giving

$$
P_{II}(7)P_{II}(3)q_{ID}=P_{II}(10)\mu.
$$

Assuming independent individuals, their joint [likelihood contribution](../../../survival-analysis.md#likelihood-contribution) is

$$
\boxed{P_{II}(7)P_{IR}(7)P_{II}(10)\mu.}
$$

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

The model assumes a [time-homogeneous Markov property](../../../markov-process.md#time-homogeneous-markov-property): transition intensities depend only on the current state, not on calendar time, infection age, or earlier history. A [Semi-Markov multi-state model](../../../survival-analysis.md#semi-markov-multi-state-model) could let recovery and death hazards depend on time since infection or entry into the current state. Weekly tests reveal recovery only by [interval censoring](../../../survival-analysis.md#interval-censoring), however, so the relevant entry and transition times are latent. Fitting the less restrictive model then requires integrating over unobserved paths, and the available data may contain too little information to identify a flexible duration-dependent hazard.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

Add a hospital state $H$ and estimate the enlarged [Q-matrix](../../../markov-process.md#transition-rate-matrix) from the cohort. If infection starts in state $I$, the expected hospital occupancy generated by one infection is the [Markov reward model](../../../markov-process.md#markov-reward-model) integral

$$
m_H=\int_0^\infty P_{IH}(t)\,dt.
$$

Equivalently, if $Q_T$ is the subgenerator on all transient states, $m_H$ is the $(I,H)$ entry of the [fundamental matrix of an absorbing continuous-time Markov chain](../../../survival-analysis.md#fundamental-matrix-of-an-absorbing-continuous-time-markov-chain) $(-Q_T)^{-1}$. The number infected in the population has expectation $Np$, so [linearity of expectation](../../../probability-theory.md#linearity-of-expectation) gives total expected hospital use $Np,m_H$ days. If only occupancy within a finite period counts, replace the upper integration limit by the remaining follow-up time for each infection and average over infection times.

## 2

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Let $\widehat p_k=X_k/n_k$, where $X_k\sim\operatorname{Binomial}(n_k,p_k)$ independently, and put

$$
\widehat V=\frac{\widehat p_1(1-\widehat p_1)}{n_1}
+\frac{\widehat p_0(1-\widehat p_0)}{n_0}.
$$

The [Wald statistic](../../../statistical-modelling.md#wald-test) is $Z=(\widehat p_1-\widehat p_0)/\sqrt{\widehat V}$. The [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) and [Slutsky theorem](../../../statistical-inference.md#slutsky-theorem) give $Z\dot\sim N(0,1)$ under $H_0$. When $p_1-p_0=\delta^*>0$,

$$
\boxed{Z\dot\sim N\!\left(
\frac{\delta^*}{\sqrt{p_1(1-p_1)/n_1+p_0(1-p_0)/n_0}},1
\right).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For equal arm size $n$, write $v^*=p_1(1-p_1)+p_0(1-p_0)$ at the clinically relevant alternative. A one-sided level-$\alpha$ [Wald test](../../../statistical-modelling.md#wald-test) rejects when $Z>z_{1-\alpha}$, and its approximate [statistical power](../../../probability-and-statistics.md#statistical-power) is

$$
1-\Phi\!\left(z_{1-\alpha}-\frac{\delta^*\sqrt n}{\sqrt{v^*}}\right).
$$

Equating this to $1-\beta$ gives the per-arm [sample size](../../../probability-and-statistics.md#sample-size)

$$
n=\frac{v^*\bigl(z_{1-\alpha}+z_{1-\beta}\bigr)^2}{(\delta^*)^2},
$$

rounded up. If the design uses a null-based critical standard error $v_0$ but an alternative standard error $v^*$, the corresponding more general formula is

$$
\boxed{n=\frac{\bigl(z_{1-\alpha}\sqrt{v_0}+z_{1-\beta}\sqrt{v^*}\bigr)^2}{(\delta^*)^2}.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A [group sequential design](../../../probability-and-statistics.md#group-sequential-design) can reduce the expected sample size by stopping at an [interim analysis](../../../probability-and-statistics.md#interim-analysis) once efficacy or futility is sufficiently clear. It does not generally reduce the prespecified maximum sample size: repeated opportunities to reject inflate the [Type I error](../../../information-theory.md#type-i-and-type-ii-errors), so valid [sequential stopping boundaries](../../../probability-and-statistics.md#sequential-stopping-boundary) usually require a modest increase in maximum information relative to a fixed-sample design with the same power. The benefit is a smaller expected sample size under alternatives that often cross an early boundary, and sometimes under the null through early futility stopping.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let

$$
v=p_1(1-p_1)+p_0(1-p_0),
\qquad I_j=\frac{m_j}{v},
$$

where $m_j$ is the cumulative sample size per arm. The [canonical joint distribution for group sequential test statistics](../../../probability-and-statistics.md#canonical-joint-distribution-for-group-sequential-test-statistics) is

$$
\begin{pmatrix}Z_1\\Z_2\end{pmatrix}
\dot\sim N_2\!\left[
\begin{pmatrix}\delta\sqrt{I_1}\\\delta\sqrt{I_2}\end{pmatrix},
\begin{pmatrix}
1&\sqrt{I_1/I_2}\\
\sqrt{I_1/I_2}&1
\end{pmatrix}
\right].
$$

**Thus $\operatorname{Corr}(Z_1,Z_2)=\sqrt{m_1/m_2}$. This correlation arises because the second statistic reuses all first-stage observations.**

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Under $H_0$, $(Z_1,Z_2)$ is a [bivariate standard normal distribution](../../../probability-and-statistics.md#bivariate-standard-normal-distribution) with correlation $\rho=\sqrt{m_1/m_2}$. Rejection occurs either at stage 1 through $Z_1\geq u_1$, or at stage 2 through $Z_2\geq u_2$ after continuation $l_1<Z_1<u_1$. Hence the [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) is

$$
\alpha_{\mathrm{actual}}
=\mathbb P_0(Z_1\geq u_1)
+\mathbb P_0(l_1<Z_1<u_1,,Z_2\geq u_2)
$$



$$
=1-\Phi(u_1)+
\int_{l_1}^{u_1}\phi(z)
\left[1-\Phi\!\left(\frac{u_2-\rho z}{\sqrt{1-\rho^2}}\right)\right]dz.
$$

The final lack-of-benefit boundary $l_2$ affects acceptance, but not the probability of crossing an efficacy boundary.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

[Response-adaptive randomization](../../../probability-and-statistics.md#response-adaptive-randomization) can assign a larger proportion of later participants to the treatment currently estimated to be better, improving outcomes for participants within the trial. Its allocation probabilities depend on earlier outcomes, which complicates [statistical inference](../../../statistical-inference.md); delayed responses and calendar-time trends can also make adaptation ineffective or biased, and an allocation aimed at patient benefit need not maximize power.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

Under [Neyman allocation](../../../probability-and-statistics.md#neyman-allocation), sample sizes are proportional to the arm standard deviations. Here

$$
\frac{n_1}{n_0}
=\frac{\sqrt{p_1(1-p_1)}}{\sqrt{p_0(1-p_0)}}
=\frac{0.5}{0.3}=\frac53.
$$

For total size $n_{\max}$, the minimized [asymptotic variance](../../../statistical-modelling.md#asymptotic-variance) is

$$
\operatorname{Var}(\widehat p_1-\widehat p_0)
=\frac{\bigl(\sqrt{0.25}+\sqrt{0.09}\bigr)^2}{n_{\max}}
=\frac{0.64}{n_{\max}}.
$$

Equal allocation gives

$$
\frac{0.25}{n_{\max}/2}+\frac{0.09}{n_{\max}/2}
=\frac{0.68}{n_{\max}}.
$$

The Neyman allocation therefore reduces the large-sample variance by $0.04/n_{\max}$, about $5.9\%$ of the equal-allocation variance.

## 3

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Let $K\in\mathbb R^{n\times n}$ have entries $K_{ij}=\kappa(x_i,x_j)$, let $k_*\in\mathbb R^n$ have entries $(k_*)_i=\kappa(x_i,x_*)$, and let $k_{**}=\kappa(x_*,x_*)$. The [Gaussian process](../../../stochastic-process.md#gaussian-process) prior and independent [Gaussian noise](../../../probability-theory.md#gaussian-noise) imply

$$
\begin{pmatrix}f(x_*)\\y\end{pmatrix}
\sim N\!\left[
\begin{pmatrix}0\\0_n\end{pmatrix},
\begin{pmatrix}
k_{**}&k_*^T\\
k_*&K+\sigma^2I_n
\end{pmatrix}
\right].
$$

Applying the [conditional multivariate normal distribution](../../../probability-and-statistics.md#conditional-multivariate-normal-distribution) gives the [Gaussian process regression posterior](../../../probability-and-statistics.md#gaussian-process-regression-posterior)

$$
f(x_*)\mid y,X,x_*
\sim N(m_*,v_*),
$$

where

$$
m_*=k_*^T(K+\sigma^2I_n)^{-1}y,
\qquad
v_*=k_{**}-k_*^T(K+\sigma^2I_n)^{-1}k_*.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Set $x_*=0.5$ in the [Gaussian process regression posterior](../../../probability-and-statistics.md#gaussian-process-regression-posterior) and compute $m_*$ and $v_*$ as in part a. [Standardization of a normal random variable](../../../probability-theory.md#standardization-of-a-normal-random-variable) then gives

$$
\mathbb P\bigl(f(0.5)<1.5\mid y,X\bigr)
=\Phi\!\left(\frac{1.5-m_*}{\sqrt{v_*}}\right),
$$

where $\Phi$ is the [standard normal cumulative distribution function](../../../probability-theory.md#standard-normal-distribution-function).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/i">i</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/i/solution">Solution</h5>

↑ **Parent:** [I](#3/c/i)

Let $N_m=|\{i:c_i=m\}|$. The label likelihood for the [mixture weights](../../../statistical-modelling.md#mixture-weight) is proportional to $\prod_{m=1}^3\pi_m^{N_m}$. Multiplication by the $\operatorname{Dirichlet}(\alpha_1,\alpha_2,\alpha_3)$ density and [Dirichlet-multinomial conjugacy](../../../statistical-inference.md#dirichlet-multinomial-conjugacy) gives

$$
(\pi_1,\pi_2,\pi_3)\mid y,c,f
\sim\operatorname{Dirichlet}(\alpha_1+N_1,\alpha_2+N_2,\alpha_3+N_3).
$$

Conditional on the labels, the observations and component means provide no further information about $\pi$.

<h4 id="3/c/ii">ii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/c/ii)

For component $m$, stack its $N_m$ assigned observations as $y_1^{(m)},\ldots,y_{N_m}^{(m)}\in\mathbb R^n$. The prior is $f_m\sim N_n(0,K)$ and each assigned vector is conditionally $N_n(f_m,\sigma^2I_n)$. [Normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
f_m\mid y,c,\pi\sim N_n(\mu_m,V_m),
$$

where

$$
V_m=\left(K^{-1}+\frac{N_m}{\sigma^2}I_n\right)^{-1},
\qquad
\mu_m=V_m\frac1{\sigma^2}\sum_{r=1}^{N_m}y_r^{(m)}.
$$

If $N_m=0$, this reduces to the prior $N_n(0,K)$.

<h4 id="3/c/iii">iii</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/c/iii)

[Bayes' theorem](../../../probability-theory.md#bayes-theorem) turns the [categorical distribution](../../../discrete-probability-distribution.md#categorical-distribution) prior probabilities and the component [multivariate normal densities](../../../probability-and-statistics.md#multivariate-normal-density) into

$$
\mathbb P(c_i=m\mid y_i,\pi,f)
=\frac{\pi_m\phi(y_i;f_m,\sigma^2I_n)}
{\sum_{\ell=1}^3\pi_\ell\phi(y_i;f_\ell,\sigma^2I_n)},
\qquad m=1,2,3.
$$

These probabilities define the label update in the [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler).

<h4 id="3/c/iv">iv</h4>

↑ **Parent:** [C](#3/c)

<h5 id="3/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/c/iv)

A [Dirichlet process mixture model](../../../statistical-modelling.md#dirichlet-process-mixture-model) avoids fixing the number of occupied functions. Let $G_0=N_n(0,K)$ be the finite-dimensional [Gaussian process](../../../stochastic-process.md#gaussian-process) law on the common input grid and specify

$$
G\sim\operatorname{DP}(\alpha,G_0),
\qquad
f_i\mid G\overset{\mathrm{iid}}\sim G,
\qquad
y_i\mid f_i\sim N_n(f_i,\sigma^2I_n).
$$

A draw from a [Dirichlet process](../../../statistical-inference.md#dirichlet-process) is almost surely discrete, so several $f_i$ coincide and thereby form clusters. The number of occupied clusters is random and can grow with the data.

## 4

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

The [risk set](../../../survival-analysis.md#risk-set) at event time $a_j$ contains individuals still under observation and event-free immediately before $a_j$. For group $k$ its size is

$$
r_j^{(k)}=\sum_{i=1}^n\mathbf1\{g_i=k,,x_i\geq a_j\}.
$$

The use of $\geq$ keeps the individual who experiences the event at $a_j$ in the risk set just before that event.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) of equal event-time distributions, every member of the combined [risk set](../../../survival-analysis.md#risk-set) has the same instantaneous chance of being the next event. Conditional on one event at $a_j$ and on the two risk-set sizes,

$$
U_j\sim\operatorname{Bernoulli}\!\left(
\frac{r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}
\right),
$$

so

$$
\mathbb E_0(U_j\mid r_j^{(0)},r_j^{(1)})
=\frac{r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}.
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The quantity

$$
u_j-\mathbb E_0U_j
=u_j-\frac{r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}
$$

is the observed-minus-expected group-1 event count at time $a_j$. A positive value is local evidence that group 1 has the greater [hazard function](../../../survival-analysis.md#hazard-function); a negative value points toward group 0.

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

Summing the observed-minus-expected contributions gives the unstandardized [log-rank statistic](../../../survival-analysis.md#log-rank-statistic)

$$
T_0=\sum_{j=1}^m
\left\{u_j-
\frac{r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}
\right\}.
$$

Under the null it is centered at zero. A two-sided [log-rank test](../../../survival-analysis.md#log-rank-test) compares its magnitude with the square root of its null variance.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Let $Y(t)$ be the [at-risk process](../../../survival-analysis.md#at-risk-process) and $N(t)$ the [counting process](../../../stochastic-process.md#counting-process) for observed events. Over a short interval, the multiplicative-intensity model gives

$$
\mathbb E\{dN(t)\mid\mathcal F_{t-}\}=Y(t)h(t),dt
=Y(t),dH(t),
$$

where $h$ is the [hazard function](../../../survival-analysis.md#hazard-function) and $H$ the [cumulative hazard function](../../../survival-analysis.md#cumulative-hazard-function). Solving this relation for the infinitesimal hazard increment suggests $d\widehat H(t)=dN(t)/Y(t)$. Summing over distinct event times gives the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator)

$$
\widehat H(t)=\sum_{j:a_j\leq t}\frac{d_j}{r_j},
$$

where $d_j$ events occur among $r_j$ individuals at risk. Here there are no ties, so $d_j=1$.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/i">i</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/i/solution">Solution</h5>

↑ **Parent:** [I](#4/c/i)

Let $u_j^{(1)}=u_j$ and $u_j^{(0)}=1-u_j$. Applying the [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) separately to group $k$ gives

$$
\widehat H_j^{(k)}
=\sum_{\ell=1}^{j}\frac{u_\ell^{(k)}}{r_\ell^{(k)}},
$$

with a zero contribution when the event at $a_\ell$ occurs in the other group.

<h4 id="4/c/ii">ii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/c/ii)

The group-specific estimated [cumulative hazard](../../../survival-analysis.md#cumulative-hazard-function) jumps only when that group experiences the event, so

$$
\Delta\widehat H_j^{(1)}=\frac{u_j}{r_j^{(1)}},
\qquad
\Delta\widehat H_j^{(0)}=\frac{1-u_j}{r_j^{(0)}}.
$$

<h4 id="4/c/iii">iii</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/c/iii)

Put $r_j=r_j^{(0)}+r_j^{(1)}$. The difference between the two [Nelson–Aalen estimator](../../../survival-analysis.md#nelson-aalen-estimator) increments is

$$
\frac{u_j}{r_j^{(1)}}-\frac{1-u_j}{r_j^{(0)}}
=\frac{r_j}{r_j^{(0)}r_j^{(1)}}
\left(u_j-\frac{r_j^{(1)}}{r_j}\right).
$$

Therefore the [log-rank weights](../../../survival-analysis.md#log-rank-weight)

$$
w_j=\frac{r_j^{(0)}r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}
$$

make each summand of $T_W$ equal the corresponding summand of $T_0$, and hence $T_W=T_0$.

<h4 id="4/c/iv">iv</h4>

↑ **Parent:** [C](#4/c)

<h5 id="4/c/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/c/iv)

The variance of an estimated hazard increment is large when its group has few individuals in the [risk set](../../../survival-analysis.md#risk-set). The [log-rank weights](../../../survival-analysis.md#log-rank-weight) are near zero when either $r_j^{(0)}$ or $r_j^{(1)}$ is small and are largest when both groups retain substantial information. They therefore suppress noisy late-event comparisons and weight each observed-minus-expected event by its available information. Unit weights would instead give equal influence to unstable increments from depleted risk sets.

## 5

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

A [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family) has [hazard functions](../../../survival-analysis.md#hazard-function) related by

$$
h(t\mid z)=c(z)h_0(t),
$$

where the [hazard ratio](../../../survival-analysis.md#hazard-ratio) $c(z)$ is positive and independent of time. Equivalently, its [cumulative hazard functions](../../../survival-analysis.md#cumulative-hazard-function) satisfy $H(t\mid z)=c(z)H_0(t)$ and its [survivor functions](../../../survival-analysis.md#survival-function) satisfy $S(t\mid z)=S_0(t)^{c(z)}$.

<h4 id="5/a/i">i</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/i/solution">Solution</h5>

↑ **Parent:** [I](#5/a/i)

Writing the two functions in the question as survivor functions, $S_2(t)=S_1(t)^\lambda$. Since $H_k(t)=-\log S_k(t)$,

$$
H_2(t)=-\log S_2(t)=-\lambda\log S_1(t)=\lambda H_1(t).
$$

Differentiating at times where the [hazard functions](../../../survival-analysis.md#hazard-function) exist gives $h_2(t)=\lambda h_1(t)$. Their [hazard ratio](../../../survival-analysis.md#hazard-ratio) is therefore the constant $\lambda$, so they form a [proportional hazards family](../../../survival-analysis.md#proportional-hazards-family).

<h4 id="5/a/ii">ii</h4>

↑ **Parent:** [A](#5/a)

<h5 id="5/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/a/ii)

The transformation is $T_k=a_kU_k^b$. Because $U_k$ has a unit-rate [exponential distribution](../../../continuous-probability-distribution.md#exponential-distribution),

$$
S_k(t)=\mathbb P\!\left(U_k>(t/a_k)^{1/b}\right)
=\exp\!\left[-(t/a_k)^{1/b}\right].
$$

Thus $T_k$ has a [Weibull distribution](../../../probability-theory.md#weibull-distribution), with

$$
H_k(t)=(t/a_k)^{1/b},
\qquad
h_k(t)=\frac1b a_k^{-1/b}t^{1/b-1}.
$$

**Consequently $h_2(t)/h_1(t)=(a_1/a_2)^{1/b}$ is constant, proving [proportional hazards](../../../survival-analysis.md#proportional-hazards-model).**

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

Choose a parametric baseline hazard $h_0(t;\eta)$ and fit

$$
h(t\mid z)=h_0(t;\eta)e^{\beta z}.
$$

Under independent [right censoring](../../../survival-analysis.md#right-censoring), the full [survival likelihood](../../../survival-analysis.md#survival-likelihood) is

$$
L(\eta,\beta)=\prod_{i=1}^n
\bigl[h_0(x_i;\eta)e^{\beta z_i}\bigr]^{v_i}
\exp\!\left[-H_0(x_i;\eta)e^{\beta z_i}\right].
$$

Estimate $(\eta,\beta)$ by [maximum likelihood estimation](../../../statistical-modelling.md#maximum-likelihood-estimation) and test $H_0:\beta=0$ with a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test), [Wald test](../../../statistical-modelling.md#wald-test), or [score test](../../../statistical-modelling.md#score-test). Equality of the two event-time distributions is exactly $\beta=0$ within this model.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

A [semiparametric proportional hazards model](../../../survival-analysis.md#semiparametric-proportional-hazards-model) specifies

$$
h(t\mid z)=h_0(t)e^{\beta z}
$$

with finite-dimensional parameter $\beta$ but an unspecified baseline hazard $h_0$. A [partial likelihood](../../../survival-analysis.md#partial-likelihood) uses a component of the data likelihood that depends on $\beta$ while eliminating the nuisance function. In the [Cox proportional-hazards model](../../../survival-analysis.md#cox-proportional-hazards-model), conditioning on which member of each [risk set](../../../survival-analysis.md#risk-set) experiences the event produces the [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood).

<h4 id="5/c/i">i</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/i/solution">Solution</h5>

↑ **Parent:** [I](#5/c/i)

For each observed event $i$ with $v_i=1$, let $R_i=\{j:x_j\geq x_i\}$ be its [risk set](../../../survival-analysis.md#risk-set). The [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) is

$$
L_p(\beta)=\prod_{i:v_i=1}
\frac{e^{\beta z_i}}{\sum_{j\in R_i}e^{\beta z_j}}.
$$

Maximize it to obtain $\widehat\beta$, estimate its variance from the observed partial information, and test $H_0:\beta=0$ using a [partial likelihood-ratio test](../../../survival-analysis.md#partial-likelihood-ratio-test), [Wald test](../../../statistical-modelling.md#wald-test), or [score test](../../../statistical-modelling.md#score-test). A positive fitted coefficient means the group with $z=1$ has the larger hazard.

<h4 id="5/c/ii">ii</h4>

↑ **Parent:** [C](#5/c)

<h5 id="5/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#5/c/ii)

Let

$$
a=e^{\beta z_{n-1}},\qquad b=e^{\beta z_n},\qquad c=e^{\beta z_{n-2}},
$$

and let $C$ be the common [partial likelihood](../../../survival-analysis.md#partial-likelihood) contribution from the first $n-3$ observations. Since $t_{n-2}>x_{n-2}$, the three possible complete-data tail orderings and their partial likelihoods are

$$
\begin{array}{c|c}
t_{n-2}<x_{n-1}<x_n&C\dfrac{c}{a+b+c}\dfrac{a}{a+b}\\[6pt]
x_{n-1}<t_{n-2}<x_n&C\dfrac{a}{a+b+c}\dfrac{c}{b+c}\\[6pt]
x_{n-1}<x_n<t_{n-2}&C\dfrac{a}{a+b+c}\dfrac{b}{b+c}.
\end{array}
$$

Their sum is

$$
C\left[
\frac{c}{a+b+c}\frac{a}{a+b}
+\frac{a}{a+b+c}\frac{c+b}{b+c}
\right]
=C\frac{a}{a+b}.
$$

When individual $n-2$ is [right-censored](../../../survival-analysis.md#right-censoring) at $x_{n-2}$, that individual leaves the [risk set](../../../survival-analysis.md#risk-set) before the event at $x_{n-1}$, so the directly calculated [Cox partial likelihood](../../../survival-analysis.md#cox-partial-likelihood) is also $C,a/(a+b)$. Summing over the unobserved compatible event orderings therefore reproduces the censored-data partial likelihood.

## 6

↑ **Parent:** [Paper 207](paper-207.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

[Empirical likelihood](../../../nonparametric-statistics.md#empirical-likelihood) assigns unknown probability masses $p_j\geq0$ to data-supported event times or intervals, imposes $\sum_jp_j=1$, and maximizes the product of each observation's probability. For event-time data, write $F(t)=\mathbb P(T\leq t)$ and $S(t)=1-F(t)$ for the [survivor function](../../../survival-analysis.md#survival-function). Exact, right-censored, left-censored, interval-censored, and truncated observations contribute the probability of their respective compatible sets.

The maximization uses that $S$ is nonincreasing and right-continuous, $S(0)=1$, and $S(t)\to0$ as $t\to\infty$. Probability mass need only be placed at endpoints that change an observation's compatible set; moving mass within any observationally indistinguishable interval leaves the likelihood unchanged. Maximizing over those masses gives the [nonparametric maximum-likelihood estimator](../../../nonparametric-statistics.md#nonparametric-maximum-likelihood-estimator) of the survivor function.

<h4 id="6/a/i">i</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/i/solution">Solution</h5>

↑ **Parent:** [I](#6/a/i)

The death time is [right-censored](../../../survival-analysis.md#right-censoring) at 36 months, so the contribution is

$$
\boxed{\mathbb P(T>36)=S(36).}
$$

<h4 id="6/a/ii">ii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/a/ii)

An exact death at 42 months contributes the probability mass at 42,

$$
\mathbb P(T=42)=F(42)-F(42^-)=S(42^-)-S(42).
$$

For a continuous model this is represented by the event density $f(42)$ rather than a point mass, but [empirical likelihood](../../../nonparametric-statistics.md#empirical-likelihood) permits discrete masses.

<h4 id="6/a/iii">iii</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#6/a/iii)

The awakening time is [left-censored](../../../survival-analysis.md#left-censoring) at 15 minutes, so its contribution is

$$
\boxed{\mathbb P(T\leq15)=F(15)=1-S(15).}
$$

<h4 id="6/a/iv">iv</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#6/a/iv)

The secondary cancer appears in the interval $(6,9]$, producing the [interval-censored](../../../survival-analysis.md#interval-censoring) contribution

$$
\boxed{\mathbb P(6<T\leq9)=F(9)-F(6)=S(6)-S(9).}
$$

<h4 id="6/a/v">v</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/v/solution">Solution</h5>

↑ **Parent:** [V](#6/a/v)

The bus may have arrived before observation began or after observation ended. Its compatible event set is $(-\infty,2)\cup(20,\infty)$, so, with endpoint conventions chosen to match whether arrivals exactly at 2 or 20 would be seen, the contribution is

$$
\mathbb P(T<2)+\mathbb P(T>20)=F(2^-)+S(20).
$$

This is [doubly censored data](../../../survival-analysis.md#doubly-censored-data), because neither the side nor the event time is known.

<h4 id="6/a/vi">vi</h4>

↑ **Parent:** [A](#6/a)

<h5 id="6/a/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#6/a/vi)

Measure time in years after age 70. Residence in the care home begins at time 3, so inclusion is conditional on $T>3$: this is [left truncation](../../../survival-analysis.md#left-truncation), also called delayed entry. Exact death at time 13 contributes

$$
\boxed{\mathbb P(T=13\mid T>3)
=\frac{F(13)-F(13^-)}{S(3)}
=\frac{S(13^-)-S(13)}{S(3)}.}
$$

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

A [period survival analysis](../../../survival-analysis.md#period-survival-analysis) estimates survival under the recent mortality conditions operating during a fixed calendar period. For calendar year 2022, each cancer patient's contribution begins at the later of diagnosis and 1 January 2022, which treats earlier diagnoses as [left-truncated](../../../survival-analysis.md#left-truncation) at the start of the year. Follow-up ends at death, loss to follow-up, or 31 December 2022, so surviving records are [right-censored](../../../survival-analysis.md#right-censoring). Combining these risk-set contributions, commonly through a [Kaplan–Meier estimator](../../../survival-analysis.md#kaplan-meier-estimator), constructs the 2022 period survivor function; records from several diagnosis cohorts may contribute different segments of follow-up.

<h4 id="6/b/i">i</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/i/solution">Solution</h5>

↑ **Parent:** [I](#6/b/i)

Construct the two countries' period-specific [risk sets](../../../survival-analysis.md#risk-set) with the same [left truncation](../../../survival-analysis.md#left-truncation) and [right censoring](../../../survival-analysis.md#right-censoring) rules, then compare their event counts by a [log-rank test](../../../survival-analysis.md#log-rank-test). This is a nonparametric comparison because it does not specify the shape of either country's [hazard function](../../../survival-analysis.md#hazard-function).

<h4 id="6/b/ii">ii</h4>

↑ **Parent:** [B](#6/b)

<h5 id="6/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#6/b/ii)

Under a country-specific [constant hazard survival model](../../../survival-analysis.md#constant-hazard-survival-model), let $D_k$ be the number of deaths and $Y_k$ the total [person-time at risk](../../../survival-analysis.md#person-time-at-risk) in country $k$. The likelihood is proportional to

$$
L_k(\lambda_k)\propto\lambda_k^{D_k}e^{-\lambda_kY_k},
$$

so the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is $\widehat\lambda_k=D_k/Y_k$. Test $H_0:\lambda_0=\lambda_1$ by a [likelihood-ratio test](../../../statistical-modelling.md#likelihood-ratio-test), [score test](../../../statistical-modelling.md#score-test), or [Wald test](../../../statistical-modelling.md#wald-test); equivalently, give $D_k$ a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with mean $\lambda_kY_k$ and test the country coefficient in a [Poisson regression](../../../statistical-modelling.md#poisson-regression) with offset $\log Y_k$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
