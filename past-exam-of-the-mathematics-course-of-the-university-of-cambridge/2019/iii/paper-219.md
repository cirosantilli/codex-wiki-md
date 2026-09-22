# Paper 219

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_219.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2019/paper_219.pdf)

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
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)

## 1

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Let

$$
C_k=\sigma_{\mathrm{int}}^2+\sigma_{m,k}^2+\sigma_{C,k}^2,
\qquad
H_i=\sigma_{\mathrm{int}}^2+\sigma_{m,i}^2.
$$

Subtracting the measured [distance modulus](../../../astrophysics.md#distance-modulus) from the measured [apparent magnitude](../../../astrophysics.md#apparent-magnitude) gives

$$
q_k=\widehat m_k-\widehat\mu_{C,k}\sim N(M_0,C_k).
$$

For the [Hubble flow](../../../cosmology.md#hubble-flow), define

$$
r_i=\widehat m_i-25-5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s^{-1}}}\right).
$$

The [Hubble law](../../../cosmology.md#hubble-s-law), with the [Hubble constant](../../../cosmology.md#hubble-constant) parametrized by $\theta=5\log_{10}h$, gives $r_i\sim N(M_0-\theta,H_i)$. After integrating over each intrinsic [absolute magnitude](../../../astrophysics.md#absolute-magnitude) and each unobserved true distance modulus, independence therefore gives the [likelihood function](../../../statistical-modelling.md#likelihood-function)

$$
\boxed{
L(M_0,\theta)=
\prod_{k=1}^K\frac{e^{-(q_k-M_0)^2/(2C_k)}}{\sqrt{2\pi C_k}}
\prod_{i=1}^N\frac{e^{-(r_i-M_0+\theta)^2/(2H_i)}}{\sqrt{2\pi H_i}}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Put $w_k=C_k^{-1}$, $u_i=H_i^{-1}$, $A=\sum_kw_k$, $B=\sum_i u_i$, and form the [weighted means](../../../arithmetic.md#weighted-arithmetic-mean)

$$
\bar q_w=\frac{\sum_kw_kq_k}{A},
\qquad
\bar r_u=\frac{\sum_i u_ir_i}{B}.
$$

The two equations obtained from the [score function](../../../statistical-modelling.md#informant-function) are

$$
A(\bar q_w-M_0)+B(\bar r_u-M_0+\theta)=0,
\qquad
-B(\bar r_u-M_0+\theta)=0.
$$

Consequently the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator) are

$$
\boxed{\widehat M_0=\bar q_w,
\qquad \widehat\theta=\bar q_w-\bar r_u.}
$$

The [Hessian matrix](../../../calculus.md#hessian-matrix) of the log likelihood is

$$
\begin{pmatrix}-(A+B)&B\\B&-B\end{pmatrix}.
$$

Its first leading principal minor is negative and its [determinant](../../../linear-algebra.md#determinant) is $AB>0$, so it is a [negative-definite matrix](../../../linear-algebra.md#negative-definite-matrix). Thus the stationary point is the unique global maximum.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Under [homoskedasticity](../../../statistical-modelling.md#homoskedasticity), write

$$
C=\sigma_{\mathrm{int}}^2+\sigma_m^2+\sigma_C^2,
\qquad H=\sigma_{\mathrm{int}}^2+\sigma_m^2.
$$

Then $\widehat M_0=\bar q$ and $\widehat\theta=\bar q-\bar r$. Both are [unbiased estimators](../../../statistical-modelling.md#unbiased-estimator), and their [covariance matrix](../../../variance.md#covariance-matrix) is

$$
\boxed{
\operatorname{Cov}\begin{pmatrix}\widehat M_0\\\widehat\theta\end{pmatrix}
=\begin{pmatrix}
C/K&C/K\\
C/K&C/K+H/N
\end{pmatrix}.}
$$

Indeed the [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) is

$$
I(M_0,\theta)=
\begin{pmatrix}K/C+N/H&-N/H\\-N/H&N/H\end{pmatrix},
$$

and its inverse is exactly the displayed covariance matrix. The estimators therefore attain the multivariate [Cramér-Rao bound](../../../statistical-modelling.md#cramer-rao-bound) and are [efficient estimators](../../../statistical-modelling.md#efficient-estimator).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

By the [invariance property of maximum likelihood estimation](../../../statistical-modelling.md#invariance-property-of-maximum-likelihood-estimation),

$$
\boxed{\widehat h=10^{\widehat\theta/5}=e^{\widehat\theta/\alpha}.}
$$

The [sampling distribution](../../../statistical-modelling.md#sampling-distribution) is $\widehat\theta\sim N(\theta,\sigma_{\widehat\theta}^2)$, where

$$
\sigma_{\widehat\theta}^2=C/K+H/N,
$$

$\widehat h$ has a [log-normal distribution](../../../probability-theory.md#log-normal-distribution) with

$$
\log\widehat h\sim N\!\left(\log h,
\frac{\sigma_{\widehat\theta}^2}{\alpha^2}\right).
$$

Writing $v=\sigma_{\widehat\theta}^2/\alpha^2$, its exact fractional bias and variance are

$$
\frac{\mathbb E\widehat h-h}{h}=e^{v/2}-1,
\qquad
\frac{\operatorname{Var}(\widehat h)}{h^2}=e^v(e^v-1).
$$

Hence, to leading order,

$$
\boxed{\frac{\mathbb E\widehat h-h}{h}\simeq
\frac{\sigma_{\widehat\theta}^2}{2\alpha^2},
\qquad
\frac{\operatorname{Var}(\widehat h)}{h^2}\simeq
\frac{\sigma_{\widehat\theta}^2}{\alpha^2}.}
$$

## 2

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The measurement model has the [Gaussian likelihood](../../../statistical-modelling.md#gaussian-likelihood)

$$
P(d\mid x)=\frac1{\sqrt{2\pi\sigma^2}}
\exp\!\left[-\frac{(d-x)^2}{2\sigma^2}\right].
$$

Marginalizing the latent angular momentum gives the normalized [posterior distribution](../../../statistical-inference.md#bayesian-posterior)

$$
\boxed{P(m\mid d)=
\frac{\int P(d\mid x)P(x,m)\,dx}
{\iint P(d\mid x)P(x,m)\,dx\,dm}.}
$$

Its [posterior mean](../../../statistical-inference.md#posterior-mean) is

$$
\boxed{\bar m=\frac{\iint mP(d\mid x)P(x,m)\,dx\,dm}
{\iint P(d\mid x)P(x,m)\,dx\,dm}.}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Treat the simulated pairs $(x_i,m_i)$ as samples from the prior $P(x,m)$. The numerator and denominator of the posterior mean are then ordinary [Monte Carlo estimators](../../../probability-and-statistics.md#monte-carlo-estimator), so

$$
\bar m\simeq\frac{\sum_{i=1}^Km_iP(d\mid x_i)}
{\sum_{j=1}^KP(d\mid x_j)}
=\sum_{i=1}^Km_iw_i,
$$

where the normalized [importance sampling](../../../probability-and-statistics.md#importance-sampling) weights are

$$
\boxed{w_i=\frac{\exp[-(d-x_i)^2/(2\sigma^2)]}
{\sum_{j=1}^K\exp[-(d-x_j)^2/(2\sigma^2)]}.}
$$

The common Gaussian normalizing constant cancels.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For arbitrary nonnegative raw weights $W_i$, let $\bar W=K^{-1}\sum_iW_i$. The empirical squared [coefficient of variation](../../../variance.md#coefficient-of-variation), using variance divisor $K$, is

$$
\widehat{\operatorname{CV}}^2(W)
=\frac{K^{-1}\sum_i(W_i-\bar W)^2}{\bar W^2}
=\frac{K\sum_iW_i^2}{(\sum_iW_i)^2}-1.
$$

Substitution into the stated definition gives the usual [effective sample size of importance sampling](../../../probability-and-statistics.md#effective-sample-size-of-importance-sampling)

$$
\boxed{\widehat{\operatorname{ESS}}
=\frac{(\sum_iW_i)^2}{\sum_iW_i^2}.}
$$

For normalized weights $w_i=W_i/\sum_jW_j$, this reduces to $\boxed{\widehat{\operatorname{ESS}}=1/\sum_iw_i^2}$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

[Conditional independence](../../../random-variable.md#conditional-independence) gives

$$
P(m\mid d_1,\ldots,d_S)
\propto P(m)\prod_{s=1}^SP(d_s\mid m),
\qquad S=N_{\rm sat}.
$$

For each satellite, [Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives $P(d_s\mid m)\propto P(m\mid d_s)/P(m)$. Therefore

$$
P(m\mid\mathbf d)\propto
P(m)^{1-S}\prod_{s=1}^SP(m\mid d_s).
$$

If $\widehat p_0(m)$ is a [kernel density estimator](../../../nonparametric-statistics.md#kernel-density-estimation) for the simulated marginal masses and $\widehat p_s(m)$ estimates the posterior based on satellite $s$, then

$$
\boxed{
\widehat{\bar m}=
\frac{\int m\,\widehat p_0(m)^{1-S}
\prod_{s=1}^S\widehat p_s(m)\,dm}
{\int \widehat p_0(m)^{1-S}
\prod_{s=1}^S\widehat p_s(m)\,dm}.}
$$

The one-dimensional integrals can be evaluated by [numerical integration](../../../numerical-analysis.md#numerical-integration) on a common mass grid.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Let $p(m)=P(m\mid\mathbf d)$ and draw independently from an importance density $q$. The unbiased estimator

$$
\widehat I=\frac1n\sum_{j=1}^n\frac{m_jp(m_j)}{q(m_j)}
$$

of $I=\int mp(m)\,dm$ has one-sample second moment

$$
\int\frac{m^2p(m)^2}{q(m)}\,dm.
$$

By the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality),

$$
\left(\int |m|p(m)\,dm\right)^2
\leq
\left(\int\frac{m^2p(m)^2}{q(m)}\,dm\right)
\left(\int q(m)\,dm\right).
$$

Equality holds precisely when $q(m)\propto|m|p(m)$, giving the [optimal importance density for a single integral](../../../probability-and-statistics.md#optimal-importance-density-for-a-single-integral)

$$
\boxed{q^*(m)=\frac{|m|p(m)}{\int|u|p(u)\,du}.}
$$

This is circular in practice: constructing and normalizing $q^*$ requires detailed knowledge of the posterior and the expectation of $|m|$. Here log masses are positive, so the unknown normalizer is the posterior mean being estimated. It is also optimal only for this one integral, not for general posterior summaries.

## 3

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Stack the observations as $y=(y_1^T,y_2^T)^T$ and set

$$
\mu_\theta=
\begin{pmatrix}c\mathbf1\\(c+\Delta m)\mathbf1\end{pmatrix}.
$$

Let $K_f(a,b)$ and $K_g(a,b)$ denote matrices obtained by evaluating the two [Gaussian process](../../../stochastic-process.md#gaussian-process) [covariance kernels](../../../random-variable.md#covariance-kernel). Independence of the [quasar light curve](../../../astrophysics.md#quasar-light-curve), [gravitational microlensing](../../../general-relativity.md#gravitational-microlensing), and [Gaussian noise](../../../probability-theory.md#gaussian-noise) processes gives

$$
C_\theta=
\begin{pmatrix}
K_f(t,t)+K_g(t,t)+E_1&K_f(t,t-\Delta t)\\
K_f(t-\Delta t,t)&K_f(t-\Delta t,t-\Delta t)+K_g(t,t)+E_2
\end{pmatrix},
$$

where $E_i=\operatorname{diag}(\sigma_{i,1}^2,\ldots,\sigma_{i,N}^2)$. Thus $y\mid\theta$ is a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) and its [Gaussian-process marginal likelihood](../../../stochastic-process.md#gaussian-process-marginal-likelihood) is

$$
\boxed{p(y_1,y_2\mid\theta)
=(2\pi)^{-N}|C_\theta|^{-1/2}
\exp\!\left[-\frac12(y-\mu_\theta)^TC_\theta^{-1}(y-\mu_\theta)\right].}
$$

The off-diagonal blocks are essential: both images contain the same delayed [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

At the fitted parameters, let $C=C_{\widehat\theta}$ and $\mu=\mu_{\widehat\theta}$. For prediction times $t_*$ define

$$
K_{**}=K_f(t_*,t_*),
\qquad
K_{*y}=\begin{pmatrix}K_f(t_*,t)&K_f(t_*,t-\widehat{\Delta t})\end{pmatrix}.
$$

The microlensing processes and measurement errors contribute no cross-covariance with the latent quasar light curve. The [Gaussian process regression posterior](../../../probability-and-statistics.md#gaussian-process-regression-posterior) is therefore

$$
\boxed{\mathbb E[f_*\mid y]=c\mathbf1+K_{*y}C^{-1}(y-\mu),}
$$



$$
\boxed{\operatorname{Cov}(f_*\mid y)
=K_{**}-K_{*y}C^{-1}K_{y*}.}
$$

The requested pointwise posterior variances are the diagonal entries of the latter matrix.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use broad proper uniform priors for $\Delta t$, $\Delta m$, and $c$ over physically plausible ranges, and broad log-uniform priors for the positive scales $A_f$ and $\tau_f$. Then

$$
\boxed{p(\theta\mid y_1,y_2)\propto
p(y_1,y_2\mid\theta)\,p(\Delta t)p(\Delta m)p(c)p(A_f)p(\tau_f).}
$$

A [Random-walk Metropolis algorithm](../../../statistical-inference.md#random-walk-metropolis-algorithm) can update $(\Delta t,\Delta m,c,\log A_f,\log\tau_f)$ with a multivariate Gaussian [proposal distribution](../../../statistical-inference.md#proposal-distribution). Initialize several dispersed chains near plausible cross-correlation delays and near the marginal-likelihood optimum; reject proposals outside the prior bounds; discard warm-up while adapting only the proposal scale and covariance; then freeze the kernel and retain a long run. Evaluate trace plots, [autocorrelations](../../../time-series.md#autocorrelation), acceptance rates, between-chain agreement, and the [effective sample size of a Markov chain](../../../statistical-inference.md#effective-sample-size-of-a-markov-chain). Posterior predictive [quasar light curves](../../../astrophysics.md#quasar-light-curve) provide a model check.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Write the target posterior density as $\pi(\theta)$ and the [proposal distribution](../../../statistical-inference.md#proposal-distribution) density as $q(\theta'\mid\theta)$. The [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm) accepts a proposed move with

$$
a(\theta,\theta')=
\min\!\left\{1,
\frac{\pi(\theta')q(\theta\mid\theta')}
{\pi(\theta)q(\theta'\mid\theta)}\right\}.
$$

For distinct states,

$$
\pi(\theta)q(\theta'\mid\theta)a(\theta,\theta')
=\min\{\pi(\theta)q(\theta'\mid\theta),
\pi(\theta')q(\theta\mid\theta')\},
$$

which is symmetric in $\theta$ and $\theta'$. The rejection probability supplies the diagonal part, so the entire transition kernel satisfies [detailed balance](../../../markov-process.md#detailed-balance). Integrating the detailed-balance identity over the starting state proves $\int\pi(\theta)P(\theta,d\theta')=\pi(\theta')d\theta'$. Hence the posterior is a [stationary distribution](../../../markov-process.md#stationary-distribution); an [irreducible Markov chain](../../../markov-process.md#irreducible-markov-chain) that is also an [aperiodic Markov chain](../../../markov-process.md#aperiodic-markov-chain) converges uniquely to it.

## 4

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

For one object, the [probabilistic graphical model](../../../statistical-model.md#probabilistic-graphical-model) factorization is

$$
\boxed{
p(x_i,y_i,\xi_i,\eta_i\mid\alpha,\beta,\sigma^2,\mu,\tau^2)
=p(x_i\mid\xi_i)p(y_i\mid\eta_i)
p(\eta_i\mid\xi_i,\alpha,\beta,\sigma^2)
p(\xi_i\mid\mu,\tau^2).}
$$

Each factor is the [normal distribution](../../../probability-theory.md#normal-distribution) density specified by the model. This factorization displays the [conditional independences](../../../random-variable.md#conditional-independence) of the [latent variables](../../../statistical-modelling.md#latent-variable) $\xi_i,\eta_i$ and the noisy observations $x_i,y_i$.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

With the stated flat priors, the full joint density, up to a constant, is

$$
\boxed{
\mathbf1_{\{\sigma^2>0,\tau^2>0\}}
\prod_{i=1}^N
N(x_i\mid\xi_i,\sigma_{x,i}^2)
N(y_i\mid\eta_i,\sigma_{y,i}^2)
N(\eta_i\mid\alpha+\beta\xi_i,\sigma^2)
N(\xi_i\mid\mu,\tau^2).}
$$

The priors on $\alpha,\beta,$ and $\mu$ contribute constants on $\mathbb R$, while those on the two variances contribute constants on $(0,\infty)$. These are [improper priors](../../../statistical-inference.md#improper-prior), so posterior propriety must be checked; the full-rank, sufficiently large-data case used below is proper.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For each $i$, place $\xi_i$ and $\eta_i$ inside a plate replicated $N$ times. The directed edges are represented by

$$
(\mu,\tau^2)\longrightarrow\xi_i\longrightarrow x_i,
\qquad
(\alpha,\beta,\sigma^2,\xi_i)\longrightarrow\eta_i\longrightarrow y_i.
$$

The shaded observed nodes are $x_i,y_i$; the unshaded nodes $\xi_i,\eta_i$ are latent; and $\alpha,\beta,\sigma^2,\mu,\tau^2$ lie outside the plate. This is the [probabilistic graphical model](../../../statistical-model.md#probabilistic-graphical-model) encoded by the joint factorization.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Every move can be drawn from a [full conditional distribution](../../../probability-theory.md#full-conditional-distribution), producing a [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) with acceptance probability one. Write $s_{x,i}^2=\sigma_{x,i}^2$ and $s_{y,i}^2=\sigma_{y,i}^2$. First update independently

$$
\xi_i\mid-\sim N\!\left(
V_{\xi i}\left[\frac\mu{\tau^2}+\frac{\beta(\eta_i-\alpha)}{\sigma^2}+\frac{x_i}{s_{x,i}^2}\right],V_{\xi i}\right),
\quad
V_{\xi i}^{-1}=\frac1{\tau^2}+\frac{\beta^2}{\sigma^2}+\frac1{s_{x,i}^2},
$$

and then

$$
\eta_i\mid-\sim N\!\left(
V_{\eta i}\left[\frac{\alpha+\beta\xi_i}{\sigma^2}+\frac{y_i}{s_{y,i}^2}\right],V_{\eta i}\right),
\quad
V_{\eta i}^{-1}=\frac1{\sigma^2}+\frac1{s_{y,i}^2}.
$$

Let $X$ have rows $(1,\xi_i)$ and $\eta=(\eta_i)$. Update the [linear regression](../../../linear-regression.md) coefficients jointly by

$$
\begin{pmatrix}\alpha\\\beta\end{pmatrix}\Bigm|-
\sim N_2\!\left((X^TX)^{-1}X^T\eta,
\sigma^2(X^TX)^{-1}\right),
$$

and update

$$
\mu\mid-\sim N\!\left(\bar\xi,\frac{\tau^2}{N}\right).
$$

Finally, the flat positive variance priors give the following full conditionals, each an [inverse-gamma distribution](../../../continuous-probability-distribution.md#inverse-gamma-distribution):

$$
\sigma^2\mid-\sim\operatorname{InvGamma}\!\left(\frac N2-1,
\frac12\sum_i(\eta_i-\alpha-\beta\xi_i)^2\right),
$$



$$
\tau^2\mid-\sim\operatorname{InvGamma}\!\left(\frac N2-1,
\frac12\sum_i(\xi_i-\mu)^2\right).
$$

A systematic sweep in the displayed order, using the newly sampled values immediately, defines the chain. The shapes are positive for $N>2$; full column rank of $X$ is also required.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2019](../../2019.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
