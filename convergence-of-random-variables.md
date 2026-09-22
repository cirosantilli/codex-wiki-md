# Convergence of random variables

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convergence_of_random_variables)

The main modes include almost-sure convergence, convergence in probability, convergence in $L^p$, and convergence in distribution.

**Table of contents**

- [Contiguity of probability measures](#contiguity-of-probability-measures)
  - [Le Cam's first lemma](#le-cam-s-first-lemma)
  - [Mutual contiguity](#mutual-contiguity)
- [Convergence in Lp](#convergence-in-lp)
  - [Convergence in L1](#convergence-in-l1)
    - [Scheffé lemma](#scheffe-lemma)
  - [Convergence in L2](#convergence-in-l2)
    - [Almost-sure convergence and convergence of second moments](#almost-sure-convergence-and-convergence-of-second-moments)
- [Convergence in distribution](#convergence-in-distribution)
  - [Atoms obstruct a continuous distributional limit](#atoms-obstruct-a-continuous-distributional-limit)
  - [Marginal weak convergence does not control sums](#marginal-weak-convergence-does-not-control-sums)
  - [Skorokhod representation theorem](#skorokhod-representation-theorem)
  - [Method of moments (probability theory)](#method-of-moments-probability-theory)
  - [Weak convergence of probability measures](#weak-convergence-of-probability-measures)
    - [Compact containment](#compact-containment)
    - [Scaling limit of a random curve](#scaling-limit-of-a-random-curve)
    - [Skorokhod J1 topology](#skorokhod-j1-topology)
    - [Weak topology of probability measures](#weak-topology-of-probability-measures)
      - [Bounded-Lipschitz metric](#bounded-lipschitz-metric)
    - [Prokhorov's theorem](#prokhorov-s-theorem)
      - [Closed uniformly tight compactness criterion](#closed-uniformly-tight-compactness-criterion)
      - [Compactness of probability measures on a compact metric space](#compactness-of-probability-measures-on-a-compact-metric-space)
  - [Bounded moment criterion for weak convergence](#bounded-moment-criterion-for-weak-convergence)
    - [Moment determinacy on a compact interval](#moment-determinacy-on-a-compact-interval)
  - [Portmanteau theorem](#portmanteau-theorem)
  - [Continuous mapping theorem](#continuous-mapping-theorem)
- [Almost sure convergence](#almost-sure-convergence)
  - [Complete convergence of random variables](#complete-convergence-of-random-variables)
  - [Almost sure equality](#almost-sure-equality)
  - [Strong law of large numbers](#strong-law-of-large-numbers)
    - [Strong law for uniformly L2-bounded uncorrelated random variables](#strong-law-for-uniformly-l2-bounded-uncorrelated-random-variables)
    - [Strong law for adjacent products](#strong-law-for-adjacent-products)
  - [Kolmogorov convergence theorem](#kolmogorov-convergence-theorem)
  - [Law of the iterated logarithm](#law-of-the-iterated-logarithm)
    - [Brownian upper law of the iterated logarithm](#brownian-upper-law-of-the-iterated-logarithm)
    - [Upper law of the iterated logarithm](#upper-law-of-the-iterated-logarithm)
    - [Law of the iterated logarithm for a simple symmetric random walk](#law-of-the-iterated-logarithm-for-a-simple-symmetric-random-walk)
- [Cramér–Wold theorem](#cramer-wold-theorem)
- [Convergence in probability](#convergence-in-probability)
  - [Uniform convergence in probability](#uniform-convergence-in-probability)
  - [Boundedness in probability](#boundedness-in-probability)
    - [Stochastic order](#stochastic-order)
      - [Uniform pointwise probability bounds do not bound a random supremum](#uniform-pointwise-probability-bounds-do-not-bound-a-random-supremum)
  - [Convergence in distribution to a constant implies convergence in probability](#convergence-in-distribution-to-a-constant-implies-convergence-in-probability)
  - [Weak law of large numbers](#weak-law-of-large-numbers)
    - [Weak law without an absolute first moment](#weak-law-without-an-absolute-first-moment)
    - [Weak law forces a characteristic-function derivative](#weak-law-forces-a-characteristic-function-derivative)
    - [Uniform law of large numbers](#uniform-law-of-large-numbers)
      - [Pointwise separable function class](#pointwise-separable-function-class)
      - [Bracketing of a function class](#bracketing-of-a-function-class)
        - [Integrable envelope of a function class](#integrable-envelope-of-a-function-class)
        - [Uniform strong law from finite L1 bracketing](#uniform-strong-law-from-finite-l1-bracketing)
          - [Uniform strong law on a compact parameter set](#uniform-strong-law-on-a-compact-parameter-set)
      - [Glivenko-Cantelli theorem](#glivenko-cantelli-theorem)
        - [Quantile proof of the Glivenko-Cantelli theorem](#quantile-proof-of-the-glivenko-cantelli-theorem)
  - [Uniqueness of a limit in probability](#uniqueness-of-a-limit-in-probability)
  - [Bounded-metric characterization of convergence in probability](#bounded-metric-characterization-of-convergence-in-probability)
  - [Almost-sure subsequence from convergence in probability](#almost-sure-subsequence-from-convergence-in-probability)
  - [Independent rare-event counterexample to almost-sure convergence](#independent-rare-event-counterexample-to-almost-sure-convergence)
- [Convergence in Lp from convergence in probability and an Lr bound](#convergence-in-lp-from-convergence-in-probability-and-an-lr-bound)
  - [Bounded second moments do not upgrade convergence in probability to convergence in L2](#bounded-second-moments-do-not-upgrade-convergence-in-probability-to-convergence-in-l2)
- [Uniform integrability](#uniform-integrability)
  - [Class D process](#class-d-process)
    - [Class DL process](#class-dl-process)
  - [Uniform integrability from an Lp bound](#uniform-integrability-from-an-lp-bound)
  - [L1 convergence implies uniform integrability](#l1-convergence-implies-uniform-integrability)
  - [Uniform integrability of conditional expectations](#uniform-integrability-of-conditional-expectations)
  - [Uniform integrability from bounded second moments](#uniform-integrability-from-bounded-second-moments)
- [Large deviation principle](#large-deviation-principle)
  - [Logarithmic probabilities of open sets for a continuous rate function](#logarithmic-probabilities-of-open-sets-for-a-continuous-rate-function)
  - [Moderate deviation principle](#moderate-deviation-principle)
    - [Poisson moderate deviation principle](#poisson-moderate-deviation-principle)
  - [Principle of the largest exponential term](#principle-of-the-largest-exponential-term)
  - [Large deviations of a scaled geometric random variable](#large-deviations-of-a-scaled-geometric-random-variable)
    - [Large deviations of a fixed sum of geometric random variables](#large-deviations-of-a-fixed-sum-of-geometric-random-variables)
  - [Fixed exponential perturbation of a Gaussian empirical mean](#fixed-exponential-perturbation-of-a-gaussian-empirical-mean)
  - [Weak large deviation principle](#weak-large-deviation-principle)
    - [Exponential tightness upgrades a weak large deviation principle](#exponential-tightness-upgrades-a-weak-large-deviation-principle)
  - [Slower-speed degeneration of a large deviation principle](#slower-speed-degeneration-of-a-large-deviation-principle)
  - [Varadhan's lemma](#varadhan-s-lemma)
    - [Exponential tail extension of Varadhan's lemma](#exponential-tail-extension-of-varadhan-s-lemma)
  - [Laplace principle (large deviations theory)](#laplace-principle-large-deviations-theory)
    - [Laplace principle for probability measures](#laplace-principle-for-probability-measures)
  - [Gärtner–Ellis theorem](#gartner-ellis-theorem)
  - [Product large-deviation principle](#product-large-deviation-principle)
  - [Contraction principle for large deviations](#contraction-principle-for-large-deviations)
    - [Rate function under scalar clipping](#rate-function-under-scalar-clipping)
    - [Large-deviation rate of a minimum of independent copies](#large-deviation-rate-of-a-minimum-of-independent-copies)
      - [High moments of a clipped minimum of exponential sample means](#high-moments-of-a-clipped-minimum-of-exponential-sample-means)
  - [Exponential equivalence](#exponential-equivalence)
  - [Exponential tightness](#exponential-tightness)
  - [Large-deviation speed](#large-deviation-speed)
    - [Hurstiness](#hurstiness)
      - [Hurstiness of independent sums](#hurstiness-of-independent-sums)
  - [Rate function](#rate-function)
    - [Local convex path action](#local-convex-path-action)
    - [Good rate function](#good-rate-function)
      - [A good rate function is separated from zero away from its minimizer](#a-good-rate-function-is-separated-from-zero-away-from-its-minimizer)
  - [Freidlin--Wentzell action](#freidlin-wentzell-action)
    - [Geometric minimum action](#geometric-minimum-action)
- [Central limit theorem](#central-limit-theorem)
  - [Lindeberg-Feller central limit theorem](#lindeberg-feller-central-limit-theorem)
    - [Lyapunov condition](#lyapunov-condition)
  - [Gaussian tails force an unbounded normalized partial-sum limsup](#gaussian-tails-force-an-unbounded-normalized-partial-sum-limsup)
  - [Normal approximation](#normal-approximation)
    - [Continuity correction](#continuity-correction)
  - [Lindeberg condition](#lindeberg-condition)
  - [Hilbert-space central limit theorem](#hilbert-space-central-limit-theorem)
  - [Self-normalized central limit theorem with a second-moment denominator](#self-normalized-central-limit-theorem-with-a-second-moment-denominator)
  - [Donsker's theorem](#donsker-s-theorem)
    - [Fourth-moment tightness of polygonal random walks](#fourth-moment-tightness-of-polygonal-random-walks)
    - [Random-walk maximum limit from Donsker invariance](#random-walk-maximum-limit-from-donsker-invariance)
    - [Integrated random-walk limit](#integrated-random-walk-limit)
  - [Multivariate central limit theorem](#multivariate-central-limit-theorem)
- [Poisson limit theorem](#poisson-limit-theorem)

## Contiguity of probability measures

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)

A sequence $Q_n$ is contiguous with respect to $P_n$ if $P_n(A_n)\to0$ implies $Q_n(A_n)\to0$ for every measurable sequence of events. It transfers negligible-event assertions, including [consistency](statistical-inference.md#consistency-statistics), between changing sampling laws. It need not imply small [total variation distance](probability-and-statistics.md#total-variation-distance).

<h3 id="le-cam-s-first-lemma">Le Cam's first lemma</h3>

↑ **Parent:** [Contiguity of probability measures](#contiguity-of-probability-measures)

Let $L_n$ be the [probability density function](continuous-probability-distribution.md#probability-density-function) of the absolutely continuous part of $Q_n$ relative to $P_n$. If $L_n$ converges in distribution under $P_n$ to $L>0$ almost surely with $\mathbb EL=1$, then $P_n,Q_n$ are [mutually contiguous](#mutual-contiguity). Indeed, $\mathbb E L_n\le1$ and convergence to a mean-one limit imply [uniform integrability](#uniform-integrability) and vanishing singular mass, giving forward [contiguity](#contiguity-of-probability-measures). For reverse [contiguity](#contiguity-of-probability-measures), $P_n(A_n)\le P_n(L_n\le c)+Q_n(A_n)/c$, and one first takes $n\to\infty$ and then $c\downarrow0$.

### Mutual contiguity

↑ **Parent:** [Contiguity of probability measures](#contiguity-of-probability-measures)

Two sequences of probability laws are [mutually contiguous](#mutual-contiguity) when [contiguity of probability measures](#contiguity-of-probability-measures) holds in both directions. A positive mean-one limit of their [likelihood ratio](statistical-modelling.md#likelihood-ratio) is a standard sufficient criterion.

## Convergence in Lp

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)

Random variables converge in $L^p$ when $\mathbb E|X_n-X|^p\to0$.

### Convergence in L1

↑ **Parent:** [Convergence in Lp](#convergence-in-lp)

[Convergence in L1](#convergence-in-l1) means that the [expected value](probability-theory.md#expected-value) of the absolute error tends to zero. It implies [convergence in probability](#convergence-in-probability) and convergence of [expected values](probability-theory.md#expected-value).

<h4 id="scheffe-lemma">Scheffé lemma</h4>

↑ **Parent:** [Convergence in L1](#convergence-in-l1)

For nonnegative [integrable](measure-theory.md#integrability) functions converging [almost everywhere](measure-theory.md#almost-everywhere) to an integrable $f$, convergence of their integrals implies [L1 convergence](#convergence-in-l1). Indeed $\min(f_n,f)\to f$ almost everywhere and is dominated by $f$, so the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) gives convergence of its integral. Use $|f_n-f|=f_n+f-2\min(f_n,f)$. This applies to [probability densities](quantum-mechanics.md#probability-density), giving convergence in [total variation distance](probability-and-statistics.md#total-variation-distance).

### Convergence in L2

↑ **Parent:** [Convergence in Lp](#convergence-in-lp)

Convergence in $L^2$ means $\mathbb E[(X_n-X)^2]\to0$. It implies [convergence in probability](#convergence-in-probability) by [Markov inequality](probability-inequality.md#markov-inequality).

#### Almost-sure convergence and convergence of second moments

↑ **Parent:** [Convergence in L2](#convergence-in-l2)

If square-integrable random variables satisfy $X_n\to X$ [almost surely](#almost-sure-convergence), then $X_n\to X$ in $L^2$ exactly when $\mathbb E[X_n^2]\to\mathbb E[X^2]$. Boundedness in $L^2$ and almost-sure convergence first give weak convergence in the Hilbert space $L^2$; weak convergence together with convergence of norms gives strong convergence.

## Convergence in distribution

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)

Random variables $X_n$ converge in distribution, or converge weakly, to $X$ when

$$
\mathbb E[f(X_n)]\longrightarrow\mathbb E[f(X)]
$$

for every bounded continuous function $f$. For real random variables this is equivalent to convergence of the distribution functions at every continuity point of the limiting distribution function.

### Atoms obstruct a continuous distributional limit

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)

If $Z_n$ has probability at least p at $z_n$, with $p>0$ and $z_n\to z$, every weak limit has probability at least p at z. Apply the closed-set bound of the [Portmanteau theorem](#portmanteau-theorem) to arbitrarily small closed intervals containing z and eventually $z_n$, then decrease their radii. Thus a persistent atom prevents convergence to a continuous law, including a chi-squared law. This provides a direct check when bounded-information estimation fails standard asymptotic-normal theory.

### Marginal weak convergence does not control sums

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)

Let $Z$ take values $1,-1$ with equal probabilities. Set $X_n=Z$ for every $n$, and $Y_n=Z$ for even $n$, $Y_n=-Z$ for odd $n$. Both marginal laws are constant, but $X_n+Y_n$ alternates between the law of $2Z$ and a point mass at zero. Thus separate [weak convergence of random variables](#convergence-in-distribution) does not determine a joint limit or a sum limit. The obstruction disappears when one marginal limit is constant, as in the [Slutsky theorem](statistical-inference.md#slutsky-theorem).

### Skorokhod representation theorem

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)

For [convergence in distribution](#convergence-in-distribution) of random elements in a separable complete [metric](topological-analysis.md#metric) space, one can construct copies of the sequence and its limit on one probability space which converge almost surely. The copies preserve the individual laws; they need not preserve the original dependence between sequence elements. Suitable more general versions permit a separably supported limit in a [metric](topological-analysis.md#metric) space.

### Method of moments (probability theory)

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Method_of_moments_(probability_theory))

If all moments of real [random variables](random-variable.md) converge to those of a moment-determinate limit law, then the variables converge to that law in the sense of [convergence in distribution](#convergence-in-distribution). [Moment determinacy](probability-theory.md#moment-determinacy) is essential; the [standard normal distribution](probability-theory.md#standard-normal-distribution) meets this condition.

### Weak convergence of probability measures

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)

Probability measures $\mu_n$ on a metric space converge weakly to $\mu$ when $\int f\,d\mu_n\to\int f\,d\mu$ for every bounded continuous real function $f$.

#### Compact containment

↑ **Parent:** [Weak convergence of probability measures](#weak-convergence-of-probability-measures)

A family of path laws satisfies compact containment when for every finite horizon and every error tolerance there is a compact set which contains the whole path up to that horizon with at least the complementary probability, uniformly over the family. In Euclidean state space this is the displayed condition. It prevents escape to distant regions where local coefficient approximations give no control. A nonnegative [Lyapunov function](dynamical-systems.md#lyapunov-function) with uniformly bounded generator growth often proves it by the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale).

#### Scaling limit of a random curve

↑ **Parent:** [Weak convergence of probability measures](#weak-convergence-of-probability-measures)

A [scaling limit](#scaling-limit-of-a-random-curve) of random curves is a [weak convergence of probability measures](#weak-convergence-of-probability-measures) after spatial rescaling, usually modulo monotone reparameterization. Tightness specifies the topology and yields subsequential limits; identification of their laws gives a unique continuum model. [SLE](stochastic-process.md#schramm-loewner-evolution) is a central family of such limiting curve laws.

#### Skorokhod J1 topology

↑ **Parent:** [Weak convergence of probability measures](#weak-convergence-of-probability-measures)

On càdlàg paths on a compact time interval, convergence in this topology means that increasing continuous bijections of the time interval can be chosen converging uniformly to the identity, while the corresponding time-changed paths converge uniformly to the limit. At a continuous limiting path this reduces to uniform convergence. It is a standard topology for weak limits of accelerated discrete-time chains, whose paths are step functions.

#### Weak topology of probability measures

↑ **Parent:** [Weak convergence of probability measures](#weak-convergence-of-probability-measures)

This is the coarsest topology making all displayed bounded-continuous test integrals continuous. On a separable [metric](topological-analysis.md#metric) space it is metrized by the [bounded-Lipschitz metric](#bounded-lipschitz-metric). This probability-[measure](measure-theory.md#measure) topology should be distinguished from the weak topology of a Banach space.

##### Bounded-Lipschitz metric

↑ **Parent:** [Weak topology of probability measures](#weak-topology-of-probability-measures)

The bounded-Lipschitz [metric](topological-analysis.md#metric) tests [probability measures](probability-theory.md#probability-measure) against a uniformly bounded Lipschitz class. It metrizes [weak convergence of probability measures](#weak-convergence-of-probability-measures) on separable [metric](topological-analysis.md#metric) spaces. With a complete compatible base [metric](topological-analysis.md#metric), it is complete on the [probability measures](probability-theory.md#probability-measure) of a [Polish space](topological-analysis.md#polish-space). Replacing the sum norm by the maximum norm changes the [metric](topological-analysis.md#metric) only by uniform constant factors.

<h4 id="prokhorov-s-theorem">Prokhorov's theorem</h4>

↑ **Parent:** [Weak convergence of probability measures](#weak-convergence-of-probability-measures)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prokhorov's_theorem)

On a Polish space, a family of probability measures is relatively compact for weak convergence exactly when it is tight. For finite measures, one additionally requires uniformly bounded total masses.

##### Closed uniformly tight compactness criterion

↑ **Parent:** [Prokhorov's theorem](#prokhorov-s-theorem)

A weakly closed [uniformly tight](probability-theory.md#uniform-tightness) family of Borel [probability measures](probability-theory.md#probability-measure) on a [Polish space](topological-analysis.md#polish-space) is weakly compact. Embed the underlying space into a compact [metric](topological-analysis.md#metric) closure, take subsequential pushforward limits, and use the closed-set [Portmanteau theorem](#portmanteau-theorem) on the common tightness compact sets. The limit retains full mass in the original space; inverse continuity of the [probability pushforward embedding theorem](measure-theory.md#probability-pushforward-embedding-theorem) then returns the weak limit.

##### Compactness of probability measures on a compact metric space

↑ **Parent:** [Prokhorov's theorem](#prokhorov-s-theorem)

On a [compact metric space](topological-analysis.md#compact-metric-space), every sequence of [Borel probability measures](measure-theory.md#borel-probability-measure) has a subsequence with [weak convergence of probability measures](#weak-convergence-of-probability-measures) to a [Borel probability measure](measure-theory.md#borel-probability-measure). To see this, choose a countable uniformly dense subset of continuous functions, extract a diagonal subsequence of their bounded integrals, and extend the resulting positive normalized functional to all continuous functions. The [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) supplies its [Borel probability measure](measure-theory.md#borel-probability-measure). This is useful for constructing an [invariant measure](measure-theory.md#invariant-measure) from orbit [empirical measures](probability-theory.md#empirical-measure).

### Bounded moment criterion for weak convergence

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)

For random variables supported in one fixed compact interval, convergence of every moment is equivalent to weak convergence. One direction tests monomials; the other follows by uniformly approximating continuous functions by polynomials.

#### Moment determinacy on a compact interval

↑ **Parent:** [Bounded moment criterion for weak convergence](#bounded-moment-criterion-for-weak-convergence)

Two [probability measures](probability-theory.md#probability-measure) supported on one compact interval are equal if all their moments are equal. Indeed, equality on monomials gives equality on [polynomials](polynomial.md), the [Weierstrass approximation theorem](functional-analysis.md#weierstrass-approximation-theorem) extends it to every continuous function on the interval, and [compactly supported continuous functions determine a finite Borel measure](probability-theory.md#compactly-supported-continuous-functions-determine-a-finite-borel-measure).

### Portmanteau theorem

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Portmanteau_theorem)

The Portmanteau theorem gives equivalent formulations of weak convergence, including inequalities on open and closed sets and convergence of expectations for every bounded measurable function whose discontinuity set has zero limiting probability.

### Continuous mapping theorem

↑ **Parent:** [Convergence in distribution](#convergence-in-distribution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuous_mapping_theorem)

If $X_n\xrightarrow dX$ and a measurable function $g$ is continuous at $X$ almost surely, then $g(X_n)\xrightarrow d g(X)$. The same principle holds for random elements of metric spaces.

## Almost sure convergence

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Almost_sure_convergence)

A sequence of random variables converges almost surely when the set of outcomes on which pointwise convergence fails has probability zero.

### Complete convergence of random variables

↑ **Parent:** [Almost sure convergence](#almost-sure-convergence)

A sequence converges completely to $X$ when $\sum_n\Pr(|X_n-X|>\epsilon)<\infty$ for every $\epsilon>0$. The first Borel-Cantelli lemma implies almost sure convergence. For independent $X_n$, any limit in probability is almost surely constant; the second Borel-Cantelli lemma then gives the converse from almost sure to complete convergence. Independence is essential: $X_n=1_{\{U\le1/n\}}$ for one uniform random variable $U$ converges almost surely to zero but its exceedance probabilities have a divergent sum.

### Almost sure equality

↑ **Parent:** [Almost sure convergence](#almost-sure-convergence)

Random variables $X$ and $Y$ are almost surely equal when $\mathbb P(X=Y)=1$. Probability theory conventionally identifies random variables that differ only on a null event.

### Strong law of large numbers

↑ **Parent:** [Almost sure convergence](#almost-sure-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_law_of_large_numbers)

If $(X_n)$ are [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with $\mathbb E|X_1|<\infty$, then

$$
\frac1n\sum_{j=1}^nX_j\longrightarrow\mathbb E[X_1]
$$

almost surely.

#### Strong law for uniformly L2-bounded uncorrelated random variables

↑ **Parent:** [Strong law of large numbers](#strong-law-of-large-numbers)

If $\sup_n\mathbb E|X_n|^2<\infty$ and the $X_n$ are pairwise [uncorrelated random variables](variance.md#uncorrelated-random-variables), then $n^{-1}\sum_{k=1}^n(X_k-\mathbb E X_k)\to0$ almost surely. [Independence](random-variable.md#independent-random-variables) is unnecessary for this version of the [strong law of large numbers](#strong-law-of-large-numbers). A uniformly bounded [martingale difference sequence](martingale.md#martingale-difference-sequence) meets its hypotheses, since the differences have mean zero and are orthogonal in $L^2$.

#### Strong law for adjacent products

↑ **Parent:** [Strong law of large numbers](#strong-law-of-large-numbers)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_j$ with $\mathbb E|X_1|<\infty$ and $m=\mathbb EX_1$, the [sample mean](variance.md#sample-mean) of $X_jX_{j+1}$ tends to $m^2$ [almost surely](#almost-sure-convergence). Split into odd and even indexed products; each subsequence consists of [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) that are [integrable random variables](probability-theory.md#integrable-random-variable). Apply the [strong law of large numbers](#strong-law-of-large-numbers) separately.

### Kolmogorov convergence theorem

↑ **Parent:** [Almost sure convergence](#almost-sure-convergence)

If independent centered random variables $(Y_n)$ satisfy $\sum_n\operatorname{Var}(Y_n)<\infty$, then $\sum_nY_n$ converges almost surely. It follows from Kolmogorov's maximal inequality and a Cauchy-tail argument.

### Law of the iterated logarithm

↑ **Parent:** [Almost sure convergence](#almost-sure-convergence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_the_iterated_logarithm)

For independent identically distributed centered variables of variance one under standard moment assumptions, the law of the iterated logarithm describes the almost-sure envelope of their partial sums on the scale $\sqrt{2n\log\log n}$.

#### Brownian upper law of the iterated logarithm

↑ **Parent:** [Law of the iterated logarithm](#law-of-the-iterated-logarithm)

For standard [Brownian motion](brownian-motion.md), the [Brownian reflection principle](brownian-motion.md#reflection-principle-wiener-process) bounds the probability that its maximum up to $a^n$ exceeds $(1+\varepsilon)\sqrt{2a^n\log\log(a^n)}$ by $2(n\log a)^{-(1+\varepsilon)^2}$. This is summable for every $a>1$ and $\varepsilon>0$. The [Borel-Cantelli first lemma](probability-theory.md#borel-cantelli-first-lemma) controls these geometric times, monotonicity of the normalizing function controls the intervening times, and countable choices $a\downarrow1$, $\varepsilon\downarrow0$ give the bound. Equality requires a separate lower-bound proof.

#### Upper law of the iterated logarithm

↑ **Parent:** [Law of the iterated logarithm](#law-of-the-iterated-logarithm)

For a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk), geometric blocking and the [Borel-Cantelli first lemma](probability-theory.md#borel-cantelli-first-lemma) yield the upper estimate $\limsup_n S_n/\sqrt{2n\log\log n}\le1$ [almost surely](#almost-sure-convergence). Equality requires a separate lower-bound argument.

#### Law of the iterated logarithm for a simple symmetric random walk

↑ **Parent:** [Law of the iterated logarithm](#law-of-the-iterated-logarithm)

For a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk), almost surely

$$
\limsup_{n\to\infty}\frac{S_n}{\sqrt{2n\log\log n}}=1,
\qquad
\liminf_{n\to\infty}\frac{S_n}{\sqrt{2n\log\log n}}=-1.
$$

<h2 id="cramer-wold-theorem">Cramér–Wold theorem</h2>

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cramér–Wold_theorem)

Random vectors $X_n$ converge weakly to $X$ exactly when every linear projection $u\cdot X_n$ converges weakly to $u\cdot X$. The reverse implication follows because these one-dimensional limits give pointwise convergence of the multivariate characteristic functions.

## Convergence in probability

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convergence_in_probability)

Random variables $X_n$ converge in probability to $X$ when

$$
\mathbb P(|X_n-X|>\varepsilon)\to0
$$

for every $\varepsilon>0$.

### Uniform convergence in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

Uniform convergence in [probability](probability-theory.md#probability) means that the supremum of the absolute discrepancy on the entire index set tends to zero in [probability](probability-theory.md#probability). It controls evaluation at random indices in that set, unlike pointwise [convergence in probability](#convergence-in-probability). On a fixed compact index set it is a special case of [uniform convergence on compacts in probability](stochastic-process.md#uniform-convergence-on-compacts-in-probability).

### Boundedness in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

A sequence of [random variables](random-variable.md) $(X_n)$ is bounded in probability when $\lim_{K\to\infty}\sup_n\mathbb P(|X_n|>K)=0$. A sequence converging in [probability](probability-theory.md#probability) to a finite [random variable](random-variable.md) has this property, and its product with a sequence tending to zero in [probability](probability-theory.md#probability) also tends to zero in [probability](probability-theory.md#probability).

#### Stochastic order

↑ **Parent:** [Boundedness in probability](#boundedness-in-probability)

The notation $Z_n=O_{\mathbb P}(a_n)$ means that $Z_n/a_n$ is [bounded in probability](#boundedness-in-probability) asymptotically: for every $\varepsilon>0$ some $C$ gives $\limsup_n\mathbb P(|Z_n|>Ca_n)\leq\varepsilon$. A tail bound $\mathbb P(|Z_n|>za_n)\leq C_0/z^2$ is sufficient. In statements involving bandwidths, specify whether the constants must be uniform over bandwidth sequences.

##### Uniform pointwise probability bounds do not bound a random supremum

↑ **Parent:** [Stochastic order](#stochastic-order)

A bound on $\sup_x\mathbb P(|Z_n(x)|>t)$ does not give the same bound on $\mathbb P(\sup_x|Z_n(x)|>t)$. Even [independent](random-variable.md#independent-random-variables) standard [normal random variables](probability-theory.md#gaussian-random-variable) each have uniformly bounded tails while their [Gaussian maximum](probability-theory.md#gaussian-maximum) over $N$ indices grows at scale $\sqrt{\log N}$. This distinction matters in [nonparametric statistics](nonparametric-statistics.md) when a shrinking bandwidth permits many spatial windows.

### Convergence in distribution to a constant implies convergence in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

If $X_n\xrightarrow d c$ for fixed real $c$, convergence of the [distribution functions](probability-theory.md#cumulative-distribution-function) at $c-\varepsilon$ and $c+\varepsilon$ shows $\mathbb P(|X_n-c|>\varepsilon)\to0$. Thus [convergence in distribution](#convergence-in-distribution) to a deterministic limit implies [convergence in probability](#convergence-in-probability) to that limit, even though the implication fails for nonconstant limits on a specified [probability space](probability-theory.md#probability-space).

### Weak law of large numbers

↑ **Parent:** [Convergence in probability](#convergence-in-probability)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Weak_law_of_large_numbers)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with finite [expected value](probability-theory.md#expected-value), the sample mean converges in probability to that expected value.

#### Weak law without an absolute first moment

↑ **Parent:** [Weak law of large numbers](#weak-law-of-large-numbers)

Let $X$ have a [symmetric probability distribution](probability-theory.md#symmetric-probability-distribution) with $\mathbb P(|X|>x)=1/(x\log x)$ for $x\ge e$, mass $1-1/e$ at zero, and no mass with $0<|X|<e$. Then $\mathbb E|X|=\infty$, but independent copies satisfy the [weak law of large numbers](#weak-law-of-large-numbers) with limit zero. Indeed $n\mathbb P(|X|>n)=1/\log n\to0$. Their symmetric truncations $Y_{n,j}=X_j\mathbf1_{\{|X_j|\le n\}}$ have mean zero and second moment $O(n/\log n)$, so [Chebyshev's inequality](probability-inequality.md#chebyshev-inequality) gives $n^{-1}\sum_{j\le n}Y_{n,j}\to0$ in probability. A union bound shows that the original and truncated sums differ with probability tending to zero. This also gives a differentiable [characteristic function](probability-theory.md#characteristic-function) at zero whose derivative cannot be interpreted as an absolutely convergent expectation.

#### Weak law forces a characteristic-function derivative

↑ **Parent:** [Weak law of large numbers](#weak-law-of-large-numbers)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) with [characteristic function](probability-theory.md#characteristic-function) $\phi$, suppose their [sample mean](variance.md#sample-mean) converges in probability to a finite constant $a$. Bounded exponential tests give $e^{-iau}\phi(u/n)^n\to1$ uniformly on bounded $u$ intervals: the error is at most $T\delta+2\mathbb P(|S_n/n-a|>\delta)$ on $|u|\le T$. Taking the continuous [complex logarithm](analysis.md#complex-logarithm) vanishing at zero shows $n\log\phi(u/n)-iau\to0$ uniformly; an integer-valued branch difference is continuous and therefore zero. For arbitrary $h\to0$, put $n=\lfloor1/|h|\rfloor$ and $u=nh$, so $1/2\le|u|\le1$. Dividing the uniform limit by $u$ proves $\log\phi(h)/h\to ia$, and thus $\phi'(0)=ia$. No absolute first moment is assumed.

#### Uniform law of large numbers

↑ **Parent:** [Weak law of large numbers](#weak-law-of-large-numbers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_law_of_large_numbers)

A class $\mathcal G$ satisfies a uniform law of large numbers when its empirical means converge uniformly to their expectations:

$$
\sup_{g\in\mathcal G}|P_ng-Pg|\to0.
$$

##### Pointwise separable function class

↑ **Parent:** [Uniform law of large numbers](#uniform-law-of-large-numbers)

A measurable-function class is pointwise separable if it has a countable subclass such that every member is the pointwise limit of a sequence from that subclass. With an integrable common envelope, [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) makes both empirical averages and population expectations converge along each such sequence. Thus the supremum of the absolute empirical errors equals the supremum over the countable subclass and is measurable. A finite integrable bracketing cover provides an integrable envelope by taking the maximum absolute value of all its endpoints.

##### Bracketing of a function class

↑ **Parent:** [Uniform law of large numbers](#uniform-law-of-large-numbers)

A bracket $[\ell,u]$ contains every measurable function $h$ satisfying $\ell\le h\le u$ pointwise. For a probability measure $P$, its $L^1(P)$ width is $P(u-\ell)$, with integrable endpoints. Finite bracketing at every positive width is a sufficient complexity condition for a [uniform law of large numbers](#uniform-law-of-large-numbers). Pointwise inequalities, or inequalities outside a single common null set, allow empirical inequalities to hold simultaneously throughout the class.

###### Integrable envelope of a function class

↑ **Parent:** [Bracketing of a function class](#bracketing-of-a-function-class)

A measurable function $M$ is an [integrable envelope of a function class](#integrable-envelope-of-a-function-class) for a class $\mathcal H$ under a probability law $P$ if $|h(x)|\le M(x)$ for every $h\in\mathcal H$ and $PM<\infty$. Such an envelope permits the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) to control shrinking [function brackets](#bracketing-of-a-function-class).

###### Uniform strong law from finite L1 bracketing

↑ **Parent:** [Bracketing of a function class](#bracketing-of-a-function-class)

Suppose an integrable measurable-function class can be covered by finitely many [function brackets](#bracketing-of-a-function-class) of every positive $L^1(P)$ width. For an independent sample with common law $P$, the [empirical measure](probability-theory.md#empirical-measure) satisfies $\sup_h|P_nh-Ph|\to0$ on a common probability-one event. For one finite $\varepsilon$-cover, the supremum is bounded by $\varepsilon$ plus the largest empirical error among its endpoints. The [strong law of large numbers](#strong-law-of-large-numbers) makes that finite maximum vanish. Taking a countable sequence of widths decreasing to zero proves the assertion. A measurable supremum can be obtained from a [pointwise separable function class](#pointwise-separable-function-class); otherwise the probability-one-event formulation expresses the same pathwise conclusion.

###### Uniform strong law on a compact parameter set

↑ **Parent:** [Uniform strong law from finite L1 bracketing](#uniform-strong-law-from-finite-l1-bracketing)

If $\Theta$ is [compact](topology.md#compact-space), $q(\theta,x)$ is continuous in $\theta$ and measurable in $x$, and $\mathbb E\sup_\Theta|q(\theta,X)|<\infty$, then an [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) sample satisfies $\sup_\Theta|P_nq_\theta-Pq_\theta|\to0$ almost surely. [Uniform continuity](topological-analysis.md#uniform-continuity) for each $x$, the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem), and finite parameter nets produce arbitrarily narrow [function brackets](#bracketing-of-a-function-class).

##### Glivenko-Cantelli theorem

↑ **Parent:** [Uniform law of large numbers](#uniform-law-of-large-numbers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Glivenko-Cantelli_theorem)

The empirical distribution function converges uniformly almost surely to the population distribution function.

###### Quantile proof of the Glivenko-Cantelli theorem

↑ **Parent:** [Glivenko-Cantelli theorem](#glivenko-cantelli-theorem)

For a [cumulative distribution function](probability-theory.md#cumulative-distribution-function) $G$, let $Q(u)=\inf\{x:G(x)\geq u\}$, $0<u<1$. Right continuity gives $Q(u)\leq x$ exactly when $u\leq G(x)$, including at atoms. Thus applying $Q$ to independent uniform variables $U_i$ constructs an independent sample with distribution function $G$. Its [empirical distribution function](probability-theory.md#empirical-distribution-function) is $G_n(x)=F_n(G(x))$, where $F_n$ is the uniform-sample empirical distribution function. Consequently $\sup_x|G_n(x)-G(x)|\leq\sup_{t\in[0,1]}|F_n(t)-t|$. For the uniform sample, monotonicity and a grid of mesh $1/m$ bound the last supremum by the largest error at grid points plus $1/m$. The [strong law of large numbers](#strong-law-of-large-numbers) on the countable union of all such grids proves the almost-sure limit. This construction proves the theorem for distributions with atoms as well as continuous distributions.

### Uniqueness of a limit in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

If $X_n$ converges in probability to both $X$ and $Y$, then $X=Y$ almost surely. Indeed, the [triangle inequality](topological-analysis.md#triangle-inequality) and a [union bound](probability-inequality.md#boole-s-inequality) show that $\mathbb P(|X-Y|>\varepsilon)=0$ for every $\varepsilon>0$.

### Bounded-metric characterization of convergence in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

Convergence in probability is equivalent to

$$
\mathbb E\big(|X_n-X|\wedge1\big)\to0.
$$

The forward implication splits at a fixed error threshold; the reverse implication is Markov's inequality.

### Almost-sure subsequence from convergence in probability

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

From $X_n\to X$ in probability, choose $n_k$ with  
$\mathbb P(|X_{n_k}-X|>2^{-k})<2^{-k}$. The first Borel--Cantelli lemma then gives $X_{n_k}\to X$ almost surely.

### Independent rare-event counterexample to almost-sure convergence

↑ **Parent:** [Convergence in probability](#convergence-in-probability)

Independent indicators with success probabilities $1/n$ converge to zero in probability, but successes occur infinitely often almost surely by the second Borel--Cantelli lemma.

## Convergence in Lp from convergence in probability and an Lr bound

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)

If $X_n\to X$ in probability and $\sup_n\lVert X_n\rVert_r<\infty$, then $X_n\to X$ in $L^p$ for every $1\leq p<r$. The $L^r$ bound gives uniform integrability of the $p$th powers, while convergence in probability controls their bounded part.

### Bounded second moments do not upgrade convergence in probability to convergence in L2

↑ **Parent:** [Convergence in Lp from convergence in probability and an Lr bound](#convergence-in-lp-from-convergence-in-probability-and-an-lr-bound)

On $([0,1],\mathcal B,\operatorname{Leb})$, the variables

$$
X_n=\sqrt n\,\mathbf1_{(0,1/n)}
$$

converge in probability and in $L^1$ to zero, while $\lVert X_n\rVert_2=1$ for every $n$.

## Uniform integrability

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Uniform_integrability)

A family of integrable random variables is uniformly integrable when

$$
\lim_{K\to\infty}\sup_{X}\mathbb E\bigl[|X|\mathbf1_{\{|X|>K\}}\bigr]=0.
$$

Almost-sure or probabilistic convergence together with uniform integrability upgrades to $L^1$ convergence.

### Class D process

↑ **Parent:** [Uniform integrability](#uniform-integrability)

On a finite time horizon, an adapted process is of class D if its values at all stopping times in that horizon form a [uniformly integrable](#uniform-integrability) family. Deterministic boundedness implies this property. The stopping-time uniformity is stronger than having an integrable value at each fixed time.

#### Class DL process

↑ **Parent:** [Class D process](#class-d-process)

An adapted process is of class DL when, for every finite $T$, the family $\{X_\tau:\tau\le T\text{ a stopping time}\}$ is uniformly integrable. A [local martingale](martingale.md#local-martingale) is a true martingale exactly when it has this property. This is a local-in-time condition, not uniform integrability over the whole half-line.

// Target: probability-and-statistics.bigb

### Uniform integrability from an Lp bound

↑ **Parent:** [Uniform integrability](#uniform-integrability)

For $p>1$, $\sup_n\mathbb E|X_n|^p=C<\infty$ gives $\sup_n\mathbb E[|X_n|\mathbf1_{|X_n|>M}]\leq C M^{1-p}\to0$. Thus an $L^p$ bound implies [uniform integrability](#uniform-integrability); a mere $L^1$ bound does not.

### L1 convergence implies uniform integrability

↑ **Parent:** [Uniform integrability](#uniform-integrability)

For [integrable random variables](probability-theory.md#integrable-random-variable) $Z,Y$,

$$
\mathbb E[|Z|\mathbf1_{\{|Z|>K\}}]\leq2\mathbb E|Z-Y|+\mathbb E[|Y|\mathbf1_{\{|Y|>K/2\}}].
$$

Apply this with $Z=X_n$ and $Y=X$ to prove that [convergence in L1](#convergence-in-l1) implies [uniform integrability](#uniform-integrability); control finitely many early terms separately.

### Uniform integrability of conditional expectations

↑ **Parent:** [Uniform integrability](#uniform-integrability)

For one [integrable random variable](probability-theory.md#integrable-random-variable) $Y$, the family $Z_{\mathcal G}=\mathbb E[Y\mid\mathcal G]$, over arbitrary [sigma-algebras](measure-theory.md#sigma-algebra) $\mathcal G$, has [uniform integrability](#uniform-integrability). On $A=\{|Z_{\mathcal G}|>K\}$, the defining property of [conditional expectation](measure-theory.md#conditional-expectation) gives $\mathbb E[|Z_{\mathcal G}|\mathbf1_A]\leq\mathbb E[|Y|\mathbf1_A]$, while $\mathbb P(A)\leq\mathbb E|Y|/K$ by the [Markov inequality](probability-inequality.md#markov-inequality). The [integrable random variable](probability-theory.md#integrable-random-variable) $Y$ has uniformly small absolute integrals over [events](probability-theory.md#event) of sufficiently small probability.

### Uniform integrability from bounded second moments

↑ **Parent:** [Uniform integrability](#uniform-integrability)

If $\sup_n\mathbb E[X_n^2]<\infty$, then $(X_n)$ is [uniformly integrable](#uniform-integrability). Indeed, the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and [Markov inequality](probability-inequality.md#markov-inequality) give

$$
\mathbb E[|X_n|\mathbf1_{\{|X_n|>K\}}]
\leq\frac{\mathbb E[X_n^2]}{K}.
$$

## Large deviation principle

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Large_deviation_principle)

A sequence $(Z_n)$ satisfies a large deviation principle with speed $n$ and rate function $I$ when probabilities of measurable sets $A$ decay exponentially between the bounds

$$
-\inf_{x\in A^\circ}I(x)
\leq\liminf_n\frac1n\log\mathbb P(Z_n\in A)
\leq\limsup_n\frac1n\log\mathbb P(Z_n\in A)
\leq-\inf_{x\in\overline A}I(x).
$$

### Logarithmic probabilities of open sets for a continuous rate function

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

If a [large deviation principle](#large-deviation-principle) has a finite [continuous](calculus.md#continuous-function) [rate function](#rate-function), then the infima on any [open set](topology.md#open-set) and its [closure](topology.md#closure-topology) agree. Approximate every closure point by points of the set and use continuity. The open-set lower and closed-set upper bounds consequently match, giving the displayed logarithmic limit, including the empty-set convention. A single-point event need not obey such an equality.

### Moderate deviation principle

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

A [large deviation principle](#large-deviation-principle) for fluctuations larger than the usual [central limit theorem](#central-limit-theorem) scale but smaller than a fixed displacement of the empirical mean. For the displayed sum scaling, the natural [large-deviation speed](#large-deviation-speed) is $b_n^2$. Under suitable exponential-moment hypotheses and positive [variance](variance.md) $\sigma^2$, its [rate function](#rate-function) is the quadratic $x^2/(2\sigma^2)$.

#### Poisson moderate deviation principle

↑ **Parent:** [Moderate deviation principle](#moderate-deviation-principle)

For a [Poisson random variable](discrete-probability-distribution.md#poisson-distribution) $S_L$ of mean $L\lambda>0$ and $0<\beta<1$, the scaled [cumulant-generating function](probability-theory.md#cumulant-generating-function) is $\lambda L^{1-\beta}(e^{\theta L^{(\beta-1)/2}}-1-\theta L^{(\beta-1)/2})$. Its [Taylor expansion](calculus.md#taylor-expansion) tends to $\lambda\theta^2/2$ for every real $\theta$. The [Gärtner–Ellis theorem](#gartner-ellis-theorem) applies because the limit is finite and differentiable everywhere. Its [Legendre-Fenchel transform](convex-optimization.md#convex-conjugate) is the displayed quadratic [good rate function](#good-rate-function).

### Principle of the largest exponential term

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

For a fixed finite number of nonnegative terms and $a_L\to\infty$, use $\max_jp_{j,L}\le\sum_jp_{j,L}\le r\max_jp_{j,L}$. The [logarithm](calculus.md#logarithm) of $r$, divided by the [large-deviation speed](#large-deviation-speed), tends to zero, and a finite maximum commutes with the [limit superior](real-analysis.md#limit-superior). If all individual logarithmic limits exist, the limit of the sum is their maximum.

### Large deviations of a scaled geometric random variable

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

For a [geometric random variable](discrete-probability-distribution.md#geometric-distribution) $X$ with $\mathbb P(X=k)=p(1-p)^{k-1}$, $0<p<1$, the family $X/L$ has [large-deviation speed](#large-deviation-speed) $L$ and [good rate function](#good-rate-function) $I(x)=ax$ for $x\geq0$, infinite otherwise, where $a=-\log(1-p)$. The exact tail $\mathbb P(X/L\geq x)=(1-p)^{\lceil Lx\rceil-1}$ gives the upper bound. A lattice point tending to any positive $x$ supplies the open-neighborhood lower bound; neighborhoods of zero have probability tending to one. Finite sublevel sets are compact intervals.

#### Large deviations of a fixed sum of geometric random variables

↑ **Parent:** [Large deviations of a scaled geometric random variable](#large-deviations-of-a-scaled-geometric-random-variable)

For fixed finitely many independent [geometric random variables](discrete-probability-distribution.md#geometric-distribution), the [product large-deviation principle](#product-large-deviation-principle) gives rate $\sum_i a_ix_i$ on the nonnegative orthant for their scaled vector, where $a_i=-\log(1-p_i)$. The [contraction principle for large deviations](#contraction-principle-for-large-deviations) under addition minimizes this over $\sum_ix_i=s$. The answer is $s\min_i a_i$, achieved by assigning all scaled excess to a coordinate with the slowest geometric tail. The rate is infinite for negative $s$. Deterministic coordinates with $p_i=1$ contribute zero on this scale; if all coordinates are deterministic, only zero has finite rate.

### Fixed exponential perturbation of a Gaussian empirical mean

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

Let $A_i$ be [independent random variables](random-variable.md#independent-random-variables) with [normal distribution](probability-theory.md#normal-distribution) $N(\mu,\sigma^2)$, $\sigma^2>0$, and let $B$ be an independent [exponential random variable](continuous-probability-distribution.md#exponential-distribution) of rate $\lambda>0$. At speed $L$, $(B+\sum_{i=1}^LA_i)/L$ has the [good rate function](#good-rate-function)

$$
K(x)=\begin{cases}(x-\mu)^2/(2\sigma^2),&x\leq\mu+\lambda\sigma^2,\\ \lambda(x-\mu)-\lambda^2\sigma^2/2,&x\geq\mu+\lambda\sigma^2.\end{cases}
$$

The [product large-deviation principle](#product-large-deviation-principle) gives the joint cost $\lambda b+(z-\mu)^2/(2\sigma^2)$ for $b\geq0$, and the [contraction principle for large deviations](#contraction-principle-for-large-deviations) gives its [infimal convolution](convex-optimization.md#infimal-convolution) under $b+z=x$. The minimum occurs at $b=(x-\mu-\lambda\sigma^2)^+$. The fixed exponential perturbation changes the far upper tail even though it vanishes in probability after division by $L$; a fixed [Gaussian random variable](probability-theory.md#gaussian-random-variable) divided by $L$ instead has [exponential equivalence](#exponential-equivalence) with zero at speed $L$.

### Weak large deviation principle

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

A weak [large deviation principle](#large-deviation-principle) has the usual lower bound on every [open set](topology.md#open-set), but requires the upper bound only on [compact sets](topology.md#compact-space). It does not by itself control probabilities escaping every [compact set](topology.md#compact-space). [Exponential tightness](#exponential-tightness) provides that missing control.

#### Exponential tightness upgrades a weak large deviation principle

↑ **Parent:** [Weak large deviation principle](#weak-large-deviation-principle)

Suppose a [weak large deviation principle](#weak-large-deviation-principle) with [rate function](#rate-function) $I$ holds on a [Hausdorff space](topology.md#hausdorff-space), at speed $a_n\to\infty$, and the random elements are [exponentially tight](#exponential-tightness). For a finite $r$, choose a [compact set](topology.md#compact-space) $K$ whose complement has upper exponential rate strictly below $-M$, with $M>r$. The open-set lower bound on $K^c$ implies $\inf_{K^c}I>M$, so $\{I\leq r\}\subset K$. [Lower semicontinuity](calculus.md#lower-semicontinuity) makes this [sublevel set](calculus.md#sublevel-set) closed, hence compact. For any [closed set](topology.md#closed-set) $F$, split its probability between the compact $F\cap K$ and $K^c$. The upper exponential rate is at most $\max\{-\inf_F I,-M\}$. Letting $M\to\infty$ proves the full [large deviation principle](#large-deviation-principle) with a [good rate function](#good-rate-function).

### Slower-speed degeneration of a large deviation principle

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

Suppose a [large deviation principle](#large-deviation-principle) at speed $a_n$ has a [good rate function](#good-rate-function) with unique zero mu. At any slower speed $b_n\to\infty$ with $a_n/b_n\to\infty$, its rate is zero at mu and infinity elsewhere. On a [closed set](topology.md#closed-set) excluding mu, the positive original rate gives decay faster than every exponential at speed $b_n$. Neighborhoods of mu have probability tending to one, giving the slower-speed open-set lower bound. The new rate is good because its finite [sublevel set](calculus.md#sublevel-set) is the singleton mu.

<h3 id="varadhan-s-lemma">Varadhan's lemma</h3>

↑ **Parent:** [Large deviation principle](#large-deviation-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Varadhan's_lemma)

If random elements satisfy a [large deviation principle](#large-deviation-principle) at speed $a_n\to\infty$ with [rate function](#rate-function) I, then a bounded continuous real function f satisfies the displayed exponential-integral identity. For the upper bound, partition its bounded range into finitely many closed intervals of width epsilon and apply the closed-set upper bound to their preimages. The largest exponential term controls the finite sum. For the lower bound, restrict to an open neighborhood where f is within epsilon of its value at a chosen point and use the open-set lower bound. Let epsilon tend to zero and optimize over the point. Boundedness avoids a separate exponential tail assumption.

<h4 id="exponential-tail-extension-of-varadhan-s-lemma">Exponential tail extension of Varadhan's lemma</h4>

↑ **Parent:** [Varadhan's lemma](#varadhan-s-lemma)

For a continuous $F$ and a family satisfying a [large deviation principle](#large-deviation-principle) at speed $L$, the displayed exponential tail condition extends [Varadhan's lemma](#varadhan-s-lemma) to $F$ unbounded above. Apply the bounded-above result to $\min(F,M)$ and split the full integral into $F\leq M$ and its tail; the tail is negligible and the truncated variational suprema increase to $\sup_x(F(x)-I(x))$. A sufficient condition is $\limsup_L L^{-1}\log\mathbb E e^{\gamma LF(X_L)}<\infty$ for some $\gamma>1$, since the tail is at most $e^{-(\gamma-1)LM}\mathbb E e^{\gamma LF(X_L)}$.

### Laplace principle (large deviations theory)

↑ **Parent:** [Large deviation principle](#large-deviation-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Laplace_principle_(large_deviations_theory))

The exponential integral of a fixed measurable function is controlled, on its logarithmic scale, by the function's [essential infimum](real-analysis.md#essential-infimum). Suppose $0<\int_Ae^{-\phi}dx<\infty$ and $\alpha=\operatorname*{ess\,inf}_A\phi$ is finite. For $\theta\geq1$, the integral is at most $e^{-(\theta-1)\alpha}\int_Ae^{-\phi}dx$. For every $\varepsilon>0$, the set $A_\varepsilon=\{x\in A:\phi(x)<\alpha+\varepsilon\}$ has positive finite [Lebesgue measure](measure-theory.md#lebesgue-measure), and the integral is at least $|A_\varepsilon|e^{-\theta(\alpha+\varepsilon)}$. Taking logarithms, dividing by $\theta$, and then letting $\varepsilon\downarrow0$ proves the displayed [limit](calculus.md#limit-of-a-function). The argument needs no isolated or nondegenerate minimizer. The [Laplace principle for probability measures](#laplace-principle-for-probability-measures) treats families whose distributions also change with the scaling parameter.

#### Laplace principle for probability measures

↑ **Parent:** [Laplace principle (large deviations theory)](#laplace-principle-large-deviations-theory)

A family satisfies this principle with speed $a_n\to\infty$ and [rate function](#rate-function) $I$ when the displayed variational identity holds for every bounded [continuous](calculus.md#continuous-function) real function $f$. A [large deviation principle](#large-deviation-principle) implies it by the [Varadhan lemma](#varadhan-s-lemma). The lower bound restricts the [expectation](probability-theory.md#expected-value) to a neighborhood of a chosen point; the upper bound partitions the bounded range of $f$ into small intervals and applies the closed-set probability bounds.

For nonnegative $X_n$, the identity also gives

$$
-\lim_n a_n^{-1}\log\mathbb E e^{-\mu a_nX_n}
=\inf_{s\geq0}[I(s)+\mu s],\qquad \mu\geq0.
$$

For $\mu>0$, truncate $f(s)=-\mu s$ below at $-\mu R$. The resulting bounded-function identity applies, while the difference of the two exponential [expectations](probability-theory.md#expected-value) is at most $e^{-\mu Ra_n}$. Choosing $R$ sufficiently large makes this error negligible on the claimed exponential scale. The case $\mu=0$ is immediate. This extension identifies moment-decay rates of a [passive scalar](fluid-mechanics.md#passive-scalar) from fluctuations of its logarithmic stretching.

<h3 id="gartner-ellis-theorem">Gärtner–Ellis theorem</h3>

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

Let $X_N\in\mathbb R^d$ and $a_N\to\infty$. Define the scaled [cumulant-generating function](probability-theory.md#cumulant-generating-function)

$$
\Lambda_N(\theta)=a_N^{-1}\log\mathbb E e^{a_N\langle\theta,X_N\rangle}.
$$

Suppose its pointwise limit $\Lambda$ exists, is [lower semicontinuous](calculus.md#lower-semicontinuity), has $0$ in the interior of its effective domain, and is essentially smooth: it is differentiable on that interior, which is nonempty, and its gradient norm diverges at every finite boundary point approached from the interior. Then $X_N$ satisfies a [large deviation principle](#large-deviation-principle) with [good rate function](#good-rate-function) given by the [Legendre-Fenchel transform](convex-optimization.md#convex-conjugate)

$$
\Lambda^*(x)=\sup_\theta\{\langle\theta,x\rangle-\Lambda(\theta)\}.
$$

The [Chernoff bound](probability-inequality.md#chernoff-bound) supplies the upper estimate. The lower estimate uses [exponential tilting](probability-theory.md#exponential-tilting) at a parameter whose gradient selects the required mean; essential smoothness supplies the boundary approximation needed for the full lower bound. A finite boundary slope can leave an affine branch of $\Lambda^*$ outside this argument, so a separate lower-bound proof is then necessary.

### Product large-deviation principle

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

Suppose $X_N$ and $Y_N$ are [independent random variables](random-variable.md#independent-random-variables) in Polish spaces, each satisfying a [large deviation principle](#large-deviation-principle) at speed $a_N$, with [good rate functions](#good-rate-function) $I$ and $K$. Their pair has [good rate function](#good-rate-function) $I(x)+K(y)$. On open rectangles, [independence](random-variable.md#independent-random-variables) makes the logarithmic lower bounds add. For the upper bound, the marginal families are [exponentially tight](#exponential-tightness), and so is their pair. Cover a closed set intersected with the product of the two compact containment sets by finitely many small rectangles and add the corresponding local upper bounds. The finite union bound and then increasing the containment level give the closed-set bound. Goodness follows because $\{I+K\leq M\}$ is closed inside $\{I\leq M\}\times\{K\leq M\}$.

### Contraction principle for large deviations

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

If $X_N$ satisfies a [large deviation principle](#large-deviation-principle) in $E$ with [good rate function](#good-rate-function) $I$ and $f:E\to F$ is a [continuous map](topology.md#continuous-map), then $f(X_N)$ has the same [large-deviation speed](#large-deviation-speed) and [good rate function](#good-rate-function)

$$
J(y)=\inf\{I(x):f(x)=y\}.
$$

The preimages of open and closed sets give the two [large deviation principle](#large-deviation-principle) inequalities. The identity $\{J\leq M\}=f(\{I\leq M\})$ follows from compactness and [lower semicontinuity](calculus.md#lower-semicontinuity) by taking minimizing sequences in the fibres; hence $J$ is good.

#### Rate function under scalar clipping

↑ **Parent:** [Contraction principle for large deviations](#contraction-principle-for-large-deviations)

For $a<b$, the [contraction principle for large deviations](#contraction-principle-for-large-deviations) under [scalar clipping](topology.md#scalar-clipping) gives $K(z)=I(z)$ in $(a,b)$, the displayed endpoint costs, and infinite cost outside $[a,b]$. The endpoint costs can differ from $I(a)$ and $I(b)$ because clipping collects a whole input tail into a single output atom.

#### Large-deviation rate of a minimum of independent copies

↑ **Parent:** [Contraction principle for large deviations](#contraction-principle-for-large-deviations)

For fixed $k$ [independent random variables](random-variable.md#independent-random-variables) whose families have the same [large deviation principle](#large-deviation-principle) with [good rate function](#good-rate-function) $I$, the [product large-deviation principle](#product-large-deviation-principle) gives the sum of coordinate costs. Under the minimum map, one coordinate must equal $m$ and the others must be at least $m$, yielding the displayed [rate function](#rate-function). If $I$ is [convex](real-analysis.md#convex-function) with unique zero $\mu$, then $J(m)=I(m)$ for $m\le\mu$ and $J(m)=kI(m)$ for $m\ge\mu$.

##### High moments of a clipped minimum of exponential sample means

↑ **Parent:** [Large-deviation rate of a minimum of independent copies](#large-deviation-rate-of-a-minimum-of-independent-copies)

Let $Z_n$ clip the minimum of $k$ independent exponential sample means into $[a,b]$, with $0<a<1/\lambda<b$. The [rate function under scalar clipping](#rate-function-under-scalar-clipping) is the minimum cost on this interval. Apply [Varadhan's lemma](#varadhan-s-lemma) to $\log z$. On the lower side its objective is increasing; on the upper side its derivative is $(k+1)/z-k\lambda$. Thus the optimum is $z_*=(k+1)/(k\lambda)$ once $k\ge(\lambda b-1)^{-1}$, giving the displayed limit. The [expectation](probability-theory.md#expected-value) is of the high power, rather than a power of the mean; the latter has limit $-\log\lambda$.

### Exponential equivalence

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

Coupled random elements $X_N,Y_N$ in a [metric space](topological-analysis.md#metric-space) are exponentially equivalent at [large-deviation speed](#large-deviation-speed) $a_N$ if for every $\eta>0$

$$
\limsup_N a_N^{-1}\log\mathbb P(d(X_N,Y_N)>\eta)=-\infty.
$$

If $X_N$ satisfies a [large deviation principle](#large-deviation-principle) with a [good rate function](#good-rate-function) $I$, then so does $Y_N$, with the same speed and [rate function](#rate-function). For the upper bound, $\{Y_N\in F\}$ is contained in $\{X_N\in F^\eta\}\cup\{d(X_N,Y_N)>\eta\}$, where $F^\eta$ is the closed $\eta$-neighborhood. Goodness gives $\inf_{F^\eta}I\to\inf_F I$ as $\eta\downarrow0$: otherwise bounded-rate almost minimizers have a convergent subsequence contradicting closedness and [lower semicontinuity](calculus.md#lower-semicontinuity). For an open-set lower bound, choose a ball about any $x\in G$ with a slightly larger ball still in $G$, subtract the superexponentially small error from the probability that $X_N$ belongs to the smaller ball, and shrink the ball. No [independence](random-variable.md#independent-random-variables) assumption is required.

### Exponential tightness

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

A family with [large-deviation speed](#large-deviation-speed) $a_N$ is exponentially tight if for every $M>0$ there is a [compact set](topology.md#compact-space) $K_M$ such that

$$
\limsup_N a_N^{-1}\log\mathbb P(X_N\notin K_M)\leq-M.
$$

Local upper bounds then imply the closed-set upper bound of a [large deviation principle](#large-deviation-principle): intersect the closed set with $K_M$, cover that compact intersection by finitely many neighborhoods on which the local bounds hold, and use a finite union bound. The remaining probability has exponent at most $-M$; let $M\to\infty$.

### Large-deviation speed

↑ **Parent:** [Large deviation principle](#large-deviation-principle)

A [large deviation principle](#large-deviation-principle) with speed $a_N\to\infty$ and [rate function](#rate-function) $I$ means that every open set $G$ and closed set $F$ satisfy

$$
-\inf_G I\leq\liminf_N a_N^{-1}\log\mathbb P(X_N\in G),\qquad
\limsup_N a_N^{-1}\log\mathbb P(X_N\in F)\leq-\inf_F I.
$$

Multiplying the [large-deviation speed](#large-deviation-speed) by $c>0$ divides the [rate function](#rate-function) by $c$. The speed must match the rare-event scale: a fixed [exponential random variable](continuous-probability-distribution.md#exponential-distribution) divided by $N^p$ has speed $N^p$, whereas a sum of $N$ [independent random variables](random-variable.md#independent-random-variables) with a [normal distribution](probability-theory.md#normal-distribution), divided by $N^p$, has speed $N^{2p-1}$ when $p>1$.

#### Hurstiness

↑ **Parent:** [Large-deviation speed](#large-deviation-speed)

A sequence has [Hurstiness](#hurstiness) H when it satisfies a [large deviation principle](#large-deviation-principle) at the displayed speed with a [good rate function](#good-rate-function) having a unique zero and at least one strictly positive finite value. This definition concerns a sequence's exponential probability scale; it does not assert a sample-path [Hurst exponent](stochastic-process.md#hurst-exponent) or self-similarity. Larger H means slower rare-event decay. The positive finite value excludes the [slower-speed degeneration of a large deviation principle](#slower-speed-degeneration-of-a-large-deviation-principle).

##### Hurstiness of independent sums

↑ **Parent:** [Hurstiness](#hurstiness)

For independent real sequences, put the faster sequence at the slower speed by [slower-speed degeneration of a large deviation principle](#slower-speed-degeneration-of-a-large-deviation-principle), then use the [product large-deviation principle](#product-large-deviation-principle) and [contraction principle for large deviations](#contraction-principle-for-large-deviations) for addition. Unequal speeds give a translate of the slower sequence's rate. Equal speeds give the [infimal convolution](convex-optimization.md#infimal-convolution) of the two rates. Its unique zero is the sum of their zero points, and a translated positive finite point has positive finite cost, since [compactness](topology.md#compact-space) attains each finite fiber [infimum](real-analysis.md#infimum). Thus the defining nondegeneracy is preserved.

// Target: queueing-theory.bigb

### Rate function

↑ **Parent:** [Large deviation principle](#large-deviation-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rate_function)

A rate function is a lower-semicontinuous map $I$ into $[0,\infty]$. It is good when every sublevel set $\{x:I(x)\leq c\}$ is compact.

#### Local convex path action

↑ **Parent:** [Rate function](#rate-function)

A local path action integrates a nonnegative convex cost g of the path's instantaneous input rate, assigning infinity to paths that are not absolutely continuous. When $g(\mu)=0$, the typical-rate path has zero cost. On any interval with prescribed total input, [Jensen inequality](real-analysis.md#jensen-s-inequality) makes a constant derivative minimize its cost. With a [queue workload](queueing-theory.md#workload-of-a-queue) constraint this leads to [constant-rate burst paths](queueing-theory.md#constant-rate-burst-path) and the [linear workload rate for a local convex action](queueing-theory.md#linear-workload-rate-for-a-local-convex-action). Such a formula alone does not establish goodness in an unspecified path topology; goodness must be checked or assumed as part of the input large-deviation principle.

#### Good rate function

↑ **Parent:** [Rate function](#rate-function)

A [rate function](#rate-function) is a [lower semicontinuous](calculus.md#lower-semicontinuity) map $I:E\to[0,\infty]$. It is good if every sublevel set $\{I\leq M\}$ is a [compact set](topology.md#compact-space). This property controls escapes to infinity and makes the minimizations in the [contraction principle for large deviations](#contraction-principle-for-large-deviations) attain their finite infima. On $\mathbb R^d$, a [lower semicontinuous](calculus.md#lower-semicontinuity) [rate function](#rate-function) tending to infinity with the norm is good.

##### A good rate function is separated from zero away from its minimizer

↑ **Parent:** [Good rate function](#good-rate-function)

If a [good rate function](#good-rate-function) has unique zero mu, every [closed set](topology.md#closed-set) missing mu has strictly positive [infimum](real-analysis.md#infimum) rate, possibly infinity. Otherwise a sequence of rates tending to zero lies eventually in the compact unit [sublevel set](calculus.md#sublevel-set); a subsequence converges to a point of the [closed set](topology.md#closed-set), and [lower semicontinuity](calculus.md#lower-semicontinuity) makes that point another zero. Compactness also ensures existence of a zero whenever the [infimum](real-analysis.md#infimum) is zero.

<h3 id="freidlin-wentzell-action">Freidlin--Wentzell action</h3>

↑ **Parent:** [Large deviation principle](#large-deviation-principle)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Freidlin--Wentzell_action)

For a small-noise diffusion $dX=a(X)dt+\sqrt\epsilon\,\sigma(X)dW$, the Freidlin--Wentzell action of a smooth path is

$$
I[\phi]=\frac12\int(\dot\phi-a)^T(\sigma\sigma^T)^{-1}(\dot\phi-a)\,dt.
$$

#### Geometric minimum action

↑ **Parent:** [Freidlin--Wentzell action](#freidlin-wentzell-action)

On a zero-Hamiltonian infinite-time fluctuation path, the Freidlin--Wentzell action can be parametrized independently of time as $I=\int\|a\|ds-a\mathbin\cdot d\phi$ in the diffusion metric.

## Central limit theorem

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Central_limit_theorem)

### Lindeberg-Feller central limit theorem

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

For each $n$, let $Z_{n,i}$ be independent centered [random variables](random-variable.md). If the sum of their [variances](variance.md) tends to $\sigma^2>0$ and $\sum_i\mathbb E[Z_{n,i}^2\mathbf1_{\{|Z_{n,i}|>\varepsilon\}}]\to0$ for every $\varepsilon>0$, their sum converges in distribution to the centered [normal distribution](probability-theory.md#normal-distribution) with variance $\sigma^2$. The second hypothesis is the [Lindeberg condition](#lindeberg-condition). If the total variance tends to zero, the corresponding degenerate limit follows directly from the [Chebyshev inequality](probability-inequality.md#chebyshev-inequality).

#### Lyapunov condition

↑ **Parent:** [Lindeberg-Feller central limit theorem](#lindeberg-feller-central-limit-theorem)

For independent centered [random variables](random-variable.md) with total [variance](variance.md) $s_n^2$, the Lyapunov condition requires the displayed expression to tend to zero for some $\delta>0$. The inequality $z^2\mathbf1_{\{|z|>\varepsilon s_n\}}\le |z|^{2+\delta}/(\varepsilon s_n)^\delta$ implies the [Lindeberg condition](#lindeberg-condition) after normalization. The [Lindeberg-Feller central limit theorem](#lindeberg-feller-central-limit-theorem) then makes the normalized sum converge to the standard [normal distribution](probability-theory.md#normal-distribution).

### Gaussian tails force an unbounded normalized partial-sum limsup

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

For independent identically distributed mean-zero variables with finite positive variance, the [central limit theorem](#central-limit-theorem) gives a positive eventual lower bound for $\mathbb P(S_n/\sqrt n\geq K)$ for every finite $K$. The decreasing events $\bigcup_{n\geq m}\{S_n/\sqrt n\geq K\}$ have probabilities bounded below, so [continuity from above of a measure](measure-theory.md#continuity-from-above-of-a-measure) gives positive probability that the limsup is at least $K$. The limsup itself is unchanged by removing any finite initial sum, hence is tail measurable. [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law) makes each event “limsup at least $K$” certain; intersect over integer $K$. The result is false for zero variance. One should apply the zero-one law to the limsup, rather than assume the exact threshold infinitely-often event is unaffected by a vanishing change.

### Normal approximation

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

A normal approximation replaces a sampling distribution by a [normal distribution](probability-theory.md#normal-distribution), often through a [central limit theorem](#central-limit-theorem). In a [Wald test](statistical-modelling.md#wald-test), approximate [statistical power](probability-and-statistics.md#statistical-power) is determined by the standardized difference under the alternative. This yields [Neyman allocation](probability-and-statistics.md#neyman-allocation) for fixed treatment-specific [variances](variance.md).

#### Continuity correction

↑ **Parent:** [Normal approximation](#normal-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continuity_correction)

A continuity correction shifts a discrete probability boundary by half a lattice spacing before using a continuous [normal approximation](#normal-approximation). For an upper-tail event $T\ge t$ on a unit lattice, the approximation is $1-\Phi((t-\tfrac12-E(T))/\sqrt{\operatorname{Var}(T)})$. Lower tails use the boundary $t+\tfrac12$. The correction is used in approximate [Wilcoxon signed-rank tests](nonparametric-statistics.md#wilcoxon-signed-rank-test) and [Wilcoxon rank sum tests](nonparametric-statistics.md#mann-whitney-u-test); tied ranks also require the appropriate variance adjustment.

### Lindeberg condition

↑ **Parent:** [Central limit theorem](#central-limit-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lindeberg_condition)

The Lindeberg condition requires the contribution of unusually large summands in a triangular array to become negligible compared with the array's total variance. Together with convergence of that variance, it gives the Lindeberg central limit theorem.

### Hilbert-space central limit theorem

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

For independent identically distributed centered random variables in a separable [Hilbert space](hilbert-space.md) with finite second moment, $n^{-1/2}\sum_{i=1}^nX_i$ converges in distribution to a centered [Gaussian random element](random-variable.md#gaussian-random-element) with the same [covariance operator](random-variable.md#covariance-operator).

### Self-normalized central limit theorem with a second-moment denominator

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

For independent identically distributed $Z_i$ with mean zero and variance one,

$$
\frac{n^{-1/2}\sum_{i=1}^nZ_i}{n^{-1}\sum_{i=1}^nZ_i^2}
\xrightarrow dN(0,1).
$$

The numerator obeys the central limit theorem, the denominator converges almost surely to one by the strong law, and Slutsky's theorem combines them.

<h3 id="donsker-s-theorem">Donsker's theorem</h3>

↑ **Parent:** [Central limit theorem](#central-limit-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Donsker's_theorem)

For independent identically distributed increments of mean zero and variance one, the diffusively rescaled, linearly interpolated random walk converges weakly in $C[0,1]$ to [Brownian motion](brownian-motion.md).

#### Fourth-moment tightness of polygonal random walks

↑ **Parent:** [Donsker's theorem](#donsker-s-theorem)

For centered unit-variance [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) increments with $m_4=\mathbb E\xi^4<\infty$, an interpolated increment is $N^{-1/2}\sum_jc_j\xi_j$. Here $c_j$ is the length of the overlap of $(Ns,Nt)$ with the $j$th unit cell, so $0\le c_j\le1$ and $\sum c_j=N(t-s)$. [Independence](random-variable.md#independent-random-variables) gives its [fourth moment](probability-theory.md#fourth-moment) as $N^{-2}[3(\sum c_j^2)^2+(m_4-3)\sum c_j^4]$. This is at most $\max(3,m_4)N^{-2}(\sum c_j^2)^2$, and $\sum c_j^2\le N(t-s)$ gives the bound, including intervals crossing a mesh point. A uniform fourth-moment continuity criterion yields [tightness of probability measures](probability-theory.md#uniform-tightness) on $C_0[0,1]$.

#### Random-walk maximum limit from Donsker invariance

↑ **Parent:** [Donsker's theorem](#donsker-s-theorem)

For a [random walk](markov-process.md#random-walk) with centered [independent](random-variable.md#independent-random-variables) identically distributed increments of [variance](variance.md) one, the maximum of its polygonal interpolation is the maximum at its grid vertices. The maximum functional is Lipschitz for the [supremum norm](functional-analysis.md#supremum-norm), so the [continuous mapping theorem](#continuous-mapping-theorem) applied to the [Donsker invariance principle](#donsker-s-theorem) proves the displayed [convergence in distribution](#convergence-in-distribution). The [Brownian reflection principle](brownian-motion.md#reflection-principle-wiener-process) then gives upper-tail limits $2(1-\Phi(a))$ at all $a>0$, since the limiting maximum has no atom there.

#### Integrated random-walk limit

↑ **Parent:** [Donsker's theorem](#donsker-s-theorem)

For a [random walk](markov-process.md#random-walk) with independent identically distributed steps of mean zero and [variance](variance.md) one, the [Donsker invariance principle](#donsker-s-theorem) and the [continuous mapping theorem](#continuous-mapping-theorem) for integration give this limit. The integral of the polygonal interpolation differs from the right-endpoint sum by $S_n/(2n^{3/2})$, whose squared [expectation](probability-theory.md#expected-value) is $1/(4n^2)$. The [Slutsky theorem](statistical-inference.md#slutsky-theorem) removes that error. The limiting variable is the time-one value of [integrated Brownian motion](brownian-motion.md#integrated-brownian-motion), with law $N(0,1/3)$.

### Multivariate central limit theorem

↑ **Parent:** [Central limit theorem](#central-limit-theorem)

For independent identically distributed random vectors $Z_i$ with mean $\mu$ and finite covariance matrix $V$,

$$
\sqrt n\left(\frac1n\sum_{i=1}^nZ_i-\mu\right)\xrightarrow dN(0,V).
$$

## Poisson limit theorem

↑ **Parent:** [Convergence of random variables](convergence-of-random-variables.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poisson_limit_theorem)

Binomial distributions with trial count tending to infinity and success probability tending to zero converge to a Poisson law when their product converges.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)
