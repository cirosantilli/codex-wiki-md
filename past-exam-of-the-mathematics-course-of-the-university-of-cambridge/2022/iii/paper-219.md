# Paper 219

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_219.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2022/paper_219.pdf)

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
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
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

## 1

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For distinct [sibling supernovae](../../../stellar-astrophysics.md#type-ia-supernova) $s$ and $s'$ in the same galaxy, the shared fluctuation is the only common random term. Independence and [linearity of covariance](../../../variance.md#linearity-of-covariance) therefore give

$$
\operatorname{Cov}(M_s,M_{s'})=\sigma_G^2,
\qquad
\operatorname{Var}(M_s)=\sigma_G^2+\sigma_I^2
\equiv\sigma_{\rm tot}^2.
$$

Their [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) is

$$
\operatorname{Corr}(M_s,M_{s'})
=\frac{\sigma_G^2}{\sigma_G^2+\sigma_I^2}.
$$

This is the [intraclass correlation coefficient](../../../variance.md#intraclass-correlation-coefficient) of the galaxy-level [random intercept](../../../statistical-modelling.md#random-intercept) model.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Write the [Cepheid](../../../stellar-astrophysics.md#cepheid-variable) measurement as $\widehat\mu=\mu+\epsilon_\mu$, where $\epsilon_\mu\sim N(0,\sigma_\mu^2)$, and define the calibrated [absolute magnitude](../../../astrophysics.md#absolute-magnitude) data

$$
q_k=m_k-\widehat\mu
=M_0+\Delta M_G+\delta M_k-\epsilon_\mu.
$$

Thus $q=(q_1,\ldots,q_K)^T$ has a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) with mean $M_0\mathbf1$ and [covariance matrix](../../../variance.md#covariance-matrix)

$$
C=\sigma_I^2I_K+(\sigma_G^2+\sigma_\mu^2)\mathbf1\mathbf1^T.
$$

The [Hubble law](../../../cosmology.md#hubble-s-law) and the definition of [distance modulus](../../../astrophysics.md#distance-modulus) give

$$
m_i=M_i+25+5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s}^{-1}}\right)-\theta.
$$

Consequently, with

$$
x_i=m_i-25-5\log_{10}\!\left(\frac{cz_i}{100\ {\rm km\,s}^{-1}}\right),
$$

the Hubble-flow observations are [independent random variables](../../../random-variable.md#independent-random-variables) satisfying $x_i\sim N(M_0-\theta,\sigma_{\rm tot}^2)$. Apart from a factor independent of the parameters, the joint [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
L(M_0,\theta)
\propto |C|^{-1/2}
\exp\!\left[-\frac12(q-M_0\mathbf1)^TC^{-1}(q-M_0\mathbf1)\right]
(\sigma_{\rm tot}^2)^{-N/2}
\exp\!\left[-\frac1{2\sigma_{\rm tot}^2}
\sum_{i=1}^N\{x_i-(M_0-\theta)\}^2\right].
$$

The expression extends by continuity to a singular limiting covariance such as $\sigma_I=0$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Let

$$
\bar q=\frac1K\sum_{k=1}^Kq_k,
\qquad
\bar x=\frac1N\sum_{i=1}^Nx_i,
$$

and set

$$
A=\operatorname{Var}(\bar q)
=\sigma_\mu^2+\sigma_G^2+\frac{\sigma_I^2}{K},
\qquad
B=\operatorname{Var}(\bar x)
=\frac{\sigma_{\rm tot}^2}{N}.
$$

The within-galaxy contrasts $q_k-\bar q$ contain no $M_0$, so the parameter-dependent [log-likelihood](../../../statistical-modelling.md#log-likelihood) reduces to

$$
\ell(M_0,\theta)
=-\frac{(\bar q-M_0)^2}{2A}
-\frac{\{\bar x-(M_0-\theta)\}^2}{2B}+\text{constant}.
$$

The [score equations](../../../statistical-modelling.md#score-equation) give the [maximum-likelihood estimators](../../../statistical-modelling.md#maximum-likelihood-estimator)

$$
\widehat M_0=\bar q,
\qquad
\widehat\theta=\bar q-\bar x.
$$

The calibrator and Hubble-flow samples are independent, so both estimators are [unbiased](../../../statistical-modelling.md#unbiased-estimator) and

$$
\operatorname{Var}(\widehat M_0)=A,
\qquad
\operatorname{Var}(\widehat\theta)=A+B.
$$

The [Fisher information matrix](../../../statistical-modelling.md#fisher-information-matrix) for $(M_0,\theta)$ is

$$
\mathcal I=
\begin{pmatrix}
A^{-1}+B^{-1}&-B^{-1}\\
-B^{-1}&B^{-1}
\end{pmatrix},
\qquad
\mathcal I^{-1}=
\begin{pmatrix}
A&A\\
A&A+B
\end{pmatrix}.
$$

**Hence $\operatorname{Var}(\widehat\theta)=(\mathcal I^{-1})_{22}$: $\widehat\theta$ attains the multiparameter [Cramér-Rao bound](../../../statistical-modelling.md#cramer-rao-bound).**

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

The [invariance property of maximum likelihood estimation](../../../statistical-modelling.md#invariance-property-of-maximum-likelihood-estimation) gives

$$
\widehat h=10^{\widehat\theta/5}
=\exp(\widehat\theta/\alpha).
$$

Since $\widehat\theta-\theta\sim N(0,\sigma_\theta^2)$, the ratio $\widehat h/h$ has a [log-normal distribution](../../../probability-theory.md#log-normal-distribution). Its exact variance is

$$
\operatorname{Var}\!\left(\frac{\widehat h}{h}\right)
=e^{\sigma_\theta^2/\alpha^2}
\left(e^{\sigma_\theta^2/\alpha^2}-1\right),
$$

and the lowest-order [delta method](../../../statistical-inference.md#delta-method) approximation is

$$
\operatorname{Var}\!\left(\frac{\widehat h}{h}\right)
=\frac{\sigma_\theta^2}{\alpha^2}+O(\sigma_\theta^4).
$$

For fixed $\sigma_{\rm tot}$, case (i) has $A=\sigma_\mu^2+\sigma_{\rm tot}^2$, whereas case (ii) has $A=\sigma_\mu^2+\sigma_{\rm tot}^2/K$. Because $K\geq2$ and $B$ is the same in both cases, independent supernova-level variation in case (ii) gives the smaller fractional variance: averaging reduces it, while a shared galaxy fluctuation does not average away.

## 2

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The vector $(y_1,y_2,y_3)$ is [Jointly Gaussian](../../../probability-and-statistics.md#multivariate-normal-distribution). Assuming $R>0$, [Gaussian conditional independence](../../../probability-and-statistics.md#gaussian-conditional-independence) gives

$$
y_3\mathbin\perp y_1\mid y_2
\quad\Longleftrightarrow\quad
\operatorname{Cov}(y_1,y_3\mid y_2)
=R_{13}-\frac{R_{12}R_{23}}R=0.
$$

Thus the required condition is $RR_{13}=R_{12}R_{23}$. Under it, conditioning on $y_1$ supplies no further information after $y_2$, and the [Gaussian process regression posterior](../../../probability-and-statistics.md#gaussian-process-regression-posterior) is

$$
y_3\mid y_2,y_1
\sim N\!\left(
\mu+\frac{R_{23}}R(y_2-\mu),
R-\frac{R_{23}^2}R
\right).
$$

Both the [conditional expectation](../../../measure-theory.md#conditional-expectation) and [conditional variance](../../../variance.md#conditional-variance) depend only on $y_2,t_2,t_3$; neither contains $y_1$ or $t_1$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For $t_1<t_2<t_3$, the condition from part a becomes

$$
(t_3-t_1)^\eta
=(t_2-t_1)^\eta+(t_3-t_2)^\eta.
$$

It holds for arbitrary positive time gaps exactly when $\eta=1$. The resulting [exponential covariance function](../../../stochastic-process.md#exponential-covariance-function) is the covariance of a stationary [Ornstein-Uhlenbeck process](../../../stochastic-process.md#ornstein-uhlenbeck-process), hence has the [Markov property](../../../markov-process.md#markov-property).

Writing $a_{32}=e^{-(t_3-t_2)/\tau}$, the predictive law is

$$
y_3\mid y_2,y_1
\sim N\!\left(\mu+a_{32}(y_2-\mu),,1-a_{32}^2\right).
$$

As $t_3\to\infty$, $a_{32}\to0$, so the predictive mean tends to the stationary mean $\mu$ and the predictive variance tends to the stationary variance $1$.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Set

$$
a=e^{-(t_2-t_1)/\tau},
\qquad
b=e^{-(t_3-t_2)/\tau}.
$$

The [Markov factorization](../../../markov-process.md#markov-factorization) and the conditional normal laws from part b give the fully univariate product

$$
p(y\mid t,\mu,\tau)
=\phi(y_1;\mu,1)
\phi\!\left(y_2;\mu+a(y_1-\mu),1-a^2\right)
\phi\!\left(y_3;\mu+b(y_2-\mu),1-b^2\right),
$$

where $\phi(\mathord\cdot;m,v)$ denotes the $N(m,v)$ density. This is a [weighted least squares](../../../statistical-modelling.md#weighted-least-squares) problem in $\mu$. Differentiating its log-likelihood gives

$$
\widehat\mu=
\frac{
y_1+\dfrac{y_2-ay_1}{1+a}+\dfrac{y_3-by_2}{1+b}
}{
1+\dfrac{1-a}{1+a}+\dfrac{1-b}{1+b}
}.
$$

Every innovation in the numerator has expectation equal to its coefficient in the denominator times $\mu$. Therefore $\mathbb E\widehat\mu=\mu$, so this maximum likelihood estimator is unbiased.

## 3

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a fixed observed colour $\widetilde c_s$, [Bayes' theorem](../../../probability-theory.md#bayes-theorem) gives

$$
p(E_s\mid\widetilde c_s)
\propto
\exp\!\left[-\frac{(\widetilde c_s-E_s-c_0)^2}{2\sigma_c^2}-\frac{E_s}{\tau}\right]
\mathbf1_{\{E_s\geq0\}}.
$$

Completing the square shows that this is a [truncated normal distribution](../../../probability-theory.md#truncated-normal-distribution) with variance $\sigma_c^2$, lower endpoint zero, and untruncated location

$$
e_s=\widetilde c_s-c_0-\frac{\sigma_c^2}{\tau}.
$$

Hence

$$
\overline E_s
\equiv\mathbb E[E_s\mid\widetilde c_s]
=e_s+\sigma_c\frac{\phi(e_s/\sigma_c)}{\Phi(e_s/\sigma_c)}.
$$

Conditioning first on $E_s$ and using the [law of total expectation](../../../measure-theory.md#law-of-total-expectation) yields the dusty colour-magnitude relation

$$
\mathbb E[\widetilde M_s\mid\widetilde c_s]
=M_0+\beta\widetilde c_s+(R-\beta)\overline E_s.
$$

As $\widetilde c_s\to-\infty$, the [Inverse Mills ratio](../../../probability-theory.md#inverse-mills-ratio) implies $\overline E_s\to0$ with vanishing derivative, so the asymptotic slope is $\beta$. As $\widetilde c_s\to+\infty$, $\overline E_s\sim\widetilde c_s-c_0-\sigma_c^2/\tau$, so the asymptotic slope is $R$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $c_s=\widetilde c_s-E_s$ and $M_s=\widetilde M_s-RE_s$. With the stated [improper hyperpriors](../../../statistical-inference.md#improper-prior), the unnormalized [posterior density](../../../statistical-inference.md#posterior-density) is

$$
\begin{aligned}
&p(\{E_s\},M_0,c_0,\beta,\sigma_M^2,\sigma_c^2,R,\tau\mid\{d_s\})\\
&\quad\propto
\mathbf1_{\{\sigma_M^2,\sigma_c^2,\tau>0\}}
\prod_{s=1}^N
\left[
\frac1{\sigma_c}\exp\!\left\{-\frac{(\widetilde c_s-E_s-c_0)^2}{2\sigma_c^2}\right\}
\frac1{\sigma_M}\exp\!\left\{-\frac{[\widetilde M_s-RE_s-M_0-\beta(\widetilde c_s-E_s)]^2}{2\sigma_M^2}\right\}
\frac1\tau e^{-E_s/\tau}\mathbf1_{\{E_s\geq0\}}
\right].
\end{aligned}
$$

Its [Directed acyclic graph](../../../combinatorics.md#directed-acyclic-graph) has, for each star, the arrows

$$
(c_0,\sigma_c^2)\to c_s,
\qquad
(M_0,\beta,\sigma_M^2,c_s)\to M_s,
\qquad
\tau\to E_s,
$$

followed by the deterministic observation arrows

$$
(c_s,E_s)\to\widetilde c_s,
\qquad
(M_s,E_s,R)\to\widetilde M_s.
$$

The [latent variables](../../../statistical-modelling.md#latent-variable) $(c_s,M_s,E_s)$ are repeated inside a plate indexed by $s=1,\ldots,N$; all hyperparameters lie outside that plate.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

A [Gibbs sampler](../../../statistical-inference.md#gibbs-sampler) draws each variable from its [full conditional distribution](../../../probability-theory.md#full-conditional-distribution), so every proposed update is accepted. At the start of a sweep define $c_s=\widetilde c_s-E_s$, $y_s=\widetilde M_s-RE_s$, and

$$
d_s=\widetilde M_s-M_0-\beta\widetilde c_s,
\qquad
v_E=\left(\frac1{\sigma_c^2}+\frac{(R-\beta)^2}{\sigma_M^2}\right)^{-1},
$$



$$
m_{E,s}=v_E\left[
\frac{\widetilde c_s-c_0}{\sigma_c^2}
+\frac{(R-\beta)d_s}{\sigma_M^2}
-\frac1\tau
\right].
$$

First update the reddenings independently as

$$
E_s\mid\text{rest}\sim TN_{[0,\infty)}(m_{E,s},v_E).
$$

Recompute $c_s$ and $y_s$, then make the Gaussian updates

$$
c_0\mid\text{rest}\sim N\!\left(\bar c,\frac{\sigma_c^2}{N}\right),
$$



$$
M_0\mid\text{rest}\sim N\!\left(
\frac1N\sum_s(y_s-\beta c_s),\frac{\sigma_M^2}{N}
\right),
$$



$$
\beta\mid\text{rest}\sim N\!\left(
\frac{\sum_sc_s(y_s-M_0)}{\sum_sc_s^2},
\frac{\sigma_M^2}{\sum_sc_s^2}
\right),
$$

and

$$
R\mid\text{rest}\sim N\!\left(
\frac{\sum_sE_s[\widetilde M_s-M_0-\beta c_s]}{\sum_sE_s^2},
\frac{\sigma_M^2}{\sum_sE_s^2}
\right).
$$

With

$$
S_c=\sum_s(c_s-c_0)^2,
\qquad
S_M=\sum_s(y_s-M_0-\beta c_s)^2,
$$

the remaining full conditionals, in the parameterization given in the question, are the [scaled inverse chi-squared laws](../../../probability-theory.md#scaled-inverse-chi-squared-distribution)

$$
\sigma_c^2\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(N-2,\frac{S_c}{N-2}\right),
$$



$$
\sigma_M^2\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(N-2,\frac{S_M}{N-2}\right),
$$



$$
\tau\mid\text{rest}
\sim\operatorname{Inv}\text{-}\chi^2\!\left(2N-2,\frac{\sum_sE_s}{N-1}\right).
$$

Repeating these updates in the displayed order gives a complete Gibbs sweep. The formulas assume $N>2$ and nondegenerate sampled predictors; posterior propriety must be checked because the hyperpriors are improper.

## 4

↑ **Parent:** [Paper 219](paper-219.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/i">i</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/i/solution">Solution</h5>

↑ **Parent:** [I](#4/a/i)

Using [Bayes' theorem](../../../probability-theory.md#bayes-theorem) and the fact that the prior is proper,

$$
\mathbb E_{\theta\mid y}\widehat I
=\int\frac1{p(y\mid\theta)}
\frac{p(y\mid\theta)p(\theta)}Z\,d\theta
=\frac1Z\int p(\theta)\,d\theta
=\frac1Z.
$$

Thus $\widehat I$ is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) of $Z^{-1}$, and the [Harmonic mean estimator of Bayesian model evidence](../../../statistical-inference.md#harmonic-mean-estimator-of-bayesian-model-evidence) is $\widehat Z=1/\widehat I$. The reciprocal is not itself generally unbiased, though it is consistent when the [strong law of large numbers](../../../convergence-of-random-variables.md#strong-law-of-large-numbers) applies.

<h4 id="4/a/ii">ii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#4/a/ii)

Multiplying the Gaussian likelihood and prior and [completing the square](../../../polynomial.md#completing-the-square) gives

$$
p(\theta\mid y)
\propto
\exp\!\left[-\frac12\left\{
\frac{(y-\theta)^2}{\sigma^2}+\frac{\theta^2}{\tau^2}
\right\}\right].
$$

Therefore [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
\boxed{\theta\mid y\sim N(m,v),
\qquad
m=\frac{\tau^2}{\sigma^2+\tau^2}y,
\qquad
v=\frac{\sigma^2\tau^2}{\sigma^2+\tau^2}.}
$$

<h4 id="4/a/iii">iii</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#4/a/iii)

The evidence is the [convolution](../../../probability-theory.md#convolution-of-independent-random-variables) of $N(0,\tau^2)$ and $N(0,\sigma^2)$, so

$$
Z=p(y)=\frac1{\sqrt{2\pi(\sigma^2+\tau^2)}}
\exp\!\left[-\frac{y^2}{2(\sigma^2+\tau^2)}\right].
$$

Part i now gives the fully simplified expectation

$$
\boxed{\mathbb E_{\theta\mid y}\widehat I
=\sqrt{2\pi(\sigma^2+\tau^2)}
\exp\!\left[\frac{y^2}{2(\sigma^2+\tau^2)}\right].}
$$

<h4 id="4/a/iv">iv</h4>

↑ **Parent:** [A](#4/a)

<h5 id="4/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#4/a/iv)

Let $S=\sigma^2+\tau^2$. For one posterior draw, the Gaussian quadratic-exponential moment is finite precisely when $\tau<\sigma$, and then

$$
\mathbb E_{\theta\mid y}[p(y\mid\theta)^{-2}]
=2\pi\sigma^2\sqrt{\frac{S}{\sigma^2-\tau^2}}
\exp\!\left[
\frac{\sigma^2y^2}{S(\sigma^2-\tau^2)}
\right].
$$

Because the $m$ posterior draws are independent,

$$
\operatorname{Var}_{\theta\mid y}(\widehat I)
=\frac{2\pi}{m}\left[
\sigma^2\sqrt{\frac{S}{\sigma^2-\tau^2}}
\exp\!\left\{\frac{\sigma^2y^2}{S(\sigma^2-\tau^2)}\right\}
-S\exp\!\left\{\frac{y^2}{S}\right\}
\right].
$$

For $\tau\geq\sigma$ the second moment, and hence the variance, is infinite. The [Harmonic mean estimator of Bayesian model evidence](../../../statistical-inference.md#harmonic-mean-estimator-of-bayesian-model-evidence) is therefore unstable in the usual diffuse-prior regime: posterior sampling does not adequately control the reciprocal likelihood in the posterior tails.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Under $M_1$, [Bayes' theorem](../../../probability-theory.md#bayes-theorem) at the nested value $\psi=0$ gives

$$
p(\psi=0\mid D,M_1)
=\frac{p(D\mid\psi=0,M_1)p(\psi=0\mid M_1)}{p(D\mid M_1)}.
$$

Separability of the prior and equality of the $\phi$ priors imply

$$
p(D\mid\psi=0,M_1)
=\int p(D\mid\phi,\psi=0,M_1)p(\phi\mid M_1)\,d\phi
=p(D\mid M_0).
$$

Rearranging proves the [Savage-Dickey density ratio](../../../statistical-inference.md#savage-dickey-density-ratio)

$$
B_{01}
=\frac{p(D\mid M_0)}{p(D\mid M_1)}
=\left.
\frac{p(\psi\mid D,M_1)}{p(\psi\mid M_1)}
\right|_{\psi=0},
$$

which is the [Bayes factor](../../../statistical-inference.md#bayes-factor) in favor of the nested model.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2022](../../2022.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
