# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2010/Paper36.pdf)

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
  - [h](#2/h)
    - [Solution](#2/h/solution)
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
  - [f](#4/f)
    - [Solution](#4/f/solution)
  - [g](#4/g)
    - [Solution](#4/g/solution)
  - [h](#4/h)
    - [Solution](#4/h/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

If $\pi_0=\mathbb P(H_0)$ and $\pi_1=\mathbb P(H_1)=1-\pi_0$, the [prior odds](../../../statistical-inference.md#prior-odds) on the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) are

$$
\boxed{O_{01}=\frac{\pi_0}{\pi_1}.}
$$

These odds concern which model is true before seeing the observations. They are separate from the [prior distribution](../../../statistical-inference.md#prior-probability) of the success probability within the alternative model.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Use the orientation that favours the [null hypothesis](../../../statistical-modelling.md#null-hypothesis):

$$
\boxed{B_{01}(y)=\frac{p(y\mid H_0)}{p(y\mid H_1)}.}
$$

For a composite model the denominator is its [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence), obtained by integrating the [likelihood](../../../statistical-modelling.md#likelihood-function) against the model's [prior distribution](../../../statistical-inference.md#prior-probability). This [Bayes factor](../../../statistical-inference.md#bayes-factor) exceeds one when the observed data have greater marginal probability under $H_0$. By [Bayes' theorem](../../../probability-theory.md#bayes-theorem),

$$
\frac{\mathbb P(H_0\mid y)}{\mathbb P(H_1\mid y)}
=\frac{p(y\mid H_0)\pi_0/p(y)}{p(y\mid H_1)\pi_1/p(y)}
=\boxed{B_{01}(y)O_{01}}.
$$

Thus the [posterior odds](../../../statistical-inference.md#posterior-odds) equal the [prior odds](../../../statistical-inference.md#prior-odds) multiplied by the [Bayes factor](../../../statistical-inference.md#bayes-factor). The reciprocal orientation instead gives $B_{10}=1/B_{01}$.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Conditional on the success probability, the count has [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution). Integrating its [likelihood](../../../statistical-modelling.md#likelihood-function) under the uniform [prior distribution](../../../statistical-inference.md#prior-probability), or equivalently a [Beta distribution](../../../probability-theory.md#beta-distribution) with parameters $(1,1)$, gives

$$
p(y\mid H_1)=\int_0^1\binom ny\theta^y(1-\theta)^{n-y}\,d\theta
=\binom ny\frac{\Gamma(y+1)\Gamma(n-y+1)}{\Gamma(n+2)}
=\boxed{\frac1{n+1}},\qquad y=0,\ldots,n.
$$

The [prior predictive distribution](../../../statistical-inference.md#bayesian-model-evidence) is therefore uniform over the possible counts. Excluding the single point $\theta=1/2$ does not alter this integral because a continuous [prior distribution](../../../statistical-inference.md#prior-probability) gives that point zero probability. This calculation is the marginalization underlying [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), $Y\sim\operatorname{Bin}(n,1/2)$, with [expected value](../../../probability-theory.md#expected-value) $n/2$ and [variance](../../../variance.md) $n/4$. Approximating its probability at an integer by the [normal distribution](../../../probability-theory.md#normal-distribution) density over a unit-width cell gives

$$
p(y\mid H_0)\approx\frac1{\sqrt{2\pi(n/4)}}\exp\left[-\frac{(y-n/2)^2}{2(n/4)}\right]
=\sqrt{\frac2{\pi n}}\exp\left[-\frac2n(y-n/2)^2\right].
$$

Dividing by the [prior predictive distribution](../../../statistical-inference.md#bayesian-model-evidence) from the preceding part gives the [uniform-alternative binomial Bayes factor](../../../statistical-inference.md#uniform-alternative-binomial-bayes-factor)

$$
B_{01}(y)\approx(n+1)\sqrt{\frac2{\pi n}}\exp\left[-\frac2n(y-n/2)^2\right]
\approx\boxed{\sqrt{\frac{2n}{\pi}}\exp\left[-\frac2n(y-n/2)^2\right]}.
$$

The second approximation replaces $n+1$ by $n$. Both are large-sample approximations for counts in the central range, rather than exact identities at extreme counts.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [normal distribution](../../../probability-theory.md#normal-distribution) standardized statistic for the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) count is

$$
Z=\frac{5150-5000}{\sqrt{10000/4}}=\boxed{3}.
$$

Because the alternative is two-sided, the approximate [p-value](../../../statistical-modelling.md#p-value) is $2\{1-\Phi(3)\}\approx0.0027$. A continuity correction replaces $3$ by $(149.5)/50=2.99$ and gives approximately $0.0028$, with the same conclusion. Thus **the result is statistically significant at both the 5% and 1% levels**. The [p-value](../../../statistical-modelling.md#p-value) is a null tail probability, not a [posterior probability](../../../statistical-inference.md#posterior-probability) that the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) is true.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

Substituting the standardized deviation into the [Bayes factor](../../../statistical-inference.md#bayes-factor) approximation gives

$$
\boxed{B_{01}\approx\sqrt{\frac{20000}{\pi}}e^{-4.5}\approx0.89,\qquad B_{10}\approx1.13.}
$$

This is only a slight preference for the alternative, despite the small [p-value](../../../statistical-modelling.md#p-value). The two procedures measure different things: the [p-value](../../../statistical-modelling.md#p-value) sums a tail under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), while the [Bayes factor](../../../statistical-inference.md#bayes-factor) compares probabilities of the observed count under both models. The uniform alternative [prior distribution](../../../statistical-inference.md#prior-probability) spreads its probability over many success probabilities that fit the observations poorly. Only a narrow range around $0.515$ has large [likelihood](../../../statistical-modelling.md#likelihood-function), and integrating over the whole alternative penalizes this diffuse prediction.

The prefactor makes the distinction especially clear. At a fixed standardized deviation $z$, the [p-value](../../../statistical-modelling.md#p-value) stays approximately $2\{1-\Phi(|z|)\}$, whereas $B_{01}\approx\sqrt{2n/\pi}e^{-z^2/2}$ eventually grows with $n$. A fixed diffuse alternative can consequently favour the point null even while a conventional test rejects it. This is the same prior-width mechanism illustrated by the [Jeffreys-Lindley paradox for a Gaussian point null](../../../statistical-inference.md#jeffreys-lindley-paradox-for-a-gaussian-point-null).

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

An alternative that allows small departures from chance, while assigning little probability to near-perfect prediction or near-perfect failure, is more plausible than a uniform [prior distribution](../../../statistical-inference.md#prior-probability). For example, a symmetric [Beta distribution](../../../probability-theory.md#beta-distribution) $\operatorname{Beta}(a,a)$ with $a>1$ is centered at $1/2$, with

$$
\mathbb E\theta=\frac12,\qquad \operatorname{Var}(\theta)=\frac1{4(2a+1)}.
$$

Choosing $a=50$ gives a prior standard deviation of about $0.05$ and concentrates on modest deviations. Its concentration should represent substantive beliefs specified before examining this experiment, rather than being tuned to the observed count. A continuous [prior distribution](../../../statistical-inference.md#prior-probability) centered at $1/2$ still places no point mass at $H_0$; the separate model [prior probability](../../../statistical-inference.md#prior-probability) supplies that mass.

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

**No.** A [Bayes factor](../../../statistical-inference.md#bayes-factor) favouring the alternative means $B_{01}<1$, but the [posterior odds](../../../statistical-inference.md#posterior-odds) are $B_{01}O_{01}$. They are less than one only if $B_{01}<1/O_{01}$. For example, [prior odds](../../../statistical-inference.md#prior-odds) of $1000:1$ on the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), combined with a [Bayes factor](../../../statistical-inference.md#bayes-factor) of $100:1$ in favour of the alternative, still give [posterior odds](../../../statistical-inference.md#posterior-odds) of $10:1$ on the [null hypothesis](../../../statistical-modelling.md#null-hypothesis). An unusual claim can require substantial evidence to overcome low initial plausibility.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take the exposure $E_i$ as known and positive. The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) [log-likelihood](../../../statistical-modelling.md#log-likelihood), up to a parameter-independent constant, is $\ell_i(\lambda_i)=y_i\log\lambda_i-E_i\lambda_i$. Its first two derivatives are

$$
\ell_i'(\lambda_i)=\frac{y_i}{\lambda_i}-E_i,\qquad \ell_i''(\lambda_i)=-\frac{y_i}{\lambda_i^2}.
$$

Since $\mathbb E(Y_i)=E_i\lambda_i$, the [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) is

$$
\mathcal I_i(\lambda_i)=-\mathbb E\ell_i''(\lambda_i)=\frac{E_i}{\lambda_i}.
$$

The [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) is proportional to its square root. Removing the constant $\sqrt{E_i}$ gives

$$
\boxed{\pi_J(\lambda_i)\propto\lambda_i^{-1/2},\qquad\lambda_i>0.}
$$

This is an [improper prior](../../../statistical-inference.md#improper-prior): its integral diverges at infinity.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Multiplying the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) [likelihood](../../../statistical-modelling.md#likelihood-function) by the [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) gives the [posterior density](../../../statistical-inference.md#posterior-density) kernel

$$
\pi(\lambda_i\mid y_i)\propto\lambda_i^{y_i-1/2}e^{-E_i\lambda_i}.
$$

Thus, in shape-rate convention,

$$
\boxed{\lambda_i\mid y_i\sim\operatorname{Gamma}(y_i+1/2,E_i).}
$$

It is a proper [posterior distribution](../../../statistical-inference.md#bayesian-posterior) even when $y_i=0$, provided $E_i>0$. The [posterior mean](../../../statistical-inference.md#posterior-mean) and [posterior variance](../../../statistical-inference.md#posterior-variance) are $(y_i+1/2)/E_i$ and $(y_i+1/2)/E_i^2$. This is [Poisson-gamma conjugacy with unequal exposures](../../../statistical-inference.md#poisson-gamma-conjugacy-with-unequal-exposures), with the zero-rate prior interpreted as an improper kernel.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A [proper gamma approximation to a Poisson Jeffreys prior](../../../statistical-modelling.md#proper-gamma-approximation-to-a-poisson-jeffreys-prior) uses shape $1/2$ and a small positive rate $\varepsilon$:

$$
\boxed{\lambda_i\sim\operatorname{Gamma}(1/2,\varepsilon),\qquad\varepsilon>0\ \text{small}.}
$$

Its density is proportional to $\lambda_i^{-1/2}e^{-\varepsilon\lambda_i}$, so where $\varepsilon\lambda_i$ is small its kernel approximates the [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior). After observing the data, [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy) gives $\operatorname{Gamma}(y_i+1/2,E_i+\varepsilon)$, which converges to the preceding [posterior distribution](../../../statistical-inference.md#bayesian-posterior) as $\varepsilon\downarrow0$. This is an approximation of an improper kernel on the relevant parameter range, not a weak limit to a normalized Jeffreys probability distribution. The shape must be $1/2$; a small-shape gamma prior would approximate a different power of $\lambda_i$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Under independent area counts and independent area [prior distributions](../../../statistical-inference.md#prior-probability), the joint [posterior distribution](../../../statistical-inference.md#bayesian-posterior) factors into the gamma posteriors. For each simulation $s=1,\ldots,S$, draw one joint vector by independently generating

$$
\lambda_i^{(s)}\sim\operatorname{Gamma}(y_i+1/2,E_i),\qquad i=1,\ldots,I.
$$

Rank the risks within that joint draw, taking rank one to mean highest risk:

$$
r_i^{(s)}=1+\sum_{k\ne i}\mathbf1\{\lambda_k^{(s)}>\lambda_i^{(s)}\}.
$$

The empirical [posterior rank distribution](../../../statistical-inference.md#posterior-rank-distribution) and highest-risk probability are

$$
\boxed{\widehat{\mathbb P}(r_i=k\mid y)=\frac1S\sum_{s=1}^S\mathbf1\{r_i^{(s)}=k\},\qquad
\widehat{\mathbb P}(i\text{ highest}\mid y)=\frac1S\sum_{s=1}^S\mathbf1\{r_i^{(s)}=1\}.}
$$

Independent gamma draws make this direct [Monte Carlo integration](../../../probability-and-statistics.md#monte-carlo-integration), so [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) is unnecessary here. Continuous posteriors give ties probability zero, and the highest-risk probabilities sum to one. The same ranking calculation can be applied to dependent joint draws from a richer [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model); ranking separate posterior means would discard the uncertainty that the program is intended to measure.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

For a shape-rate [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) $\operatorname{Gamma}(a,b)$, the mean and [variance](../../../variance.md) conditions require

$$
\frac ab=1,\qquad \frac a{b^2}=0.25^2=\frac1{16}.
$$

The first equation gives $a=b$, and the second then gives $a=b=16$. Hence

$$
\boxed{\lambda_i\sim\operatorname{Gamma}(16,16).}
$$

This proper [prior distribution](../../../statistical-inference.md#prior-probability) is centered on the national reference risk, while allowing genuine between-area variation.

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

The new [prior density](../../../statistical-inference.md#prior-density) contributes the factor $\lambda_i^{15}e^{-16\lambda_i}$. Multiplication by the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) [likelihood](../../../statistical-modelling.md#likelihood-function) gives

$$
\boxed{\lambda_i\mid y_i\sim\operatorname{Gamma}(y_i+16,E_i+16).}
$$

Its [posterior mean](../../../statistical-inference.md#posterior-mean) displays the resulting shrinkage:

$$
\mathbb E(\lambda_i\mid y_i)=\frac{y_i+16}{E_i+16}
=\frac{E_i}{E_i+16}\frac{y_i}{E_i}+\frac{16}{E_i+16}\cdot1.
$$

The observed risk ratio $y_i/E_i$ is pulled towards one, most strongly for small exposures. The [posterior variance](../../../statistical-inference.md#posterior-variance) is $(y_i+16)/(E_i+16)^2$.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

The informative [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) [prior distribution](../../../statistical-inference.md#prior-probability) discourages extreme risks caused by small denominators. Its influence is strongest where the exposure is small, while large-exposure areas are predominantly determined by their [likelihood](../../../statistical-modelling.md#likelihood-function). Consequently an area previously appearing near the top because of a noisy high raw risk ratio may have its highest-risk probability reduced, and the [posterior rank distributions](../../../statistical-inference.md#posterior-rank-distribution) of poorly observed areas tend to overlap more rather than suggesting a precise league table.

There is no universal claim that every rank distribution becomes wider or narrower: unequal exposures produce unequal shrinkage and can change the ordering, while the new prior also changes the uncertainty in the risks. In the limiting case of negligible information for every area, all area posteriors approach the same independent continuous [prior distribution](../../../statistical-inference.md#prior-probability). Symmetry then gives each area probability $1/I$ of occupying each rank. This illustrates why modest differences between weakly observed areas should not yield confident rankings.

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

The [posterior probability](../../../statistical-inference.md#posterior-probability) $q_i=\mathbb P(\lambda_i>1\mid y_i)$ answers a natural directional question: how likely is this area's risk to exceed the reference risk? It accounts for uncertainty rather than declaring an increase from the point estimate alone. However, it does not distinguish a negligible increase from a clinically important one, and it combines prior beliefs with evidence from the data. With an informative [prior distribution](../../../statistical-inference.md#prior-probability), a large probability may already have been present before observation, or a genuinely surprising count may be strongly moderated by the prior.

To measure the evidence supplied by the observations, compare posterior and prior odds. If $q_0=\mathbb P(\lambda_i>1)$ under the chosen proper [prior distribution](../../../statistical-inference.md#prior-probability), the [Bayes factor](../../../statistical-inference.md#bayes-factor) for increased versus nonincreased risk is

$$
\boxed{B_{+,-}(y_i)=\frac{q_i/(1-q_i)}{q_0/(1-q_0)}.}
$$

This follows from the [posterior odds](../../../statistical-inference.md#posterior-odds) identity when the two models use the original prior conditioned respectively on $\lambda_i>1$ and $\lambda_i\le1$. For the specified prior, $q_0$ is the upper tail at one of $\operatorname{Gamma}(16,16)$; centering its mean at one does not make this tail probability exactly $1/2$. To address seriousness itself, choose a substantive excess $c>0$ and report **the posterior probability of $\lambda_i>1+c$**, together with an interval for the size of the excess. An evidence ratio and a meaningful risk threshold answer different, complementary questions.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

The logarithm is strictly increasing, so maximizing the [likelihood function](../../../statistical-modelling.md#likelihood-function) is equivalent to maximizing its logarithm. Multiplication by $-2$ reverses that ordering. Thus, whenever the maximum is attained,

$$
\boxed{\widehat\theta\in\operatorname*{arg\,max}_\theta p(y\mid\theta)
\quad\Longleftrightarrow\quad
\widehat\theta\in\operatorname*{arg\,min}_\theta D(\theta).}
$$

Here the [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) includes the likelihood constants. Parameter-independent constants do not alter the minimizer, but a common convention must be retained when comparing criteria between models.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Under the usual regular, identifiable, fixed-dimensional setting, the [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator) is an interior point with vanishing [log-likelihood](../../../statistical-modelling.md#log-likelihood) gradient, and the observed information is positive definite. Define

$$
J=\frac12\nabla^2D(\widehat\theta)=-\nabla^2\log p(y\mid\widehat\theta).
$$

The second-order [Taylor expansion](../../../calculus.md#taylor-expansion) of the [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) is

$$
D(\theta)\approx D(\widehat\theta)+(\theta-\widehat\theta)^TJ(\theta-\widehat\theta).
$$

With a [prior density](../../../statistical-inference.md#prior-density) approximately constant over the likelihood's concentration region, the [posterior density](../../../statistical-inference.md#posterior-density) is therefore proportional to

$$
\exp\{-D(\theta)/2\}\approx\text{constant}\times
\exp\left[-\frac12(\theta-\widehat\theta)^TJ(\theta-\widehat\theta)\right].
$$

Recognizing the [multivariate normal density](../../../probability-and-statistics.md#multivariate-normal-density) gives

$$
\boxed{\theta\mid y\ \dot\sim\ N_p\left(\widehat\theta,\left[\tfrac12\nabla^2D(\widehat\theta)\right]^{-1}\right).}
$$

Typically $J$ grows at rate $n$ and the posterior concentrates in a region of radius $n^{-1/2}$, making higher-order terms negligible under the regularity assumptions. The local flatness assumption concerns this region, not necessarily the entire parameter space. Boundary maxima, unidentified directions, or persistent multiple modes can invalidate this approximation.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Conditional on the observed data, the preceding [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) approximation implies that

$$
Z=J^{1/2}(\theta-\widehat\theta)\ \dot\sim\ N_p(0,I).
$$

The deviance expansion consequently gives

$$
D(\theta)-D(\widehat\theta)\approx(\theta-\widehat\theta)^TJ(\theta-\widehat\theta)=Z^TZ.
$$

The sum of squares of $p$ independent standard [normal distribution](../../../probability-theory.md#normal-distribution) variables has [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $p$ degrees of freedom. Hence, as a statement about the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) of the [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance),

$$
\boxed{D(\theta)\mid y\ \dot\sim\ D(\widehat\theta)+\chi_p^2.}
$$

The data are fixed here and the parameter varies according to its posterior; this is not a claim about resampling the data.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $\overline\theta=\mathbb E(\theta\mid y)$ and $\overline D=\mathbb E\{D(\theta)\mid y\}$. The usual [effective parameter count in DIC](../../../statistical-modelling.md#effective-parameter-count-in-dic) is

$$
\boxed{p_D=\overline D-D(\overline\theta).}
$$

With the locally flat [prior distribution](../../../statistical-inference.md#prior-probability), $\overline\theta\approx\widehat\theta$ and the mean of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) excess is $p$. Thus $\overline D\approx D(\widehat\theta)+p$, while $D(\overline\theta)\approx D(\widehat\theta)$, giving **$p_D\approx p$**.

More generally, the [quadratic posterior deviance moments](../../../statistical-modelling.md#quadratic-posterior-deviance-moments) give the effective count. Within the same approximation, let the [posterior covariance matrix](../../../statistical-inference.md#posterior-covariance-matrix) be $\Sigma$. The expectation of a [quadratic form](../../../linear-algebra.md#quadratic-form) gives

$$
\overline D\approx D(\widehat\theta)+(\overline\theta-\widehat\theta)^TJ(\overline\theta-\widehat\theta)+\operatorname{tr}(J\Sigma),
$$

whereas evaluation at $\overline\theta$ omits the trace term. Therefore $p_D\approx\operatorname{tr}(J\Sigma)$. For a flat prior, $\Sigma\approx J^{-1}$ and the trace is $p$; informative prior shrinkage can reduce this effective count.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Using the same [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) convention, the [deviance information criterion](../../../statistical-modelling.md#deviance-information-criterion) and [Akaike information criterion](../../../statistical-modelling.md#akaike-information-criterion) are

$$
\boxed{\operatorname{DIC}=\overline D+p_D=D(\overline\theta)+2p_D,\qquad
\operatorname{AIC}=D(\widehat\theta)+2p.}
$$

Both combine a lack-of-fit term with a complexity penalty; smaller values are preferred among comparable models. Under the locally flat [prior distribution](../../../statistical-inference.md#prior-probability) and the regular [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) approximation, $D(\overline\theta)\approx D(\widehat\theta)$ and $p_D\approx p$, so

$$
\boxed{\operatorname{DIC}\approx D(\widehat\theta)+2p=\operatorname{AIC}.}
$$

All fitted parameters counted in the likelihood, including unknown dispersion parameters, belong in $p$. The equivalence need not hold for informative priors, nonregular models, or different choices of the likelihood's latent-variable representation.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

For retained [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) draws $\theta^{(1)},\ldots,\theta^{(S)}$, calculate both the parameter average $\widehat m=S^{-1}\sum_s\theta^{(s)}$ and the average deviance $\widehat D_{\mathrm{av}}=S^{-1}\sum_sD(\theta^{(s)})$. Two estimates are

$$
\boxed{\widehat D_{\min,1}=D(\widehat m),\qquad
\widehat D_{\min,2}=\widehat D_{\mathrm{av}}-p.}
$$

The first uses the approximate equality of the [posterior mean](../../../statistical-inference.md#posterior-mean) and [maximum-likelihood estimator](../../../statistical-modelling.md#maximum-likelihood-estimator). The second subtracts the mean $p$ of the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) deviance excess. These are different operations: evaluation after averaging versus averaging after evaluation. Both rely on a well-mixed chain and the regular locally flat-prior approximation. The smallest sampled deviance is an upper bound on the true minimum, but merely taking that minimum can be inefficient in high dimension because few draws approach the mode closely.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

The alternative effective count is

$$
\boxed{p_V=\frac12\operatorname{Var}\{D(\theta)\mid y\}.}
$$

Under the locally flat-prior approximation, the constant $D(\widehat\theta)$ contributes no [variance](../../../variance.md), and the remaining [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) term has [variance](../../../variance.md) $2p$. Hence $p_V\approx p$, the same calibration as the usual [effective parameter count in DIC](../../../statistical-modelling.md#effective-parameter-count-in-dic). It can be estimated by half the sample variance of deviance draws, without evaluating deviance at a parameter average.

This is a calibrated alternative, not a general identity with $p_D$. For example, with a quadratic deviance and a [multivariate normal distribution](../../../probability-and-statistics.md#multivariate-normal-distribution) posterior of mean $m$ and covariance $\Sigma$, putting $b=m-\widehat\theta$ gives

$$
p_V=\operatorname{tr}\{(J\Sigma)^2\}+2b^TJ\Sigma Jb,
\qquad p_D=\operatorname{tr}(J\Sigma).
$$

They agree when $b=0$ and $\Sigma=J^{-1}$, but informative priors can change both the covariance and the displacement of the posterior mean. Their equality should therefore not be assumed outside the stated regime.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The common [normal distribution](../../../probability-theory.md#normal-distribution) for the child-specific [random intercepts](../../../statistical-modelling.md#random-intercept) produces [partial pooling](../../../statistical-inference.md#partial-pooling). Children with little information borrow strength from the common population, while well-observed children retain more of their individual estimate. For fixed slopes and hyperparameters, let $\overline r_i$ average the three responses after subtracting their slope terms. Multiplying the normal [likelihood](../../../statistical-modelling.md#likelihood-function) by the normal intercept [prior distribution](../../../statistical-inference.md#prior-probability) gives

$$
\mathbb E(\alpha_i\mid\text{others},y)=w\overline r_i+(1-w)\delta,\qquad
w=\frac{3\tau^2}{\sigma^2+3\tau^2},
$$

with conditional [variance](../../../variance.md) $(3/\sigma^2+1/\tau^2)^{-1}$. Thus small between-child variation produces stronger shrinkage towards $\delta$. The common mean and variation are themselves learned from all children in this [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model).

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Center the log-time predictor and the baseline log measurement near their sample means, so the intercept describes a typical predictor configuration. This reduces intercept-slope posterior correlation and can improve [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) mixing. If exactly the original model is required, transform the intercept prior consistently when changing coordinates rather than silently assigning a different independent prior.

For weakly informed child effects, a [non-centered Gaussian random-effect parameterization](../../../statistical-inference.md#non-centered-gaussian-random-effect-parameterization) can also help:

$$
z_i\sim N(0,1),\qquad\boxed{\alpha_i=\delta+\tau z_i.}
$$

This retains the same conditional [prior distribution](../../../statistical-inference.md#prior-probability) for $\alpha_i$ but removes its prior-scale dependence from the sampled $z_i$. It can reduce strong dependence between the effects and $\tau$. A centered parameterization can be better when each child's effect is very accurately observed, so improvement is not automatic. Blocking strongly correlated coefficients is another option. Check the resulting chains with [Markov chain Monte Carlo convergence diagnostics](../../../statistical-inference.md#markov-chain-monte-carlo-convergence-diagnostics) and [effective sample size of a Markov chain](../../../statistical-inference.md#effective-sample-size-of-a-markov-chain), rather than judging convergence from the number of iterations alone.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

The bounded uniform [prior distributions](../../../statistical-inference.md#prior-probability) on the slopes and population intercept are proper and broad on their stated scale. They allow either sign but are not invariant to changes of units. The residual [precision parameter](../../../statistical-modelling.md#precision-parameter) $q=1/\sigma^2$ has a proper shape-rate $\operatorname{Gamma}(0.001,0.001)$ prior. Equivalently, $\sigma^2$ has [inverse-gamma distribution](../../../continuous-probability-distribution.md#inverse-gamma-distribution) with the same shape and scale. This is a commonly used diffuse choice, but it is not literally noninformative and its tail behaviour merits sensitivity analysis.

The prior for $\tau$ is uniform on $(0,100)$, so the induced density of $v=\tau^2$ is

$$
\boxed{\pi(v)=\frac1{200\sqrt v},\qquad0<v<10000.}
$$

It is integrable at zero, unlike the usual scale-invariant variance kernel $\pi(v)\propto1/v$. The latter kernel, often called the standard variance [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior), would cause an [improper posterior from a log-uniform random-effect scale prior](../../../statistical-inference.md#improper-posterior-from-a-log-uniform-random-effect-scale-prior) here. After integrating the child intercepts, each child's response vector has a normal likelihood with [covariance matrix](../../../variance.md#covariance-matrix) $\sigma^2I_3+v\mathbf1\mathbf1^T$. For fixed positive $\sigma^2$, this covariance remains nonsingular at $v=0$, and the marginal likelihood has a positive finite limit there. On a compact set of the other parameters its positivity gives

$$
\int_0^\varepsilon L(v)\frac{dv}{v}=\infty.
$$

Consequently the scale-invariant kernel cannot be normalized to a [posterior distribution](../../../statistical-inference.md#bayesian-posterior). A proper prior on the standard deviation avoids this problem. This familiar scale prior is not necessarily the actual [Jeffreys prior for an additive variance component](../../../statistical-modelling.md#jeffreys-prior-for-an-additive-variance-component) derived from the observed-data likelihood; the latter can be finite at zero.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The baseline assay is a noisy measurement just like the follow-up assays. On the log scale, a [normal distribution](../../../probability-theory.md#normal-distribution) for its error is a reasonable approximation if variability is approximately multiplicative on the original titre scale. The latent $\mu_{0i}$ represents the true baseline log-titre, with

$$
\boxed{y_{0i}\mid\mu_{0i},\sigma^2\sim N(\mu_{0i},\sigma^2).}
$$

Using a common [variance](../../../variance.md) is a simplifying assumption justified if baseline and follow-up measurements have comparable assay variability; it should not be treated as a fact guaranteed by the study design. Treating $y_{0i}$ as exact ignores [measurement error](../../../probability-and-statistics.md#measurement-error) in a predictor and can lead to [attenuation bias from classical measurement error](../../../linear-regression.md#attenuation-bias-from-classical-measurement-error) and understated uncertainty.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Model 2 is an [errors-in-variables model](../../../probability-and-statistics.md#errors-in-variables-model): the follow-up regression depends on a latent true baseline rather than substituting its noisy observation. A common [normal distribution](../../../probability-theory.md#normal-distribution) for the true baselines provides [partial pooling](../../../statistical-inference.md#partial-pooling) and allows uncertainty about each baseline to propagate to the regression coefficients and predictions. Conditional on the shared parameters, the child-specific factorization is

$$
p(\alpha_i\mid\delta,\tau)\,p(\mu_{0i}\mid\theta,\psi)\,p(y_{0i}\mid\mu_{0i},q)
\prod_{j=1}^3p(y_{ij}\mid\alpha_i,\mu_{0i},\beta,\gamma,q,t_{ij}),\qquad q=1/\sigma^2.
$$

The [Directed acyclic graph](../../../combinatorics.md#directed-acyclic-graph) below includes the shared parameters, the two local [latent variables](../../../statistical-modelling.md#latent-variable), both observed measurements, and the deterministic regression mean. The outer plate repeats over children and the inner plate over follow-up visits. Filled nodes are observed; rectangular mean nodes are deterministic.

<a id="4/e/image-directed-graph-of-the-latent-baseline-random-intercept-model-including-shared-priors-baseline-measurement-error-and-repeated-follow-up-visits"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-36-model-2.png)

**[Figure 1](#4/e/image-directed-graph-of-the-latent-baseline-random-intercept-model-including-shared-priors-baseline-measurement-error-and-repeated-follow-up-visits). Directed graph of the latent-baseline random-intercept model, including shared priors, baseline measurement error and repeated follow-up visits**.

One complete adapted [BUGS](../../../statistical-inference.md#bugs) specification uses the non-centered form of the [random intercept](../../../statistical-modelling.md#random-intercept), retaining the original priors and adding proper broad priors for $\theta$ and $\psi$:

```
for (i in 1:N) {
  z[i] ~ dnorm(0, 1)
  alpha[i] <- delta + tau*z[i]
  truebase[i] ~ dnorm(theta, baseprec)
  baseline[i] ~ dnorm(truebase[i], noiseprec)
  for (j in 1:3) {
    followmean[i,j] <- alpha[i] + beta*log(time[i,j]) + gamma*truebase[i]
    followup[i,j] ~ dnorm(followmean[i,j], noiseprec)
  }
}
noiseprec ~ dgamma(0.001, 0.001)
beta ~ dunif(-100, 100)
gamma ~ dunif(-100, 100)
delta ~ dunif(-100, 100)
tau ~ dunif(0, 100)
theta ~ dunif(-100, 100)
psi ~ dunif(0, 100)
baseprec <- 1/(psi*psi)
```

Here $N$ is the number of children, `baseline` and `followup` contain the observed data, and `dnorm` uses precision rather than variance. The priors on the newly introduced population baseline mean and standard deviation are explicit choices, not consequences of the likelihood; sensible alternatives can be checked for sensitivity. The code uses the noisy baseline only in its own measurement likelihood, and uses `truebase` in every follow-up mean.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

The PDF output places $-1$ inside the 95% [credible interval](../../../statistical-inference.md#credible-interval) for the time slope, whose endpoints are approximately $-1.329$ and $-0.7955$, and places $1$ inside the baseline slope interval, approximately $0.7915$ to $1.231$. Relative to their posterior standard deviations, the proposed fixed values are only

$$
\frac{-1-(-1.064)}{0.1352}\approx0.47,\qquad
\frac{1-1.023}{0.1145}\approx-0.20
$$

from the posterior means. Thus **the simpler choice $\beta=-1,\gamma=1$ is compatible with the fitted coefficient summaries** and has a natural proportional-decay interpretation. It is a reasonable constrained model to compare, not proof of the exact equalities: separate marginal intervals do not establish a joint constraint, and a continuous [posterior distribution](../../../statistical-inference.md#bayesian-posterior) assigns a specified point probability zero.

The reported [Monte Carlo errors](../../../probability-and-statistics.md#monte-carlo-error) measure numerical uncertainty in the estimated posterior means, not uncertainty about the coefficients themselves. In particular, the baseline slope's Monte Carlo error is about 9% of its posterior standard deviation, appreciably larger than the corresponding proportion for the time slope. Longer or better-mixed chains may be needed for precise summaries.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

The reported [deviance information criterion](../../../statistical-modelling.md#deviance-information-criterion) differs by

$$
\boxed{\operatorname{DIC}_2-\operatorname{DIC}_3=1.9.}
$$

Model 3 has a mean [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) worse by only $0.2$, but its [effective parameter count in DIC](../../../statistical-modelling.md#effective-parameter-count-in-dic) is lower by $2.1$. The small fit cost is more than offset by the reduced complexity penalty, so the criterion gives a mild preference to Model 3. A difference this small should not be presented as decisive evidence, especially without the [Monte Carlo error](../../../probability-and-statistics.md#monte-carlo-error) of the criterion difference.

The counts $143.6$ and $141.5$ are effective rather than literal parameter numbers. The likelihood includes child-specific intercepts and uncertain true baselines as well as global coefficients. With 106 of each local quantity and seven global parameters, Model 2 has 219 stochastic unknowns in a natural full representation, but [partial pooling](../../../statistical-inference.md#partial-pooling) and other prior information reduce their effective contribution. Fixing two slopes lowers the effective count by about two, with a further small change from the fitted posterior. There is no reason for $p_D$ to be an integer, or to equal just the number of population-level regression coefficients.

For illustration, the deviances evaluated at posterior means implied by the table are $\overline D-p_D=984.5$ for Model 2 and $986.8$ for Model 3. These differ from the average deviances because averaging a nonlinear deviance is not the same as evaluating it at an averaged parameter. This interpretation presumes the same observed-data likelihood convention in both fits; integrating local variables out before forming the deviance would define a different comparison. The [DIC](../../../statistical-modelling.md#deviance-information-criterion) difference is not a [Bayes factor](../../../statistical-inference.md#bayes-factor).

<h3 id="4/h">h</h3>

↑ **Parent:** [4](#4)

<h4 id="4/h/solution">Solution</h4>

↑ **Parent:** [H](#4/h)

Let $T_{0i}=e^{\mu_{0i}}$ denote the child's latent true baseline titre. With the constrained slopes, the conditional mean of log follow-up titre is

$$
\mu_i(t)=\alpha_i-\log t+\mu_{0i}.
$$

Exponentiating this log-scale center gives

$$
\boxed{\frac{e^{\mu_i(t)}}{T_{0i}}=\frac{e^{\alpha_i}}t.}
$$

Thus the conditional median, or geometric-mean titre, expressed as a fraction of true baseline titre, decays inversely with elapsed time; the child-specific intercept supplies the proportionality constant. It is not an exponential decay in time, and the formula is a follow-up model for $t>0$, not an extrapolation to the immunisation instant $t=0$.

For the arithmetic conditional mean, the [lognormal distribution](../../../probability-theory.md#log-normal-distribution) correction gives

$$
\frac{\mathbb E\{T_i(t)\mid\alpha_i,\mu_{0i},\sigma^2\}}{T_{0i}}
=\frac{e^{\alpha_i+\sigma^2/2}}t.
$$

The correction changes the constant but not the inverse-time dependence when the residual variance is constant. Averaging over random intercepts similarly preserves the time factor whenever the required expectation is finite.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2010](../../2010.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
