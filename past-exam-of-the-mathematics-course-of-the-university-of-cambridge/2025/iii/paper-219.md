# Paper 219

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_219.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2025/III_Paper_219.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An apparent magnitude is the sum of absolute magnitude and [distance modulus](../../../astrophysics.md#distance-modulus). Thus

$$
\bar m_{\mathrm{LMC}}
\sim N\!\left(M_0^*+\mu_{\mathrm{LMC}},
\frac{\sigma_*^2}{N_{\mathrm{LMC}}}\right).
$$

The independent unbiased distance-modulus estimate is $N(\mu_{\mathrm{LMC}},\sigma_{\mathrm{LMC}}^2)$, so closure of independent [normal distributions](../../../probability-theory.md#normal-distribution) under linear combinations gives

$$
\widehat S_1\sim N(M_0^*,V_1),
\qquad
V_1=\frac{\sigma_*^2}{N_{\mathrm{LMC}}}+\sigma_{\mathrm{LMC}}^2.
$$

**Hence $\mathbb E\widehat S_1=M_0^*$ and $\operatorname{Var}(\widehat S_1)=V_1$.**

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The common distance modulus of calibrator galaxy $g$ cancels between its supernova and mean Cepheid apparent magnitudes. Their independent intrinsic scatters therefore give

$$
\widehat S_2^g\sim N(\Delta M,V_2),
\qquad
\Delta M=M_0^{\mathrm{SN}}-M_0^*,
\qquad
V_2=\sigma_{\mathrm{SN}}^2+\frac{\sigma_*^2}{N_{\mathrm{Ceph}}}.
$$

**Thus $\mathbb E\widehat S_2^g=\Delta M$ and $\operatorname{Var}(\widehat S_2^g)=V_2$.**

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The [Hubble law](../../../cosmology.md#hubble-s-law) gives $d_i=cz_i/(100h)$ Mpc, so its distance modulus is

$$
25+5\log_{10}\frac{cz_i}{100h}
=f(z_i)-5\log_{10}h=f(z_i)-\theta.
$$

Consequently

$$
\boxed{\widehat S_3^i=m_{\mathrm{SN}}^i-f(z_i)
=M_i^{\mathrm{SN}}-\theta
\sim N(\mathcal M,\sigma_{\mathrm{SN}}^2),
\qquad
\mathcal M=M_0^{\mathrm{SN}}-\theta.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

All three sets of statistics are independent. With $s_1=\widehat S_1$, $s_{2g}=\widehat S_2^g$, and $s_{3i}=\widehat S_3^i$, their [likelihood function](../../../statistical-modelling.md#likelihood-function), up to a parameter-independent factor, is

$$
\boxed{L(M_0^*,\Delta M,\mathcal M)
\propto
\exp\!\left[-\frac{(s_1-M_0^*)^2}{2V_1}
-\sum_{g=1}^G\frac{(s_{2g}-\Delta M)^2}{2V_2}
-\sum_{i=1}^{N_{\mathrm{SN}}}\frac{(s_{3i}-\mathcal M)^2}{2\sigma_{\mathrm{SN}}^2}
\right].}
$$

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Differentiating the log-likelihood gives the unique stationary point

$$
\widehat M_0^*=s_1,
\qquad
\widehat{\Delta M}=\frac1G\sum_gs_{2g},
\qquad
\widehat{\mathcal M}=\frac1{N_{\mathrm{SN}}}\sum_is_{3i}.
$$

Its Hessian is diagonal with entries $-1/V_1$, $-G/V_2$, and $-N_{\mathrm{SN}}/\sigma_{\mathrm{SN}}^2$, so it is the unique maximum. The estimators are unbiased and have variances

$$
V_1,
\qquad
\frac{V_2}{G},
\qquad
\frac{\sigma_{\mathrm{SN}}^2}{N_{\mathrm{SN}}},
$$

which equal their [Cramér-Rao lower bounds](../../../statistical-modelling.md#cramer-rao-bound) because the normal location statistics are efficient.

Since $\theta=M_0^*+\Delta M-\mathcal M$, invariance of the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) gives

$$
\widehat\theta=\widehat M_0^*+\widehat{\Delta M}-\widehat{\mathcal M}.
$$

It is unbiased and normal with variance

$$
\boxed{\sigma_\theta^2
=V_1+\frac{V_2}{G}
+\frac{\sigma_{\mathrm{SN}}^2}{N_{\mathrm{SN}}}.}
$$

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

By invariance of maximum likelihood,

$$
\widehat h=10^{\widehat\theta/5}
=\exp(\widehat\theta/\alpha).
$$

Because $\widehat\theta-\theta\sim N(0,\sigma_\theta^2)$, the ratio $\widehat h/h$ is [log-normal](../../../probability-theory.md#log-normal-distribution). Its exact variance is

$$
\operatorname{Var}\!\left(\frac{\widehat h}{h}\right)
=e^{\sigma_\theta^2/\alpha^2}
\left(e^{\sigma_\theta^2/\alpha^2}-1\right)
=\frac{\sigma_\theta^2}{\alpha^2}+O(\sigma_\theta^4).
$$

As $N_{\mathrm{SN}},G,N_{\mathrm{LMC}}\to\infty$, all sampling terms vanish but $V_1$ retains $\sigma_{\mathrm{LMC}}^2$. The dominant remaining uncertainty is therefore the parallax calibration of the LMC distance modulus.

## 2

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Writing $\varphi(u;m,v)$ for the $N(m,v)$ density, the conditional-independence structure of the [latent-variable model](../../../statistical-modelling.md#latent-variable-model) gives

$$
\boxed{p(y_i,x_i,\eta_i,\xi_i\mid\alpha,\beta,\sigma^2,\mu,\tau^2)
=\varphi(\xi_i;\mu,\tau^2)
\varphi(\eta_i;\alpha+\beta\xi_i,\sigma^2)
\varphi(x_i;\xi_i,\sigma_x^2)
\varphi(y_i;\eta_i,\sigma_y^2).}
$$

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

First integrate out $\eta_i$: conditional on $\xi_i$, $y_i\sim N(\alpha+\beta\xi_i,s^2)$ with $s^2=\sigma^2+\sigma_y^2$. Since $(x_i,y_i)$ is an affine transformation of independent normal variables, it is [bivariate normal](../../../probability-and-statistics.md#multivariate-normal-distribution) with mean

$$
m=\binom{\mu}{\alpha+\beta\mu}
$$

and covariance

$$
\Sigma=
\begin{pmatrix}
A&B\\B&C
\end{pmatrix},
\quad
A=\tau^2+\sigma_x^2,
\quad B=\beta\tau^2,
\quad C=\beta^2\tau^2+s^2.
$$

Its determinant simplifies to

$$
D=AC-B^2=(\tau^2+\sigma_x^2)s^2+\beta^2\tau^2\sigma_x^2.
$$

For $r_i=(x_i-\mu,y_i-\alpha-\beta\mu)^T$, the observed-data likelihood is therefore

$$
L=(2\pi)^{-N}D^{-N/2}
\exp\!\left[-\frac12\sum_{i=1}^N
r_i^T\Sigma^{-1}r_i\right],
\qquad
\Sigma^{-1}=\frac1D\begin{pmatrix}C&-B\\-B&A\end{pmatrix}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Take flat priors on $\alpha,\beta,\mu$ and scale priors $\pi(\sigma^2,\tau^2)\propto(\sigma^2\tau^2)^{-1}$ on the positive variances. The [posterior distribution](../../../statistical-inference.md#bayesian-posterior) is then

$$
\pi(\alpha,\beta,\sigma^2,\mu,\tau^2\mid\mathcal D)
\propto\frac{L(\alpha,\beta,\sigma^2,\mu,\tau^2)}{\sigma^2\tau^2}.
$$

A random-walk [Metropolis–Hastings algorithm](../../../statistical-inference.md#metropolis-hastings-algorithm) can update $(\alpha,\beta,\mu,\log\sigma^2,\log\tau^2)$ with a symmetric proposal and accept a proposed state $z'$ from $z$ with probability $1\wedge\pi(z'\mid\mathcal D)/\pi(z\mid\mathcal D)$, including the Jacobian if the target is represented in transformed coordinates. Its transition kernel satisfies

$$
\pi(z)q(z,z')a(z,z')
=\min\{\pi(z)q(z,z'),\pi(z')q(z',z)\}
=\pi(z')q(z',z)a(z',z),
$$

which is [detailed balance](../../../markov-process.md#detailed-balance); hence the posterior is stationary.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The marginal predictor density is

$$
x_i\sim N(\mu,A),
\qquad A=\tau^2+\sigma_x^2.
$$

[Gaussian conditional expectation](../../../statistical-modelling.md#gaussian-conditional-expectation) gives

$$
\xi_i\mid x_i\sim N\!\left(
\mu+\kappa(x_i-mu),v\right),
\qquad
\kappa=\frac{\tau^2}{A},
\qquad
v=\frac{\tau^2\sigma_x^2}{A}.
$$

Integrating this conditional distribution through the response model yields

$$
y_i\mid x_i\sim N\!\left(
\alpha+\beta[\mu+\kappa(x_i-mu)],
s^2+\beta^2v\right).
$$

When $\tau\gg\sigma_x$, $\kappa\to1$, $v\to\sigma_x^2$, and $A\sim\tau^2$. Hence

$$
L\simeq L_1(\alpha,\beta,\sigma^2)L_2(\mu,\tau^2),
$$

where

$$
L_1=\prod_i\varphi\!\left(y_i;\alpha+\beta x_i,
\sigma^2+\sigma_y^2+\beta^2\sigma_x^2\right),
\qquad
L_2=\prod_i\varphi(x_i;\mu,\tau^2).
$$

The approximate maximum-likelihood estimators are

$$
\boxed{\widehat\mu=\bar x,
\qquad
\widehat{\tau^2}=\frac1N\sum_i(x_i-\bar x)^2.}
$$

## 3

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Put $\rho=e^{-\Delta t/\tau}=e^{-x}$ and retain $R=k(0,0)$, which equals one for the stated [exponential covariance function](../../../stochastic-process.md#exponential-covariance-function). The covariance matrix of $(y_1,y_2,y_3)$ is

$$
R\begin{pmatrix}1&\rho&\rho^2\\\rho&1&\rho\\\rho^2&\rho&1\end{pmatrix}.
$$

Conditioning a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) and simplifying gives

$$
y_3\mid y_1,y_2
\sim N\!\left(\mu+\rho(y_2-mu),R(1-\rho^2)\right).
$$

The absence of $y_1$ from both conditional moments shows that $y_3$ and $y_1$ are conditionally independent given $y_2$. Equivalently, the exponential-kernel [Gaussian process](../../../stochastic-process.md#gaussian-process) is the stationary [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process), which is Markov.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

As $\Delta t/\tau\to\infty$, $\rho\to0$. Therefore the posterior predictive mean tends to $\mu$ and its variance tends to $R$: a sufficiently distant observation has reverted to the stationary prior distribution.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

The Markov factorization is

$$
p(\mathbf y\mid\mathbf t,\mu,\tau)
=\varphi(y_1;\mu,R)
\prod_{j=2}^3
\varphi\!\left(y_j;\mu+\rho(y_{j-1}-\mu),R(1-\rho^2)\right).
$$

Differentiating its log-likelihood with respect to $\mu$ gives

$$
\widehat\mu
=\frac{y_1+(1-\rho)y_2+y_3}{3-\rho}.
$$

Its coefficients sum to one, so it is unbiased. Direct covariance calculation, equivalently inversion of its [Fisher information](../../../statistical-modelling.md#fisher-information-matrix), gives

$$
\operatorname{Var}(\widehat\mu)
=R\frac{1+\rho}{3-\rho}.
$$

**Thus the variance tends to $R$ as $\Delta t/\tau\to0$, because the observations become perfectly correlated, and to $R/3$ as $\Delta t/\tau\to\infty$, because they become three independent draws.**

## 4

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

One simple algorithm is [importance sampling](../../../probability-and-statistics.md#importance-sampling) from the prior. Draw $(\theta_j,\boldsymbol\alpha_j)$ independently from $\pi(\theta)\pi(\boldsymbol\alpha)$ and assign weight $w_j=L_A(\theta_j,\boldsymbol\alpha_j)$. Then

$$
\widehat{\mathcal Z}_A=\frac1J\sum_{j=1}^Jw_j
$$

estimates the [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence), and the normalized weights $w_j/\sum_kw_k$ represent the posterior. A weighted histogram or [kernel density estimation](../../../nonparametric-statistics.md#kernel-density-estimation) of the $\theta_j$ estimates the marginal $\mathcal P_A(\theta)$; discarding $\boldsymbol\alpha_j$ performs the marginalization.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Independence of the experiments gives

$$
\mathcal P_{AB}(\theta,\boldsymbol\alpha,\boldsymbol\beta)
=\frac{L_A(\theta,\boldsymbol\alpha)L_B(\theta,\boldsymbol\beta)
\pi(\theta)\pi(\boldsymbol\alpha)\pi(\boldsymbol\beta)}
{\mathcal Z_{AB}},
$$

where

$$
\mathcal Z_{AB}=\iiint
L_AL_B\pi(\theta)\pi(\boldsymbol\alpha)\pi(\boldsymbol\beta)
\,d\theta\,d\boldsymbol\alpha\,d\boldsymbol\beta.
$$

The marginal posterior is obtained by integrating the displayed joint posterior over both nuisance-parameter vectors.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Define the prior-predictive nuisance integrals

$$
f_A(\theta)=\int L_A(\theta,\boldsymbol\alpha)
\pi(\boldsymbol\alpha)\,d\boldsymbol\alpha,
\qquad
f_B(\theta)=\int L_B(\theta,\boldsymbol\beta)
\pi(\boldsymbol\beta)\,d\boldsymbol\beta.
$$

Then

$$
\mathcal P_{AB}(\theta)\mathcal Z_{AB}
=f_A(\theta)f_B(\theta)\pi(\theta).
$$

For each individual analysis, [Bayes' theorem](../../../probability-theory.md#bayes-theorem) also gives

$$
\boxed{f_A(\theta)=\frac{\mathcal Z_A\mathcal P_A(\theta)}{\pi(\theta)},
\qquad
f_B(\theta)=\frac{\mathcal Z_B\mathcal P_B(\theta)}{\pi(\theta)}.}
$$

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Estimate each one-dimensional marginal posterior from its individual experiment's weighted samples, for example by weighted [kernel density estimation](../../../nonparametric-statistics.md#kernel-density-estimation). Combining that density estimate with the individual evidence estimate gives

$$
\widehat f_A(\theta)
=\frac{\widehat{\mathcal Z}_A\widehat{\mathcal P}_A(\theta)}{\pi(\theta)},
\qquad
\widehat f_B(\theta)
=\frac{\widehat{\mathcal Z}_B\widehat{\mathcal P}_B(\theta)}{\pi(\theta)}.
$$

Their product with $\pi(\theta)$ can be normalized on the one-dimensional $\theta$ space, avoiding all joint nuisance-parameter sampling.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Compute the joint evidence by one-dimensional numerical integration,

$$
\mathcal Z_{AB}=\int f_A(\theta)f_B(\theta)\pi(\theta)\,d\theta.
$$

Equivalently, the individual outputs give

$$
\mathcal Z_{AB}
=\mathcal Z_A\mathcal Z_B
\int\frac{\mathcal P_A(\theta)\mathcal P_B(\theta)}{\pi(\theta)}\,d\theta.
$$

Quadrature or one-dimensional [importance sampling](../../../probability-and-statistics.md#importance-sampling) evaluates this integral without entering the $(\theta,\boldsymbol\alpha,\boldsymbol\beta)$ space.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2025](../../2025.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
