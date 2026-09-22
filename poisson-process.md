# Poisson process

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_process)

A [Homogeneous Poisson process](poisson-process.md) models arrivals at a constant rate $\lambda>0$. Its [counting process](stochastic-process.md#counting-process) $N_t=N(t)$ counts arrivals in $(0,t]$, with $N_0=0$. Its paths are [right-continuous](calculus.md#right-continuous-function) [nondecreasing functions](calculus.md#nondecreasing-function), take nonnegative [integer](integer.md) values, and have unit jumps [almost surely](convergence-of-random-variables.md#almost-sure-convergence). The defining [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of each increment is

$$
\mathbb P(N_{s+t}-N_s=k)=e^{-\lambda t}\frac{(\lambda t)^k}{k!},\qquad s\geq0,\quad t>0,\quad k=0,1,2,\ldots.
$$

It has [stationary increments](stochastic-process.md#stationary-increments): the [probability distribution](probability-distribution.md) above depends on the duration $t$, not the starting time $s$. It also has [independent increments](stochastic-process.md#independent-increments): counts in any finite collection of disjoint time intervals are [independent random variables](random-variable.md#independent-random-variables). Together these conditions specify the joint count laws, not merely the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) at a single time.[pp. 78-79: counting-process definition and its equivalence to exponential interarrival times](mathematics-bibliography.md#discrete-stochastic-processes-draft-of-2nd-edition-31-january-2011-by-robert-gallager/poisson-processes-chapter-2)

The rate has units of arrivals per unit time; $\lambda t$ is dimensionless. The [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) gives

$$
\mathbb E[N_{s+t}-N_s]=\operatorname{Var}(N_{s+t}-N_s)=\lambda t.
$$

For a toy rate $\lambda=2$ per minute and a duration of $1.5$ minutes, the [expected value](expected-value.md) and [variance](variance.md) of the count are both $3$. The [probability](probability-theory.md#probability) of no arrival is $e^{-3}\approx0.049787$, and the [probability](probability-theory.md#probability) of exactly three is $3^3e^{-3}/3!=\tfrac92e^{-3}\approx0.224042$. In two consecutive one-minute intervals, the [probability](probability-theory.md#probability) of exactly two arrivals in the first and exactly one in the second is $(2e^{-2})(2e^{-2})=4e^{-4}\approx0.073263$, using [independent increments](stochastic-process.md#independent-increments). These are exact model calculations with rounded decimals, not measured frequencies.

<a id="image-synthetic-arrival-times-and-their-right-continuous-counting-path-compared-with-the-exact-mean-at-two-arrivals-per-minute"></a>
![](poisson-arrival-events-counting-path.png)

**[Figure 1](#image-synthetic-arrival-times-and-their-right-continuous-counting-path-compared-with-the-exact-mean-at-two-arrivals-per-minute). Synthetic arrival times and their right-continuous counting path, compared with the exact mean at two arrivals per minute**.

The diagram's nine hand-chosen arrivals illustrate a path; the line $\lambda t$ is an [expected value](expected-value.md), not a prescribed trajectory. Constant rate does not imply evenly spaced arrivals. [Poisson interarrival times](#poisson-interarrival-times) connect the count description to waiting, while [Poisson thinning](#poisson-thinning) explains how independently routing arrivals produces separate streams. This makes the [Poisson process](poisson-process.md) useful as a simple arrival model for a [queue](queueing-theory.md#queue-queueing-theory), provided constant rate and [independent increments](stochastic-process.md#independent-increments) are plausible. For a deterministic changing rate, use an [Inhomogeneous Poisson process](#inhomogeneous-poisson-process); bunching or history-dependent arrivals need additional assumptions. Conditional on $N_t=n$, the arrival times are the [order statistics](probability-theory.md#order-statistic) of $n$ [independent](random-variable.md#independent-random-variables) [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,t]$, as developed in [Poisson process conditional arrival times](#poisson-process-conditional-arrival-times).

**Table of contents**

- [Poisson interarrival times](#poisson-interarrival-times)
- [Poisson observation scheme and rate likelihood](#poisson-observation-scheme-and-rate-likelihood)
- [Strong law for Poisson arrival times](#strong-law-for-poisson-arrival-times)
- [Poisson exponential martingale](#poisson-exponential-martingale)
- [Poisson maximal concentration bound](#poisson-maximal-concentration-bound)
- [Every second Poisson arrival has underdispersed counts](#every-second-poisson-arrival-has-underdispersed-counts)
- [Cox process](#cox-process)
  - [Poisson offspring clusters directed by their parent process](#poisson-offspring-clusters-directed-by-their-parent-process)
  - [Random directing measure of a Cox process](#random-directing-measure-of-a-cox-process)
- [Inhomogeneous Poisson process](#inhomogeneous-poisson-process)
  - [Time change of an inhomogeneous Poisson process](#time-change-of-an-inhomogeneous-poisson-process)
- [Symmetric Poisson difference process](#symmetric-poisson-difference-process)
- [Poisson thinning](#poisson-thinning)
  - [Dependence in Poisson thinning](#dependence-in-poisson-thinning)
  - [Poisson characterization by independent binomial splitting](#poisson-characterization-by-independent-binomial-splitting)
  - [Categorical thinning of a Poisson claim count](#categorical-thinning-of-a-poisson-claim-count)
  - [Poisson onset-bin independence](#poisson-onset-bin-independence)
  - [Binomial thinning conditional on a total](#binomial-thinning-conditional-on-a-total)
  - [Infinite-server queue transient distribution](#infinite-server-queue-transient-distribution)
- [Kolmogorov forward equation for a Poisson process](#kolmogorov-forward-equation-for-a-poisson-process)
- [Poisson process conditional arrival times](#poisson-process-conditional-arrival-times)
- [Number of one Poisson type before another](#number-of-one-poisson-type-before-another)
- [Exponential formula for a marked Poisson sum](#exponential-formula-for-a-marked-poisson-sum)
- [Age of a Poisson process](#age-of-a-poisson-process)

## Poisson interarrival times

↑ **Parent:** [Poisson process](poisson-process.md)

Let $T_n=\inf\{t\geq0:N_t\geq n\}$ be the $n$th arrival time, and set $T_0=0$. In a [Homogeneous Poisson process](poisson-process.md) of rate $\lambda>0$, the gaps $W_n=T_n-T_{n-1}$ are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with an [exponential distribution](continuous-probability-distribution.md#exponential-distribution):

$$
\mathbb P(W_n>w)=e^{-\lambda w},\qquad f_{W_n}(w)=\lambda e^{-\lambda w},\qquad w\geq0;
\qquad \mathbb E[W_n]=\frac1\lambda,\quad \operatorname{Var}(W_n)=\frac1{\lambda^2}.
$$

Here $\operatorname{Exp}(\lambda)$ uses the rate convention. Under the scale convention $\theta=1/\lambda$, the same [probability density function](continuous-probability-distribution.md#probability-density-function) is $\theta^{-1}e^{-w/\theta}$; a simulation function accepting a scale must receive $1/\lambda$. Conversely, summing [independent](random-variable.md#independent-random-variables) rate-$\lambda$ [exponential random variables](continuous-probability-distribution.md#exponential-distribution) to form $T_n$ and counting those sums constructs a [Homogeneous Poisson process](poisson-process.md).[Theorem 7.2, printed p. 59: interval theorem characterizing independent exponential gaps](mathematics-bibliography.md#lectures-on-the-poisson-process-by-gunter-last-and-others)

The first-gap formula follows immediately from $\{W_1>w\}=\{N_w=0\}$ and the [Poisson distribution](discrete-probability-distribution.md#poisson-distribution). Independence of all successive gaps is the additional interval-theorem assertion; deterministic-time [independent increments](stochastic-process.md#independent-increments) alone should not simply be substituted at random arrival times without justification. The [memorylessness of the exponential distribution](continuous-probability-distribution.md#memorylessness-of-the-exponential-distribution) gives

$$
\mathbb P(W_n>a+w\mid W_n>a)=e^{-\lambda w},\qquad a,w\geq0.
$$

At the toy rate of two per minute, the [mean](expected-value.md) gap is half a minute, the [median](probability-distribution.md#median) is $(\log2)/2\approx0.346574$ minutes, and the [probability](probability-theory.md#probability) of waiting longer than half a minute is $e^{-1}\approx0.367879$. Here $\log$ is the [natural logarithm](calculus.md#natural-logarithm). Already having waited a minute without an arrival leaves this same [conditional probability](probability-theory.md#conditional-probability) of waiting another half minute. The [exponential distribution](continuous-probability-distribution.md#exponential-distribution) describes a model with no aging of the remaining wait; a scheduled arrival with a fixed gap has no such property.

## Poisson observation scheme and rate likelihood

↑ **Parent:** [Poisson process](poisson-process.md)

A [Poisson process](poisson-process.md) observed for a fixed duration $H$ has likelihood proportional to $\lambda^{N_H}e^{-\lambda H}$. Complete independent [exponential distribution](continuous-probability-distribution.md#exponential-distribution) gaps observed until a fixed event count $n$ have likelihood $\lambda^ne^{-\lambda T_n}$. Both give count divided by exposure, but the exposure is random in the second design. Under fixed exposure the total count is sufficient: conditional on it, the event locations are independent of the rate, so exact timestamps add no rate information to interval counts. Gap estimates and fixed-horizon estimates should not be compared without distinguishing their stopping rules and any final censored gap.

## Strong law for Poisson arrival times

↑ **Parent:** [Poisson process](poisson-process.md)

For a homogeneous [Poisson process](poisson-process.md) of rate $\lambda>0$, $N(t)/t\to\lambda$ almost surely: unit-time increments are independent Poisson variables and the [strong law of large numbers](convergence-of-random-variables.md#strong-law-of-large-numbers) applies, then monotonicity fills the intervals between integers. At its $n$th point $Y_n$, simplicity gives $N(Y_n)=n$. Consequently $Y_n/n\to1/\lambda$. Rate and mean interarrival time are reciprocals.

## Poisson exponential martingale

↑ **Parent:** [Poisson process](poisson-process.md)

For a unit-rate [Poisson process](poisson-process.md) and real $\theta$, the displayed process is a nonnegative [martingale](martingale.md) with initial value one. Independent increments give $\mathbb E e^{\theta(N_t-N_s)}=\exp((t-s)(e^\theta-1))$, proving its conditional mean property. The [Ville inequality](martingale.md#ville-inequality) turns this exponential moment into a maximal tail bound.

## Poisson maximal concentration bound

↑ **Parent:** [Poisson process](poisson-process.md)

For a unit-rate [Poisson process](poisson-process.md), $h(\eta)=(1+\eta)\log(1+\eta)-\eta$ gives the displayed maximal deviation bound for $L,\eta>0$. [Poisson exponential martingales](#poisson-exponential-martingale) and the [Ville inequality](martingale.md#ville-inequality) control upper and lower deviations; the upper-tail rate $h$ also bounds the lower-tail probability. Since $h(0)=0$ and $h'(\eta)=\log(1+\eta)>0$, the rate is strictly positive for every positive deviation level.

## Every second Poisson arrival has underdispersed counts

↑ **Parent:** [Poisson process](poisson-process.md)

For a rate-$\lambda$ [Poisson process](poisson-process.md), keeping every second arrival gives a renewal process with independent interarrival times equal to sums of two exponential waiting times. Put $x=\lambda t$. Its count mean and variance are $(2x+e^{-2x}-1)/4$ and $(4x-8xe^{-2x}-e^{-4x}+1)/16$. The variance is strictly smaller than the mean for $x>0$: sixteen times their difference has derivative $4[-1+4xe^{-2x}+e^{-4x}]<0$ and is zero at zero, because $\sinh(2x)>2x$. Therefore this process is not a [Cox process](#cox-process).

## Cox process

↑ **Parent:** [Poisson process](poisson-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cox_process)

A counting process which, conditional on a random nonnegative locally integrable intensity $\Lambda$, is an [Inhomogeneous Poisson process](#inhomogeneous-poisson-process). For $L_t=\int_0^t\Lambda(s)\,ds$, conditioning gives $\mathbb EN(t)=\mathbb EL_t$ and $\operatorname{Var}N(t)=\mathbb EL_t+\operatorname{Var}L_t$. Thus finite-variance counts are never underdispersed. Randomness of the intensity may induce dependence between increments which are independent conditionally.

### Poisson offspring clusters directed by their parent process

↑ **Parent:** [Cox process](#cox-process)

When each parent has a Poisson number of independently displaced offspring, the conditional offspring process has the displayed directing measure. For disjoint target sets, [multinomial distribution](discrete-probability-distribution.md#multinomial-distribution) splitting of a parent's Poisson count gives joint [probability generating function](probability-distribution.md#probability-generating-function) $\exp(\mu\sum_j\kappa(A_j-z)(s_j-1))$. Multiply over [independent](random-variable.md#independent-random-variables) parents to obtain [independent](random-variable.md#independent-random-variables) Poisson counts conditional on the parents. Compactly supported displacement ensures local finiteness for a locally finite parent process.

// Destination: discrete-probability-distribution.bigb

### Random directing measure of a Cox process

↑ **Parent:** [Cox process](#cox-process)

A [Cox process](#cox-process) can be directed by a random locally [finite measure](measure.md#finite-measure), which need not have a density. Conditional counts in disjoint sets are [independent](random-variable.md#independent-random-variables) Poisson variables with that measure's masses. Uniform circular offspring displacements give a directing measure supported on random circles; its unconditional mean can still be a multiple of planar [Lebesgue measure](measure-theory.md#lebesgue-measure). A random intensity function is the special case in which the directing measure is absolutely continuous.

## Inhomogeneous Poisson process

↑ **Parent:** [Poisson process](poisson-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Inhomogeneous_Poisson_process)

An inhomogeneous Poisson process with locally integrable intensity $\lambda(t)\geq0$ has independent increments and

$$
N_t-N_s\sim\operatorname{Poisson}\left(\int_s^t\lambda(u)\,du\right)
$$

for $0\leq s<t$. Its cumulative intensity is $\Lambda(t)=\int_0^t\lambda(u)\,du$.

### Time change of an inhomogeneous Poisson process

↑ **Parent:** [Inhomogeneous Poisson process](#inhomogeneous-poisson-process)

If $\lambda>0$ and $g=\Lambda^{-1}$, then $M_t=N_{g(t)}$ is a rate-one [Poisson process](poisson-process.md), because

$$
\Lambda(g(t))-\Lambda(g(s))=t-s.
$$

Conversely, $N_t=M_{\Lambda(t)}$, so $N_t$ has a Poisson distribution of mean $\Lambda(t)$.

## Symmetric Poisson difference process

↑ **Parent:** [Poisson process](poisson-process.md)

The difference of two independent rate-$\lambda$ [Poisson processes](poisson-process.md) is a continuous-time simple symmetric random walk with total jump rate $2\lambda$ and variance $2\lambda t$ at time $t$.

## Poisson thinning

↑ **Parent:** [Poisson process](poisson-process.md)

[Poisson thinning](#poisson-thinning) splits a [Poisson process](poisson-process.md) by independently marking each arrival as retained or rejected. Let the original [Homogeneous Poisson process](poisson-process.md) have rate $\lambda>0$, and let $p(s)\in[0,1]$ be a deterministic [measurable function](measure-theory.md#measurable-function) of time. Attach [independent](random-variable.md#independent-random-variables) [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) $U_1,U_2,\ldots$ on $(0,1)$, independent of the entire original [Poisson process](poisson-process.md). At arrival time $T_i$, retain the arrival if $U_i\leq p(T_i)$. Given all arrival times, these decisions are [independent](random-variable.md#independent-random-variables) and have the specified retention [probabilities](probability-theory.md#probability). Define the two [counting processes](stochastic-process.md#counting-process) using an [indicator function](measure-theory.md#indicator-function):

$$
R_t=\sum_{i:T_i\leq t}\mathbf1_{\{U_i\leq p(T_i)\}},\qquad D_t=N_t-R_t.
$$

The [Poisson thinning theorem](poisson-point-process.md#poisson-thinning-theorem) gives [independent](random-variable.md#independent-random-variables) retained and rejected [Inhomogeneous Poisson processes](#inhomogeneous-poisson-process). Their rates are $\lambda p(s)$ and $\lambda(1-p(s))$, respectively, in the sense of the [intensity function of a point process](poisson-point-process.md#intensity-function-of-a-point-process). In particular, for $0\leq a<b$,

$$
R_b-R_a\sim\operatorname{Poisson}\!\left(\lambda\int_a^b p(s)\,ds\right),\qquad D_b-D_a\sim\operatorname{Poisson}\!\left(\lambda\int_a^b(1-p(s))\,ds\right).
$$

The [independence](random-variable.md#independent-random-variables) is of the two whole processes: every finite collection of retained counts is [independent](random-variable.md#independent-random-variables) of every finite collection of rejected counts. It is not merely zero [covariance](variance.md#covariance) for one interval. For constant $p$, the streams are [Homogeneous Poisson processes](poisson-process.md) of rates $\lambda p$ and $\lambda(1-p)$; the endpoints $p=0,1$ include the identically zero stream.[Definition 5.7, Proposition 5.5, Theorem 5.8 and Corollary 5.9, printed pp. 42-44: location-dependent independent marking, intensities, and independence of the split processes](mathematics-bibliography.md#lectures-on-the-poisson-process-by-gunter-last-and-others)

For an exact toy calculation, take $\lambda=2$ per minute and retain with $p(s)=1/4$ on $(0,2]$ and $p(s)=3/4$ on $(2,4]$. In the first two minutes, the retained and rejected [expected values](expected-value.md) are $2\cdot2\cdot1/4=1$ and $2\cdot2\cdot3/4=3$. In the next two minutes they are $3$ and $1$. Over all four minutes, $R_4,D_4$ are [independent](random-variable.md#independent-random-variables) [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) with [mean](expected-value.md) $4$ each, and their sum $N_4$ has [mean](expected-value.md) $8$. Thus

$$
\mathbb P(R_4=0,D_4=0)=e^{-4}e^{-4}=e^{-8},\qquad \mathbb P(R_4=2,D_4=3)=e^{-8}\frac{4^2}{2!}\frac{4^3}{3!}=\frac{256}{3}e^{-8}.
$$

These [probabilities](probability-theory.md#probability) and [expected values](expected-value.md) describe the model, not empirical measurements. In the diagram, the original nine synthetic arrivals split into five retained and four rejected arrivals; those realized counts need not equal their [expected values](expected-value.md).

<a id="image-independent-marks-split-a-synthetic-poisson-arrival-path-with-exact-expected-counts-for-two-time-dependent-retention-probabilities"></a>
![](poisson-independent-thinning-expected-counts.png)

**[Figure 2](#image-independent-marks-split-a-synthetic-poisson-arrival-path-with-exact-expected-counts-for-two-time-dependent-retention-probabilities). Independent marks split a synthetic Poisson arrival path, with exact expected counts for two time-dependent retention probabilities**.

The mechanism explains why mutually exclusive labels can yield [independent](random-variable.md#independent-random-variables) counts: randomness of the original total offsets the dependence from allocating a fixed total. For constant $p$ and an interval with original [mean](expected-value.md) $m$, the conditional retained count has a [binomial distribution](discrete-probability-distribution.md#binomial-distribution) given $N=n$. The joint [probability generating function](probability-distribution.md#probability-generating-function) is

$$
\mathbb E[z^Rw^D]=\mathbb E[(pz+(1-p)w)^N]=\exp\{m(pz+(1-p)w-1)\}=e^{mp(z-1)}e^{m(1-p)(w-1)},\qquad 0\leq z,w\leq1.
$$

This factorization proves the two [independent](random-variable.md#independent-random-variables) [Poisson distributions](discrete-probability-distribution.md#poisson-distribution); disjoint original intervals give [independent](random-variable.md#independent-random-variables) pairs. For varying $p(s)$, the [Independent marking theorem for Poisson point processes](poisson-point-process.md#independent-marking-theorem-for-poisson-point-processes) gives the same conclusion with the two integrated intensities. The [joint red and green Poisson count formula](poisson-point-process.md#joint-red-and-green-poisson-count-formula) gives the corresponding direct calculation with [probability mass functions](probability-distribution.md#probability-mass-function).

Independence here is unconditional. After conditioning on $N=n$, the identity $D=n-R$ gives [covariance](variance.md#covariance) $\operatorname{Cov}(R,D\mid N=n)=-np(1-p)$ for constant $p$. Thus the retained and rejected counts are dependent for $n>0$ and $0<p<1$, even though their unconditional [covariance](variance.md#covariance) is zero. [Poisson thinning](#poisson-thinning) can model independent routing of arrivals, or independent detection of arrivals with a known efficiency schedule; using only a retention fraction without checking the marking mechanism can give a wrong count law.

### Dependence in Poisson thinning

↑ **Parent:** [Poisson thinning](#poisson-thinning)

Independent marking is the hypothesis that guarantees the [Poisson thinning theorem](poisson-point-process.md#poisson-thinning-theorem). Equal marginal retention [probabilities](probability-theory.md#probability) do not guarantee it. Consider one [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) $B$ with success [probability](probability-theory.md#probability) $p\in(0,1)$, independent of a [Poisson process](poisson-process.md), and retain every arrival when $B=1$ and none when $B=0$. Each arrival is retained with [probability](probability-theory.md#probability) $p$, but the marks share the same coin. In an interval whose original count has [Poisson distribution](discrete-probability-distribution.md#poisson-distribution) of [mean](expected-value.md) $m>0$, the retained count is $R=BN$ and the rejected count is $D=(1-B)N$, so

$$
\mathbb E[R]=pm,\qquad \operatorname{Var}(R)=pm+p(1-p)m^2,\qquad \operatorname{Cov}(R,D)=-p(1-p)m^2.
$$

The extra [variance](variance.md) shows that $R$ is not [Poisson distributed](discrete-probability-distribution.md#poisson-distribution); the negative [covariance](variance.md#covariance) proves dependence. Its no-arrival [probability](probability-theory.md#probability) is $1-p+pe^{-m}$, rather than $e^{-pm}$. For the toy values $p=1/2,m=2$, both rules have retained [mean](expected-value.md) $1$, but the common-coin rule has [variance](variance.md) $2$ and no-arrival [probability](probability-theory.md#probability) $(1+e^{-2})/2\approx0.567668$, compared with [variance](variance.md) $1$ and no-arrival [probability](probability-theory.md#probability) $e^{-1}\approx0.367879$ for independent marking. These formulas follow by conditioning on $B$ and using the [law of total variance](probability-theory.md#law-of-total-variance).

An arrival-dependent or adversarial retention rule can change the law just as strongly. Keeping every second arrival gives $R_t=\lfloor N_t/2\rfloor$. Its successive retained gaps are sums of two [independent](random-variable.md#independent-random-variables) [exponential random variables](continuous-probability-distribution.md#exponential-distribution), hence have the [Erlang distribution](continuous-probability-distribution.md#erlang-distribution) of shape two and rate $\lambda$, not an [exponential distribution](continuous-probability-distribution.md#exponential-distribution). The resulting [renewal process](probability-theory.md#renewal-process) and its count [variance](variance.md) are analyzed in [Every second Poisson arrival has underdispersed counts](#every-second-poisson-arrival-has-underdispersed-counts), and the two dependent streams in [alternating split of a Poisson process](probability-theory.md#alternating-split-of-a-poisson-process). As an even more restrictive rule, keeping only the first arrival ever gives $R_t=\mathbf1_{\{N_t\geq1\}}$, a [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution) at each $t>0$, so it cannot have a positive-mean [Poisson distribution](discrete-probability-distribution.md#poisson-distribution). A thinning rule must specify how decisions depend on arrivals and on one another; the independent-marking conclusion cannot be applied automatically to arbitrary deletion.

### Poisson characterization by independent binomial splitting

↑ **Parent:** [Poisson thinning](#poisson-thinning)

Let $N$ be a nonnegative integer-valued [random variable](random-variable.md) with finite [expected value](expected-value.md) $\mu$, and independently label each of its items with either of two equally likely labels. If the two resulting counts are [independent random variables](random-variable.md#independent-random-variables), then $N$ has a [Poisson distribution](discrete-probability-distribution.md#poisson-distribution). Indeed, its [probability generating function](probability-distribution.md#probability-generating-function) obeys $G(s)=G((1+s)/2)^2$. With $H(t)=G(1-t)$, iteration gives $H(t)=H(t/2^k)^{2^k}$. Finite [expected value](expected-value.md) gives $H(h)=1-\mu h+o(h)$, hence $H(t)=e^{-\mu t}$ and $G(s)=e^{\mu(s-1)}$. Conversely, [Poisson thinning](#poisson-thinning) produces independent [Poisson distributions](discrete-probability-distribution.md#poisson-distribution) for the two counts.

### Categorical thinning of a Poisson claim count

↑ **Parent:** [Poisson thinning](#poisson-thinning)

Assign each of $N\sim\operatorname{Pois}(\lambda)$ claims with [independent](random-variable.md#independent-random-variables) category labels to one of finitely many categories with [probabilities](probability-theory.md#probability) $p_i$. Conditional counts have a [multinomial distribution](discrete-probability-distribution.md#multinomial-distribution) with [probability generating function](probability-distribution.md#probability-generating-function) $(\sum_i p_i z_i)^N$. Averaging over $N$ gives $\exp(\lambda(\sum_i p_i z_i-1))=\prod_i\exp(\lambda p_i(z_i-1))$. This proves [independent](random-variable.md#independent-random-variables) category counts and supports discrete-severity [compound Poisson distribution](actuarial-statistics.md#compound-poisson-distribution) representations.

### Poisson onset-bin independence

↑ **Parent:** [Poisson thinning](#poisson-thinning)

Mark each member of an independent Poisson infection cohort by its symptom-onset interval, using independent delays. [Poisson thinning](#poisson-thinning) gives independent onset-bin counts, and sums over independent cohorts remain independent Poisson counts. Fixed cohort totals instead induce multinomial dependence. The marking assumptions are essential.

### Binomial thinning conditional on a total

↑ **Parent:** [Poisson thinning](#poisson-thinning)

Conditioned on a total of $n$ Poisson points, the number falling in a region of relative intensity $p$ is $\operatorname{Binomial}(n,p)$.

### Infinite-server queue transient distribution

↑ **Parent:** [Poisson thinning](#poisson-thinning)

For an [M-M-infinity queue](continuous-time-markov-chain.md#m-m-∞-queue) with empty initial state, Poisson arrivals of rate $\lambda$ and exponential lifetimes of rate $\mu$ produce a Poisson occupancy of mean $\lambda(1-e^{-\mu t})/\mu$ at time $t$.

## Kolmogorov forward equation for a Poisson process

↑ **Parent:** [Poisson process](poisson-process.md)

The state probabilities satisfy $p_0'=-\lambda p_0$ and $p_n'=\lambda p_{n-1}-\lambda p_n$, yielding the Poisson law of mean $\lambda t$.

## Poisson process conditional arrival times

↑ **Parent:** [Poisson process](poisson-process.md)

Conditioned on $N_t=n$, the arrival times are distributed as the order statistics of $n$ independent uniform points on $[0,t]$. Their conditional joint density on

$$
0<s_1<\cdots<s_n<t
$$

is $n!/t^n$, obtained by dividing the Poisson-process density $\lambda^ne^{-\lambda t}$ by $\mathbb P(N_t=n)$.

## Number of one Poisson type before another

↑ **Parent:** [Poisson process](poisson-process.md)

For independent Poisson processes of rates $\lambda_1$ and $\lambda_2$, the number $K$ of type-two arrivals before the first type-one arrival satisfies

$$
\mathbb P(K=k)
=\left(\frac{\lambda_2}{\lambda_1+\lambda_2}\right)^k
\frac{\lambda_1}{\lambda_1+\lambda_2}.
$$

This follows by marking the superposed process by its arrival type.

## Exponential formula for a marked Poisson sum

↑ **Parent:** [Poisson process](poisson-process.md)

Let $J_i$ be the points of a rate-$\lambda$ Poisson process and let independent identically distributed marks $X_i$ be independent of the process. Then

$$
\mathbb E\exp\left(\theta\sum_{i=1}^{N_t}g(J_i,X_i)\right)
=\exp\left\{\lambda\int_0^t
\left(\mathbb E e^{\theta g(s,X_1)}-1\right)ds\right\}.
$$

Condition on $N_t$, use uniform order statistics, and sum the resulting exponential series.

## Age of a Poisson process

↑ **Parent:** [Poisson process](poisson-process.md)

With $J_0=0$, the age $A(t)=t-J_{N_t}$ of a rate-$\lambda$ Poisson process has mean

$$
\mathbb EA(t)=\frac{1-e^{-\lambda t}}{\lambda}.
$$

Given $N_t=n$, the last arrival is the maximum of $n$ uniform points and $\mathbb E[A(t)\mid N_t=n]=t/(n+1)$, including $n=0$.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (171)

- [Accidental coincidence](particle-detection.md#accidental-coincidence)
- [Alternating split of a Poisson process](probability-theory.md#alternating-split-of-a-poisson-process)
- [Atomic compound Poisson process with drift](stochastic-process.md#atomic-compound-poisson-process-with-drift)
- [Burke theorem for a multi-server queue](queueing-theory.md#burke-theorem-for-a-multi-server-queue)
- [Burke theorem for an M-M-infinity queue](continuous-time-markov-chain.md#burke-theorem-for-an-m-m-infinity-queue)
- [Classical risk model](actuarial-statistics.md#classical-risk-model)
- [Compound Poisson process](stochastic-process.md#compound-poisson-process)
- [Continuous-time symmetric simple random walk](stochastic-process.md#continuous-time-symmetric-simple-random-walk)
- [Delayed neutron-capture coincidence window](physics.md#delayed-neutron-capture-coincidence-window)
- [Dependence in Poisson thinning](#dependence-in-poisson-thinning)
- [Detector dead time](particle-detection.md#detector-dead-time)
- [Difference of independent Poisson processes](stochastic-process.md#difference-of-independent-poisson-processes)
- [Every second Poisson arrival has underdispersed counts](#every-second-poisson-arrival-has-underdispersed-counts)
- [Exponential Laplace martingale of a compound Poisson process](stochastic-process.md#exponential-laplace-martingale-of-a-compound-poisson-process)
- [Flow-level network model](queueing-theory.md#flow-level-network-model)
- [Geometric galaxy-encounter rate](galaxy.md#geometric-galaxy-encounter-rate)
- [Graphical representation of the contact process](stochastic-process.md#graphical-representation-of-the-contact-process)
- [Heterogeneous two-server queue](queueing-theory.md#heterogeneous-two-server-queue)
- [Increment](stochastic-process.md#increment)
- [Independent increments](stochastic-process.md#independent-increments)
- [Insensitivity of loss networks](queueing-theory.md#insensitivity-of-loss-networks)
- [Inverse-power sum over Poisson arrivals](poisson-point-process.md#inverse-power-sum-over-poisson-arrivals)
- [Little's law](queueing-theory.md#little-s-law)
- [Loss given default](mathematical-finance.md#loss-given-default)
- [Loss network](queueing-theory.md#loss-network)
- [M/D/1 queue](queueing-theory.md#m-d-1-queue)
- [M/M/1 utilization and delay](queueing-theory.md#m-m-1-utilization-and-delay)
- [M-M-s-K queue](continuous-time-markov-chain.md#m-m-s-k-queue)
- [M/M/∞ queue](continuous-time-markov-chain.md#m-m-∞-queue)
- [Mutation count on a neutral coalescent tree](continuous-time-markov-chain.md#mutation-count-on-a-neutral-coalescent-tree)
- [Neuronal refractory period](neuroscience.md#neuronal-refractory-period)
- [Nonexplosion of a continuous-time Markov chain](continuous-time-markov-chain.md#nonexplosion-of-a-continuous-time-markov-chain)
- [Open migration process](queueing-theory.md#open-migration-process)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-73.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-30.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-34.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-39.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-29.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-1.md#26i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-36.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-34.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-36.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-45.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-45.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-46.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-73.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#26i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-4.md#26i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-89.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-3.md#26j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#26j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4.md#26j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-30.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-37.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#27i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#27i/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-3.md#26i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3.md#26j/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-32.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-40.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-28.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-37.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-72.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-35.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-62.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#24k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-2.md#24k/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-3.md#23k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-35.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-39.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-207.md#3/f/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-213.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-320.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2.md#25k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2.md#27j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#27j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-213.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-316.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#27k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-201.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-346.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#27k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#27k/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#27k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3.md#27j/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-201.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-325.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1.md#28j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#27j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-3.md#27j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-3.md#27l/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1.md#28k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#6/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-353.md#4/a/i/solution)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1.md#section-d/d13/a/solution)
- [Photon correlation loss and background model](quantum-optics.md#photon-correlation-loss-and-background-model)
- [Poisson arrivals see time averages](queueing-theory.md#poisson-arrivals-see-time-averages)
- [Poisson distribution](discrete-probability-distribution.md#poisson-distribution)
- [Poisson exponential martingale](#poisson-exponential-martingale)
- [Poisson maximal concentration bound](#poisson-maximal-concentration-bound)
- [Poisson migration stream without a return path](queueing-theory.md#poisson-migration-stream-without-a-return-path)
- [Poisson observation scheme and rate likelihood](#poisson-observation-scheme-and-rate-likelihood)
- [Poisson process](poisson-process.md)
- [Poisson-sampled continuous-time Markov chain](continuous-time-markov-chain.md#poisson-sampled-continuous-time-markov-chain)
- [Poisson superposition of insurance portfolios](actuarial-statistics.md#poisson-superposition-of-insurance-portfolios)
- [Poisson thinning](#poisson-thinning)
- [Poisson time-change representation of a Markov chain](continuous-time-markov-chain.md#poisson-time-change-representation-of-a-markov-chain)
- [Poissonization](probability-theory.md#poissonization)
- [Queueing theory](queueing-theory.md)
- [Quota-share retention under exponential utility](actuarial-statistics.md#quota-share-retention-under-exponential-utility)
- [Rearrangeable triangular loss network](queueing-theory.md#rearrangeable-triangular-loss-network)
- [Refractory limits on neuronal firing](neuroscience.md#refractory-limits-on-neuronal-firing)
- [Ruin integro-differential equation](actuarial-statistics.md#ruin-integro-differential-equation)
- [Sample path](stochastic-process.md#sample-path)
- [Sample-path area identity for Little's law](queueing-theory.md#sample-path-area-identity-for-little-s-law)
- [Shot noise](electrical-engineering.md#shot-noise)
- [Shot noise departures from Poisson statistics](electrical-engineering.md#shot-noise-departures-from-poisson-statistics)
- [SN 1987A neutrino burst](stellar-astrophysics.md#sn-1987a-neutrino-burst)
- [Stationary increments](stochastic-process.md#stationary-increments)
- [Stochastic process](stochastic-process.md)
- [Strong law for Poisson arrival times](#strong-law-for-poisson-arrival-times)
- [Survival integro-differential equation for a classical risk model](actuarial-statistics.md#survival-integro-differential-equation-for-a-classical-risk-model)
- [Survival renewal equation for a classical risk model](actuarial-statistics.md#survival-renewal-equation-for-a-classical-risk-model)
- [Symmetric Poisson difference process](#symmetric-poisson-difference-process)
- [Symmetric simple exclusion process](stochastic-process.md#symmetric-simple-exclusion-process)
- [Time change of an inhomogeneous Poisson process](#time-change-of-an-inhomogeneous-poisson-process)
- [Trapped-ion fluorescence count model](atomic-physics.md#trapped-ion-fluorescence-count-model)
- [Two-sided order statistics of a boundary-singular Poisson process](poisson-point-process.md#two-sided-order-statistics-of-a-boundary-singular-poisson-process)
- [Voter-model duality](stochastic-process.md#voter-model-duality)
