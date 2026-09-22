# Paper 219

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20219.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20219.pdf)

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
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
  - [f](#3/f)
    - [Solution](#3/f/solution)
- [4](#4)
  - [a](#4/a)
    - [i](#4/a/i)
      - [Solution](#4/a/i/solution)
    - [ii](#4/a/ii)
      - [Solution](#4/a/ii/solution)
  - [b](#4/b)
    - [i](#4/b/i)
      - [Solution](#4/b/i/solution)
    - [ii](#4/b/ii)
      - [Solution](#4/b/ii/solution)

## 1

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

A spherical shell contributes a factor $4\pi r^2$ to the number of stars. Since $\int_0^\infty r^2e^{-r/r_0}dr=2r_0^3$, the normalized distance density is

$$
p(r_s)=\frac{r_s^2}{2r_0^3}e^{-r_s/r_0},
\qquad r_s>0.
$$

**Thus $C=(2r_0^3)^{-1}$, $\alpha=2$, and $\beta=1$. This is a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) with shape three and scale $r_0$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Ignoring terms independent of $r_0$, the [log-likelihood](../../../statistical-modelling.md#log-likelihood) is

$$
\ell(r_0)=-3N\log r_0-\frac1{r_0}\sum_{s=1}^Nr_s.
$$

Its score vanishes at

$$
\widehat r_0=\frac1{3N}\sum_{s=1}^Nr_s.
$$

The expected [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) is

$$
\mathcal I_N(r_0)=-\mathbb E\ell''(r_0)=\frac{3N}{r_0^2}.
$$

Because a shape-three gamma variable has mean $3r_0$ and variance $3r_0^2$,

$$
\mathbb E\widehat r_0=r_0,
\qquad
\operatorname{Var}(\widehat r_0)=\frac{r_0^2}{3N}.
$$

The estimator is unbiased and attains the [Cramér-Rao lower bound](../../../statistical-modelling.md#cramer-rao-bound) $\mathcal I_N(r_0)^{-1}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [inverse-square law](../../../physics.md#inverse-square-law) gives $f_s=L_0/(4\pi r_s^2)$, so a star is observed exactly when

$$
r_s\leq R=\sqrt{\frac{L_0}{4\pi f_{\min}}}.
$$

Writing $a=R/r_0$, integration of the shape-three gamma density gives

$$
\mathbb P(r_s\leq R)=1-e^{-a}\left(1+a+\frac{a^2}{2}\right).
$$

Therefore the fully normalized [truncated distribution](../../../probability-theory.md#truncated-distribution) is

$$
\boxed{p(r_s\mid I_s=1)=
\frac{r_s^2e^{-r_s/r_0}}
{2r_0^3\left[1-e^{-a}(1+a+a^2/2)\right]}
\mathbf1_{(0,R]}(r_s).}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

At distance $r_s$, detection requires $L_s\geq4\pi r_s^2f_{\min}$. Hence

$$
\mathbb P(I_s=1\mid r_s)
=1-\Phi\left(\frac{4\pi r_s^2f_{\min}-L_0}{\sigma_L}\right)
=\Phi\left(\frac{L_0-4\pi r_s^2f_{\min}}{\sigma_L}\right).
$$

The probability is $1/2$ when its normal quantile is zero, namely at

$$
\boxed{r_s=\sqrt{\frac{L_0}{4\pi f_{\min}}}.}
$$

## 2

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The likelihood is

$$
p(d\mid x)=\frac1{\sqrt{2\pi\sigma^2}}
\exp\left[-\frac{(d-x)^2}{2\sigma^2}\right].
$$

Using the conditional independence $d\perp m\mid x$ and the joint prior $p(x,m)$,

$$
p(m\mid d)=
\frac{\int p(d\mid x)p(x,m)\,dx}
{\iint p(d\mid x)p(x,m)\,dx\,dm},
$$

and

$$
\mathbb E[m\mid d]=
\frac{\iint m,p(d\mid x)p(x,m)\,dx\,dm}
{\iint p(d\mid x)p(x,m)\,dx\,dm}.
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The simulation catalog is a sample from the joint prior. [Self-normalized importance sampling](../../../probability-and-statistics.md#self-normalized-importance-sampling) therefore estimates the posterior mean by

$$
\overline m_w=\sum_{i=1}^Km_iw_i,
\qquad
w_i=\frac{p(d\mid x_i)}{\sum_{j=1}^Kp(d\mid x_j)}.
$$

The likelihood weights update each simulated system according to how well its satellite resembles the measured one.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

If equally informative independent draws have variance $s_m^2$, an ordinary mean of $K_{\mathrm{eff}}$ draws has variance $s_m^2/K_{\mathrm{eff}}$. The weighted mean has the corresponding variance $s_m^2\sum_iw_i^2$. Equating them gives the [effective sample size of importance sampling](../../../probability-and-statistics.md#effective-sample-size-of-importance-sampling)

$$
K_{\mathrm{eff}}=\frac1{\sum_{i=1}^Kw_i^2}
=\frac{\left(\sum_i p(d\mid x_i)\right)^2}
{\sum_i p(d\mid x_i)^2}\leq K,
$$

where the inequality follows from [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality).

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The stated conditional independences give

$$
p(\mathbf d\mid\mathbf x_i,m_i)=
\prod_{s=1}^{N_{\mathrm{sat}}}
\frac1{\sqrt{2\pi\sigma_s^2}}
\exp\left[-\frac{(d_s-x_{si})^2}{2\sigma_s^2}\right].
$$

Thus

$$
\widehat{\mathbb E[m\mid\mathbf d]}=\sum_{i=1}^Km_iw_i,
\qquad
w_i=\frac{\prod_s p(d_s\mid x_{si})}
{\sum_j\prod_s p(d_s\mid x_{sj})}.
$$

The dependence among satellite properties and host mass remains encoded in each jointly simulated row.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For normalized target density $p(m\mid d)$ and proposal $q$, the unbiased importance estimator $K^{-1}\sum_i m_i p(m_i\mid d)/q(m_i)$ has variance

$$
\frac1K\left[
\int\frac{m^2p(m\mid d)^2}{q(m)}\,dm
-\mathbb E[m\mid d]^2
\right].
$$

By [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\int\frac{m^2p(m\mid d)^2}{q(m)}\,dm
\geq\left(\int|m|p(m\mid d)\,dm\right)^2,
$$

with equality exactly when

$$
q^*(m)=\frac{|m|p(m\mid d)}{\int|m|p(m\mid d)\,dm}.
$$

This is rarely useful because constructing and sampling from it already requires detailed knowledge of the posterior and its absolute first moment, the objects importance sampling was meant to avoid computing.

## 3

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Stack $y=(y_1^\top,y_2^\top)^\top$. After integrating out the [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process),

$$
y\mid t,\theta\sim N_{2N}(\mu_\theta,\Sigma_\theta),
\qquad
\mu_\theta=
\begin{pmatrix}c\mathbf1\\(c+\Delta m)\mathbf1\end{pmatrix}.
$$

Writing $k(a,b)=A^2e^{-|a-b|/\tau}$, the covariance blocks are

$$
(\Sigma_{11})_{jk}=k(t_j,t_k)+\sigma_{1,j}^2\mathbf1_{\{j=k\}},
$$



$$
(\Sigma_{22})_{jk}=k(t_j-\Delta t,t_k-\Delta t)+\sigma_{2,j}^2\mathbf1_{\{j=k\}},
$$

and $(\Sigma_{12})_{jk}=k(t_j,t_k-\Delta t)$, with $\Sigma_{21}=\Sigma_{12}^\top$. Therefore

$$
\boxed{p(y_1,y_2\mid t,\theta)
=(2\pi)^{-N}|\Sigma_\theta|^{-1/2}
\exp\left[-\frac12(y-\mu_\theta)^\top
\Sigma_\theta^{-1}(y-\mu_\theta)\right].}
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

With $D=(y_1,y_2,t)$ and $\nu=(\Delta m,c,A,\tau)$,

$$
p(\theta\mid D)\propto
p(y_1,y_2\mid t,\theta)
\exp\left(-\frac{\Delta t^2}{2\sigma_{\mathrm{prior}}^2}\right)p(\nu).
$$

A [Random-walk Metropolis algorithm](../../../statistical-inference.md#random-walk-metropolis-algorithm) proposes $\theta'=\theta+Z$ from a symmetric multivariate normal increment, conveniently using logarithmic coordinates for $A,\tau>0$, and accepts with probability

$$
\min\left\{1,
\frac{p(\theta'\mid D)}{p(\theta\mid D)}
\right\}.
$$

After burn-in, retain a suitably long chain and assess convergence and [effective sample size of a Markov chain](../../../statistical-inference.md#effective-sample-size-of-a-markov-chain).

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Let $\pi$ denote the posterior and let the proposal density satisfy $q(\theta'\mid\theta)=q(\theta\mid\theta')$. For distinct states, the Metropolis transition density is

$$
P(\theta,\theta')=q(\theta'\mid\theta)
\min\{1,\pi(\theta')/\pi(\theta)\}.
$$

Consequently

$$
\pi(\theta)P(\theta,\theta')
=q(\theta'\mid\theta)\min\{\pi(\theta),\pi(\theta')\}
=\pi(\theta')P(\theta',\theta).
$$

The rejection mass on the diagonal also satisfies [detailed balance](../../../markov-process.md#detailed-balance), so the posterior is invariant.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Discard burn-in from the MCMC output and retain the sampled $\Delta t$ coordinate. A normalized histogram or [kernel density estimation](../../../nonparametric-statistics.md#kernel-density-estimation) of these draws approximates $p(\Delta t\mid D)$. Autocorrelation changes the Monte Carlo uncertainty, so uncertainty bands should use the chain's effective sample size rather than its raw length.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

The light-curve posterior used the analysis prior $\pi_0(\Delta t)=N(0,\sigma_{\mathrm{prior}}^2)$, so its marginal likelihood as a function of delay is proportional to $p(\Delta t\mid D)/\pi_0(\Delta t)$. Therefore

$$
p(H_0\mid D,M_l)\propto
\mathbf1_{[H_{0\min},H_{0\max}]}(H_0)
\int
\frac{p(\Delta t\mid D)}{\pi_0(\Delta t)}
p(\Delta t\mid H_0,M_l)\,d\Delta t.
$$

The integral can be evaluated numerically using the approximation from part (d).

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

With equal model prior probabilities, [Bayesian model averaging](../../../statistical-inference.md#bayesian-model-averaging) gives the unnormalized density

$$
p(H_0\mid D)\propto
\mathbf1_{[H_{0\min},H_{0\max}]}(H_0)
\frac1m\sum_{l=1}^m
\int
\frac{p(\Delta t\mid D)}{\pi_0(\Delta t)}
p(\Delta t\mid H_0,M_l)\,d\Delta t.
$$

Normalizing this expression over the allowed interval automatically incorporates each lens model's evidence and hence its posterior model probability.

## 4

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

[Normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
p(\theta\mid y)=N(\widetilde\theta,\sigma_\theta^2),
\qquad
\sigma_\theta^2=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2},
\qquad
\widetilde\theta=\frac{\tau^2}{\sigma^2+\tau^2}y.
$$

The three quantities in the proposed identity are

$$
\log Z=-\frac12\left[
\log(2\pi(\sigma^2+\tau^2))+
\frac{y^2}{\sigma^2+\tau^2}
\right],
$$



$$
\mathbb E_{\theta\mid y}\log L(\theta)
=-\frac12\log(2\pi\sigma^2)
-\frac{(y-\widetilde\theta)^2+\sigma_\theta^2}{2\sigma^2},
$$

and, by the [Kullback-Leibler divergence between normal distributions](../../../probability-and-statistics.md#kullback-leibler-divergence-between-normal-distributions),

$$
D_{\mathrm{KL}}(p(\theta\mid y)\Vert\pi)
=\frac12\left[
\log\frac{\tau^2}{\sigma_\theta^2}
+\frac{\sigma_\theta^2+\widetilde\theta^2}{\tau^2}-1
\right].
$$

Substitution and simplification show that the latter two expressions differ by exactly $\log Z$, so the equality holds.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

[Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives

$$
\log p(\theta\mid y)=\log L(\theta)+\log\pi(\theta)-\log Z.
$$

Taking its posterior expectation after subtracting $\log\pi(\theta)$ yields

$$
D_{\mathrm{KL}}(p(\theta\mid y)\Vert\pi)
=\mathbb E_{\theta\mid y}\log L(\theta)-\log Z.
$$

**Thus the equality holds for every proper prior and valid likelihood for which the displayed expectations are well-defined.**

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/i">i</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/i/solution">Solution</h5>

↑ **Parent:** [I](#4/b/i)

For any approximating density $q_\phi$,

$$
\begin{aligned}
\log Z
&=\mathbb E_{q_\phi}
\log\frac{L(\theta)\pi(\theta)}{q_\phi(\theta)}
+D_{\mathrm{KL}}(q_\phi\Vert p(\theta\mid y))\\
&=\operatorname{ELBO}(\phi)
+D_{\mathrm{KL}}(q_\phi\Vert p(\theta\mid y)).
\end{aligned}
$$

The [evidence lower bound](../../../statistical-inference.md#evidence-lower-bound) is therefore

$$
\operatorname{ELBO}(\phi)
=\mathbb E_{q_\phi}\log L(\theta)
-D_{\mathrm{KL}}(q_\phi\Vert\pi).
$$

Since $\log Z$ does not depend on $\phi$, maximizing the ELBO is equivalent to minimizing the divergence from $q_\phi$ to the posterior.

<h4 id="4/b/ii">ii</h4>

↑ **Parent:** [B](#4/b)

<h5 id="4/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/b/ii)

For $q_\phi=N(\mu_Q,\sigma_Q^2)$,

$$
\operatorname{ELBO}(\mu_Q,\sigma_Q^2)
=-\frac12\log(2\pi\sigma^2)
-\frac{(y-\mu_Q)^2+\sigma_Q^2}{2\sigma^2}
-\frac12\left[
\log\frac{\tau^2}{\sigma_Q^2}
+\frac{\sigma_Q^2+\mu_Q^2}{\tau^2}-1
\right].
$$

Differentiation gives

$$
\mu_Q^*=\frac{\tau^2}{\sigma^2+\tau^2}y=\widetilde\theta,
\qquad
(\sigma_Q^2)^*=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2}=\sigma_\theta^2.
$$

The Gaussian variational family contains the exact posterior, so its best member is the posterior itself and the maximized ELBO equals $\log Z$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
