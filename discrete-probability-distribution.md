# Discrete probability distribution

↑ **Parent:** [Probability distribution](probability-theory.md#probability-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_probability_distribution)

A discrete probability distribution is supported on a finite or countable set.

**Table of contents**

- [Benford law](#benford-law)
  - [Scale invariance of decimal significands](#scale-invariance-of-decimal-significands)
  - [Benford law from logarithmic uniformity](#benford-law-from-logarithmic-uniformity)
  - [Benford frequencies for powers of an integer](#benford-frequencies-for-powers-of-an-integer)
- [Discrete uniform distribution](#discrete-uniform-distribution)
  - [Nondecreasing uniform samples](#nondecreasing-uniform-samples)
- [Bernoulli distribution](#bernoulli-distribution)
  - [Estimating Bernoulli variance](#estimating-bernoulli-variance)
  - [Bernoulli trial](#bernoulli-trial)
  - [Bernoulli thinning](#bernoulli-thinning)
- [Geometric distribution](#geometric-distribution)
  - [Geometric return count before absorption](#geometric-return-count-before-absorption)
  - [Geometric count under Bernoulli thinning](#geometric-count-under-bernoulli-thinning)
  - [Capped geometric waiting time](#capped-geometric-waiting-time)
  - [Coupon collector problem](#coupon-collector-problem)
    - [Poissonized coupon completion time and count](#poissonized-coupon-completion-time-and-count)
    - [Waiting time to observe both Bernoulli outcomes](#waiting-time-to-observe-both-bernoulli-outcomes)
    - [Coupon collector waiting-time variance](#coupon-collector-waiting-time-variance)
- [Negative binomial distribution](#negative-binomial-distribution)
  - [Negative binomial stopping argument](#negative-binomial-stopping-argument)
  - [Poisson-gamma mixture](#poisson-gamma-mixture)
- [Binomial distribution](#binomial-distribution)
  - [Binomial proportion](#binomial-proportion)
    - [Grouped Bernoulli failure counts](#grouped-bernoulli-failure-counts)
  - [Zero-event binomial upper confidence bound](#zero-event-binomial-upper-confidence-bound)
  - [Zero-truncated binomial distribution](#zero-truncated-binomial-distribution)
  - [Fourth centered moment of a binomial distribution](#fourth-centered-moment-of-a-binomial-distribution)
  - [Sample proportion](#sample-proportion)
  - [Binomial likelihood](#binomial-likelihood)
- [Hypergeometric distribution](#hypergeometric-distribution)
- [Multinomial distribution](#multinomial-distribution)
  - [Constrained Poisson and multinomial likelihood equivalence](#constrained-poisson-and-multinomial-likelihood-equivalence)
  - [Negative multinomial distribution](#negative-multinomial-distribution)
    - [Finite-sample bias in a negative multinomial probability estimator](#finite-sample-bias-in-a-negative-multinomial-probability-estimator)
  - [Multinomial central limit theorem](#multinomial-central-limit-theorem)
  - [Uniform balls-in-bins allocation](#uniform-balls-in-bins-allocation)
    - [Poisson limit for occupancy fractions](#poisson-limit-for-occupancy-fractions)
  - [Multinomial likelihood](#multinomial-likelihood)
    - [Multinomial deviance](#multinomial-deviance)
  - [Categorical distribution](#categorical-distribution)
- [Poisson distribution](#poisson-distribution)
  - [Skellam distribution](#skellam-distribution)
  - [Mixed Poisson distribution](#mixed-poisson-distribution)
    - [Overdispersion of nondegenerate mixed Poisson counts](#overdispersion-of-nondegenerate-mixed-poisson-counts)
    - [Posterior mean from adjacent mixed Poisson probabilities](#posterior-mean-from-adjacent-mixed-poisson-probabilities)
  - [Poisson entropy monotonicity](#poisson-entropy-monotonicity)
  - [Stein-Chen method](#stein-chen-method)
    - [Stein-Chen bound with the Poisson Stein factor](#stein-chen-bound-with-the-poisson-stein-factor)
    - [Poisson approximation with dependency neighborhoods](#poisson-approximation-with-dependency-neighborhoods)
    - [Poisson Stein equation](#poisson-stein-equation)
  - [Poisson size-bias identity](#poisson-size-bias-identity)
  - [Upper-truncated Poisson distribution](#upper-truncated-poisson-distribution)
  - [Poisson mixture](#poisson-mixture)
    - [Poisson-uniform posterior mean](#poisson-uniform-posterior-mean)
    - [Shifted-exponential Poisson mixture](#shifted-exponential-poisson-mixture)
      - [Shifted-exponential Poisson count recursion](#shifted-exponential-poisson-count-recursion)
  - [Zero-truncated Poisson distribution](#zero-truncated-poisson-distribution)
    - [Parity estimator for a zero-truncated Poisson count](#parity-estimator-for-a-zero-truncated-poisson-count)
  - [Addition of independent Poisson random variables](#addition-of-independent-poisson-random-variables)
  - [Poisson approximation bound for dependent Bernoulli variables](#poisson-approximation-bound-for-dependent-bernoulli-variables)
  - [Poisson observation model](#poisson-observation-model)
    - [Poisson observation](#poisson-observation)
  - [Zero-inflated Poisson distribution](#zero-inflated-poisson-distribution)
    - [Zero-inflated Poisson regression](#zero-inflated-poisson-regression)
      - [Posterior structural-zero probability](#posterior-structural-zero-probability)
      - [Component and marginal effects in zero-inflated regression](#component-and-marginal-effects-in-zero-inflated-regression)
      - [EM algorithm for zero-inflated Poisson regression](#em-algorithm-for-zero-inflated-poisson-regression)
  - [Poisson central limit theorem](#poisson-central-limit-theorem)
    - [Poisson cumulative probability at its growing mean](#poisson-cumulative-probability-at-its-growing-mean)
  - [Poisson-multinomial conditioning](#poisson-multinomial-conditioning)
    - [Poisson trick](#poisson-trick)
      - [Flat log-rate marginalization gives the multinomial likelihood](#flat-log-rate-marginalization-gives-the-multinomial-likelihood)
        - [Gaussian log-rate correction to the Poisson trick](#gaussian-log-rate-correction-to-the-poisson-trick)
  - [Normal approximation to the Poisson distribution](#normal-approximation-to-the-poisson-distribution)

## Benford law

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)

Benford law assigns leading base-ten digit $d\in\{1,\ldots,9\}$ probability $\log_{10}(1+1/d)$. This distribution arises when the fractional part of a base-ten logarithm is uniform: digit $d$ corresponds to the interval $[\log_{10}d,\log_{10}(d+1))$.

### Scale invariance of decimal significands

↑ **Parent:** [Benford law](#benford-law)

A decimal significand lies in $[1,10)$, obtained by removing the integer power of ten from a positive number. Multiplication by a constant rotates the fractional logarithm modulo one. Invariance under every such rotation makes the fractional logarithm uniform and hence implies [Benford law](#benford-law). This is an invariant significand distribution, not a proper scale-invariant distribution for the entire positive number.

### Benford law from logarithmic uniformity

↑ **Parent:** [Benford law](#benford-law)

The leading decimal digit is determined by the fractional part of $\log_{10}X$. A uniform fractional logarithm gives [Benford law](#benford-law) by the lengths of the intervals $[\log_{10}i,\log_{10}(i+1))$. A [log-uniform distribution](continuous-probability-distribution.md#log-uniform-distribution) whose logarithmic span is an integer has this property. Arbitrary partial-decade truncations generally do not.

### Benford frequencies for powers of an integer

↑ **Parent:** [Benford law](#benford-law)

If $a\ge2$ is an integer with irrational $\log_{10}a$, then the leading digit $d$ of $a^n$ has limiting frequency $\log_{10}(1+1/d)$. Indeed the logarithmic fractional parts are the orbit of zero under an [irrational rotation of the circle](measure-theory.md#irrational-rotation), so [everywhere interval frequency under an irrational rotation](measure-theory.md#everywhere-interval-frequency-under-an-irrational-rotation) applies. Thus for $a=2$, digit seven has frequency $(\log8-\log7)/\log10$.

## Discrete uniform distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_uniform_distribution)

The discrete uniform distribution on a finite set $S$ assigns probability $1/|S|$ to every element of $S$.

### Nondecreasing uniform samples

↑ **Parent:** [Discrete uniform distribution](#discrete-uniform-distribution)

An ordered sample from $n$ equally likely values is nondecreasing exactly when it is the unique sorted representative of its multiplicities. [Stars and bars](combinatorics.md#stars-and-bars-combinatorics) counts the nonnegative multiplicities summing to $r$; repeated values are included automatically.

## Bernoulli distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_distribution)

A Bernoulli random variable equals one with probability $p$ and zero with probability $1-p$. Its mean is $p$ and its variance is $p(1-p)$.

### Estimating Bernoulli variance

↑ **Parent:** [Bernoulli distribution](#bernoulli-distribution)

For $n\geq2$ independent Bernoulli observations with sum $K$, the extended maximum-likelihood estimator is $\widehat\phi=(K/n)(1-K/n)$. Its unbiased improvement is $K(n-K)/[n(n-1)]=n\widehat\phi/(n-1)$, obtained by conditioning $X_1(1-X_2)$ on $K$. The [Rao-Blackwell theorem](probability-and-statistics.md#rao-blackwell-theorem) gives strict variance reduction for $0<\theta<1$. With a uniform prior on $\theta$ and squared-error loss for $\phi$, the Bayes estimator is $(K+1)(n-K+1)/[(n+2)(n+3)]$. For parameter space strictly $(0,1)$, samples with $K=0$ or $n$ have only a boundary likelihood supremum, not an attained maximum.

### Bernoulli trial

↑ **Parent:** [Bernoulli distribution](#bernoulli-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_trial)

A random experiment with two outcomes, success and failure, whose success indicator has a [Bernoulli distribution](#bernoulli-distribution). Repeated trials sharing success probability $\theta$ give a [binomial distribution](#binomial-distribution) for their success count if they are independent conditional on $\theta$; integrating over an uncertain common $\theta$ generally makes the trials dependent marginally.

### Bernoulli thinning

↑ **Parent:** [Bernoulli distribution](#bernoulli-distribution)

If an event occurs with probability $p$ and is independently retained with conditional probability $q$, its retained indicator is Bernoulli with probability $pq$. Applying this independently to a binomial count turns $\operatorname{Binomial}(n,p)$ into $\operatorname{Binomial}(n,pq)$.

## Geometric distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_distribution)

A geometric distribution models the number of independent Bernoulli trials needed to obtain the first success. On the convention supported by $1,2,\ldots$, its mass is $(1-p)^{k-1}p$ and its mean is $1/p$. On the failures-before-first-success convention supported by $0,1,\ldots$, its mass is $(1-p)^kp$ and its mean is $(1-p)/p$. Both conventions have variance $(1-p)/p^2$.

### Geometric return count before absorption

↑ **Parent:** [Geometric distribution](#geometric-distribution)

Start a [Markov chain](markov-process.md#markov-chain) at a nonabsorbing state $i$. If each departure from $i$ has probability $p>0$ of absorption before the next return, the [Strong Markov property](markov-process.md#strong-markov-property) makes the number of visits to $i$, including the initial one, a positive-integer [geometric random variable](#geometric-distribution) of parameter $p$. For a [continuous-time Markov chain](markov-process.md#continuous-time-markov-chain) whose [holding times](markov-process.md#holding-time) at $i$ are independent rate-$\lambda_i$ exponentials, independently of the embedded jump chain, the total [occupation time](markov-process.md#occupation-time-of-a-continuous-time-markov-chain) at $i$ is a sum of $K$ such holding times and has [expected value](probability-theory.md#expected-value) $1/(p\lambda_i)$.

### Geometric count under Bernoulli thinning

↑ **Parent:** [Geometric distribution](#geometric-distribution)

Independently retain each event of a zero-based [geometric distribution](#geometric-distribution) count with probability $\alpha$. Conditional on the original count, the retained count is binomial, so its [probability generating function](probability-theory.md#probability-generating-function) is $p/[1-(1-p)(1-\alpha+\alpha z)]$. This is again a zero-based [geometric distribution](#geometric-distribution), with success parameter $p_\alpha$ and mean $\alpha(1-p)/p$. In [excess of loss reinsurance](actuarial-statistics.md#excess-of-loss-reinsurance), $\alpha$ is the probability that a claim exceeds the retention.

### Capped geometric waiting time

↑ **Parent:** [Geometric distribution](#geometric-distribution)

For a positive-integer [geometric distribution](#geometric-distribution) $P(N=j)=pq^{j-1}$ with $q=1-p$, the capped time has masses $pq^{j-1}$ for $1\leq j<k$ and $q^{k-1}$ at $k$. The last mass includes all later arrivals, not only $N=k$. Its [probability generating function](probability-theory.md#probability-generating-function) and [expected value](probability-theory.md#expected-value) are

$$
G_X(s)=p\sum_{j=1}^{k-1}q^{j-1}s^j+q^{k-1}s^k,\qquad \mathbb E X=\frac{1-q^k}{p}.
$$

The expectation follows either by differentiating the [PGF](probability-theory.md#probability-generating-function) or summing the tail [probabilities](probability-theory.md#probability) up to $k$.

### Coupon collector problem

↑ **Parent:** [Geometric distribution](#geometric-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coupon_collector_problem)

When independent uniform draws are made from $n$ types, the time $T_n$ until every type has appeared decomposes as a sum of independent geometric waiting times with parameters

$$
1,\frac{n-1}{n},\ldots,\frac1n.
$$

Consequently

$$
\mathbb ET_n=nH_n,
\qquad
\operatorname{var}(T_n)\leq n^2\sum_{j=1}^{\infty}\frac1{j^2},
$$

and Chebyshev's inequality gives $T_n/(n\log n)\to1$ in probability.

#### Poissonized coupon completion time and count

↑ **Parent:** [Coupon collector problem](#coupon-collector-problem)

For independent coupon labels arriving at rate $\lambda$, [Poisson thinning](probability-theory.md#poisson-thinning) makes the type-specific first arrival times independent exponentials of rates $\lambda p_j$. Completion time is their maximum. Its distribution is $\mathbb P(T<t)=\prod_j(1-e^{-\lambda p_jt})$. The completion count $L$ depends only on the labels and is independent of the exponential interarrival sequence. Therefore $T=\sum_{k\ge1}E_k\mathbf1_{\{L\ge k\}}$ and nonnegative integration gives the displayed identity. Completion count and its expectation do not depend on arrival rate.

#### Waiting time to observe both Bernoulli outcomes

↑ **Parent:** [Coupon collector problem](#coupon-collector-problem)

In independent trials with two outcomes of [probabilities](probability-theory.md#probability) $p$ and $q=1-p$, let $N$ include the first trial and the trial that first completes the pair. Conditional on the first outcome, $N-1$ has a [geometric distribution](#geometric-distribution) of parameter $q$ or $p$, with mixture weights $p,q$. The [law of total expectation](measure-theory.md#law-of-total-expectation) and [law of total variance](probability-theory.md#law-of-total-variance) give

$$
EN=1+\frac pq+\frac qp=\frac1{pq}-1,\qquad
\operatorname{Var}N=\frac{p^2}{q^2}+\frac{q^2}{p^2}+\frac{(p-q)^2}{pq}
=\frac1{p^2q^2}-\frac3{pq}-2.
$$

The final term in the unsimplified variance is the [variance](variance.md) of the two conditional means; omitting it is incorrect unless $p=q$. Both outcomes must have positive [probability](probability-theory.md#probability) for these finite formulas.

#### Coupon collector waiting-time variance

↑ **Parent:** [Coupon collector problem](#coupon-collector-problem)

For uniform independent draws of $n$ coupon types, the waiting times with $r$ unseen types remaining are independent positive-support [geometric distributions](#geometric-distribution) of parameter $r/n$. Summing their means gives $n\sum_{r=1}^n1/r$, and summing their variances gives the displayed formula. [Independence](random-variable.md#independent-random-variables) follows from fresh draws after each discovery and the fact that the next stage's conditional distribution depends only on the count of remaining types.

## Negative binomial distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negative_binomial_distribution)

On the failures-before-the-$r$th-success convention, a negative binomial variable with success probability $p$ has probability mass function

$$
\mathbb P(X=x)=\binom{x+r-1}{x}(1-p)^x p^r,
\qquad x=0,1,\ldots.
$$

It has expected value $r(1-p)/p$ and variance $r(1-p)/p^2$.

### Negative binomial stopping argument

↑ **Parent:** [Negative binomial distribution](#negative-binomial-distribution)

For the $r$th success to occur after exactly $x$ failures, the final trial must be a success, while the preceding $x+r-1$ trials contain $x$ failures and $r-1$ successes. Choosing the failure locations gives the factor $\binom{x+r-1}{x}$.

### Poisson-gamma mixture

↑ **Parent:** [Negative binomial distribution](#negative-binomial-distribution)

If $Y\mid\Lambda\sim\operatorname{Poisson}(\Lambda)$ and $\Lambda$ has a [gamma distribution](continuous-probability-distribution.md#gamma-distribution), then $Y$ has a [negative binomial distribution](#negative-binomial-distribution). For gamma shape $\nu$ and scale $\alpha$,

$$
\mathbb EY=\alpha\nu,
\qquad
\operatorname{Var}(Y)=\alpha\nu+\alpha^2\nu.
$$

## Binomial distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binomial_distribution)

The binomial distribution counts successes in independent Bernoulli trials with common success probability.

### Binomial proportion

↑ **Parent:** [Binomial distribution](#binomial-distribution)

For $D\sim\operatorname{Bin}(n,p)$ with $n>0$, the sample binomial proportion is $D/n$. Its [expectation](probability-theory.md#expected-value) is p and its [variance](variance.md) is $p(1-p)/n$. The [central limit theorem](convergence-of-random-variables.md#central-limit-theorem) gives a [normal approximation](convergence-of-random-variables.md#normal-approximation) when both expected outcome counts are sufficiently large. These moments determine a [standard error](statistical-inference.md#standard-error) and model-based [control limits](statistical-inference.md#control-limits).

#### Grouped Bernoulli failure counts

↑ **Parent:** [Binomial proportion](#binomial-proportion)

With $m$ groups of $q$ trials and common marginal failure [probability](probability-theory.md#probability) $p$, each count $X_j$ has [expectation](probability-theory.md#expected-value) $qp$, so the displayed estimate is unbiased without assuming independence within groups. Independent individual trials give [variance](variance.md) $p(1-p)/(mq)$. If only groups are independent, estimate the [variance](variance.md) instead by $s_X^2/(mq^2)$, retaining within-group dependence. Equal marginal probabilities alone do not justify a binomial [confidence interval](statistical-inference.md#confidence-interval).

### Zero-event binomial upper confidence bound

↑ **Parent:** [Binomial distribution](#binomial-distribution)

If $X\sim\operatorname{Bin}(n,p)$ and $X=0$ is observed, the [maximum-likelihood estimate](statistical-modelling.md#maximum-likelihood-estimator) of $p$ is zero. A one-sided $1-\alpha$ upper [confidence bound](statistical-inference.md#confidence-bound) solves $P_{p_U}(X=0)=(1-p_U)^n=\alpha$, so $p_U=1-\alpha^{1/n}$. For large $n$, $p_U\simeq-\log(\alpha)/n$, giving approximately $3/n$ at 95% confidence. This describes uncertainty after no observed events, rather than proving that the underlying [probability](probability-theory.md#probability) is zero. It assumes independent observations with a common event probability; [clustered data](statistical-modelling.md#clustered-data) require a different uncertainty calculation.

### Zero-truncated binomial distribution

↑ **Parent:** [Binomial distribution](#binomial-distribution)

The [zero-truncated binomial distribution](#zero-truncated-binomial-distribution) has probabilities $\binom nx p^x(1-p)^{n-x}/[1-(1-p)^n]$ for $1\leq x\leq n$. Its natural parameter is $\phi=\log[p/(1-p)]$ and its cumulant is $\log[(1+e^\phi)^n-1]$. Mean and variance are $np/s$ and $np(1-p)/s-n^2p^2(1-p)^n/s^2$, where $s=1-(1-p)^n$. The conditional normalizer depends on $p$, so its likelihood is not proportional to the untruncated likelihood even after a positive observation. At $X=1$ and $n>1$, its likelihood supremum is at $p\downarrow0$ rather than at $1/n$.

### Fourth centered moment of a binomial distribution

↑ **Parent:** [Binomial distribution](#binomial-distribution)

For $W\sim\operatorname{Bin}(n,p)$, expand the fourth power of the sum of centered independent Bernoulli variables. Terms with an index occurring once vanish; single-index fourth moments contribute $nq(1-3q)$ and paired second moments contribute $3n(n-1)q^2$. Their sum is the displayed formula. Scaling by $n^4$ yields a uniform $O(n^{-2})$ fourth moment for $W/n-p$.

### Sample proportion

↑ **Parent:** [Binomial distribution](#binomial-distribution)

For independent Bernoulli observations with success probability $p$, the sample proportion is the success count divided by the sample size. It is an unbiased [estimator](statistical-modelling.md#estimator) with variance $p(1-p)/n$. It supplies the arm-specific risks in a [risk ratio](statistical-modelling.md#risk-ratio) and the mean difference in a two-proportion comparison.

### Binomial likelihood

↑ **Parent:** [Binomial distribution](#binomial-distribution)

If $x$ successes occur in $n$ independent Bernoulli trials, the binomial likelihood for the success probability $p$ is proportional to $p^x(1-p)^{n-x}$.

## Hypergeometric distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hypergeometric_distribution)

If a sample of size $r$ is drawn uniformly without replacement from a population of size $n$ containing $c$ marked objects, the number $K$ of marked objects sampled has mass

$$
\mathbb P(K=k)=\frac{\binom ck\binom{n-c}{r-k}}{\binom nr}.
$$

## Multinomial distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multinomial_distribution)

The multinomial distribution gives the category counts from $n$ independent trials with category probabilities $p_1,\ldots,p_k$.

### Constrained Poisson and multinomial likelihood equivalence

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)

For cell means $\mu_j$ with $\sum_j\mu_j=n$, the independent [Poisson distribution](#poisson-distribution) likelihood and the [multinomial distribution](#multinomial-distribution) likelihood with probabilities $\mu_j/n$ differ by a parameter-independent factor. Thus a [maximum-likelihood estimator](statistical-modelling.md#maximum-likelihood-estimator) for the unrestricted Poisson model whose fitted total is $n$ is also an estimator for the constrained multinomial model. Equality of named parameter estimates presumes identifiability and uniqueness; without these, the conclusion concerns the sets of maximizers. A free intercept in a log-linear Poisson model enforces the fitted-total equation.

### Negative multinomial distribution

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Negative_multinomial_distribution)

Counts of several categories before a fixed number of stopping-category outcomes have a negative multinomial distribution. For one stopping outcome of probability $r=1-\alpha-\beta$, the two-count mass function is $r\binom{x+y}{x}\alpha^x\beta^y$. Its [probability generating function](probability-theory.md#probability-generating-function) is $r/(1-\alpha s-\beta t)$ and its means are $\alpha/r$ and $\beta/r$.

#### Finite-sample bias in a negative multinomial probability estimator

↑ **Parent:** [Negative multinomial distribution](#negative-multinomial-distribution)

For $n$ independent one-stop [negative multinomial distribution](#negative-multinomial-distribution) observations, the natural estimates are $\widehat\alpha=S_X/(n+S_X+S_Y)$ and $\widehat\beta=S_Y/(n+S_X+S_Y)$. Their sum is $g((S_X+S_Y)/n)$ with strictly concave $g(z)=z/(1+z)$, so [Jensen's inequality](real-analysis.md#jensen-s-inequality) makes its expectation strictly below $\alpha+\beta$. Conditional category proportions split this bias between both estimates. With zero observed counts of a category, that estimate lies at zero; in a parameter space requiring strict positivity the likelihood supremum is not attained.

### Multinomial central limit theorem

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)

The vector of category counts is the sum of independent categorical indicator vectors. Their means are $p$ and covariance is $\operatorname{diag}p-pp^T$, so the [multivariate central limit theorem](convergence-of-random-variables.md#multivariate-central-limit-theorem) gives the displayed limit. At uniform probabilities on $k$ categories, Pearson-standardized deviations have covariance equal to the orthogonal projection onto the $(k-1)$-dimensional subspace of zero-sum vectors. Their squared norm has an asymptotic [chi-squared distribution](probability-theory.md#chi-squared-distribution) with $k-1$ degrees of freedom.

### Uniform balls-in-bins allocation

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)

Place $n$ labelled balls independently into $m$ labelled bins, each with probability $1/m$. The vector of bin counts has a [multinomial distribution](#multinomial-distribution), and each count separately has the [binomial distribution](#binomial-distribution) $\operatorname{Bin}(n,1/m)$. Distinct bin counts have [covariance](variance.md#covariance) $-n/m^2$, so they are dependent for $n>0$ and $m>1$. Counts of bins of a specified size are sums of [indicator variables](statistical-modelling.md#indicator-variable); their [expectations](probability-theory.md#expected-value) follow from the [linearity of expectation](probability-theory.md#linearity-of-expectation), without any independence between bins.

#### Poisson limit for occupancy fractions

↑ **Parent:** [Uniform balls-in-bins allocation](#uniform-balls-in-bins-allocation)

In a [uniform balls-in-bins allocation](#uniform-balls-in-bins-allocation) with $m\to\infty$ and $n/m\to\lambda\in(0,\infty)$, a fixed bin count has [convergence in distribution](convergence-of-random-variables.md#convergence-in-distribution) to a [Poisson distribution](#poisson-distribution) variable of mean $\lambda$ by the [Poisson limit theorem](convergence-of-random-variables.md#poisson-limit-theorem). If $N_j$ counts bins containing exactly $j$ balls, symmetry and the [linearity of expectation](probability-theory.md#linearity-of-expectation) give $\mathbb E[N_j]/m=\mathbb P(B_1=j)\to e^{-\lambda}\lambda^j/j!$ for each fixed $j$. In particular the expected empty fraction tends to $e^{-\lambda}$, and the expected fraction with at least two balls tends to $1-(1+\lambda)e^{-\lambda}$. These are statements about expectations; convergence of the random fractions requires an additional argument.

### Multinomial likelihood

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)

For category counts $y_1,\ldots,y_k$ with fixed total $n$ and probabilities $p_1,\ldots,p_k$, the multinomial likelihood is

$$
L(p_1,\ldots,p_k)
=\frac{n!}{\prod_jy_j!}\prod_jp_j^{y_j},
\qquad \sum_jp_j=1.
$$

Its [maximum-likelihood fitted probabilities](statistical-modelling.md#maximum-likelihood-fitted-probability) are $\widehat p_j=y_j/n$.

#### Multinomial deviance

↑ **Parent:** [Multinomial likelihood](#multinomial-likelihood)

For counts with a [multinomial distribution](#multinomial-distribution), this is twice the log likelihood ratio of the saturated cell-probability estimate to fixed probabilities $p_i$. Zero-count terms have limiting value zero. Simulation under the specified probabilities gives a direct reference distribution when asymptotic approximations are unsuitable.

### Categorical distribution

↑ **Parent:** [Multinomial distribution](#multinomial-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Categorical_distribution)

The categorical distribution describes one draw from finitely many categories with probabilities $p_1,\ldots,p_k$.

## Poisson distribution

↑ **Parent:** [Discrete probability distribution](discrete-probability-distribution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_distribution)

The Poisson distribution with mean lambda assigns mass $e^{-\lambda}\lambda^k/k!$.

### Skellam distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)

The distribution of $N_+-N_-$ for independent [Poisson random variables](#poisson-distribution) with means $\lambda_+,\lambda_-$ is the Skellam distribution. Its [characteristic function](probability-theory.md#characteristic-function) is $\exp(\lambda_+(e^{iu}-1)+\lambda_-(e^{-iu}-1))$, its mean is $\lambda_+-\lambda_-$ and its variance is $\lambda_++\lambda_-$. For equal means $\lambda>0$,

$$
\mathbb P(N_+-N_-=k)=e^{-2\lambda}\sum_{j=0}^\infty\frac{\lambda^{2j+|k|}}{j!(j+|k|)!},\qquad k\in\mathbb Z.
$$

This is the fixed-time law of a [symmetric Poisson difference process](probability-theory.md#symmetric-poisson-difference-process).

// Target: markov-process.bigb

### Mixed Poisson distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mixed_Poisson_distribution)

A mixture of [Poisson distributions](#poisson-distribution) over a nonnegative random intensity. With exposure $n>0$ and [prior density](statistical-inference.md#prior-density) $\pi(\theta)$, its [probability mass function](probability-theory.md#probability-mass-function) is $p_n(s)=\int_0^\infty e^{-n\theta}(n\theta)^s\pi(\theta)\,d\theta/s!$. A gamma mixing distribution gives a [negative binomial distribution](#negative-binomial-distribution). Counts sharing the same latent intensity are [conditionally independent](random-variable.md#conditional-independence), but generally dependent after mixing.

#### Overdispersion of nondegenerate mixed Poisson counts

↑ **Parent:** [Mixed Poisson distribution](#mixed-poisson-distribution)

If $N\mid L$ has Poisson mean $L$, [conditional expectation](measure-theory.md#conditional-expectation) and the [law of total variance](probability-theory.md#law-of-total-variance) give the display. A positive [variance](variance.md) of the random mean prevents the unconditional count from being Poisson. For Poisson parents of density $\lambda$ and offspring mean $\mu$, the count in $A$ has excess [variance](variance.md) $\lambda\mu^2\int\kappa(A-z)^2dz$, which is positive for a bounded positive-area set and a nontrivial model.

#### Posterior mean from adjacent mixed Poisson probabilities

↑ **Parent:** [Mixed Poisson distribution](#mixed-poisson-distribution)

For a [mixed Poisson distribution](#mixed-poisson-distribution) with known exposure $n>0$, multiply the unnormalized [posterior density](statistical-inference.md#posterior-density) $\theta^s e^{-n\theta}\pi(\theta)$ by $\theta$ and compare its integral with the next [probability](probability-theory.md#probability) mass. The factors $n^s/s!$ give the displayed identity whenever $p_n(s)>0$. Both mass [probabilities](probability-theory.md#probability) have the same exposure $n$. For a future [conditionally independent](random-variable.md#conditional-independence) unit-exposure [Poisson distribution](#poisson-distribution) count, this is also its [posterior predictive](statistical-inference.md#posterior-predictive-distribution) [expected value](probability-theory.md#expected-value). It holds for arbitrary proper mixing distributions, with integrals taken against the [prior](statistical-inference.md#prior-probability) measure when there is no density.

### Poisson entropy monotonicity

↑ **Parent:** [Poisson distribution](#poisson-distribution)

The [information entropy](information-theory.md#information-entropy) $F(\lambda)$ of a [Poisson distribution](#poisson-distribution) is strictly increasing for $\lambda>0$. Given $\lambda_2>\lambda_1$, take independent $U\sim\operatorname{Pois}(\lambda_1)$ and $V\sim\operatorname{Pois}(\lambda_2-\lambda_1)$. Their sum has [Poisson distribution](#poisson-distribution) with mean $\lambda_2$, so [entropy monotonicity under independent addition](information-theory.md#entropy-monotonicity-under-independent-addition) gives $F(\lambda_2)\geq F(\lambda_1)$. All these [information entropies](information-theory.md#information-entropy) are finite, and $\operatorname{Cov}(U+V,V)=\operatorname{Var}(V)>0$ excludes equality.

// Target: probability-and-statistics.bigb

### Stein-Chen method

↑ **Parent:** [Poisson distribution](#poisson-distribution)

The Stein-Chen method compares an integer-valued count with a [Poisson distribution](#poisson-distribution) by solving the [Poisson Stein equation](#poisson-stein-equation) and estimating its [expectation](probability-theory.md#expected-value) at the count. For sums of [indicator random variables](probability-theory.md#indicator-random-variable), dependency neighborhoods expose local overlap errors. This gives [total variation distance](probability-and-statistics.md#total-variation-distance) bounds without having to compute the entire count distribution.

#### Stein-Chen bound with the Poisson Stein factor

↑ **Parent:** [Stein-Chen method](#stein-chen-method)

Let $W=\sum_i I_i$ and $\lambda=\sum_i p_i>0$, where each [indicator random variable](probability-theory.md#indicator-random-variable) $I_i$ is independent of all indicators outside $\{i\}\cup J_i$ jointly. Write $V_i=\sum_{j\in J_i}I_j$ and $W_i=W-I_i-V_i$. For a test-event solution of the [Poisson Stein equation](#poisson-stein-equation), independence gives

$$
\lambda\mathbb Eg(W+1)-\mathbb EWg(W)
=\sum_i p_i\mathbb E[g(W+1)-g(W_i+1)]
+\sum_i\mathbb EI_i[g(W_i+1)-g(W)].
$$

Telescoping each difference and using $\|\Delta g\|_\infty\leq\min(1,\lambda^{-1})$ bounds the [total variation distance](probability-and-statistics.md#total-variation-distance) by that factor times $\sum_i p_i^2+\sum_i\sum_{j\in J_i}(p_ip_j+\mathbb EI_iI_j)$. Directed dependence neighborhoods are allowed. If $\lambda=0$, the count is identically zero.

#### Poisson approximation with dependency neighborhoods

↑ **Parent:** [Stein-Chen method](#stein-chen-method)

For indicators $I_a$ with means $p_a$, let $B_a$ contain $a$ and suppose $I_a$ is independent of the entire family outside $B_a$. Put $\mu=\sum_ap_a$, $b_1=\sum_a\sum_{b\in B_a}p_ap_b$ and $b_2=\sum_a\sum_{b\in B_a\setminus\{a\}}\mathbb E(I_aI_b)$. The [Poisson Stein equation](#poisson-stein-equation) and its bound $\|\Delta f\|_\infty\le1$ give the displayed [total variation distance](probability-and-statistics.md#total-variation-distance) estimate. Stronger Stein factors can improve the bound when $\mu$ is large.

#### Poisson Stein equation

↑ **Parent:** [Stein-Chen method](#stein-chen-method)

For indicator test functions $g$, the equation has a solution with $\|\Delta f\|_\infty\le1$. One proof uses an [immigration--death process](mathematical-biology.md#immigration-death-process) with immigration rate $\mu$ and per-particle death rate one. Its potential $u(k)=-\int_0^\infty(\mathbb Eg(Z_t^k)-\mathbb Eg(Z))\,dt$ satisfies its generator equation, and $f(k)=u(k)-u(k-1)$. Coupling two additional initial particles bounds the second difference of $u$ by $\int_0^\infty2e^{-2t}dt=1$.

### Poisson size-bias identity

↑ **Parent:** [Poisson distribution](#poisson-distribution)

For $N$ with [Poisson distribution](#poisson-distribution) of mean $\lambda$, the equality $n\mathbb P(N=n)=\lambda\mathbb P(N=n-1)$ proves the identity by summation. For an independent [random sum of independent claims](actuarial-statistics.md#random-sum-of-independent-claims) $S$ with this count, exchangeability of the summands gives $\mathbb E[S h(S)]=\lambda\mathbb E[X h(S+X)]$, where $X$ on the right is independent of $S$ and has the severity law. These identities hold for nonnegative measurable functions, and for integrable signed functions. They obtain [moments](probability-theory.md#moment) without assuming that a positive [exponential moment](probability-theory.md#exponential-moment) exists.

### Upper-truncated Poisson distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)

A [Poisson distribution](#poisson-distribution) of parameter $a$ conditioned to lie in $\{0,\ldots,C\}$. It is the occupancy law of a unit-resource [loss network](queueing-theory.md#loss-network). Its mean is the [carried load of an Erlang loss resource](queueing-theory.md#carried-load-of-an-erlang-loss-resource), $a[1-E(C,a)]$. Differentiating the mean with respect to $\log a$ gives its [variance](variance.md), which is positive for $a>0$ and $C\geq1$; this proves strict monotonicity of the carried load.

### Poisson mixture

↑ **Parent:** [Poisson distribution](#poisson-distribution)

A model with $Y\mid\Lambda\sim\operatorname{Poisson}(\Lambda)$ for a nonnegative random intensity. [Conditional expectation](measure-theory.md#conditional-expectation) and total [variance](variance.md) give $\mathbb E Y=\mathbb E\Lambda$ and $\operatorname{Var}Y=\mathbb E\Lambda+\operatorname{Var}\Lambda$, explaining [overdispersion](exponential-family.md#overdispersion). A [Poisson-gamma mixture](#poisson-gamma-mixture) gives the [negative binomial distribution](#negative-binomial-distribution).

#### Poisson-uniform posterior mean

↑ **Parent:** [Poisson mixture](#poisson-mixture)

For a uniform [prior distribution](statistical-inference.md#prior-probability) on $(l,u)$ with $0<l<u$, conditionally independent [Poisson distribution](#poisson-distribution) observations have sufficient count $s=\sum_i x_i$. Their [Bayesian posterior](statistical-inference.md#bayesian-posterior) density is proportional to $t^s e^{-nt}$ on that bounded interval. The displayed [posterior mean](statistical-inference.md#posterior-mean) is the [Bayes estimator under squared error loss](statistical-inference.md#bayes-estimator-under-squared-error-loss), and is generally not the affine [Bühlmann credibility estimate](actuarial-statistics.md#buhlmann-credibility-premium).

#### Shifted-exponential Poisson mixture

↑ **Parent:** [Poisson mixture](#poisson-mixture)

When the random intensity is $\alpha+Y$ with $Y$ having an [exponential distribution](continuous-probability-distribution.md#exponential-distribution) of rate $\beta$, the mixed count is the sum of independent [Poisson distribution](#poisson-distribution) and support-zero [geometric distribution](#geometric-distribution) counts. The Poisson parameter is $\alpha$ and the geometric success probability is $\beta/(\beta+1)$. At $\alpha=0$ the law is geometric.

##### Shifted-exponential Poisson count recursion

↑ **Parent:** [Shifted-exponential Poisson mixture](#shifted-exponential-poisson-mixture)

For the [shifted-exponential Poisson mixture](#shifted-exponential-poisson-mixture), the displayed relation holds for $n\ge2$, initialized by $p_0=e^{-\alpha}\beta/(\beta+1)$ and $p_1=(\alpha+1/(\beta+1))p_0$. It follows by differentiating the [probability generating function](probability-theory.md#probability-generating-function) and comparing coefficients. Nonnegativity follows from the independent Poisson-geometric [convolution of independent random variables](probability-theory.md#convolution-of-independent-random-variables) representation.

### Zero-truncated Poisson distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)

A [Poisson distribution](#poisson-distribution) conditioned on a positive count has [probability mass function](probability-theory.md#probability-mass-function) $\mathbb P(Y=y)=\theta^y/[y!(e^\theta-1)]$ for $y\ge1$ and $\theta>0$.

#### Parity estimator for a zero-truncated Poisson count

↑ **Parent:** [Zero-truncated Poisson distribution](#zero-truncated-poisson-distribution)

For the [zero-truncated Poisson distribution](#zero-truncated-poisson-distribution), $2\mathbf1_{\{Y\text{ even}\}}$ is the unique integrable nonrandomized [unbiased estimator](statistical-modelling.md#unbiased-estimator) of $p=1-e^{-\theta}$. Indeed unbiasedness gives $\sum_{y\ge1}t(y)\theta^y/y!=e^\theta+e^{-\theta}-2$, and [power series](real-analysis.md#power-series) coefficients force the parity values. Its [variance](variance.md) is $2p-p^2$; clipping it to $\mathbf1_{\{Y\text{ even}\}}$ gives [mean squared error](statistical-modelling.md#mean-squared-error) $p/2$, strictly smaller for $0<p<1$.

### Addition of independent Poisson random variables

↑ **Parent:** [Poisson distribution](#poisson-distribution)

The sum of independent Poisson random variables is Poisson, with parameter equal to the sum of their parameters. This follows by multiplying their probability generating functions $\exp(\lambda_i(z-1))$.

### Poisson approximation bound for dependent Bernoulli variables

↑ **Parent:** [Poisson distribution](#poisson-distribution)

For Bernoulli random variables $X_1,\ldots,X_n$, which need not be independent, put $p_i=\mathbb P(X_i=1)$, $S=\sum_iX_i$, and $\lambda=\sum_ip_i$. Then

$$
D_e\bigl(\mathcal L(S)\Vert\operatorname{Poisson}(\lambda)\bigr)
\leq\sum_ip_i^2+\sum_iH_e(X_i)-H_e(X_1,\ldots,X_n).
$$

The dependence penalty is the [total correlation](information-theory.md#total-correlation). The proof compares the joint Bernoulli law with the product of Poisson laws of means $p_i$, then applies the [data processing inequality for relative entropy](probability-and-statistics.md#data-processing-inequality-for-relative-entropy) to addition.

### Poisson observation model

↑ **Parent:** [Poisson distribution](#poisson-distribution)

A Poisson observation model represents a nonnegative count as conditionally Poisson with a mean supplied by an underlying process or regression model.

#### Poisson observation

↑ **Parent:** [Poisson observation model](#poisson-observation-model)

A Poisson observation is an integer-valued count modeled by a [Poisson distribution](#poisson-distribution) of specified intensity, possibly conditionally on a latent field. Independent [Poisson observations](#poisson-observation) motivate [Poisson data fidelity](inverse-problem.md#poisson-data-fidelity) through their [log-likelihood](statistical-modelling.md#log-likelihood).

### Zero-inflated Poisson distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)

A zero-inflated Poisson distribution is a mixture of a point mass at zero and a [Poisson distribution](#poisson-distribution). If the Poisson component has weight $\pi$ and mean $\lambda$, then its mean is $\pi\lambda$ and its variance is $\pi\lambda+\pi(1-\pi)\lambda^2$.

#### Zero-inflated Poisson regression

↑ **Parent:** [Zero-inflated Poisson distribution](#zero-inflated-poisson-distribution)

A zero-inflated Poisson regression specifies a structural-zero probability $\pi$ and a susceptible-component [Poisson distribution](#poisson-distribution) mean $\mu$. In this parametrization,

$$
P(Y=0)=\pi+(1-\pi)e^{-\mu},\qquad P(Y=y)=(1-\pi)e^{-\mu}\mu^y/y!\quad(y>0).
$$

The mean is $(1-\pi)\mu$. Logistic predictors for $\pi$ and logarithmic predictors for $\mu$ allow covariates to affect component membership and count intensity differently. A susceptible individual can still generate a zero count; susceptibility is not equivalent to an observed positive response.

##### Posterior structural-zero probability

↑ **Parent:** [Zero-inflated Poisson regression](#zero-inflated-poisson-regression)

In a [zero-inflated Poisson regression](#zero-inflated-poisson-regression), [Bayes' theorem](probability-theory.md#bayes-theorem) separates structural zeros from susceptible zero counts. A positive count rules out the structural-zero class; a zero raises its posterior probability according to the displayed formula, but usually does not determine class membership with certainty. This same probability supplies the E-step of the [EM algorithm for zero-inflated Poisson regression](#em-algorithm-for-zero-inflated-poisson-regression).

##### Component and marginal effects in zero-inflated regression

↑ **Parent:** [Zero-inflated Poisson regression](#zero-inflated-poisson-regression)

A logarithmic count-component contrast $b$ multiplies the susceptible mean by $e^b$, while a zero-logit contrast $g$ multiplies the structural-zero odds by $e^g$. If the baseline zero predictor is $\eta$, the marginal mean ratio is

$$
e^b\frac{1+e^{\eta}}{1+e^{\eta+g}}.
$$

Thus the count ratio alone is not a population-average effect when a covariate changes both components. With [interaction terms](statistical-model.md#interaction-term), the relevant count contrast must first include the interactions for the stated reference group.

##### EM algorithm for zero-inflated Poisson regression

↑ **Parent:** [Zero-inflated Poisson regression](#zero-inflated-poisson-regression)

The [expectation-maximization algorithm](statistical-modelling.md#expectation-maximization-algorithm) introduces $Z_i=1$ for a structural zero. Its E-step gives $\tau_i=0$ at positive counts and $\tau_i=\pi_i/[\pi_i+(1-\pi_i)e^{-\mu_i}]$ at zero. The M-step maximizes a logistic [log-likelihood](statistical-modelling.md#log-likelihood) with fractional responses $\tau_i$ and a Poisson [log-likelihood](statistical-modelling.md#log-likelihood) with weights $1-\tau_i$. With only a binary predictor, write $n_j$ for group size, $S_j=\sum_{x_i=j}\tau_i$ and $C_j=\sum_{x_i=j}Y_i$; the explicit updates are $\pi_j=S_j/n_j$ and $\mu_j=C_j/(n_j-S_j)$. Log and logit group contrasts recover the regression coefficients, with boundary values interpreted through limits.

### Poisson central limit theorem

↑ **Parent:** [Poisson distribution](#poisson-distribution)

If $N_\lambda\sim\operatorname{Pois}(\lambda)$ and $\lambda\to\infty$, then

$$
\frac{N_\lambda-\lambda}{\sqrt\lambda}
\ \xrightarrow{\mathrm d}\ N(0,1).
$$

Indeed, its [characteristic function](probability-theory.md#characteristic-function) is

$$
\exp\!\left(\lambda\left(e^{it/\sqrt\lambda}-1-\frac{it}{\sqrt\lambda}\right)\right)
\longrightarrow e^{-t^2/2}.
$$

#### Poisson cumulative probability at its growing mean

↑ **Parent:** [Poisson central limit theorem](#poisson-central-limit-theorem)

If $X_\lambda$ has a [Poisson distribution](#poisson-distribution), then $\mathbb P(X_\lambda\leq\lfloor\lambda\rfloor)\to1/2$ as $\lambda\to\infty$. The [Poisson central limit theorem](#poisson-central-limit-theorem) standardizes by mean $\lambda$ and [variance](variance.md) $\lambda$; the cutoff $(\lfloor\lambda\rfloor-\lambda)/\sqrt\lambda$ tends to zero. Squeezing between fixed nearby cutoffs and using continuity of the standard [normal distribution](probability-theory.md#normal-distribution) function gives the limit.

### Poisson-multinomial conditioning

↑ **Parent:** [Poisson distribution](#poisson-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson-multinomial_conditioning)

Independent Poisson counts conditioned on their sum have a multinomial distribution.

#### Poisson trick

↑ **Parent:** [Poisson-multinomial conditioning](#poisson-multinomial-conditioning)

For each group $g$, let independent cell counts have Poisson means $\mu_{gj}$. Conditional on their total $n_g$, the cells have a [multinomial distribution](#multinomial-distribution) with probabilities

$$
\pi_{gj}=\frac{\mu_{gj}}{\sum_k\mu_{gk}}.
$$

Including a free group main effect in the Poisson log-linear model makes its profiled likelihood for the remaining parameters proportional to the corresponding multinomial likelihood. The two fits therefore give the same fitted proportions and likelihood-ratio comparisons.

##### Flat log-rate marginalization gives the multinomial likelihood

↑ **Parent:** [Poisson trick](#poisson-trick)

For positive group totals, the [improper prior](statistical-inference.md#improper-prior) $du/u$ on an independent Poisson baseline yields the [multinomial likelihood](#multinomial-likelihood) kernel after integration. This prior is flat in $\log u$. A proper finite-variance log-rate prior generally introduces an additional coefficient-dependent factor.

###### Gaussian log-rate correction to the Poisson trick

↑ **Parent:** [Flat log-rate marginalization gives the multinomial likelihood](#flat-log-rate-marginalization-gives-the-multinomial-likelihood)

A mean-zero [normal distribution](probability-theory.md#normal-distribution) prior of variance $s^2$ on the log baseline multiplies the multinomial kernel by the displayed correction, up to a constant independent of coefficients. The factor is not constant in $S$, so the posterior equivalence is approximate. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) makes it tend to one as $s^2$ tends to infinity.

### Normal approximation to the Poisson distribution

↑ **Parent:** [Poisson distribution](#poisson-distribution)

For large $\lambda$, a Poisson random variable of mean $\lambda$ is approximately normal with mean and variance $\lambda$.

## ↑ Ancestors (6)

1. [Probability distribution](probability-theory.md#probability-distribution)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33.md#1/solution)
