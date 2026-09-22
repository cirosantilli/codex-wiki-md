# Paper 35

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_35.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_35.pdf)

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
    - [1](#2/e/1)
      - [Solution](#2/e/1/solution)
    - [2](#2/e/2)
      - [Solution](#2/e/2/solution)
    - [3](#2/e/3)
      - [Solution](#2/e/3/solution)
    - [4](#2/e/4)
      - [Solution](#2/e/4/solution)
  - [f](#2/f)
    - [Solution](#2/f/solution)
  - [g](#2/g)
    - [Solution](#2/g/solution)
  - [h](#2/h)
    - [Solution](#2/h/solution)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [j](#2/j)
    - [Solution](#2/j/solution)
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
  - [i](#3/i)
    - [Solution](#3/i/solution)
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
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [j](#4/j)
    - [Solution](#4/j/solution)

## 1

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [likelihood function](../../../statistical-modelling.md#likelihood-function) for the ordered arrival times of a [Poisson process](../../../probability-theory.md#poisson-process), including the absence of further arrivals before $T$, is

$$
\boxed{L(\lambda)=\lambda^n e^{-\lambda T}},\qquad 0<t_1<\cdots<t_n<T.
$$

The arrival-time constraint does not depend on $\lambda$. Equivalently, the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) of the total count gives $L(\lambda)=e^{-\lambda T}(\lambda T)^n/n!$, which differs by a parameter-independent factor. Conditional on the count, the [Poisson process conditional arrival times](../../../probability-theory.md#poisson-process-conditional-arrival-times) have density $n!/T^n$, independent of $\lambda$. Thus **the total count contains all the information about the rate when the exposure is known**; it is a [sufficient statistic](../../../probability-and-statistics.md#sufficient-statistic).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

A [conjugate prior](../../../exponential-family.md#conjugate-prior) is a family of [prior distributions](../../../statistical-inference.md#prior-probability) whose members remain in that family after updating by the [likelihood function](../../../statistical-modelling.md#likelihood-function). Here multiplying a shape-rate [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) density by the [Poisson process](../../../probability-theory.md#poisson-process) likelihood changes its power of $\lambda$ and its exponential rate, leaving a [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution). The parameters change with the observations; [conjugate prior](../../../exponential-family.md#conjugate-prior) does not mean that the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) equals the [prior distribution](../../../statistical-inference.md#prior-probability).

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

By [Poisson-gamma conjugacy](../../../statistical-inference.md#poisson-gamma-conjugacy), the [posterior density](../../../statistical-inference.md#posterior-density) is proportional to

$$
\lambda^{a-1}e^{-b\lambda}\lambda^n e^{-T\lambda}
=\lambda^{a+n-1}e^{-(b+T)\lambda}.
$$

Thus **the shape-rate posterior is**

$$
\boxed{\lambda\mid\mathcal D\sim\operatorname{Gamma}(A,B),\quad A=a+n,\quad B=b+T.}
$$

Its [posterior mean](../../../statistical-inference.md#posterior-mean) is $A/B$ and its [variance](../../../variance.md) is $A/B^2$. The parameter $B$ is a rate, rather than a scale.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

Independent increments of the [Poisson process](../../../probability-theory.md#poisson-process) give $M\mid\lambda\sim\operatorname{Poisson}(\lambda)$ for a one-hour interval. The [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) therefore gives

$$
\boxed{\mathbb P(M=0\mid\lambda)=e^{-\lambda}.}
$$

This conditional probability still depends on the unknown rate.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

The [posterior predictive probability](../../../statistical-inference.md#posterior-predictive-probability) averages the conditional probability over the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior). Using its [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) density,

$$
p_0=\frac{B^A}{\Gamma(A)}\int_0^\infty\lambda^{A-1}e^{-(B+1)\lambda}\,d\lambda
=\boxed{\left(\frac{b+T}{b+T+1}\right)^{a+n}}.
$$

For fixed $a,b$ and $n/T\to\widehat\lambda<\infty$,

$$
\log p_0=-A\log(1+1/B)=-\frac{A}{B}+O(A/B^2)=-\frac nT+o(1).
$$

Consequently $p_0/e^{-n/T}\to1$, and both tend to $e^{-\widehat\lambda}$. This is reasonable because the [posterior mean](../../../statistical-inference.md#posterior-mean) tends to the observed rate and the [posterior variance](../../../statistical-inference.md#posterior-variance) tends to zero. Averaging $e^{-\lambda}$ then approaches evaluating it at the estimated rate: **with abundant observations, predictive uncertainty about the rate vanishes**.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

There is a notation problem here. The [posterior predictive probability](../../../statistical-inference.md#posterior-predictive-probability) $p_0$ calculated above is already a fixed number conditional on $a,b,n,T$. Literally,

$$
\boxed{\mathbb P(p_0<1/2\mid\mathcal D)=\mathbf1\!\left\{(B/(B+1))^A<1/2\right\}.}
$$

No simulation is needed for that interpretation. The known exposure $T$ is also necessary, despite its omission from this part's list of inputs.

The natural uncertain quantity is instead $q(\lambda)=\mathbb P(M=0\mid\lambda)=e^{-\lambda}$. For its [posterior probability](../../../statistical-inference.md#posterior-probability) of being below one half, draw the rate from its [gamma distribution](../../../continuous-probability-distribution.md#gamma-distribution) [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) and average an indicator. Rough [BUGS](../../../statistical-inference.md#bugs) code is
```
model {
  lambda ~ dgamma(a+n, b+T)
  q <- exp(-lambda)
  belowHalf <- step(lambda-log(2))
}
```
The monitored average of `belowHalf` estimates **$\mathbb P(\lambda>\log2\mid\mathcal D)$**, equivalently $1-F_{\operatorname{Gamma}(A,B)}(\log2)$. The equality boundary has zero probability. This code samples the already updated [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior); adding the count [likelihood function](../../../statistical-modelling.md#likelihood-function) again would count the data twice.

<h3 id="1/g">g</h3>

↑ **Parent:** [1](#1)

<h4 id="1/g/solution">Solution</h4>

↑ **Parent:** [G](#1/g)

For an [Inhomogeneous Poisson process](../../../probability-theory.md#inhomogeneous-poisson-process), the [likelihood function](../../../statistical-modelling.md#likelihood-function) is the product of the intensities at arrivals times the exponential of minus the integrated intensity. The integrated intensity is $\theta+2(T-\theta)=2T-\theta$. There are $j(\theta)$ arrivals at rate one and $n-j(\theta)$ at rate two, so

$$
\boxed{L(\theta)=e^{\theta-2T}2^{n-j(\theta)}\ \propto\ e^\theta2^{-j(\theta)},\qquad 0<\theta<T.}
$$

Set $t_0=0$ and $t_{n+1}=T$ to include changes before the first or after the last arrival. An arrival exactly at the change has probability zero, so the convention for $j$ at that point does not affect the [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior).

<h3 id="1/h">h</h3>

↑ **Parent:** [1](#1)

<h4 id="1/h/solution">Solution</h4>

↑ **Parent:** [H](#1/h)

A [uniform prior](../../../statistical-inference.md#uniform-prior) on $(0,T)$ makes the [posterior density](../../../statistical-inference.md#posterior-density) proportional to the [Poisson change-point posterior](../../../probability-and-statistics.md#poisson-change-point-posterior) likelihood above. The [zeros trick](../../../statistical-inference.md#zeros-trick) introduces an observed zero with [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) mean $K-\log L(\theta)$, making its [likelihood function](../../../statistical-modelling.md#likelihood-function) equal to $e^{-K}L(\theta)$. Choose $K=T+n\log2+1$; since $\log L(\theta)\le n\log2$, this mean is strictly positive. Rough [BUGS](../../../statistical-inference.md#bugs) code, with `zero=0` supplied as data, is
```
model {
  theta ~ dunif(0,T)
  for (i in 1:n) {
    before[i] <- step(theta-time[i])
  }
  j <- sum(before[])
  logL <- theta-2*T+(n-j)*log(2)
  zero ~ dpois(K-logL)
}
```
For $n=0$, omit the array and set `j <- 0`. Monitor the sampled `theta` to obtain its [posterior mean](../../../statistical-inference.md#posterior-mean), [credible interval](../../../statistical-inference.md#credible-interval) and interval probabilities.

There is also an exact sampling method. On $(t_j,t_{j+1})$ the [posterior density](../../../statistical-inference.md#posterior-density) is proportional to $2^{-j}e^\theta$, so choose the interval with weights

$$
w_j=2^{-j}(e^{t_{j+1}}-e^{t_j}),\qquad j=0,\ldots,n.
$$

Then draw $U$ from a [uniform distribution](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on $(0,1)$ and set $\theta=\log(e^{t_j}+U(e^{t_{j+1}}-e^{t_j}))$. **These weighted interval draws sample the posterior directly**, without asking a local [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) update to cross its discontinuities.

## 2

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For a regular one-parameter [sampling distribution](../../../statistical-modelling.md#sampling-distribution), the [Fisher information](../../../statistical-modelling.md#fisher-information-matrix) and [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) are

$$
I(\theta)=\mathbb E_\theta\left[\left(\frac{\partial}{\partial\theta}\log p_Y(Y\mid\theta)\right)^2\right],
\qquad \boxed{\pi_J(\theta)\propto\sqrt{I(\theta)}}.
$$

Under the usual differentiation and integrability conditions, $I(\theta)=-\mathbb E_\theta[\partial_\theta^2\log p_Y(Y\mid\theta)]$. This [prior distribution](../../../statistical-inference.md#prior-probability) transforms as a density under smooth one-to-one reparameterizations, so the rule is coordinate invariant. Its integral need not be finite; [posterior propriety](../../../statistical-inference.md#posterior-propriety) must still be established if it is an [improper prior](../../../statistical-inference.md#improper-prior).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For a [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution), the [score function](../../../statistical-modelling.md#informant-function) is

$$
\frac{Y}{\theta}-\frac{n-Y}{1-\theta}
=\frac{Y-n\theta}{\theta(1-\theta)}.
$$

Its squared [expected value](../../../probability-theory.md#expected-value) is $I(\theta)=n/[\theta(1-\theta)]$, using the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) [variance](../../../variance.md) $n\theta(1-\theta)$. Hence the [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) is

$$
\boxed{\pi_J(\theta)=\frac1{\pi\sqrt{\theta(1-\theta)}},\quad 0<\theta<1,}
$$

the [Beta distribution](../../../probability-theory.md#beta-distribution) $\operatorname{Beta}(1/2,1/2)$. The factor $\sqrt n$ is independent of $\theta$ and disappears on normalization.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Independent [Jeffreys priors](../../../statistical-modelling.md#jeffreys-prior) and the two independent [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) likelihood factors give, by [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy),

$$
\boxed{p_M\mid\mathcal D\sim\operatorname{Beta}(7/2,3/2),\qquad p_T\mid\mathcal D\sim\operatorname{Beta}(3/2,7/2).}
$$

The [Bayesian posteriors](../../../statistical-inference.md#bayesian-posterior) remain independent because each observation factor involves only its own probability. Their [posterior means](../../../statistical-inference.md#posterior-mean) are respectively **$0.7$ and $0.3$**. Notice that $p_T$ is the probability of saying milk first when tea was first, rather than the probability of a correct tea identification.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

In [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo), retain the derived quantity $\delta=p_M-p_T$ at every iteration. Rough [BUGS](../../../statistical-inference.md#bugs) code using the actual observations is
```
model {
  pM ~ dbeta(0.5,0.5)
  pT ~ dbeta(0.5,0.5)
  milkAnswers ~ dbin(pM,4)
  teaAnswers ~ dbin(pT,4)
  delta <- pM-pT
  positive <- step(delta)
}
```
Supply `milkAnswers=3` and `teaAnswers=1`. Summarize `delta` by its [posterior mean](../../../statistical-inference.md#posterior-mean), empirical [quantiles](../../../probability-theory.md#quantile-function) and [credible interval](../../../statistical-inference.md#credible-interval); the average of `positive` estimates $\mathbb P(p_M>p_T\mid\mathcal D)$. Here **$\mathbb E[\delta\mid\mathcal D]=0.4$**. Check [Markov chain Monte Carlo convergence diagnostics](../../../statistical-inference.md#markov-chain-monte-carlo-convergence-diagnostics) before interpreting the simulation. Since both [Bayesian posteriors](../../../statistical-inference.md#bayesian-posterior) are independent known [Beta distributions](../../../probability-theory.md#beta-distribution), direct independent sampling is an equally valid, simpler way to obtain the same summaries.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/1">1</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/1/solution">Solution</h5>

↑ **Parent:** [1](#2/e/1)

Start with the [Beta distribution](../../../probability-theory.md#beta-distribution) draw in the [Beta-binomial exchangeable coupling](../../../statistical-inference.md#beta-binomial-exchangeable-coupling). Write $s=\alpha+\beta$ and

$$
m=\frac\alpha s,\qquad v=\frac{\alpha\beta}{s^2(s+1)}.
$$

These are the [expected value](../../../probability-theory.md#expected-value) and [variance](../../../variance.md) of $p_M$. The fixed $n$ in this coupling is a dependence parameter chosen by the investigator, not necessarily the observed number of cups. The four numbered stages together address the single printed correlation request.

<h4 id="2/e/2">2</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/2/solution">Solution</h5>

↑ **Parent:** [2](#2/e/2)

Conditional on $p_M$, the auxiliary [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) gives $\mathbb E[X/n\mid p_M]=p_M$ and $\operatorname{Var}(X/n\mid p_M)=p_M(1-p_M)/n$. Thus **large $n$ makes $X/n$ close to $p_M$**. The [law of total variance](../../../probability-theory.md#law-of-total-variance) also gives

$$
\operatorname{Var}(X)=n m(1-m)+n(n-1)v
=\frac{n\alpha\beta(s+n)}{s^2(s+1)}.
$$

The [latent variable](../../../statistical-modelling.md#latent-variable) encodes the first draw increasingly accurately.

<h4 id="2/e/3">3</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/3/solution">Solution</h5>

↑ **Parent:** [3](#2/e/3)

The next [Beta distribution](../../../probability-theory.md#beta-distribution) has conditional [expected value](../../../probability-theory.md#expected-value) and [variance](../../../variance.md)

$$
\mathbb E[p_T\mid X]=\frac{\alpha+X}{s+n},\qquad
\operatorname{Var}(p_T\mid X)=\frac{(\alpha+X)(\beta+n-X)}{(s+n)^2(s+n+1)}.
$$

For large $n$, its [expected value](../../../probability-theory.md#expected-value) approaches $X/n$, while its [variance](../../../variance.md) is at most $1/[4(s+n+1)]$. The final draw therefore stays close to the first. These are [prior distributions](../../../statistical-inference.md#prior-probability) for the cup probabilities: the auxiliary count is a device for constructing dependence, rather than additional observed tea data.

<h4 id="2/e/4">4</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/4/solution">Solution</h5>

↑ **Parent:** [4](#2/e/4)

The [law of iterated expectation](../../../measure-theory.md#law-of-total-expectation) yields

$$
\mathbb E[p_T\mid p_M]=\frac{\alpha+n p_M}{s+n},\qquad
\operatorname{Cov}(p_M,p_T)=\frac n{s+n}v.
$$

One may obtain $\operatorname{Var}(p_T)=v$ either from its unchanged [marginal distribution](../../../probability-theory.md#marginal-distribution) proved below or directly from the [law of total variance](../../../probability-theory.md#law-of-total-variance): the variance of its conditional mean is $nv/(s+n)$ and its expected conditional variance is $sv/(s+n)$. Hence the [correlation coefficient](../../../variance.md#pearson-correlation-coefficient) is exactly

$$
\boxed{\operatorname{Corr}(p_M,p_T)=\frac n{n+\alpha+\beta}\longrightarrow1.}
$$

Also $\mathbb E[(p_T-p_M)^2]=2v s/(s+n)\to0$. **The two probabilities become close while keeping their original beta marginals.**

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Apply the [law of iterated expectation](../../../measure-theory.md#law-of-total-expectation) to the auxiliary [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution):

$$
\boxed{\mathbb E[X]=\mathbb E[\mathbb E[X\mid p_M]]=n\mathbb E[p_M]=\frac{n\alpha}{\alpha+\beta}.}
$$

This expectation is over the full [prior distribution](../../../statistical-inference.md#prior-probability) construction, not over a particular observed auxiliary count.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

Using the conditional [Beta distribution](../../../probability-theory.md#beta-distribution) [expected value](../../../probability-theory.md#expected-value) and the [law of iterated expectation](../../../measure-theory.md#law-of-total-expectation),

$$
\mathbb E[p_T]=\mathbb E\left[\frac{\alpha+X}{s+n}\right]
=\frac{\alpha+n\alpha/s}{s+n}
=\boxed{\frac\alpha{\alpha+\beta}}.
$$

Equality of the [expected values](../../../probability-theory.md#expected-value) alone does not prove equality of the [marginal distributions](../../../probability-theory.md#marginal-distribution); the later [exchangeability](../../../probability-theory.md#exchangeable-random-variables) argument does.

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

Multiply the [Beta distribution](../../../probability-theory.md#beta-distribution) density of $p_M$, the conditional [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) mass of $X$, and the conditional [Beta distribution](../../../probability-theory.md#beta-distribution) density of $p_T$. With $B(a,b)$ the [beta function](../../../complex-analysis.md#beta-function), the full joint density, relative to counting measure in $x$ and Lebesgue measure in the two probabilities, is

$$
\boxed{f(p_T,x,p_M)=\frac{\binom nx}{B(\alpha,\beta)B(\alpha+x,\beta+n-x)}
(p_Tp_M)^{\alpha+x-1}[(1-p_T)(1-p_M)]^{\beta+n-x-1}.}
$$

Here $x=0,\ldots,n$ and both probabilities lie in $(0,1)$. **The printed joint expression omits the factor $1/B(\alpha+x,\beta+n-x)$.** It is a constant when $x$ is fixed and only the two probabilities vary, but is not a constant for the full [joint probability distribution](../../../probability-theory.md#joint-probability-distribution). Keeping it is essential when summing over the [latent variable](../../../statistical-modelling.md#latent-variable).

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

Two [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables) satisfy $(X,Y)\overset d=(Y,X)$: their [joint probability distribution](../../../probability-theory.md#joint-probability-distribution) is unchanged by swapping the coordinates. Thus for every measurable set $A$,

$$
\mathbb P(X\in A)=\mathbb P((X,Y)\in A\times\mathcal Y)
=\mathbb P((Y,X)\in A\times\mathcal Y)=\mathbb P(Y\in A).
$$

**[Exchangeability](../../../probability-theory.md#exchangeable-random-variables) implies identical [marginal distributions](../../../probability-theory.md#marginal-distribution)**, but does not imply [independence](../../../random-variable.md#independent-random-variables).

<h3 id="2/j">j</h3>

↑ **Parent:** [2](#2)

<h4 id="2/j/solution">Solution</h4>

↑ **Parent:** [J](#2/j)

For each auxiliary count $x$, the correctly normalized joint expression above is symmetric in $p_M,p_T$. Summing it over $x=0,\ldots,n$ preserves that symmetry, so these are [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables). Their [marginal distributions](../../../probability-theory.md#marginal-distribution) are therefore identical. Since $p_M$ was generated from a [Beta distribution](../../../probability-theory.md#beta-distribution),

$$
\boxed{p_T\sim\operatorname{Beta}(\alpha,\beta).}
$$

The [Beta-binomial exchangeable coupling](../../../statistical-inference.md#beta-binomial-exchangeable-coupling) changes the dependence, while leaving both [prior distributions](../../../statistical-inference.md#prior-probability) unchanged.

<h2 id="3">3</h2>

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

At zero a centered [normal distribution](../../../probability-theory.md#normal-distribution) with [standard deviation](../../../variance.md#standard-deviation) $\sigma$ has density $1/(\sqrt{2\pi}\sigma)$. The two prior standard deviations are $1/\sqrt{n_0}$ and $c/\sqrt{n_0}$, giving

$$
\boxed{p_0(0)/p_1(0)=c.}
$$

The wider [prior distribution](../../../statistical-inference.md#prior-probability) has a lower density at its center.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $q_0=n_0$, $q_1=n_0/c^2$ and $y=\overline y$. These are the two prior [precision parameters](../../../statistical-modelling.md#precision-parameter). Completing the square in $n(\beta-y)^2+q_i\beta^2$ gives the [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) update

$$
\boxed{\beta\mid y,H_i\sim N\left(\frac{n}{n+q_i}y,\frac1{n+q_i}\right),\qquad i=0,1.}
$$

Thus the [posterior mean](../../../statistical-inference.md#posterior-mean) is a precision-weighted average of the observed mean and the prior center zero. The [posterior variance](../../../statistical-inference.md#posterior-variance) is the reciprocal of the total precision.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $\overline Y=\beta+\varepsilon$, with independent $\varepsilon\sim N(0,1/n)$ and $\beta\mid H_i\sim N(0,1/q_i)$. The [convolution of independent random variables](../../../probability-theory.md#convolution-of-independent-random-variables) is again a [normal distribution](../../../probability-theory.md#normal-distribution), so the prior predictive laws are

$$
\boxed{\overline Y\mid H_i\sim N(0,V_i),\qquad V_i=1/n+1/q_i.}
$$

These are predictive distributions before observing $y$, hence the [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence) for the observed mean. The residual information in the original observations is common to both models and cancels in their [Bayes factor](../../../statistical-inference.md#bayes-factor).

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Divide the two [normal distribution](../../../probability-theory.md#normal-distribution) predictive densities to obtain the [Bayes factor](../../../statistical-inference.md#bayes-factor)

$$
\boxed{B_{01}(y)=\sqrt{\frac{V_1}{V_0}}\exp\left[-\frac{y^2}{2}\left(\frac1{V_0}-\frac1{V_1}\right)\right].}
$$

At $y=0$ this becomes

$$
\boxed{B_{01}(0)=\sqrt{\frac{n_0/n+c^2}{n_0/n+1}}.}
$$

The wider [prior distribution](../../../statistical-inference.md#prior-probability) spreads its predictive mass over more possible means, giving the narrower model more [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence) for observations very near zero. Away from zero, the exponential term opposes that factor.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Under the point hypothesis $\beta=0$, the [test statistic](../../../statistical-modelling.md#test-statistic) $\sqrt n\,\overline Y$ has a standard [normal distribution](../../../probability-theory.md#normal-distribution). The observed statistic is three, giving a two-sided [p-value](../../../statistical-modelling.md#p-value) $2[1-\Phi(3)]\simeq0.00270$. This is conventionally strong evidence against that point hypothesis. The narrow model $H_0$ is a continuous [prior distribution](../../../statistical-inference.md#prior-probability) around zero, rather than a point hypothesis.

For $n_0/n=100$ and $c=100$, [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
\boxed{\beta\mid y,H_0\sim N\left(\frac{3}{101\sqrt n},\frac1{101n}\right),\qquad
\beta\mid y,H_1\sim N\left(\frac{300}{101\sqrt n},\frac{100}{101n}\right).}
$$

The narrow-model [posterior mean](../../../statistical-inference.md#posterior-mean) is strongly pulled toward zero and its [standard deviation](../../../variance.md#standard-deviation) is about $0.0995/\sqrt n$. The wide-model [posterior mean](../../../statistical-inference.md#posterior-mean) is about $2.9703/\sqrt n$, very close to the observation, with [standard deviation](../../../variance.md#standard-deviation) about $0.9950/\sqrt n$. **Each model produces a markedly different posterior**, so choosing between them requires their predictive evidence.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

**The requested conclusion is false for the printed parameter values.** They give $V_0=1.01/n$ and $V_1=101/n$. Substituting $y=3/\sqrt n$ in the [Bayes factor](../../../statistical-inference.md#bayes-factor) yields

$$
\boxed{B_{01}=10\exp\left(-\frac{891}{202}\right)\simeq0.12144<1.}
$$

Thus **the Bayes factor favours $H_1$ by about $8.23$ to one**, not $H_0$. Nor does the conclusion hold for arbitrary large $n_0,c$: both parameters enter the expression explicitly. With $n_0/n=100$, taking a much wider alternative, for example $c=1000$, would instead give $B_{01}\simeq1.1563>1$. That is a different prior assumption and cannot repair the printed calculation silently.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

With equal model [prior probabilities](../../../statistical-inference.md#prior-probability), [Bayes factor](../../../statistical-inference.md#bayes-factor) updating gives $w_0=B_{01}/(1+B_{01})$ and $w_1=1/(1+B_{01})$. The [Bayesian model averaging](../../../statistical-inference.md#bayesian-model-averaging) [posterior density](../../../statistical-inference.md#posterior-density) is therefore

$$
\boxed{p(\beta\mid y)=\frac{B_{01}}{1+B_{01}}p_0(\beta\mid y)+\frac1{1+B_{01}}p_1(\beta\mid y).}
$$

This is a two-component [mixture model](../../../statistical-modelling.md#mixture-model) of the [normal distributions](../../../probability-theory.md#normal-distribution) already derived. For the numerical observation above, **$w_0\simeq0.10829$ and $w_1\simeq0.89171$**. Consequently it is predominantly the wide-model posterior, not predominantly the narrow one.

<h3 id="3/h">h</h3>

↑ **Parent:** [3](#3)

<h4 id="3/h/solution">Solution</h4>

↑ **Parent:** [H](#3/h)

Put $\kappa_i=n/(n+q_i)$. The [posterior mean](../../../statistical-inference.md#posterior-mean) of the [Gaussian practical-null mixture](../../../statistical-inference.md#gaussian-practical-null-mixture) is

$$
\mathbb E[\beta\mid y]=[w_0(y)\kappa_0+w_1(y)\kappa_1]y.
$$

Near zero, $B_{01}(0)>1$, so the narrow component has high [posterior probability](../../../statistical-inference.md#posterior-probability) and $\kappa_0$ is small when $n_0\gg n$. This pulls the [Bayesian model averaging](../../../statistical-inference.md#bayesian-model-averaging) posterior toward zero. For the given ratios, writing $z=\sqrt n\,y$ gives

$$
B_{01}(y)=10e^{-99z^2/202},\qquad B_{01}>1\ \Longleftrightarrow\ |z|<2.16753\ldots.
$$

Thus the order statement $y=O(n^{-1/2})$ alone does not guarantee strong pull toward zero: $z=3$ already has the opposite model preference.

As $|y|$ grows, $V_1>V_0$ makes $B_{01}(y)\to0$, and the [mixture model](../../../statistical-modelling.md#mixture-model) approaches $N(\kappa_1 y,1/(n+q_1))$. **Its center is exactly $\kappa_1 y$, and approximately $y$ only for a sufficiently diffuse wide prior**, meaning $q_1\ll n$. Here $\kappa_1=100/101$, so the relative displacement is about one percent. Large observations alone do not remove this finite-prior shrinkage.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

In a [normal linear model](../../../statistical-modelling.md#normal-linear-model), attach a [continuous spike-and-slab prior](../../../statistical-inference.md#continuous-spike-and-slab-prior) to each [regression coefficient](../../../linear-regression.md#regression-coefficient). With suitably scaled predictors, introduce indicators $\gamma_j\sim\operatorname{Bernoulli}(\pi)$ and set

$$
\beta_j\mid\gamma_j=0\sim N(0,s_{0j}^2),\qquad
\beta_j\mid\gamma_j=1\sim N(0,s_{1j}^2),\quad s_{0j}\ll s_{1j}.
$$

The narrow component describes practically negligible effects; the wide component permits substantial ones. Fit the joint [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior) of coefficients, indicators and any unknown residual variance. [Bayesian model averaging](../../../statistical-inference.md#bayesian-model-averaging) gives shrinkage toward zero for poorly supported effects, while $\mathbb P(\gamma_j=1\mid\mathcal D)$ quantifies wide-component support. A shared [Beta distribution](../../../probability-theory.md#beta-distribution) prior on $\pi$ can represent uncertainty about how many effects are substantial.

**Select on scientifically meaningful effect size**, for example a high $\mathbb P(|\beta_j|>\delta_j\mid\mathcal D)$ for a prechosen threshold in meaningful predictor units. Membership in the wide component alone does not imply a large realized effect: its [normal distribution](../../../probability-theory.md#normal-distribution) still permits values near zero. Correlated predictors also require interpretation of the joint [Bayesian posterior](../../../statistical-inference.md#bayesian-posterior), rather than treating each coefficient as an isolated test.

<h2 id="4">4</h2>

↑ **Parent:** [Paper 35](paper-35.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

The [log odds ratio](../../../statistical-modelling.md#log-odds-ratio) for treatment relative to control is the difference of the two [log odds](../../../statistical-modelling.md#log-odds):

$$
\log\frac{\theta_T/(1-\theta_T)}{\theta_C/(1-\theta_C)}
=(\alpha+\beta/2)-(\alpha-\beta/2)=\boxed{\beta}.
$$

Thus the treatment-to-control [odds ratio](../../../statistical-modelling.md#odds-ratio) is **$e^\beta$**. Its direction refers to whatever event the binomial count records.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The intercept is the midpoint of the two [log odds](../../../statistical-modelling.md#log-odds):

$$
\boxed{\alpha=\tfrac12[\operatorname{logit}\theta_C+\operatorname{logit}\theta_T].}
$$

Equivalently $e^\alpha$ is the geometric mean of the two odds. The [logistic function](../../../statistical-learning.md#logistic-function) evaluated at $\alpha$ represents a central event probability, and approximates the average of the two group probabilities when $\beta$ is small. **It is not generally their arithmetic average**, nor is $\alpha$ specifically the control-group [log odds](../../../statistical-modelling.md#log-odds).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Use a proper [normal distribution](../../../probability-theory.md#normal-distribution) prior centered at zero on the [log odds ratio](../../../statistical-modelling.md#log-odds-ratio). For example,

$$
\boxed{\beta\sim N(0,1)}
$$

puts approximately 95 percent of its mass between $-2$ and $2$, giving [odds ratios](../../../statistical-modelling.md#odds-ratio) roughly between $e^{-2}$ and $e^2$, close to $1/8$ and $8$. Centering at zero treats reciprocal [odds ratios](../../../statistical-modelling.md#odds-ratio) symmetrically. If the desired central 95 percent interval is exactly $(1/8,8)$, use [standard deviation](../../../variance.md#standard-deviation) $\log8/\Phi^{-1}(0.975)\simeq1.0610$. **A soft prior is appropriate for implausibility**, whereas a bounded [uniform prior](../../../statistical-inference.md#uniform-prior) would declare effects outside the limits impossible.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Calling the effects [exchangeable random variables](../../../probability-theory.md#exchangeable-random-variables) means that their joint [prior distribution](../../../statistical-inference.md#prior-probability) is unchanged by permuting study labels. In a [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model), conditional independent draws $\beta_j\mid\mu,\tau\sim N(\mu,\tau^2)$ achieve this, and integrating shared [hyperparameters](../../../statistical-inference.md#hyperparameter) induces dependence between studies. This permits [partial pooling](../../../statistical-inference.md#partial-pooling) without asserting that all effects are identical.

The assumption is reasonable when the studies concern comparable treatments, populations, outcomes and follow-up, and no known study characteristic gives one effect a systematically different prior center. Relevant differences can instead enter a [linear regression](../../../linear-regression.md) for study effects, after which the residual effects may be exchangeable. **The numerical table counts deaths**, so its event probabilities are mortality probabilities and $\beta_j<0$ indicates a lower mortality [odds ratio](../../../statistical-modelling.md#odds-ratio). Interpreting those counts as beneficial responses would reverse the clinical meaning.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

The overall mean $\mu$ and the [between-study heterogeneity](../../../statistical-inference.md#between-study-heterogeneity) $\tau$ encode different information. A proper broad [normal distribution](../../../probability-theory.md#normal-distribution) prior such as $\mu\sim N(0,2^2)$ is one possible weak prior for the mean [log odds ratio](../../../statistical-modelling.md#log-odds-ratio); information about the spread of trials alone does not determine its center.

A concrete [prior calibration for normal random-effect range](../../../statistical-inference.md#prior-calibration-for-normal-random-effect-range) can make the factor-of-50 statement simultaneous across all six trials. Conditional on $\tau$, each pair difference has [normal distribution](../../../probability-theory.md#normal-distribution) $\beta_j-\beta_k\sim N(0,2\tau^2)$. Set $R=\log50$, $m=\binom62=15$, $z=\Phi^{-1}(1-0.05/(2m))$ and

$$
\boxed{\tau\sim\operatorname{Uniform}(0,A),\qquad A=\frac{R}{\sqrt2\,z}\simeq0.9424.}
$$

For every $\tau\le A$, each pair exceeds $R$ in absolute value with probability at most $0.05/m$. The [union bound](../../../probability-inequality.md#boole-s-inequality) therefore gives $\mathbb P(\max_j\beta_j-\min_j\beta_j>R)\le0.05$, and integrating over the [uniform prior](../../../statistical-inference.md#uniform-prior) preserves that bound. This is one explicit interpretation of “very unlikely”; a different elicited probability would change the bound. A smoother proper scale prior could be calibrated similarly.

The proposed $1/\tau$ [improper prior](../../../statistical-inference.md#improper-prior) is unsuitable. The observed-data [likelihood function](../../../statistical-modelling.md#likelihood-function) approaches the positive common-effect likelihood as $\tau\downarrow0$. After restricting $\mu$ and the intercepts to a compact interior region, it is bounded below there by a positive constant. Hence

$$
\int_0^\varepsilon L(\mu,\tau)\frac{d\tau}{\tau}=\infty.
$$

This is an [improper posterior from a log-uniform random-effect scale prior](../../../statistical-inference.md#improper-posterior-from-a-log-uniform-random-effect-scale-prior). **Proper conditional sampling distributions do not repair the improper joint posterior**, and an arbitrary tiny cutoff would make inference depend on that cutoff.

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Represent the independent locally flat intercept [prior distributions](../../../statistical-inference.md#prior-probability) by broad finite [uniform priors](../../../statistical-inference.md#uniform-prior), for example on $(-10,10)$; this is proper and approximately constant over plausible mortality logits. With $A$ calibrated above, rough [BUGS](../../../statistical-inference.md#bugs) code is
```
model {
  mu ~ dnorm(0,0.25)
  tau ~ dunif(0,A)
  invtau2 <- pow(tau,-2)
  for (j in 1:J) {
    alpha[j] ~ dunif(-10,10)
    beta[j] ~ dnorm(mu,invtau2)
    logit(thetaC[j]) <- alpha[j]-beta[j]/2
    logit(thetaT[j]) <- alpha[j]+beta[j]/2
    rC[j] ~ dbin(thetaC[j],nC[j])
    rT[j] ~ dbin(thetaT[j],nT[j])
    oddsRatio[j] <- exp(beta[j])
  }
}
```
Use $J=6$ and supply treated death counts $(3,7,5,102,32,22)$ with totals $(38,114,69,1533,209,680)$, and control death counts $(3,14,11,127,40,39)$ with totals $(39,116,93,1520,218,674)$. In [BUGS](../../../statistical-inference.md#bugs), the second `dnorm` argument is a [precision parameter](../../../statistical-modelling.md#precision-parameter), so `0.25` corresponds to [variance](../../../variance.md) four. Initialize the positive scale away from zero. Monitor $\mu,\tau$ and study [odds ratios](../../../statistical-modelling.md#odds-ratio), checking [Markov chain Monte Carlo convergence diagnostics](../../../statistical-inference.md#markov-chain-monte-carlo-convergence-diagnostics) and sensitivity to the finite intercept bounds and scale [prior distribution](../../../statistical-inference.md#prior-probability). **The fitted hierarchy combines binomial sampling uncertainty with between-study heterogeneity.**

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

For the common [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) convention $D=-2\log L$ used in all three models,

$$
p_D=\overline D-D(\overline\theta),\qquad
\operatorname{DIC}=\overline D+p_D=D(\overline\theta)+2p_D.
$$

Here `Dhat` is $D(\overline\theta)$, an at-posterior-mean fit measure, and $p_D$ is an effective parameter count. The independent model's `Dhat` of 53.1 is almost identical to the exchangeable model's 53.2; both improve on the common model's 57.8. The common model's $p_D=7$ corresponds to six intercepts plus one shared effect. Independence uses roughly twelve effective parameters. [Partial pooling](../../../statistical-inference.md#partial-pooling) reduces the exchangeable model's effective complexity to about 8.7 while retaining nearly the same fitted [likelihood function](../../../statistical-modelling.md#likelihood-function) as independence.

**The exchangeable model has the lowest reported DIC, but the common model is competitive.** Their difference is only about 1.3, whereas independence is worse by about 6.3. The [deviance information criterion](../../../statistical-modelling.md#deviance-information-criterion) measures penalized fit for a predictive comparison, not model [posterior probabilities](../../../statistical-inference.md#posterior-probability), and these numbers do not establish overwhelming evidence for heterogeneity. The displayed exchangeable $\overline D+p_D$ is $61.9+8.7=70.6$, rather than the printed 70.5; rounding of the underlying values can account for a tenth and does not change this interpretation.

<h3 id="4/h">h</h3>

↑ **Parent:** [4](#4)

<h4 id="4/h/solution">Solution</h4>

↑ **Parent:** [H](#4/h)

Conditional on $\mu,\psi>0$, let $\lambda\sim\chi^2_4$ and independently $Z\sim N(0,1)$. The [normal distribution](../../../probability-theory.md#normal-distribution) with the stated [precision parameter](../../../statistical-modelling.md#precision-parameter) can be generated as

$$
\beta_j=\mu+\frac{2\psi Z}{\sqrt\lambda}.
$$

Therefore

$$
\boxed{\frac{\beta_j-\mu}{\psi}=\frac Z{\sqrt{\lambda/4}}\sim t_4,}
$$

by the defining [normal distribution](../../../probability-theory.md#normal-distribution) and [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) representation of [Student's t-distribution](../../../continuous-probability-distribution.md#student-s-t-distribution). Its density is

$$
f(\beta_j\mid\mu,\psi)=\frac3{8\psi}\left(1+\frac{(\beta_j-\mu)^2}{4\psi^2}\right)^{-5/2}.
$$

Thus **$\mu$ is the location and $\psi$ is the scale**, not the [standard deviation](../../../variance.md#standard-deviation): $\operatorname{Var}(\beta_j\mid\mu,\psi)=2\psi^2$. Each study gets its own independent chi-squared draw in this [Student t random-effect model](../../../statistical-inference.md#student-t-random-effect-model).

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

The [Student t random-effect model](../../../statistical-inference.md#student-t-random-effect-model) is useful when most studies are comparable but occasional genuine departures are more frequent than a [normal distribution](../../../probability-theory.md#normal-distribution) hierarchy allows. Its heavier tails permit a study effect far from $\mu$ without forcing a large common [between-study heterogeneity](../../../statistical-inference.md#between-study-heterogeneity) scale on every study. In the [Gaussian scale mixture](../../../statistical-modelling.md#gaussian-scale-mixture) representation, a small study-specific $\lambda_j$ lowers its [precision parameter](../../../statistical-modelling.md#precision-parameter) and weakens its shrinkage.

**Use this as robust partial pooling when occasional atypical effects are plausible.** Known systematic population or design differences should still be modeled explicitly; a heavy tail cannot identify or correct [within-study bias](../../../statistical-inference.md#within-study-bias) by itself.

<h3 id="4/j">j</h3>

↑ **Parent:** [4](#4)

<h4 id="4/j/solution">Solution</h4>

↑ **Parent:** [J](#4/j)

Fit both the normal and [Student t random-effect model](../../../statistical-inference.md#student-t-random-effect-model) with comparable proper [prior distributions](../../../statistical-inference.md#prior-probability). Compare priors on the same spread measure: a [normal distribution](../../../probability-theory.md#normal-distribution) scale $\tau$ is a [standard deviation](../../../variance.md#standard-deviation), whereas the $t_4$ [standard deviation](../../../variance.md#standard-deviation) is $\sqrt2\psi$.

Use a [posterior predictive check](../../../statistical-inference.md#posterior-predictive-check): draw study effects and binomial counts from each fitted hierarchy and compare replicated dispersion and extreme study contrasts with the observations. For predicting a new study, generate a new effect from the hierarchy rather than reusing an existing fitted effect. A [Leave-one-out cross-validation](../../../statistical-learning.md#leave-one-out-cross-validation) with entire studies held out can compare integrated predictive probabilities for both arms of each omitted trial, averaging over [hyperparameters](../../../statistical-inference.md#hyperparameter) and its unobserved study effect. [Leave-one-study-out influence analysis](../../../statistical-inference.md#leave-one-study-out-influence-analysis) also reveals whether the difference is driven by a single trial.

**Prefer the heavier-tailed hierarchy if it improves the relevant predictive checks and held-out study predictions robustly to reasonable prior choices.** The [deviance information criterion](../../../statistical-modelling.md#deviance-information-criterion) can supplement the comparison, but its effective parameter count can depend on the latent-variable representation, and six studies give limited information about tail shape. A small numerical criterion difference alone is insufficient evidence.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
