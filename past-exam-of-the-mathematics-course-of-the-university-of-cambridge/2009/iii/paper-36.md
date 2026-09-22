# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2009/Paper36.pdf)

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
  - [h](#3/h)
    - [Solution](#3/h/solution)
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

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [binomial likelihood](../../../discrete-probability-distribution.md#binomial-likelihood) is $p(x\mid\theta)=\binom mx\theta^x(1-\theta)^{m-x}$. Multiplication by the [Beta distribution](../../../probability-theory.md#beta-distribution) [prior density](../../../statistical-inference.md#prior-density) and [Bayes' theorem](../../../probability-theory.md#bayes-theorem) give the [posterior density](../../../statistical-inference.md#posterior-density) kernel $\theta^{a+x-1}(1-\theta)^{b+m-x-1}$. Normalizing by the [beta function](../../../complex-analysis.md#beta-function) yields [Beta-binomial conjugacy](../../../statistical-inference.md#beta-binomial-conjugacy):

$$
\boxed{\theta\mid x\sim\operatorname{Beta}(a+x,b+m-x).}
$$

This is proper for $a,b>0$ and $0\leq x\leq m$, including counts at either boundary.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

For the $m$ independent [Bernoulli trials](../../../discrete-probability-distribution.md#bernoulli-trial), the log [likelihood function](../../../statistical-modelling.md#likelihood-function), apart from its constant, is $\ell(\theta)=x\log\theta+(m-x)\log(1-\theta)$. Its negative expected second derivative, the [Fisher information](../../../statistical-modelling.md#fisher-information-matrix), is

$$
I_m(\theta)=\frac{\mathbb E[X]}{\theta^2}+\frac{m-\mathbb E[X]}{(1-\theta)^2}
=\frac{m}{\theta(1-\theta)}.
$$

For $m>0$, the [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) is proportional to its square root. Since $\mathrm B(1/2,1/2)=\pi$, its normalized form is

$$
\boxed{\pi_J(\theta)=\frac1{\pi\sqrt{\theta(1-\theta)}},\qquad
\theta\sim\operatorname{Beta}(1/2,1/2).}
$$

The [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior) is invariant under smooth one-to-one reparameterization as a measure. If $\phi=h(\theta)$, then $I_\phi(\phi)=I_\theta(\theta)(d\theta/d\phi)^2$, so $\sqrt{I_\phi}\,d\phi=\sqrt{I_\theta}\,|d\theta|$. Thus recomputing it in the new coordinate gives precisely the transformed prior, rather than a new prior. In several dimensions the corresponding density is $\sqrt{\det I(\theta)}$, with the same Jacobian transformation property.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $\alpha=a+x$, $\beta=b+m-x$, and $S=\alpha+\beta=m+a+b$. Integrate the future [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) against the current [Beta distribution](../../../probability-theory.md#beta-distribution) [posterior density](../../../statistical-inference.md#posterior-density):

$$
p(y\mid x)=\binom ny\frac{\mathrm B(\alpha+y,\beta+n-y)}{\mathrm B(\alpha,\beta)},\qquad y=0,\ldots,n.
$$

This is the [beta-binomial distribution](../../../statistical-inference.md#beta-binomial-distribution). For positive integer $a,b$, the [gamma function](../../../complex-analysis.md#gamma-function) values reduce to factorials, giving

$$
p(y\mid x)=\frac{n!}{y!(n-y)!}
\frac{(\alpha+y-1)!(\beta+n-y-1)!(S-1)!}
{(\alpha-1)!(\beta-1)!(S+n-1)!}.
$$

Using $(S-1)!=(S-1)(S-2)!$ and $(S+n-1)!=(S+n-1)(S+n-2)!$ rewrites this as

$$
\boxed{p(y\mid x)=\frac{S-1}{S+n-1}
\frac{\binom{\alpha+y-1}{y}\binom{\beta+n-y-1}{n-y}}
{\binom{S+n-2}{n}}.}
$$

Substitution of $\alpha,\beta,S$ gives exactly the two required factors. The probability is zero outside $0\leq y\leq n$.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

With a uniform [Beta distribution](../../../probability-theory.md#beta-distribution) [prior](../../../statistical-inference.md#prior-probability), the [posterior predictive distribution](../../../statistical-inference.md#posterior-predictive-distribution) for another batch of the same size is

$$
p(y\mid x)=\binom my
\frac{\mathrm B(x+y+1,2m-x-y+1)}{\mathrm B(x+1,m-x+1)}.
$$

But $\mathrm B(x+1,m-x+1)=1/[(m+1)\binom mx]$. Hence

$$
\boxed{p(y\mid x)=(m+1)\binom mx\binom my\,
\mathrm B(x+y+1,2m-x-y+1)=p(x\mid y).}
$$

The displayed expression is symmetric in $x,y$. This is the [uniform-count predictive property](../../../statistical-inference.md#uniform-count-predictive-property): the joint batch counts are exchangeable and both marginal counts are uniform. Conditional reversal is not a general property of arbitrary priors; it holds here because those marginal probabilities coincide.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Before collecting any observations, a uniform success-chance [prior distribution](../../../statistical-inference.md#prior-probability) gives

$$
\Pr(Y=y)=\binom ny\int_0^1\theta^y(1-\theta)^{n-y}\,d\theta
=\binom ny\mathrm B(y+1,n-y+1)
=\boxed{\frac1{n+1}},\qquad y=0,\ldots,n.
$$

Thus the [uniform-count predictive property](../../../statistical-inference.md#uniform-count-predictive-property) assigns equal probability to every possible number of successes in a fixed-size batch under the [prior predictive distribution](../../../statistical-inference.md#bayesian-model-evidence). It is uniform over counts, not over all ordered binary sequences. After observing $x$ successes in $m$ trials, its familiar one-step [posterior predictive probability](../../../statistical-inference.md#posterior-predictive-probability) is $(x+1)/(m+2)$; the count-uniform property refers to prediction before those data are observed.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

For the uniform [prior](../../../statistical-inference.md#prior-probability), write $s=x+y$ for the pooled success count in $m+n$ trials. Conditional on $s$, exchangeability makes all placements of the successes equally likely. The successes in the second batch therefore have a [hypergeometric distribution](../../../discrete-probability-distribution.md#hypergeometric-distribution), and the factor in question is

$$
B=\frac{\binom{s}{y}\binom{m+n-s}{n-y}}{\binom{m+n}{n}}
=\Pr(Y=y\mid X+Y=s)\quad\text{at }s=x+y.
$$

This is [hypergeometric allocation of exchangeable Bernoulli counts](../../../statistical-inference.md#hypergeometric-allocation-of-exchangeable-bernoulli-counts): sample $n$ positions without replacement from a population of $m+n$ positions containing $s$ successes. The [uniform-count predictive property](../../../statistical-inference.md#uniform-count-predictive-property) gives $\Pr(X+Y=s)=1/(m+n+1)$ and $\Pr(X=x)=1/(m+1)$, so

$$
\boxed{\Pr(Y=y\mid X=x)=\frac{m+1}{m+n+1}\,B.}
$$

As $y$ varies with $x$ fixed, $s=x+y$ also varies. Therefore $B$ alone is not a normalized [hypergeometric distribution](../../../discrete-probability-distribution.md#hypergeometric-distribution) over $y$; its normalization factor is essential.

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Under the [discrete uniform distribution](../../../discrete-probability-distribution.md#discrete-uniform-distribution), the observation has probability $1/N$ when its value is an available label, and zero otherwise. Therefore the [likelihood function](../../../statistical-modelling.md#likelihood-function) is

$$
\boxed{L(N;y)=\frac1N\mathbf1_{\{N\geq y\}},\qquad N\in\{1,2,\ldots\}.}
$$

This is the [discrete uniform endpoint posterior](../../../statistical-inference.md#discrete-uniform-endpoint-posterior) model's likelihood; all endpoints smaller than the observed label are excluded.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

On its admissible support the [likelihood function](../../../statistical-modelling.md#likelihood-function) $1/N$ strictly decreases. Its [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) is consequently the smallest admissible endpoint:

$$
\boxed{\widehat N_{\mathrm{ML}}=y=100.}
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

A constant [improper prior](../../../statistical-inference.md#improper-prior) would give the formal [posterior density](../../../statistical-inference.md#posterior-density) kernel $N^{-1}\mathbf1_{\{N\geq y\}}$. However,

$$
\sum_{N=y}^{\infty}\frac1N=\infty.
$$

**There is no normalized posterior distribution under this prior.** The failure is not simply that the [prior](../../../statistical-inference.md#prior-probability) is improper: some improper priors give proper posteriors. Here [posterior propriety](../../../statistical-inference.md#posterior-propriety) itself fails after this single observation, so probabilities, quantiles and a [posterior mean](../../../statistical-inference.md#posterior-mean) cannot be assigned to that kernel.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Write $H_k=\sum_{j=1}^k1/j$, with $H_0=0$. The truncated uniform [prior](../../../statistical-inference.md#prior-probability) gives the [posterior distribution](../../../statistical-inference.md#bayesian-posterior)

$$
p(N\mid y,M)=\frac{N^{-1}}{H_M-H_{y-1}},\qquad y\leq N\leq M.
$$

Its [posterior mean](../../../statistical-inference.md#posterior-mean) is

$$
\boxed{\mathbb E[N\mid y,M]=\frac{M-y+1}{H_M-H_{y-1}}.}
$$

Each term in the numerator of the expectation is $N/N=1$, which explains the exact count $M-y+1$.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Keep $y$ fixed. Integral bounds for the decreasing function $1/t$ give $H_M=\log M+O(1)$, so $H_M-H_{y-1}=\log M+O_y(1)$. Consequently

$$
\boxed{\mathbb E[N\mid y,M]\frac{\log M}{M}
=\frac{M-y+1}{M}\frac{\log M}{H_M-H_{y-1}}\longrightarrow1.}
$$

The [posterior mean](../../../statistical-inference.md#posterior-mean) thus grows like $M/\log M$ instead of approaching a data-determined limit. Even the [posterior distribution](../../../statistical-inference.md#bayesian-posterior) mass below a fixed endpoint $n$ is $(H_n-H_{y-1})/(H_M-H_{y-1})\to0$. Hence increasing the supposedly innocuous prior cutoff moves the inference to larger and larger endpoints. In an integral approximation its median is of order $\sqrt{yM}$, also depending strongly on the cutoff. This explains the sensitivity of the entire inference, not just of its [posterior mean](../../../statistical-inference.md#posterior-mean).

<h3 id="2/f">f</h3>

↑ **Parent:** [2](#2)

<h4 id="2/f/solution">Solution</h4>

↑ **Parent:** [F](#2/f)

Multiplying the reciprocal [improper prior](../../../statistical-inference.md#improper-prior) by the [likelihood function](../../../statistical-modelling.md#likelihood-function) gives

$$
p(N\mid y)=\frac{N^{-2}}{S_y},\qquad N\geq y,
\qquad S_y=\sum_{k=y}^{\infty}k^{-2}<\infty.
$$

Thus this [discrete uniform endpoint posterior](../../../statistical-inference.md#discrete-uniform-endpoint-posterior) is proper. Its exact cumulative probability is $S_y^{-1}\sum_{k=y}^n k^{-2}$. Integral approximation gives $S_y\approx\int_y^\infty t^{-2}\,dt=1/y$ and $\sum_{k=y}^n k^{-2}\approx\int_y^n t^{-2}\,dt=1/y-1/n$, so

$$
\boxed{\Pr(N\leq n\mid y)\approx1-\frac yn,\qquad
\operatorname{median}(N\mid y)\approx2y=200.}
$$

These approximations are useful when $y$ is moderately large and are not exact discrete identities. For example the exact untruncated median at $y=100$ is $199$. Although its [quantiles](../../../probability-theory.md#quantile-function) are finite, its [posterior mean](../../../statistical-inference.md#posterior-mean) is infinite, since its expectation numerator is the divergent sum $\sum_{N=y}^\infty1/N$.

<h3 id="2/g">g</h3>

↑ **Parent:** [2](#2)

<h4 id="2/g/solution">Solution</h4>

↑ **Parent:** [G](#2/g)

The [WinBUGS](../../../statistical-inference.md#winbugs) model uses a finite truncation of the reciprocal [prior](../../../statistical-inference.md#prior-probability). The numbered lines have the following roles:

- Line (1) forms $p_j=(1/j)/H_{5000}$, the normalized prior probability vector on the integer labels $1,\ldots,5000$. The deterministic sum may be declared after its use because the model is declarative.
- Line (2) assigns $N$ that [categorical distribution](../../../discrete-probability-distribution.md#categorical-distribution). The following observation model treats the supplied value $y=100$ as observed data, rather than as an unknown parameter.
- Line (3) forms observation probabilities $p[j]=1/N$ for $j\leq N$ and zero for $j>N$. For integer $N,j$, the small positive offset in `step(N-j+0.01)` includes the endpoint $j=N$ without depending on the convention at zero. There are exactly $N$ nonzero entries, so this vector sums to one.

Combining that [categorical distribution](../../../discrete-probability-distribution.md#categorical-distribution) observation likelihood with the truncated reciprocal [prior](../../../statistical-inference.md#prior-probability) produces

$$
\boxed{p(N\mid y)\propto N^{-2}\mathbf1_{\{y\leq N\leq5000\}}.}
$$

The [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) output approximates this posterior. The actual PDF separates the observation line from the preceding comment; it must remain an active stochastic statement.

<h3 id="2/h">h</h3>

↑ **Parent:** [2](#2)

<h4 id="2/h/solution">Solution</h4>

↑ **Parent:** [H](#2/h)

The [posterior distribution](../../../statistical-inference.md#bayesian-posterior) has a long right tail. Its [posterior mean](../../../statistical-inference.md#posterior-mean) is pulled upward by relatively rare large endpoints and is sensitive to the artificial upper cutoff; its untruncated [posterior mean](../../../statistical-inference.md#posterior-mean) does not exist. The median is a central [quantile](../../../probability-theory.md#quantile-function) that stays finite as the cutoff is removed and is much less sensitive to extreme draws. It is also the [Bayes estimator](../../../statistical-inference.md#bayes-estimator) under absolute-error loss, whereas a mean corresponds to squared-error loss when the relevant expectation exists.

**The median better represents the typical posterior endpoint in this strongly right-skewed distribution.** It need not be preferable for every decision problem, since the loss function matters. For comparison, exact summation of the truncated kernel at cutoff $5000$ gives median $195$ and mean about $397.67$; the displayed simulation summaries are Monte Carlo estimates, not exact posterior calculations.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

At several doses the three replicate plates differ much more than the square-root-of-mean scale expected from a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution). For example the group at dose $100$ has sample mean about $42.67$ and sample [variance](../../../variance.md) about $274.33$, rather than variance near $42.67$. Its counts span a range of $33$, compared with a Poisson standard deviation about $6.53$. The dose-$33$ and dose-$1000$ groups likewise have variances above their means. Thus extra plate-to-plate variation is plausible. With only three replicates per dose this is evidence suggesting [overdispersion](../../../exponential-family.md#overdispersion), rather than a precise determination of it; not every group has excess sample variance.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $\eta_i=\alpha+\beta\log(x_i+10)+\gamma x_i$. The [Poisson-lognormal random-effect model](../../../statistical-modelling.md#poisson-lognormal-random-effect-model) assigns each plate a random intensity $\mu_{ij}=e^{\eta_i+\lambda_{ij}}$. Conditional on that intensity its [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) has mean and variance both $\mu_{ij}$, but marginalizing over the [normal distribution](../../../probability-theory.md#normal-distribution) of the [random effect](../../../statistical-modelling.md#random-effect) gives

$$
m_i=\mathbb E[Y_{ij}\mid\alpha,\beta,\gamma,\tau]
=e^{\eta_i+\tau^2/2}.
$$

The [law of total variance](../../../probability-theory.md#law-of-total-variance) yields

$$
\operatorname{Var}(Y_{ij})=\mathbb E[\mu_{ij}]+\operatorname{Var}(\mu_{ij})
=\boxed{m_i+m_i^2(e^{\tau^2}-1)}.
$$

This exceeds the mean whenever $\tau>0$. The independent plate effects supply additional heterogeneity without inducing dependence between plates conditional on the global parameters. Also $e^{\eta_i}$ is the median random intensity, not its marginal mean; the factor $e^{\tau^2/2}$ matters for population predictions.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Centre and scale both predictors, particularly the raw dose whose scale is much larger than that of $\log(x_i+10)$. For example use $z_{1i}=[\log(x_i+10)-c_1]/s_1$, $z_{2i}=(x_i-c_2)/s_2$ and the [linear predictor](../../../statistical-modelling.md#linear-predictor) $\eta_i=a_0+b_1z_{1i}+b_2z_{2i}$. This reduces the intercept-slope correlations and numerical scale disparities; further orthogonalizing correlated columns or updating coefficients jointly can improve [Markov chain Monte Carlo](../../../statistical-inference.md#markov-chain-monte-carlo) mixing. The exact old prior can be retained through the corresponding coefficient transformation; assigning new independent priors to transformed coefficients would instead change the prior.

For weakly informed plate effects or small $\tau$, use the [non-centred Gaussian random-effect parameterisation](../../../statistical-inference.md#non-centered-gaussian-random-effect-parameterization) $\lambda_{ij}=\tau z_{ij}$ with $z_{ij}\sim N(0,1)$. This often reduces dependence between the scale and local effects; it is not guaranteed to outperform the centred version when plate effects are strongly informed. Sensibly calibrated proper priors also avoid the enormous initial log intensities permitted by the stated coefficient ranges. Use dispersed chains and [Markov chain Monte Carlo convergence diagnostics](../../../statistical-inference.md#markov-chain-monte-carlo-convergence-diagnostics) to assess stationarity, agreement between chains and [effective sample size of a Markov chain](../../../statistical-inference.md#effective-sample-size-of-a-markov-chain). **Reparameterization can improve mixing; simply retaining more iterations does not remove poor mixing.**

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

The regression coefficients have independent proper [uniform distributions](../../../continuous-probability-distribution.md#continuous-uniform-distribution) on very wide finite intervals. These are flat in the coefficients, not flat in fitted rates, and can be highly informative on the rate scale. The scale $\tau$ is uniform on $(0,100)$, and [WinBUGS](../../../statistical-inference.md#winbugs) receives the corresponding precision $1/\tau^2$ for each [normal distribution](../../../probability-theory.md#normal-distribution) random effect. Writing $v=\tau^2$, the induced [prior density](../../../statistical-inference.md#prior-density) is

$$
\boxed{p(v)=\frac1{200\sqrt v}\mathbf1_{(0,10000)}(v).}
$$

It is proper and integrable at zero.

The usual scale-invariant variance prior $p(v)\propto1/v$ would instead cause an [improper posterior from a log-uniform random-effect scale prior](../../../statistical-inference.md#improper-posterior-from-a-log-uniform-random-effect-scale-prior). After integrating out the plate effects, the [likelihood function](../../../statistical-modelling.md#likelihood-function) tends as $v\downarrow0$ to the ordinary positive Poisson likelihood. On any compact interior set of coefficient values this limit is positive and bounded away from zero. Hence the posterior normalizing integral contains a divergent factor $\int_0^\varepsilon dv/v$. There is no [posterior distribution](../../../statistical-inference.md#bayesian-posterior) under that prior, even if formal full conditional distributions appear usable. Thus **a proper prior with integrable mass near zero is needed here**. The reciprocal-scale rule is the standard pure-scale [Jeffreys prior](../../../statistical-modelling.md#jeffreys-prior); it should not be confused with the model-specific information prior for an additive variance component.

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Delete the plate [random effects](../../../statistical-modelling.md#random-effect) from the [linear predictor](../../../statistical-modelling.md#linear-predictor) and remove their stochastic nodes and the unused scale/precision nodes. The observation layer then remains a [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) with

$$
\boxed{\log\mu_{ij}=\alpha+\beta\log(x_i+10)+\gamma x_i.}
$$

For example the essential [WinBUGS](../../../statistical-inference.md#winbugs) observation block can be written as
```
for (i in 1:doses) {
for (j in 1:plates) {
y[i,j] ~ dpois(mu[i,j])
log(mu[i,j]) <- alpha + beta*log(x[i]+10) + gamma*x[i]
}
}
```
Retain the coefficient priors. This is the $\tau=0$ sampling model implemented directly; attempting to keep `1/(tau*tau)` while fixing `tau` to zero would divide by zero.

<h3 id="3/f">f</h3>

↑ **Parent:** [3](#3)

<h4 id="3/f/solution">Solution</h4>

↑ **Parent:** [F](#3/f)

Under the common observation-level [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) convention, [DIC](../../../statistical-modelling.md#deviance-information-criterion) is $\overline D+p_D$, with the [effective parameter count in DIC](../../../statistical-modelling.md#effective-parameter-count-in-dic) defined by $p_D=\overline D-D(\overline\psi)$. The no-random-effect model's effective count is near three, corresponding to its three fitted regression coefficients. With plate [random effects](../../../statistical-modelling.md#random-effect), the effective count rises to $13.6$: the local effects add flexibility, but their partial pooling means they do not count as eighteen fully independent unrestricted fitted parameters. The effective count need not be an integer or equal the raw parameter count; the scale parameter controls that shrinkage.

Adding the plate effects reduces the average [Bayesian deviance](../../../statistical-modelling.md#bayesian-deviance) by $28.6$ at an effective-complexity cost of $10.7$. Therefore its [DIC](../../../statistical-modelling.md#deviance-information-criterion) is lower by

$$
\boxed{142.1-124.2=17.9.}
$$

**The reported criterion favours the overdispersed model.** This is a fit-complexity comparison, not a posterior probability or [Bayes factor](../../../statistical-inference.md#bayes-factor). In a [hierarchical Bayesian model](../../../statistical-inference.md#hierarchical-bayesian-model), the interpretation depends on whether deviance is conditional on local effects or has marginalized them out; these figures use the supplied observation-level convention.

<h3 id="3/g">g</h3>

↑ **Parent:** [3](#3)

<h4 id="3/g/solution">Solution</h4>

↑ **Parent:** [G](#3/g)

For each plate use its conditional fitted intensity, including the fitted [random effect](../../../statistical-modelling.md#random-effect). At a [posterior](../../../statistical-inference.md#bayesian-posterior) draw $s$ form the [Pearson residual](../../../statistical-modelling.md#pearson-residual)

$$
\boxed{r_{ij}^{(s)}=\frac{y_{ij}-\mu_{ij}^{(s)}}{\sqrt{\mu_{ij}^{(s)}}}.}
$$

A simpler plot uses $\widehat\mu_{ij}$ in this expression, but posterior draws also display uncertainty in the fitted values. Look for residuals centred around zero, unexpectedly large tails or isolated outliers, and patterns with dose, fitted intensity or plate grouping. For known conditional parameters the [Poisson distribution](../../../discrete-probability-distribution.md#poisson-distribution) gives mean zero and variance one for this residual; approximate normality is reasonable only at adequate count sizes. Fitting the same data and estimating latent effects changes its calibration, so compare the diagnostics with residuals from conditional [posterior predictive checks](../../../statistical-inference.md#posterior-predictive-check), rather than treating them as independent exact standard normals.

This checks the plate-level Poisson sampling layer given the effects and can reveal remaining unmodelled variation. It does not by itself establish the population dose-response curve: fitted plate effects can absorb departures from that curve.

<h3 id="3/h">h</h3>

↑ **Parent:** [3](#3)

<h4 id="3/h/solution">Solution</h4>

↑ **Parent:** [H](#3/h)

Use [conditional versus marginal posterior predictive checks](../../../statistical-inference.md#conditional-versus-marginal-posterior-predictive-checks) to replicate new plates, rather than recycling the fitted plate effects. For each joint [posterior](../../../statistical-inference.md#bayesian-posterior) draw of $(\alpha,\beta,\gamma,\tau)$, draw fresh independent $\lambda_{ij}^{\mathrm{rep}}\sim N(0,\tau^2)$ and then

$$
Y_{ij}^{\mathrm{rep}}\sim\operatorname{Poisson}
\left(\exp\{\alpha+\beta\log(x_i+10)+\gamma x_i+\lambda_{ij}^{\mathrm{rep}}\}\right).
$$

Use the same doses and three-plate design, giving the [posterior predictive distribution](../../../statistical-inference.md#posterior-predictive-distribution) for repeated experiments. Compare observed dose means and their trend, the high-dose downturn, within-dose spreads, and outliers with the replicated curves and intervals. For example compare a discrepancy

$$
T(y;\psi)=\sum_i\frac{(\overline y_i-m_i)^2}{[m_i+m_i^2(e^{\tau^2}-1)]/3},
\qquad m_i=e^{\eta_i+\tau^2/2},
$$

with $T(y^{\mathrm{rep}};\psi)$ draw by draw. The resulting posterior predictive tail fraction or graphical rank assesses whether the observed trend is unusual under this model. **Fresh plate effects are needed to assess the population dose-response assumption.** Reusing the fitted effects would mainly check the conditional sampling layer and could hide systematic departures from the proposed curve.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Compute the [Bayesian model evidence](../../../statistical-inference.md#bayesian-model-evidence) for each model by integrating its sampling density against its parameter prior:

$$
m_i(y)=\int p_Y(y\mid\psi_i,M_i)p(\psi_i\mid M_i)\,d\psi_i.
$$

The [posterior odds](../../../statistical-inference.md#posterior-odds) are the [prior odds](../../../statistical-inference.md#prior-odds) multiplied by the [Bayes factor](../../../statistical-inference.md#bayes-factor):

$$
\boxed{\frac{\Pr(M_1\mid y)}{\Pr(M_2\mid y)}
=\frac{\Pr(M_1)}{\Pr(M_2)}\frac{m_1(y)}{m_2(y)}.}
$$

The parameter priors used for evidence must be normalized; arbitrary normalization constants in model-specific improper priors would make this comparison undefined.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

Within the positive component, [normal-normal conjugacy](../../../probability-and-statistics.md#normal-normal-conjugacy-with-known-observation-variance) gives

$$
p(\theta_i\mid y_i,+)\propto
\exp\left\{-\frac12(y_i-\theta_i)^2-\frac{\theta_i^2}{2V}\right\}.
$$

Completing the square yields

$$
\theta_i\mid y_i,+\sim N\left(\frac{V}{1+V}y_i,\frac{V}{1+V}\right),
\qquad\boxed{\mathbb E[\theta_i\mid y_i,+]=\frac{V}{1+V}y_i.}
$$

Here positive denotes membership in the variable-effect component, not the condition $\theta_i>0$; its normal prior permits effects of either sign.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Integrating the positive component's [normal distribution](../../../probability-theory.md#normal-distribution) prior gives its [prior predictive distribution](../../../statistical-inference.md#bayesian-model-evidence):

$$
\boxed{Y_i\mid+,V\sim N(0,1+V).}
$$

The negative component gives $Y_i\mid-\sim N(0,1)$. Let $f_1(y)=\phi_{1+V}(y)$ and $f_0(y)=\phi_1(y)$ denote those centred normal densities. The [point-null mixture prior](../../../statistical-inference.md#point-null-mixture-prior) assigns component odds $q/(1-q)$, so the [posterior odds](../../../statistical-inference.md#posterior-odds) of the positive component are

$$
\boxed{O_i(y_i)=\frac q{1-q}\frac1{\sqrt{1+V}}
\exp\left\{\frac{Vy_i^2}{2(1+V)}\right\}.}
$$

Its [posterior probability](../../../statistical-inference.md#posterior-probability) is $O_i/(1+O_i)$. Evidence depends on $y_i^2$, so large effects of either sign favour the positive component. This is the marginal distribution before observing $y_i$, not the posterior predictive law for a second observation conditional on it.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Under the independent-gene version of the model, integrating both component labels and effects gives

$$
\boxed{p(y\mid q,V)=\prod_{i=1}^N\{(1-q)f_0(y_i)+qf_1(y_i)\}.}
$$

This product uses independence of the gene effects and observation errors conditional on the shared parameters. Maximize its logarithm over $0\leq q\leq1$, for example with a one-dimensional bounded optimizer or a grid followed by refinement. Its derivatives are

$$
\ell'(q)=\sum_i\frac{f_1(y_i)-f_0(y_i)}{(1-q)f_0(y_i)+qf_1(y_i)},
\qquad
\ell''(q)=-\sum_i\frac{[f_1(y_i)-f_0(y_i)]^2}{[(1-q)f_0(y_i)+qf_1(y_i)]^2}\leq0.
$$

Thus the log [likelihood function](../../../statistical-modelling.md#likelihood-function) is concave. An interior [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) solves the score equation; otherwise it is at zero or one, determined by the endpoint score signs. An alternative [expectation-maximization algorithm](../../../statistical-modelling.md#expectation-maximization-algorithm) iterates

$$
w_i=\frac{qf_1(y_i)}{(1-q)f_0(y_i)+qf_1(y_i)},\qquad
q_{\mathrm{new}}=\frac1N\sum_iw_i.
$$

For $V=0$, the components coincide and $q$ is not identifiable; for $V>0$ the full observation values carry information about the mixing fraction.

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

Use [prior elicitation](../../../statistical-inference.md#prior-elicitation) to make the qualitative judgments quantitative: ask whether $10\%$ represents a mean, median or mode, and what probability “unlikely above $15\%$” should mean, for example a $5\%$ upper-tail probability. A [Beta distribution](../../../probability-theory.md#beta-distribution) on $(0,1)$ is a convenient family. If $0.1$ is taken as the mean, write its parameters as $a_q=0.1\kappa$, $b_q=0.9\kappa$, then choose $\kappa$ so that the desired tail probability above $0.15$ is obtained. Check its quantiles and [prior predictive distribution](../../../statistical-inference.md#bayesian-model-evidence) for plausibility, and assess sensitivity to reasonable alternative elicited values. **The information suggests an informative prior near $0.1$, but does not uniquely determine its parameters.**

<h3 id="4/f">f</h3>

↑ **Parent:** [4](#4)

<h4 id="4/f/solution">Solution</h4>

↑ **Parent:** [F](#4/f)

Introduce independent component indicators $z_i\mid q\sim\operatorname{Bernoulli}(q)$, and auxiliary slab effects $u_i\sim N(0,V)$, independent of the indicators. Set $\theta_i=z_i u_i$. Then inactive genes have exactly zero effect, while active genes have the stipulated normal distribution. With $V>0$ supplied as known data and elicited positive beta shapes, one suitable [WinBUGS](../../../statistical-inference.md#winbugs) model is
```
model {
q ~ dbeta(aq, bq)
for (i in 1:N) {
z[i] ~ dbern(q)
u[i] ~ dnorm(0, 1/V)
theta[i] <- z[i]*u[i]
y[i] ~ dnorm(theta[i], 1)
}
}
```
The normal arguments are precisions, not variances. Supply all observed `y` values, monitor `q`, `theta` and optionally `z`, and assess [Markov chain Monte Carlo convergence diagnostics](../../../statistical-inference.md#markov-chain-monte-carlo-convergence-diagnostics). The proper auxiliary prior remains defined for inactive genes, where $u_i$ is not informed by the likelihood. This represents the exact [point-null mixture prior](../../../statistical-inference.md#point-null-mixture-prior), rather than replacing its point mass by a narrow continuous spike. Conditional on the indicators, $q\mid z$ has [Beta distribution](../../../probability-theory.md#beta-distribution) $\operatorname{Beta}(a_q+\sum_i z_i,b_q+N-\sum_i z_i)$, providing a useful check on the update.

<h3 id="4/g">g</h3>

↑ **Parent:** [4](#4)

<h4 id="4/g/solution">Solution</h4>

↑ **Parent:** [G](#4/g)

Let $p_0=\overline\Phi(2)$ and $p_1=\overline\Phi(2/\sqrt{1+V})$, where $\overline\Phi$ is the standard [normal distribution](../../../probability-theory.md#normal-distribution) upper-tail probability. The [mixture model](../../../statistical-modelling.md#mixture-model) gives

$$
\Pr(Y_i>2\mid q,V)=(1-q)p_0+qp_1.
$$

For $V>0$, [threshold inference for a mixture proportion](../../../statistical-modelling.md#threshold-inference-for-a-mixture-proportion) therefore gives

$$
\boxed{\widehat q=\frac{0.15-\overline\Phi(2)}
{\overline\Phi(2/\sqrt{1+V})-\overline\Phi(2)}.}
$$

This is a method-of-moments estimate when it lies in $[0,1]$. More formally, if $K$ of the $N$ independent genes exceed the threshold, then $K\sim\operatorname{Binomial}(N,(1-q)p_0+qp_1)$, and its constrained [maximum-likelihood estimate](../../../statistical-modelling.md#maximum-likelihood-estimator) clips the displayed value to $[0,1]$. No numerical estimate is determined without the given value of $V$.

Here $p_0\approx0.02275$. Matching $15\%$ exactly requires $p_1\geq0.15$, equivalently $V\geq[2/\Phi^{-1}(0.85)]^2-1\approx2.724$. For smaller positive $V$, the maximum is at $q=1$, and a large-sample exceedance fraction this high suggests a mismatch with the prescribed component variances. Sampling fluctuation is still possible; an observed fraction need not equal its expectation. If $V=0$, the denominator vanishes and this summary gives no information about $q$. Because $p_1<1/2$ for finite $V$, matching $15\%$ in expectation also forces $q>(0.15-p_0)/(0.5-p_0)\approx0.267$. Thus the summary suggests tension with the earlier prior concentrated near $0.1$, under this mean-zero alternative model. The event is the one-sided exceedance $Y_i>2$, not $|Y_i|>2$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2009](../../2009.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
