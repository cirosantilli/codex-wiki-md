# Stochastic calculus

↑ **Parent:** [Stochastic process](stochastic-process.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_calculus)

Stochastic calculus extends integration and differential calculus to stochastic processes such as [Brownian motion](brownian-motion.md) and [semimartingales](#semimartingale).

**Table of contents**

- [Itô process](#ito-process)
- [Stochastic Fubini theorem](#stochastic-fubini-theorem)
- [Semimartingale](#semimartingale)
  - [Continuous semimartingale](#continuous-semimartingale)
  - [Semimartingale stability under an absolutely continuous measure change](#semimartingale-stability-under-an-absolutely-continuous-measure-change)
    - [Stochastic integral under an absolutely continuous measure change](#stochastic-integral-under-an-absolutely-continuous-measure-change)
  - [Bichteler-Dellacherie theorem](#bichteler-dellacherie-theorem)
  - [Finite-variation process](#finite-variation-process)
    - [Total-variation process](#total-variation-process)
      - [Càdlàg regularity of finite total variation](#cadlag-regularity-of-finite-total-variation)
  - [Semimartingale decomposition](#semimartingale-decomposition)
    - [Continuous semimartingale decomposition](#continuous-semimartingale-decomposition)
      - [Initial-value integrability in normalized semimartingale decompositions](#initial-value-integrability-in-normalized-semimartingale-decompositions)
- [Quadratic variation](#quadratic-variation)
  - [Predictable quadratic variation](#predictable-quadratic-variation)
  - [Uniqueness of an increasing square compensator](#uniqueness-of-an-increasing-square-compensator)
  - [Dyadic quadratic variation of a bounded continuous martingale](#dyadic-quadratic-variation-of-a-bounded-continuous-martingale)
  - [Finite-variation terms do not change quadratic variation](#finite-variation-terms-do-not-change-quadratic-variation)
  - [Localization and patching of quadratic variation](#localization-and-patching-of-quadratic-variation)
  - [Quadratic variation from completed grid increments](#quadratic-variation-from-completed-grid-increments)
  - [Weighted realized variance](#weighted-realized-variance)
    - [Spot variance](#spot-variance)
  - [Quadratic variation obstruction to Hölder regularity](#quadratic-variation-obstruction-to-holder-regularity)
  - [Dyadic quadratic variation of Brownian motion](#dyadic-quadratic-variation-of-brownian-motion)
  - [Dyadic power variation of a continuous local martingale](#dyadic-power-variation-of-a-continuous-local-martingale)
  - [Quadratic covariation](#quadratic-covariation)
    - [Quadratic covariations of an analytic Brownian image](#quadratic-covariations-of-an-analytic-brownian-image)
    - [Covariance identity for continuous square-integrable martingales](#covariance-identity-for-continuous-square-integrable-martingales)
    - [Weakly orthogonal continuous martingales](#weakly-orthogonal-continuous-martingales)
    - [Orthogonal continuous local martingales](#orthogonal-continuous-local-martingales)
      - [Knight theorem for orthogonal martingales](#knight-theorem-for-orthogonal-martingales)
      - [Complex exponential of two orthogonal Brownian motions](#complex-exponential-of-two-orthogonal-brownian-motions)
    - [Quadratic covariation under an absolutely continuous measure change](#quadratic-covariation-under-an-absolutely-continuous-measure-change)
      - [Quadratic variation under an absolutely continuous measure change](#quadratic-variation-under-an-absolutely-continuous-measure-change)
    - [Martingale product identity](#martingale-product-identity)
    - [Kunita-Watanabe inequality](#kunita-watanabe-inequality)
    - [Realized absolute covariation](#realized-absolute-covariation)
  - [Pathwise quadratic variation distinguishes Brownian speeds](#pathwise-quadratic-variation-distinguishes-brownian-speeds)
- [Stochastic integral](#stochastic-integral)
  - [Semimartingale integration by parts](#semimartingale-integration-by-parts)
  - [Stochastic dominated convergence theorem](#stochastic-dominated-convergence-theorem)
  - [Left-endpoint approximation of a continuous semimartingale integral](#left-endpoint-approximation-of-a-continuous-semimartingale-integral)
  - [Stopping-time shift of a stochastic integral](#stopping-time-shift-of-a-stochastic-integral)
  - [Conditionally Gaussian stochastic integral with an independent integrator](#conditionally-gaussian-stochastic-integral-with-an-independent-integrator)
  - [Stratonovich integral](#stratonovich-integral)
    - [Stratonovich chain rule](#stratonovich-chain-rule)
  - [Itô integral](#ito-integral)
    - [Gaussianity of deterministic Brownian stochastic integrals](#gaussianity-of-deterministic-brownian-stochastic-integrals)
    - [Gaussian coordinates of deterministic orthonormal Wiener integrands](#gaussian-coordinates-of-deterministic-orthonormal-wiener-integrands)
    - [Recovery of a continuous Brownian integrand from short increments](#recovery-of-a-continuous-brownian-integrand-from-short-increments)
  - [Associativity of stochastic integration](#associativity-of-stochastic-integration)
  - [Itô isometry](#ito-isometry)
    - [Square-integrable stochastic integrand](#square-integrable-stochastic-integrand)
    - [Fractional-moment control of Brownian increment ratios](#fractional-moment-control-of-brownian-increment-ratios)
    - [Conditional bracket isometry for stopped martingale increments](#conditional-bracket-isometry-for-stopped-martingale-increments)
    - [Quadratic-variation measure](#quadratic-variation-measure)
  - [Quadratic variation of a stochastic integral](#quadratic-variation-of-a-stochastic-integral)
    - [Localized isometry proof of stochastic-integral quadratic variation](#localized-isometry-proof-of-stochastic-integral-quadratic-variation)
- [Itô's lemma](#ito-s-lemma)
  - [Polynomial Itô formula from integration by parts](#polynomial-ito-formula-from-integration-by-parts)
  - [Itô formula for semimartingales with jumps](#ito-formula-for-semimartingales-with-jumps)
  - [Itô product rule](#ito-product-rule)
  - [Tanaka's formula](#tanaka-s-formula)
    - [Smooth convex approximation proof of the Tanaka formula](#smooth-convex-approximation-proof-of-the-tanaka-formula)
    - [Discrete Tanaka formula](#discrete-tanaka-formula)
- [Local time (mathematics)](#local-time-mathematics)
  - [Local time of a semimartingale](#local-time-of-a-semimartingale)
    - [Brownian local time](#brownian-local-time)
      - [Occupation approximations for Brownian local time](#occupation-approximations-for-brownian-local-time)
        - [Ratio-one interpolation for shrinking-window occupation integrals](#ratio-one-interpolation-for-shrinking-window-occupation-integrals)
    - [Right local time of a continuous semimartingale](#right-local-time-of-a-continuous-semimartingale)
- [Stochastic differential equation](#stochastic-differential-equation)
  - [Bounded diffusion coefficient gives square martingales](#bounded-diffusion-coefficient-gives-square-martingales)
  - [Bernoulli stochastic differential equation](#bernoulli-stochastic-differential-equation)
    - [Explosion threshold for a Bernoulli stochastic differential equation](#explosion-threshold-for-a-bernoulli-stochastic-differential-equation)
  - [Brownian rotation in the plane](#brownian-rotation-in-the-plane)
  - [Stroock-Varadhan support theorem](#stroock-varadhan-support-theorem)
  - [Square-root branching diffusion](#square-root-branching-diffusion)
    - [Cutoff construction of an absorbed square-root diffusion](#cutoff-construction-of-an-absorbed-square-root-diffusion)
    - [Addition law for square-root branching diffusions](#addition-law-for-square-root-branching-diffusions)
  - [Strict order preservation for scalar Lipschitz diffusions](#strict-order-preservation-for-scalar-lipschitz-diffusions)
    - [Reciprocal barrier proof of scalar diffusion comparison](#reciprocal-barrier-proof-of-scalar-diffusion-comparison)
  - [Global existence theorem for stochastic differential equations with Lipschitz coefficients](#global-existence-theorem-for-stochastic-differential-equations-with-lipschitz-coefficients)
  - [Tanaka equation](#tanaka-equation)
  - [Itô diffusion](#ito-diffusion)
    - [Exponential small-noise concentration for a Lipschitz diffusion](#exponential-small-noise-concentration-for-a-lipschitz-diffusion)
    - [Generator of an SDE diffusion](#generator-of-an-sde-diffusion)
    - [Initial mean and variance derivatives of an Itô diffusion](#initial-mean-and-variance-derivatives-of-an-ito-diffusion)
    - [Wright–Fisher diffusion](#wright-fisher-diffusion)
      - [Wright–Fisher binomial sampling chain](#wright-fisher-binomial-sampling-chain)
    - [Diffusion with hyperbolic tangent drift](#diffusion-with-hyperbolic-tangent-drift)
    - [Diffusion amplitude](#diffusion-amplitude)
    - [Diffusion occupation time](#diffusion-occupation-time)
    - [Power diffusion](#power-diffusion)
      - [Finite lifetime threshold for a power diffusion](#finite-lifetime-threshold-for-a-power-diffusion)
    - [Lamperti transform (diffusion)](#lamperti-transform-diffusion)
    - [Drift coefficient](#drift-coefficient)
      - [Drift estimator](#drift-estimator)
    - [Geometric Brownian motion](#geometric-brownian-motion)
      - [Killed geometric Brownian heat kernel](#killed-geometric-brownian-heat-kernel)
  - [Invariant distribution of an Itô diffusion](#invariant-distribution-of-an-ito-diffusion)
  - [Underdamped Langevin dynamics](#underdamped-langevin-dynamics)
    - [Inertial Brownian displacement with zero initial velocity](#inertial-brownian-displacement-with-zero-initial-velocity)
  - [Overdamped Langevin dynamics](#overdamped-langevin-dynamics)
    - [Isothermal diffusion with position-dependent drag](#isothermal-diffusion-with-position-dependent-drag)
    - [Tilted washboard potential](#tilted-washboard-potential)
    - [Kramers escape rate](#kramers-escape-rate)
  - [Euler-Maruyama method](#euler-maruyama-method)
    - [Milstein method](#milstein-method)
  - [Strong convergence of a stochastic numerical method](#strong-convergence-of-a-stochastic-numerical-method)
  - [Weak convergence of a stochastic numerical method](#weak-convergence-of-a-stochastic-numerical-method)
  - [Markov diffusion](#markov-diffusion)
    - [Driftless square-root diffusion](#driftless-square-root-diffusion)
      - [Compound Poisson transition law of a driftless square-root diffusion](#compound-poisson-transition-law-of-a-driftless-square-root-diffusion)
    - [Diffusion limit](#diffusion-limit)
    - [Speed density of a one-dimensional diffusion](#speed-density-of-a-one-dimensional-diffusion)
      - [Finite-interval diffusion exit Green kernel](#finite-interval-diffusion-exit-green-kernel)
  - [Maximal local solution of a stochastic differential equation](#maximal-local-solution-of-a-stochastic-differential-equation)
    - [Existence and pathwise uniqueness theorem for a stochastic differential equation](#existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation)
      - [Linear growth condition for an SDE](#linear-growth-condition-for-an-sde)
        - [Maximal second-moment bound under linear growth](#maximal-second-moment-bound-under-linear-growth)
  - [Scale function (stochastic processes)](#scale-function-stochastic-processes)
    - [Arctangent transform of a two-noise affine diffusion](#arctangent-transform-of-a-two-noise-affine-diffusion)
      - [Endpoint convergence of a bounded angle diffusion](#endpoint-convergence-of-a-bounded-angle-diffusion)
    - [Scale transform for an additive-noise diffusion](#scale-transform-for-an-additive-noise-diffusion)
      - [Strong well-posedness of additive-noise equations with bounded continuous drift](#strong-well-posedness-of-additive-noise-equations-with-bounded-continuous-drift)
      - [Zero extension of a scale diffusion coefficient at finite endpoints](#zero-extension-of-a-scale-diffusion-coefficient-at-finite-endpoints)
    - [Boundary hitting probability from a diffusion scale function](#boundary-hitting-probability-from-a-diffusion-scale-function)
      - [Hypotheses for a diffusion scale hitting formula](#hypotheses-for-a-diffusion-scale-hitting-formula)
  - [Weak solution of a stochastic differential equation](#weak-solution-of-a-stochastic-differential-equation)
    - [Weak existence and uniqueness in law for an additive-noise SDE with bounded drift](#weak-existence-and-uniqueness-in-law-for-an-additive-noise-sde-with-bounded-drift)
  - [Strong solution of a stochastic differential equation](#strong-solution-of-a-stochastic-differential-equation)
    - [Strong existence](#strong-existence)
    - [Strong existence theorem for additive-noise SDEs with bounded measurable drift](#strong-existence-theorem-for-additive-noise-sdes-with-bounded-measurable-drift)
  - [Pathwise uniqueness](#pathwise-uniqueness)
  - [Uniqueness in law](#uniqueness-in-law)
  - [Kolmogorov backward equation](#kolmogorov-backward-equation)
    - [Bounded backward-equation stochastic representation](#bounded-backward-equation-stochastic-representation)
    - [Feynman-Kac formula](#feynman-kac-formula)
      - [Critical quadratic potential for the Ornstein-Uhlenbeck generator](#critical-quadratic-potential-for-the-ornstein-uhlenbeck-generator)
      - [Elliptic Feynman-Kac formula](#elliptic-feynman-kac-formula)
      - [Parabolic Feynman-Kac formula with a source](#parabolic-feynman-kac-formula-with-a-source)
      - [Discounted boundary-hitting representation](#discounted-boundary-hitting-representation)
      - [Feynman-Kac formula with a bounded potential](#feynman-kac-formula-with-a-bounded-potential)
        - [Soft killing limit for Brownian nonnegative survival](#soft-killing-limit-for-brownian-nonnegative-survival)
        - [Zero-noise limit with a bounded potential](#zero-noise-limit-with-a-bounded-potential)
        - [Positive-potential growth from Brownian recurrence](#positive-potential-growth-from-brownian-recurrence)
  - [Martingale problem](#martingale-problem)
    - [Martingale problem for Brownian motion](#martingale-problem-for-brownian-motion)
    - [Diffusion approximation theorem](#diffusion-approximation-theorem)
    - [Well-posed martingale problem](#well-posed-martingale-problem)
    - [Diffusion martingale problem](#diffusion-martingale-problem)
      - [Bounded-domain harmonic uniqueness for a diffusion](#bounded-domain-harmonic-uniqueness-for-a-diffusion)
      - [Projection unboundedness of a uniformly elliptic diffusion](#projection-unboundedness-of-a-uniformly-elliptic-diffusion)
      - [Time-dependent test functions for a diffusion martingale problem](#time-dependent-test-functions-for-a-diffusion-martingale-problem)
- [Doléans-Dade exponential](#doleans-dade-exponential)
  - [Pathwise uniqueness for a multiplicative martingale equation](#pathwise-uniqueness-for-a-multiplicative-martingale-equation)
  - [Stochastic logarithm](#stochastic-logarithm)
    - [Divergent logarithmic clock for a positive local martingale tending to zero](#divergent-logarithmic-clock-for-a-positive-local-martingale-tending-to-zero)
  - [Kazamaki's condition](#kazamaki-s-condition)
  - [Terminal scaling inequality for stochastic exponentials](#terminal-scaling-inequality-for-stochastic-exponentials)
  - [Hölder factorization of stochastic exponentials](#holder-factorization-of-stochastic-exponentials)
    - [Half-threshold for the exponential-martingale Hölder bound](#half-threshold-for-the-exponential-martingale-holder-bound)
  - [Novikov's condition](#novikov-s-condition)
    - [Bounded-bracket criterion for a stochastic exponential](#bounded-bracket-criterion-for-a-stochastic-exponential)
    - [Dambis-Dubins-Schwarz proof of the Novikov condition](#dambis-dubins-schwarz-proof-of-the-novikov-condition)
  - [Girsanov theorem](#girsanov-theorem)
    - [Ornstein-Uhlenbeck likelihood relative to Wiener measure](#ornstein-uhlenbeck-likelihood-relative-to-wiener-measure)
    - [Bounded Girsanov density for exit of an unstable linear diffusion](#bounded-girsanov-density-for-exit-of-an-unstable-linear-diffusion)
    - [Semimartingale invariance under equivalent measures](#semimartingale-invariance-under-equivalent-measures)
    - [Finite-horizon drift replacement by a change of measure](#finite-horizon-drift-replacement-by-a-change-of-measure)
    - [Girsanov density for a stopped Bessel process](#girsanov-density-for-a-stopped-bessel-process)
      - [Brownian conditioning by a stopped Bessel density](#brownian-conditioning-by-a-stopped-bessel-density)
    - [Martingale transfer under a density process](#martingale-transfer-under-a-density-process)
      - [Initial integrability under a density change](#initial-integrability-under-a-density-change)
      - [Bounded-process density-product criterion](#bounded-process-density-product-criterion)

<h2 id="ito-process">Itô process</h2>

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)

An Itô process is a continuous [semimartingale](#semimartingale) expressible as the displayed sum, with adapted coefficients locally integrable for the time integral and locally square integrable for the [Itô integral](#ito-integral). The coefficients may depend on the whole past; an [Itô diffusion](#ito-diffusion) usually specifies them as functions of the current state and time. A continuously differentiable deterministic process is an Itô process with zero Brownian coefficient. The [Itô formula](#ito-s-lemma) and [Itô product rule](#ito-product-rule) apply to these processes.

## Stochastic Fubini theorem

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)

A theorem interchanging a parameter integral with an [Itô integral](#ito-integral), under appropriate measurability and integrability hypotheses. For a bounded deterministic integrand on a finite parameter-time rectangle, the square-integrability conditions hold; triangular domains can be handled by an indicator of the domain.

## Semimartingale

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semimartingale)

A semimartingale is the sum of a [local martingale](martingale.md#local-martingale) and an adapted finite-variation process. This is the broad class of integrators for which the Itô stochastic integral is defined.

### Continuous semimartingale

↑ **Parent:** [Semimartingale](#semimartingale)

A continuous [semimartingale](#semimartingale) is a continuous adapted process admitting a decomposition $X=X_0+N+V$, with $N$ a zero-starting [continuous local martingale](martingale.md#continuous-local-martingale) and $V$ continuous adapted [finite variation](real-analysis.md#total-variation-of-a-function). The decomposition is unique because a continuous finite-variation local [martingale](martingale.md) starting at zero vanishes. Its [quadratic variation](#quadratic-variation) is $[X]=[N]$.

### Semimartingale stability under an absolutely continuous measure change

↑ **Parent:** [Semimartingale](#semimartingale)

If $X$ is a [semimartingale](#semimartingale) under $P$ and $Q\ll P$, then it is a [semimartingale](#semimartingale) under $Q$. The [Bichteler-Dellacherie theorem](#bichteler-dellacherie-theorem) gives a short proof: terminal elementary integrals associated with uniformly small [elementary predictable processes with stopping-time intervals](martingale.md#elementary-predictable-process-with-stopping-time-intervals) converge to zero in $P$-[probability](probability-theory.md#probability). [Uniform convergence on compacts in probability under an absolutely continuous measure change](stochastic-process.md#uniform-convergence-on-compacts-in-probability-under-an-absolutely-continuous-measure-change), or its single-random-variable proof, transfers convergence to $Q$. The same good-integrator characterization now applies under $Q$. Adaptedness and [càdlàg](calculus.md#cadlag) paths are preserved because $P$-null sets remain $Q$-null; if necessary use the usual $Q$-completion of the same [filtration](stochastic-process.md#filtration-probability-theory). If the integrands are bounded only outside $Q$-null sets, clip their coefficients to the specified deterministic bounds before applying the $P$-criterion; this preserves their $Q$-versions. Completion adds only equivalent versions of measurable coefficients. This theorem does not preserve the [local martingale](martingale.md#local-martingale) property.

#### Stochastic integral under an absolutely continuous measure change

↑ **Parent:** [Semimartingale stability under an absolutely continuous measure change](#semimartingale-stability-under-an-absolutely-continuous-measure-change)

If $Q\ll P$ and $X$ is a semimartingale under both measures, the two integrals of any locally bounded predictable $H$ against $X$ agree up to $Q$-indistinguishability. Elementary integrals are the same increment sums. Bounded pointwise convergence of integrands, stochastic dominated convergence, and transfer of probability convergence from $P$ to $Q$ extend equality by the monotone-class theorem. Localize to remove boundedness.

// Target: probability-and-statistics.bigb

### Bichteler-Dellacherie theorem

↑ **Parent:** [Semimartingale](#semimartingale)

An adapted [càdlàg process](stochastic-process.md#cadlag-process) is a [semimartingale](#semimartingale) exactly when it is a good integrator: on each finite horizon, for every sequence of bounded [elementary predictable processes with stopping-time intervals](martingale.md#elementary-predictable-process-with-stopping-time-intervals) $H^n$ whose deterministic uniform bounds tend to zero, the elementary terminal integrals $(H^n\mathbin\cdot X)_T$ tend to zero in [probability](probability-theory.md#probability). The elementary integral is a finite sum of measurable coefficients times subsequent increments; the characterization says precisely when this operation extends continuously to stochastic integration. The theorem is used here as a standard characterization, not proved from first principles.

### Finite-variation process

↑ **Parent:** [Semimartingale](#semimartingale)

A process $A$ has finite variation on compact intervals when every sample path has finite [total variation of a function](real-analysis.md#total-variation-of-a-function) there. Such a process can be integrated pathwise by the Lebesgue-Stieltjes integral.

#### Total-variation process

↑ **Parent:** [Finite-variation process](#finite-variation-process)

For a path of [finite variation](real-analysis.md#total-variation-of-a-function), its total-variation process is

$$
V_t(A)=\sup_\pi\sum_{[u,v]\in\pi}|A_v-A_u|,
$$

where the [supremum](real-analysis.md#supremum) is over every [partition of an interval](real-analysis.md#partition-of-an-interval) of $[0,t]$. It is an increasing process, and the signed measure $dA$ satisfies $|dA|=dV(A)$.

<h5 id="cadlag-regularity-of-finite-total-variation">Càdlàg regularity of finite total variation</h5>

↑ **Parent:** [Total-variation process](#total-variation-process)

If a [càdlàg function](calculus.md#cadlag) has [finite variation](real-analysis.md#total-variation-of-a-function) on compact intervals, its [total-variation process](#total-variation-process) is finite, nondecreasing, and [càdlàg](calculus.md#cadlag). Left limits follow from monotonicity. For right continuity, approximate the variation on $[t,s]$ by one finite partition. Changing its first endpoint from $t$ to $u\downarrow t$ changes the sum by at most $|X_u-X_t|$, which tends to zero. Additivity of variation then bounds $V(u)-V(t)$ by an arbitrarily small error. Its jump is the absolute jump of $X$. Without locally finite variation, right continuity can fail even as an extended-valued assertion: $X_t=t\sin(1/t)$ with $X_0=0$ has infinite variation on every interval starting at zero.

### Semimartingale decomposition

↑ **Parent:** [Semimartingale](#semimartingale)

A semimartingale has a decomposition $X=X_0+M+A$ into a [local martingale](martingale.md#local-martingale) $M$ and an adapted [finite-variation process](#finite-variation-process) $A$. Under standard normalizations the decomposition is unique.

#### Continuous semimartingale decomposition

↑ **Parent:** [Semimartingale decomposition](#semimartingale-decomposition)

A continuous semimartingale has a decomposition in which both the local-martingale and finite-variation parts are continuous.

##### Initial-value integrability in normalized semimartingale decompositions

↑ **Parent:** [Continuous semimartingale decomposition](#continuous-semimartingale-decomposition)

With the [local martingale](martingale.md#local-martingale) definition requiring each stopped process itself to be a [martingale](martingale.md), the initial value is integrable. A normalized [continuous semimartingale decomposition](#continuous-semimartingale-decomposition) $X=M+A$ with $A_0=0$ can therefore have a local-martingale part only if $X_0$ is integrable. A smooth transformation need not preserve this condition: take $M=0$, $A_t=G$ for an initially known standard [normal random variable](probability-theory.md#gaussian-random-variable), and $f(x,a)=e^{a^2}$. Then $f(M_0,A_0)$ is finite almost surely but has infinite expectation. The always-valid decomposition is instead $X=X_0+N+V$ with a zero-starting [continuous local martingale](martingale.md#continuous-local-martingale) $N$ and a continuous [finite-variation process](#finite-variation-process) $V$ starting at zero.

## Quadratic variation

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_variation)

The quadratic variation of a continuous semimartingale is the limit in probability

$$
[X]_t=\lim_{|\pi|\to0}\sum_{[u,v]\in\pi}(X_v-X_u)^2.
$$

Finite-variation processes have zero quadratic variation, while a Brownian motion satisfies $[B]_t=t$.

### Predictable quadratic variation

↑ **Parent:** [Quadratic variation](#quadratic-variation)

For a zero-starting square-integrable martingale, the predictable quadratic variation is the predictable increasing process $A$ for which $M^2-A$ is a martingale. For a compensated jump process it integrates squared jump sizes against their rates. Unlike optional quadratic variation, it need not equal the sum of squared realized jumps. For continuous local martingales, the two brackets coincide after localization.

// Target: probability-and-statistics.bigb

### Uniqueness of an increasing square compensator

↑ **Parent:** [Quadratic variation](#quadratic-variation)

For a [continuous local martingale](martingale.md#continuous-local-martingale) $M$, at most one continuous adapted increasing process $A$ starting at zero makes $M^2-A$ a [local martingale](martingale.md#local-martingale). The difference of two candidates is a continuous [finite-variation process](#finite-variation-process) and a [local martingale](martingale.md#local-martingale), hence constant; its initial value is zero. Without the initial-value normalization only uniqueness up to an initial constant is possible.

### Dyadic quadratic variation of a bounded continuous martingale

↑ **Parent:** [Quadratic variation](#quadratic-variation)

Let $X$ be a continuous martingale on $[0,1]$ with $X_0=0$ and $|X_t|\le C$. For the dyadic squared-increment sums, including the unfinished increment at time $t$, set $A_t^{(n)}=\sum_k(X_{k2^{-n}\wedge t}-X_{(k-1)2^{-n}\wedge t})^2$. The associated martingale transform $M_t^{(n)}=(X_t^2-A_t^{(n)})/2$ satisfies $\mathbb E(M_1^{(n)})^2\le C^4$ and $\mathbb E(A_1^{(n)})^2\le10C^4$. Discrete martingale orthogonality, the path modulus of continuity and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) show that the terminal transforms are Cauchy in $L^2$. The [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) then gives $\mathbb E\sup_{t\le1}|A_t^{(n)}-A_t^{(m)}|^2\to0$. The sums need not be increasing in time before taking the limit. This provides an elementary construction of [quadratic variation](#quadratic-variation) under boundedness.

### Finite-variation terms do not change quadratic variation

↑ **Parent:** [Quadratic variation](#quadratic-variation)

On a compact interval, squared increments of a continuous [finite variation](real-analysis.md#total-variation-of-a-function) process are bounded by its modulus of continuity at the mesh size times its total variation, and therefore vanish. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bounds the mixed increment sum by the square root of the product of the two squared-increment sums. The local-[martingale](martingale.md) sum is bounded in probability, so the mixed term also vanishes.

### Localization and patching of quadratic variation

↑ **Parent:** [Quadratic variation](#quadratic-variation)

Stop a [continuous local martingale](martingale.md#continuous-local-martingale) at increasing level-and-time stopping times to obtain bounded [martingales](martingale.md). Their limits of discrete [quadratic variation](#quadratic-variation) sums agree before the earlier stopping time, because the sums commute exactly with stopping. These continuous limits patch into a continuous adapted nondecreasing process. On each compact interval, the chance that the stopping time occurs early tends to zero, giving [uniform convergence on compacts in probability](stochastic-process.md#uniform-convergence-on-compacts-in-probability) for the original sums.

### Quadratic variation from completed grid increments

↑ **Parent:** [Quadratic variation](#quadratic-variation)

Completed squared increments form a nondecreasing step process. The continuous sum that includes the last partial increment differs by at most the square of the path's modulus of continuity over one mesh interval. Therefore both have the same limit in [uniform convergence on compacts in probability](stochastic-process.md#uniform-convergence-on-compacts-in-probability). This proves monotonicity of the limiting [quadratic variation](#quadratic-variation) without incorrectly asserting monotonicity of each continuous partial-increment sum.

### Weighted realized variance

↑ **Parent:** [Quadratic variation](#quadratic-variation)

For observations of an [Itô integral](#ito-integral) on a [partition of an interval](real-analysis.md#partition-of-an-interval), the statistic $\sum_i g(t_{i-1})(X_{t_i}-X_{t_{i-1}})^2$ estimates $\int g(t)\sigma(t)^2\,dt$. With a deterministic noise coefficient the squared increments are [independent](random-variable.md#independent-random-variables), and the fluctuation has [variance](variance.md) $2\sum_i g(t_{i-1})^2(\int_{t_{i-1}}^{t_i}\sigma^2)^2$.

#### Spot variance

↑ **Parent:** [Weighted realized variance](#weighted-realized-variance)

The spot variance is the instantaneous squared noise coefficient $\sigma(t)^2$ of an [Itô integral](#ito-integral). It can be estimated by averaging the [weighted realized variance](#weighted-realized-variance) over a shrinking time window. A [Hölder continuity](sobolev-space.md#holder-condition) assumption bounds the smoothing [bias](statistical-modelling.md#bias-of-an-estimator).

<h3 id="quadratic-variation-obstruction-to-holder-regularity">Quadratic variation obstruction to Hölder regularity</h3>

↑ **Parent:** [Quadratic variation](#quadratic-variation)

A function with finite [Hölder seminorm](sobolev-space.md#holder-seminorm) of exponent $\alpha>1/2$ has squared-increment sum on a uniform $N$-interval partition bounded by $C^2N^{1-2\alpha}$, hence tending to zero. This conflicts with a nonzero quadratic-variation limit. In particular [dyadic quadratic variation of Brownian motion](#dyadic-quadratic-variation-of-brownian-motion) prevents a Brownian coordinate law supported on such a [Hölder space](sobolev-space.md#holder-space). This argument alone gives no conclusion at the critical exponent $1/2$.

### Dyadic quadratic variation of Brownian motion

↑ **Parent:** [Quadratic variation](#quadratic-variation)

On $[0,1]$, the sum $Q_n$ of squared adjacent dyadic increments of standard [Brownian motion](brownian-motion.md) has $\mathbb E Q_n=1$ and $\operatorname{var}(Q_n)=2^{1-n}$. Therefore $Q_n\to1$ in $L^2$. On an interval of length $t$, scaling gives mean $t$ and [variance](variance.md) $2t^2 2^{-n}$. [Independence](random-variable.md#independent-random-variables) is used within each grid, not between different grids.

### Dyadic power variation of a continuous local martingale

↑ **Parent:** [Quadratic variation](#quadratic-variation)

Along the dyadic [partitions of an interval](real-analysis.md#partition-of-an-interval) of $[0,1]$, the sums $\sum_i|\Delta_iM|^p$ of a [continuous local martingale](martingale.md#continuous-local-martingale) tend to zero in [probability](probability-theory.md#probability) for $p>2$. If $0<p<2$ and these sums are eventually bounded [almost surely](convergence-of-random-variables.md#almost-sure-convergence), then $M$ is constant on $[0,1]$: compare them with the sums defining [quadratic variation](#quadratic-variation), using the maximum increment, which tends to zero by [uniform continuity](topological-analysis.md#uniform-continuity).

### Quadratic covariation

↑ **Parent:** [Quadratic variation](#quadratic-variation)

The quadratic covariation of two continuous semimartingales is the limit in probability

$$
[M,N]_t=\lim_{|\pi|\to0}\sum_{[u,v]\in\pi}(M_v-M_u)(N_v-N_u).
$$

The [polarization identity](linear-algebra.md#polarization-identity) gives $[M,N]=\frac14([M+N]-[M-N])$.

#### Quadratic covariations of an analytic Brownian image

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For an [analytic function](complex-analysis.md#space-of-holomorphic-functions) $f=u+iv$ and planar [Brownian motion](brownian-motion.md) $Z=X+iY$ with [independent](random-variable.md#independent-random-variables) standard coordinates, the [Cauchy-Riemann equations](analysis.md#cauchy-riemann-equations) make $u,v$ harmonic. The [Itô formula](#ito-s-lemma) gives $dU=u_xdX+u_ydY$ and $dV=-u_ydX+u_xdY$. Localizing the derivatives proves both coordinates are [local martingales](martingale.md#local-martingale). Squaring their diffusion coefficients and multiplying the two rows gives the displayed [quadratic variations](#quadratic-variation) and zero [quadratic covariation](#quadratic-covariation).

#### Covariance identity for continuous square-integrable martingales

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For two zero-starting continuous martingales square-integrable at time $t$, the [Itô isometry](#ito-isometry) gives $\mathbb E(M_t\pm N_t)^2=\mathbb E[M\pm N]_t$. The [polarization identity](linear-algebra.md#polarization-identity) yields the displayed identity. Integrability of the cross-bracket follows from the [Kunita-Watanabe inequality](#kunita-watanabe-inequality) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

#### Weakly orthogonal continuous martingales

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For zero-starting [L2-bounded continuous martingales](martingale.md#l2-bounded-continuous-martingale), this condition is equivalent to $\mathbb E[M_tN_t]=0$ at equal times, by conditioning the later factor. The [covariance identity for continuous square-integrable martingales](#covariance-identity-for-continuous-square-integrable-martingales) also makes it equivalent to $\mathbb E[M,N]_t=0$. It is weaker than the vanishing bracket condition for [orthogonal continuous local martingales](#orthogonal-continuous-local-martingales): $B_{t\wedge1}$ and $B_{t\wedge1}^2-(t\wedge1)$ have zero equal-time covariance but nonzero bracket $2\int_0^{t\wedge1}B_sds$.

#### Orthogonal continuous local martingales

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

Two [continuous local martingales](martingale.md#continuous-local-martingale) are orthogonal when their [quadratic covariation](#quadratic-covariation) is zero. With zero initial values, the [martingale product identity](#martingale-product-identity) says that their product is a [local martingale](martingale.md#local-martingale). For two [Brownian motions](brownian-motion.md) in a common [filtration](stochastic-process.md#filtration-probability-theory), orthogonality and the [Lévy characterization of multidimensional Brownian motion](brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion) make the pair a two-dimensional [Brownian motion](brownian-motion.md) and imply independence. Merely having the two marginal [Brownian motion](brownian-motion.md) laws on the same space does not imply orthogonality.

##### Knight theorem for orthogonal martingales

↑ **Parent:** [Orthogonal continuous local martingales](#orthogonal-continuous-local-martingales)

Let $M_1,\ldots,M_N$ be continuous [local martingales](martingale.md#local-martingale) starting at zero, with $\langle M_i,M_j\rangle=0$ for $i\ne j$ and $\langle M_j\rangle_\infty=\infty$ almost surely. The individual [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) time changes produce [independent](random-variable.md#independent-random-variables) standard [Brownian motions](brownian-motion.md) $B_j$ with $M_j(t)=B_j(\langle M_j\rangle_t)$. Independence is between the [Brownian motions](brownian-motion.md); each may still depend on its own clock.

##### Complex exponential of two orthogonal Brownian motions

↑ **Parent:** [Orthogonal continuous local martingales](#orthogonal-continuous-local-martingales)

For [orthogonal continuous local martingales](#orthogonal-continuous-local-martingales) $B,\vartheta$ that are standard [Brownian motions](brownian-motion.md), the [real part](complex-analysis.md#real-part) $X=e^B\cos\vartheta$ and [imaginary part](complex-analysis.md#imaginary-part) $Y=e^B\sin\vartheta$ are [continuous local martingales](martingale.md#continuous-local-martingale). The [Itô formula](#ito-s-lemma) gives $dX=X\,dB-Y\,d\vartheta$ and $dY=Y\,dB+X\,d\vartheta$, since the two diagonal second-order terms cancel. Their [quadratic variations](#quadratic-variation) equal $\int_0^te^{2B_s}ds$ and their [quadratic covariation](#quadratic-covariation) is zero. If $C=[B,\vartheta]$ is nonzero, the omitted drift terms are respectively $-Y\,dC$ and $X\,dC$, so the orthogonality hypothesis is essential.

#### Quadratic covariation under an absolutely continuous measure change

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For continuous [semimartingales](#semimartingale) and $Q\ll P$, their [quadratic covariation](#quadratic-covariation) has the same version under the two [probability measures](probability-theory.md#probability-measure), up to $Q$-[indistinguishability of stochastic processes](stochastic-process.md#indistinguishability-of-stochastic-processes). The dyadic product sums have the same limit by [uniform convergence on compacts in probability under an absolutely continuous measure change](stochastic-process.md#uniform-convergence-on-compacts-in-probability-under-an-absolutely-continuous-measure-change). Uniqueness of a limit in [probability](probability-theory.md#probability) identifies that limit with the bracket under $Q$. [Semimartingale stability under an absolutely continuous measure change](#semimartingale-stability-under-an-absolutely-continuous-measure-change) supplies the correct class under $Q$: a [local martingale](martingale.md#local-martingale) need not remain a [local martingale](martingale.md#local-martingale). Taking the two processes equal proves the same statement for [quadratic variation](#quadratic-variation) without a separate assumption.

##### Quadratic variation under an absolutely continuous measure change

↑ **Parent:** [Quadratic covariation under an absolutely continuous measure change](#quadratic-covariation-under-an-absolutely-continuous-measure-change)

If $Q\ll P$ and a [continuous semimartingale](#continuous-semimartingale) is a [semimartingale](#semimartingale) under both measures, its quadratic variations agree $Q$-indistinguishably. The same squared-increment sums converge uniformly on compacts in probability under both measures: absolute continuity transfers the original convergence, and uniqueness of the limit identifies the two continuous versions. Equivalence of measures is unnecessary.

#### Martingale product identity

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For continuous local martingales $M$ and $N$, the [Itô product rule](#ito-product-rule) says that

$$
M_tN_t-M_0N_0-[M,N]_t
$$

is a [local martingale](martingale.md#local-martingale). If the martingales are square-integrable and converge in $L^2$, then

$$
\mathbb E[M_\infty N_\infty]=\mathbb E[M_0N_0]+\mathbb E[M,N]_\infty.
$$

#### Kunita-Watanabe inequality

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For continuous local martingales, the [total-variation process](#total-variation-process) of their [quadratic covariation](#quadratic-covariation) satisfies

$$
V_t([M,N])\leq[M]_t^{1/2}[N]_t^{1/2}.
$$

It is the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) for the matrix-valued measure formed by their [quadratic variations](#quadratic-variation) and [quadratic covariation](#quadratic-covariation).

#### Realized absolute covariation

↑ **Parent:** [Quadratic covariation](#quadratic-covariation)

For continuous local martingales $M,N$ and a sequence in which each term is a [partition of an interval](real-analysis.md#partition-of-an-interval) whose mesh tends to zero, the sums

$$
\widetilde V_t^n=\sum_k|\Delta_kM|\,|\Delta_kN|
$$

converge in the sense of [uniform convergence on compacts in probability](stochastic-process.md#uniform-convergence-on-compacts-in-probability) to a continuous increasing process. To identify the limit, put $C=[M]+[N]$ and choose [Radon-Nikodym derivatives](measure-theory.md#radon-nikodym-derivative)

$$
a=\frac{d[M]}{dC},\qquad b=\frac{d[N]}{dC},\qquad c=\frac{d[M,N]}{dC}.
$$

If $(U,V)$ is a centered [bivariate normal distribution](probability-and-statistics.md#bivariate-normal-distribution) with covariance matrix $\left(\begin{smallmatrix}a&c\\c&b\end{smallmatrix}\right)$, then

$$
\widetilde V_t=\int_0^t\mathbb E|UV|\,dC.
$$

Localizing, representing the pair as [stochastic integrals](#stochastic-integral) against a two-dimensional [Brownian motion](brownian-motion.md), and approximating the integrands by bounded predictable step processes proves the convergence. The step-process case follows from the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) for independent Gaussian increments; the [Burkholder-Davis-Gundy inequality](martingale.md#burkholder-davis-gundy-inequalities) controls the approximation error. Since $|\mathbb E[UV]|\leq\mathbb E|UV|\leq\sqrt{\mathbb EU^2\mathbb EV^2}$,

$$
V_t([M,N])\leq\widetilde V_t\leq[M]_t^{1/2}[N]_t^{1/2}.
$$

### Pathwise quadratic variation distinguishes Brownian speeds

↑ **Parent:** [Quadratic variation](#quadratic-variation)

On $[0,T]$, a standard [Brownian motion](brownian-motion.md) has pathwise [quadratic variation](#quadratic-variation) $t$, whereas the time-rescaled process $B_{ct}$ has quadratic variation $ct$. Therefore their path laws are mutually singular when $c\ne1$.

## Stochastic integral

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)

The stochastic integral $\int H\,dX$ integrates a predictable process against a semimartingale. It extends pathwise integration against finite-variation processes and the Itô integral against local martingales.

### Semimartingale integration by parts

↑ **Parent:** [Stochastic integral](#stochastic-integral)

For càdlàg semimartingales, the product rule uses left-limit integrands and quadratic covariation including jump products. For continuous semimartingales it reduces to the [Itô product rule](#ito-product-rule) without left-limit notation. This rule permits an induction proof of the Itô formula for polynomial functions.

### Stochastic dominated convergence theorem

↑ **Parent:** [Stochastic integral](#stochastic-integral)

If uniformly bounded predictable processes $H_n$ converge pointwise to $H$, then their integrals against a fixed semimartingale converge to $H\cdot X$ uniformly on compact intervals in probability. Localized domination gives corresponding extensions. This continuity permits a functional monotone-class argument from elementary predictable integrands to all bounded predictable integrands.

// Target: probability-and-statistics.bigb

### Left-endpoint approximation of a continuous semimartingale integral

↑ **Parent:** [Stochastic integral](#stochastic-integral)

For a left-continuous locally bounded [adapted process](stochastic-process.md#adapted-process) $H$ and a [continuous semimartingale](#continuous-semimartingale) $X$, the elementary predictable left-endpoint approximations tend pointwise to $H$. Decompose $X$ into a [continuous local martingale](martingale.md#continuous-local-martingale) and a continuous [finite-variation process](#finite-variation-process). After localization, dominated convergence with respect to the variation measure handles the finite-variation integral. The [Itô isometry](#ito-isometry) and [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) handle the martingale integral. The omitted partial last interval is bounded by the local bound on $H$ times the modulus of continuity of $X$. This proves [uniform convergence on compacts in probability](stochastic-process.md#uniform-convergence-on-compacts-in-probability) and is the grid-sum foundation of the [Itô product rule](#ito-product-rule).

### Stopping-time shift of a stochastic integral

↑ **Parent:** [Stochastic integral](#stochastic-integral)

For a finite [stopping time](martingale.md#stopping-time) $T$, use the shifted filtration $\mathcal G_s=\mathcal F_{T+s}$. An [martingale](martingale.md) with a bounded $L^2$ norm shifts to the [martingale](martingale.md) $M_{T+s}-M_T$; a continuous bounded adapted integrand shifts to a predictable integrand. Their [quadratic variation](#quadratic-variation) and integration intervals shift by subtracting the value at $T$. Both integrals have identical left-endpoint sums, and the [Itô isometry](#ito-isometry) passes the equality to the limit. The starting jump at $T$ is excluded.

### Conditionally Gaussian stochastic integral with an independent integrator

↑ **Parent:** [Stochastic integral](#stochastic-integral)

If the entire integrand path is independent of the integrating [Brownian motion](brownian-motion.md), conditioning on that path gives a deterministic square-integrable integrand. The [Itô isometry](#ito-isometry) and Gaussian approximation by simple integrands show that its [stochastic integral](#stochastic-integral) is conditionally centered normal with the stated variance. A strictly positive finite conditional variance implies that the unconditional distribution has no atoms.

### Stratonovich integral

↑ **Parent:** [Stochastic integral](#stochastic-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stratonovich_integral)

For continuous [semimartingales](#semimartingale), the Stratonovich integral is defined by $\int_0^tY_s\circ dX_s=\int_0^tY_s\,dX_s+\frac12[Y,X]_t$, where the first term is an [Itô integral](#ito-integral) and the correction is [quadratic covariation](#quadratic-covariation). It obeys the ordinary chain rule and is the limit in [probability](probability-theory.md#probability) of symmetric endpoint sums.

#### Stratonovich chain rule

↑ **Parent:** [Stratonovich integral](#stratonovich-integral)

For a continuous [semimartingale](#semimartingale) $X$ and a sufficiently smooth $f$, the [Stratonovich integral](#stratonovich-integral) obeys $f(X_t)-f(X_0)=\int_0^tf'(X_s)\circ dX_s$. In general $f'(X)$ is a [semimartingale](#semimartingale), so the definition must allow this larger class of integrands.

<h3 id="ito-integral">Itô integral</h3>

↑ **Parent:** [Stochastic integral](#stochastic-integral)

The Itô integral $\int_0^tH_s\,dW_s$ integrates a predictable square-integrable process against [Brownian motion](brownian-motion.md). It is defined first for predictable step processes and then completed using the [Itô isometry](#ito-isometry).

#### Gaussianity of deterministic Brownian stochastic integrals

↑ **Parent:** [Itô integral](#ito-integral)

For deterministic square-integrable $h$, approximate by step functions. Their [Itô integrals](#ito-integral) are sums of independent normal [Brownian increments](brownian-motion.md#brownian-increment). The [Itô isometry](#ito-isometry) gives convergence in $L^2$, and the variances converge to $\int h^2$; convergence of [characteristic functions](probability-theory.md#characteristic-function) proves the normal limit. Each linear combination of finitely many such integrals is another deterministic stochastic integral, so they are jointly [Gaussian](probability-theory.md#normal-distribution).

#### Gaussian coordinates of deterministic orthonormal Wiener integrands

↑ **Parent:** [Itô integral](#ito-integral)

Deterministic Itô integrals are jointly centered Gaussian by approximation from step functions and the [Itô isometry](#ito-isometry). Their covariance is the L2 inner product of their integrands. Orthonormal integrands therefore produce independent standard-normal coordinates, with independence of a countable family understood through all finite subfamilies.

#### Recovery of a continuous Brownian integrand from short increments

↑ **Parent:** [Itô integral](#ito-integral)

For a bounded continuous [adapted process](stochastic-process.md#adapted-process) $H$ and a [Brownian motion](brownian-motion.md) $B$, $\int_t^{t+h}H_s\,dB_s/(B_{t+h}-B_t)$ converges in [probability](probability-theory.md#probability) to $H_t$ as $h\downarrow0$. The [Itô isometry](#ito-isometry) makes the error numerator small relative to $\sqrt h$; the [normal distribution](probability-theory.md#normal-distribution) of the denominator controls its chance of being too close to zero.

### Associativity of stochastic integration

↑ **Parent:** [Stochastic integral](#stochastic-integral)

Whenever the integrands are admissible,

$$
\int K\,d\!\left(\int H\,dX\right)=\int KH\,dX.
$$

<h3 id="ito-isometry">Itô isometry</h3>

↑ **Parent:** [Stochastic integral](#stochastic-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Itô_isometry)

For a square-integrable predictable process $H$ and Brownian motion $W$,

$$
\mathbb E\left|\int_0^tH_s\,dW_s\right|^2
=\mathbb E\int_0^tH_s^2\,ds.
$$

More generally, for a continuous $L^2$-bounded martingale $M$,

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\mathbb E\int_0^\infty H_s^2\,d[M]_s.
$$

#### Square-integrable stochastic integrand

↑ **Parent:** [Itô isometry](#ito-isometry)

For a zero-starting L2-bounded continuous martingale $M$, the space $L^2(M)$ consists of predictable $H$ with $\mathbb E\int_0^\infty H_s^2\,d[M]_s<\infty$, identifying processes equal almost everywhere for the quadratic-variation measure. The finite-horizon version stops the integral at $T$. The [Itô integral](#ito-integral) is the isometric extension from elementary predictable integrands.

// Target: probability-and-statistics.bigb

#### Fractional-moment control of Brownian increment ratios

↑ **Parent:** [Itô isometry](#ito-isometry)

The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and [Jensen inequality](real-analysis.md#jensen-s-inequality) give the displayed estimate, with $C=(\mathbb E|N|^{-1/2})^{1/2}<\infty$. No independence between $R_\varepsilon$ and $B_\varepsilon$ is required. If $R_\varepsilon=\int_0^\varepsilon(H_s-H_0)dB_s$ for a bounded continuous adapted process, the [Itô isometry](#ito-isometry) and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) make the right side tend to zero. Time shifting proves recovery of $H_t$ in probability from the ratio of a short stochastic integral to its Brownian increment.

#### Conditional bracket isometry for stopped martingale increments

↑ **Parent:** [Itô isometry](#ito-isometry)

For an [L2-bounded continuous martingale](martingale.md#l2-bounded-continuous-martingale) and ordered possibly infinite [stopping times](martingale.md#stopping-time) $\sigma\leq\tau$, interpret the terminal stopped value as $M_\infty$. The [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) bounds the expected squared path supremum. Localization of $M^2-[M]$ then gives $\mathbb E[M]_\infty<\infty$, so this square-minus-bracket local martingale has integrable supremum and is uniformly integrable. Apply the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale) to it and to $M$. Expanding $(M_\tau-M_\sigma)^2$ makes the cross term vanish conditionally, proving the identity. Bounded $\mathcal F_\sigma$-measurable factors can be multiplied into either side.

#### Quadratic-variation measure

↑ **Parent:** [Itô isometry](#ito-isometry)

For a [L2-bounded continuous martingale](martingale.md#l2-bounded-continuous-martingale) $M$, define a finite [measure](measure-theory.md#measure) on the [predictable sigma-algebra](martingale.md#predictable-sigma-algebra) by $\nu_M(A)=\mathbb E\int_0^\infty\mathbf1_A\,d[M]$. Its total mass is $\mathbb E[M]_\infty=\mathbb E M_\infty^2-\mathbb E M_0^2$. The [Lebesgue space](measure-theory.md#lp-space) $L^2(\nu_M)$ identifies [predictable processes](martingale.md#predictable-process) that agree $\nu_M$-almost everywhere. Integration against $M$ is an isometry from this space into [L2-bounded continuous martingales](martingale.md#l2-bounded-continuous-martingale) starting at zero by the [Itô isometry](#ito-isometry). This gives the correct integrand space even when the [quadratic variation](#quadratic-variation) is random or is not absolutely continuous in time.

### Quadratic variation of a stochastic integral

↑ **Parent:** [Stochastic integral](#stochastic-integral)

For a continuous local martingale $M$,

$$
\left[\int H\,dM\right]_t=\int_0^tH_s^2\,d[M]_s.
$$

#### Localized isometry proof of stochastic-integral quadratic variation

↑ **Parent:** [Quadratic variation of a stochastic integral](#quadratic-variation-of-a-stochastic-integral)

For a [continuous local martingale](martingale.md#continuous-local-martingale) and a locally bounded [predictable process](martingale.md#predictable-process), stop at a localizing time, an integrand bound, a time bound, and level bounds for the centered martingale and its bracket. The stopped martingale is bounded and its bracket and integrand are deterministically bounded. The [Itô isometry](#ito-isometry), applied to $\mathbf1_F\mathbf1_{(s,t]}H$ for $F\in\mathcal F_s$, gives the conditional second-moment identity. Expanding the square proves that $(H\cdot M)^2-H^2\cdot[M]$ is a martingale after stopping. [Uniqueness of an increasing square compensator](#uniqueness-of-an-increasing-square-compensator) identifies the bracket, and increasing stopping times patch the identities into the displayed local result.

<h2 id="ito-s-lemma">Itô's lemma</h2>

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Itô's_lemma)

For an Itô process $dX_t=b_t\,dt+\sigma_t\,dB_t$ and a twice differentiable function $f$,

$$
df(X_t)=f'(X_t)\,dX_t+\frac12f''(X_t)\sigma_t^2\,dt.
$$

The second-order term reflects the nonzero quadratic variation of [Brownian motion](brownian-motion.md).

<h3 id="polynomial-ito-formula-from-integration-by-parts">Polynomial Itô formula from integration by parts</h3>

↑ **Parent:** [Itô's lemma](#ito-s-lemma)

The one-dimensional Itô formula for polynomials follows by induction on powers using the stochastic product rule. If it holds for $X^k$, its martingale part gives $[X^k,X]=kX^{k-1}\cdot[X]$. The product rule for $X^kX$ then yields the coefficient $k(k+1)/2$ of the bracket term for $X^{k+1}$.

// Target: probability-and-statistics.bigb

<h3 id="ito-formula-for-semimartingales-with-jumps">Itô formula for semimartingales with jumps</h3>

↑ **Parent:** [Itô's lemma](#ito-s-lemma)

For a [semimartingale](#semimartingale) with [càdlàg](calculus.md#cadlag) paths $X$ and $f\in C^2$, the [Itô formula](#ito-s-lemma) uses the left-limit gradient in $\int f'(X_{s-})dX_s$, the continuous [quadratic variation](#quadratic-variation) in its second-order integral, and the jump correction $\sum_{s\leq t}[f(X_s)-f(X_{s-})-f'(X_{s-})\Delta X_s]$. In several dimensions use the corresponding gradient, Hessian and continuous bracket matrix. The correction is the part of each jump not captured by first-order linearization.

<h3 id="ito-product-rule">Itô product rule</h3>

↑ **Parent:** [Itô's lemma](#ito-s-lemma)

For continuous semimartingales,

$$
d(X_tY_t)=X_t\,dY_t+Y_t\,dX_t+d[X,Y]_t.
$$

It is the stochastic counterpart of the ordinary [product rule](calculus.md#product-rule); the [quadratic covariation](#quadratic-covariation) supplies the additional second-order term.

<h3 id="tanaka-s-formula">Tanaka's formula</h3>

↑ **Parent:** [Itô's lemma](#ito-s-lemma)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tanaka's_formula)

For a continuous semimartingale $X$,

$$
|X_t|=|X_0|+\int_0^t\operatorname{sgn}(X_s)\,dX_s+L_t^0(X),
$$

where $L^0(X)$ is the [local time of a semimartingale](#local-time-of-a-semimartingale) at zero.

#### Smooth convex approximation proof of the Tanaka formula

↑ **Parent:** [Tanaka's formula](#tanaka-s-formula)

Choose $f_n(0)=0$ and $f_n'(x)=\phi(nx)$, where $\phi$ is continuously differentiable, nondecreasing, equal to $-1$ on $(-\infty,0]$ and $1$ on $[1,\infty)$. Then $f_n''\geq0$ and $0\leq|x|-f_n(x)\leq2/n$. For $X=M+A$ with continuous adapted finite-variation $A$, the [Itô isometry](#ito-isometry) and [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) give local uniform convergence in probability of the martingale integrals. Dominated convergence against the total-variation measure gives pathwise uniform convergence of the drift integrals. The nondecreasing corrections $\frac12\int f_n''(X)d[M]$ therefore converge locally uniformly in probability to $|X|-\int\operatorname{sgn}_-(X)dX$. A subsequence on one probability-one event shows that the limit is continuous and nondecreasing. Localization removes the deterministic bounds used in the argument.

#### Discrete Tanaka formula

↑ **Parent:** [Tanaka's formula](#tanaka-s-formula)

For integer paths with increments in $\{-1,0,1\}$, the [positive part](function.md#positive-part-of-a-real-valued-function) obeys a telescoping identity with slope $f(x)=\mathbf1_{\{x>0\}}+\frac12\mathbf1_{\{x=0\}}$ and a correction $\frac12\mathbf1_{\{S_{t-1}=K\}}(\Delta S_t)^2$ at the kink. For a [martingale](martingale.md), the slope term is a [martingale transform](martingale.md#martingale-transform).

## Local time (mathematics)

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_time_(mathematics))

Local time records how much a [stochastic process](stochastic-process.md) visits a level. Its normalization depends on the process: when the [state space](dynamical-systems.md#state-space) is a [discrete space](topology.md#discrete-space), it is occupation time at a state, while [local time of a semimartingale](#local-time-of-a-semimartingale) is an occupation density weighted by [quadratic variation](#quadratic-variation). [Brownian local time](#brownian-local-time) is a special case.

### Local time of a semimartingale

↑ **Parent:** [Local time (mathematics)](#local-time-mathematics)

Local time measures how intensely a semimartingale visits a level. For a continuous semimartingale it appears as the increasing correction term in the [Tanaka formula](#tanaka-s-formula).

#### Brownian local time

↑ **Parent:** [Local time of a semimartingale](#local-time-of-a-semimartingale)

For [Brownian motion](brownian-motion.md) with generator $\tfrac12\Delta$, its local time is the occupation density normalized by $\int_0^t h(B_s)ds=\int_{\mathbb R}h(a)L_t^a\,da$ for nonnegative Borel $h$. In the [Tanaka formula](#tanaka-s-formula) it satisfies $|B_t-a|=|B_0-a|+\int_0^t\operatorname{sgn}(B_s-a)dB_s+L_t^a$. The symmetric-window approximation is $(2\varepsilon)^{-1}\int_0^t\mathbf1_{\{|B_s-a|<\varepsilon\}}ds$. The factor two is essential. [Occupation approximations for Brownian local time](#occupation-approximations-for-brownian-local-time) give a direct derivation at level zero from smooth approximations and maximal martingale estimates.

##### Occupation approximations for Brownian local time

↑ **Parent:** [Brownian local time](#brownian-local-time)

For [Brownian motion](brownian-motion.md) started at zero, let $f_n$ equal $|x|$ outside $(-1/n,1/n)$ and $nx^2/2+1/(2n)$ inside. Its derivative is the clipped sign function $g_n(x)=\max\{-1,\min\{1,nx\}\}$. The [Itô integral](#ito-integral) $M_t^{(n)}=\int_0^t g_n(B_s)dB_s$ converges uniformly on bounded time intervals in $L^2$ to a [continuous martingale](martingale.md#continuous-martingale) $M$, by the [Itô isometry](#ito-isometry) and [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality): the squared maximal error is at most $8\sqrt{2T/\pi}/n$. The [Itô formula](#ito-s-lemma) gives $\frac n2\int_0^t\mathbf1_{\{|B_s|<1/n\}}ds=f_n(B_t)-f_n(0)-M_t^{(n)}$. Along $n=k^2$, the maximal errors are summable, so [First Borel-Cantelli lemma](probability-theory.md#borel-cantelli-first-lemma) gives uniform almost-sure convergence. The [ratio-one interpolation for shrinking-window occupation integrals](#ratio-one-interpolation-for-shrinking-window-occupation-integrals) extends it to every integer $n$. The limit is $|B_t|-M_t=L_t^0$, the [local time of a semimartingale](#local-time-of-a-semimartingale) in the [Tanaka formula](#tanaka-s-formula) convention. The unnormalized factor $n$ gives twice this limit.

###### Ratio-one interpolation for shrinking-window occupation integrals

↑ **Parent:** [Occupation approximations for Brownian local time](#occupation-approximations-for-brownian-local-time)

For any measurable real path $x$, put $A_n(t)=n\int_0^t\mathbf1_{\{|x(s)|<1/n\}}ds$. If $n_k\le n\le n_{k+1}$, nested windows give $(n/n_{k+1})A_{n_{k+1}}(t)\le A_n(t)\le(n/n_k)A_{n_k}(t)$. Consequently, when $n_{k+1}/n_k\to1$ and the subsequence $A_{n_k}$ converges uniformly on bounded time intervals, the full sequence does also, to the same limit. This deterministic interpolation turns summable-subsequence [First Borel-Cantelli lemma](probability-theory.md#borel-cantelli-first-lemma) estimates into almost-sure convergence without incorrectly claiming that convergence in $L^2$ alone implies full-sequence almost-sure convergence.

#### Right local time of a continuous semimartingale

↑ **Parent:** [Local time of a semimartingale](#local-time-of-a-semimartingale)

This normalization uses the left derivative of absolute value in the [Tanaka formula](#tanaka-s-formula). Its increasing correction is the right-sided spatial local time; equivalently $(X_t-a)^+=(X_0-a)^++\int_0^t\mathbf1_{\{X_s>a\}}dX_s+\tfrac12L_t^{a,+}$. It need not equal symmetric local time for a general continuous semimartingale with finite-variation mass at the level. In the [smooth convex approximation proof of the Tanaka formula](#smooth-convex-approximation-proof-of-the-tanaka-formula), the second derivatives are supported on the positive side of the level, agreeing with this convention.

## Stochastic differential equation

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stochastic_differential_equation)

A stochastic differential equation specifies infinitesimal drift and random diffusion through a stochastic integral equation.

### Bounded diffusion coefficient gives square martingales

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

For a zero-starting solution with $|\sigma|\le C$, the [Itô isometry](#ito-isometry) gives $\mathbb EX_t^2\le C^2t$, so $X$ is a true [martingale](martingale.md) on every finite horizon. The [Itô formula](#ito-s-lemma) represents the displayed process as $2\int_0^tX_s\sigma(X_s)dB_s$, whose expected squared integrand integral is at most $2C^4t^2$. Thus it too is a true square-integrable [martingale](martingale.md). No [continuity](calculus.md#continuous-function) or Lipschitz condition on the coefficient is needed once a solution is given.

### Bernoulli stochastic differential equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

On the positive half-line, divide by the [stochastic exponential](#doleans-dade-exponential) $F_t=e^{\alpha B_t-\alpha^2t/2}$. The [Itô product rule](#ito-product-rule) reduces the equation to the random [Bernoulli differential equation](differential-equation.md#bernoulli-differential-equation) $d(X/F)/dt=F^{\delta-1}(X/F)^\delta$. For $\delta\ne1$ this gives $X_t=F_t[x_0^{1-\delta}+(1-\delta)\int_0^tF_s^{\delta-1}ds]^{1/(1-\delta)}$, until the bracket vanishes; for $\delta=1$, $X_t=x_0F_te^t$.

#### Explosion threshold for a Bernoulli stochastic differential equation

↑ **Parent:** [Bernoulli stochastic differential equation](#bernoulli-stochastic-differential-equation)

The explicit [Bernoulli stochastic differential equation](#bernoulli-stochastic-differential-equation) solution remains positive and finite on every finite interval when $0<\delta\le1$. For $\delta>1$ it diverges when the displayed integral reaches its threshold. At $\alpha=0$ this occurs deterministically. At $\alpha\ne0$, Brownian motion has positive probability of making the integral exceed any threshold on a fixed interval, so global existence is not almost sure. The distinction between positive explosion probability and certain explosion matters: the negative linear drift of $\log F$ makes its total positive-power exponential integral finite almost surely when $\alpha\ne0$.

### Brownian rotation in the plane

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

The SDE $dX=-Y\,dB-X\,dt/2$, $dY=X\,dB-Y\,dt/2$ has the unique strong solution obtained by rotating $(X_0,Y_0)$ through angle $B_t$. Its coefficients are globally Lipschitz with linear growth, and $X_t^2+Y_t^2=X_0^2+Y_0^2$. The origin is absorbing and every other solution remains on its initial circle.

### Stroock-Varadhan support theorem

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

For smooth bounded vector fields, the support of a Stratonovich diffusion in uniform path topology is the closure of solutions to the controlled [ordinary differential equation](differential-equation.md#ordinary-differential-equation) with the same drift and controls in the [Cameron-Martin space of Wiener measure](brownian-motion.md#cameron-martin-space-of-wiener-measure). The [support of enhanced Brownian motion](analysis.md#support-of-enhanced-brownian-motion) and the [universal limit theorem](analysis.md#universal-limit-theorem) prove this through continuity of the enhanced solution map. For an equation written in Itô form, the controlled drift is the Itô drift minus $\tfrac12\sum_iDV_iV_i$.

### Square-root branching diffusion

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A nonnegative diffusion with zero absorbing, often called the critical Feller branching diffusion; other conventions multiply the coefficient by a fixed positive constant. Its diffusion coefficient is not Lipschitz at zero. Independent copies add according to the [addition law for square-root branching diffusions](#addition-law-for-square-root-branching-diffusions), and a [cutoff construction of an absorbed square-root diffusion](#cutoff-construction-of-an-absorbed-square-root-diffusion) gives strong existence without applying the global Lipschitz theorem to the original coefficient.

#### Cutoff construction of an absorbed square-root diffusion

↑ **Parent:** [Square-root branching diffusion](#square-root-branching-diffusion)

Replace the square-root coefficient near zero by smooth globally Lipschitz cutoffs that vanish below half the cutoff level. With a common Brownian driver, local [pathwise uniqueness](#pathwise-uniqueness) makes the solutions agree until the larger cutoff level. The exit times increase as the levels decrease. The compatible integrands $\mathbf1_{\{s\leq T_n\}}\sqrt{Z_s}$ have increasing squares and expected time-integrals at most $zt$ by the [nonnegative local martingale](martingale.md#nonnegative-local-martingale) bound. Their limit is square-integrable on every finite horizon. The [Itô isometry](#ito-isometry) gives a continuous global limiting stochastic integral; at a finite limiting exit time its value is zero, and it remains absorbed afterward.

#### Addition law for square-root branching diffusions

↑ **Parent:** [Square-root branching diffusion](#square-root-branching-diffusion)

For solutions with independent Brownian drivers in a common filtration, combine the drivers with weights $\sqrt{Z/(Z+Z')}$ and $\sqrt{Z'/(Z+Z')}$ where the sum is positive. At zero use one original driver. The resulting continuous [local martingale](martingale.md#local-martingale) has bracket $t$ and is [Brownian motion](brownian-motion.md) by the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion). Multiplying its differential by $\sqrt{Z+Z'}$ gives exactly the sum of the original stochastic differentials.

### Strict order preservation for scalar Lipschitz diffusions

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

Two scalar SDEs driven by the same [Brownian motion](brownian-motion.md), with the same globally Lipschitz diffusion coefficient and ordered globally Lipschitz drifts, preserve a strict initial order at every finite time. If $Z=Y-X$ starts positive, apply a reciprocal barrier to the first hit of zero. A Gronwall bound on $(Z+\epsilon)^{-1}$ makes the hitting probability at most $\epsilon e^{(L+K^2)t}/(Z_0+\epsilon)$, which tends to zero. Common noise and the Lipschitz bound on the diffusion difference are essential to this argument.

#### Reciprocal barrier proof of scalar diffusion comparison

↑ **Parent:** [Strict order preservation for scalar Lipschitz diffusions](#strict-order-preservation-for-scalar-lipschitz-diffusions)

Before the difference $Z$ hits zero, its diffusion coefficient has magnitude at most $KZ$ and its drift is at least $-LZ$. Itô's formula bounds the drift of $f_\epsilon(Z)$ by $(L+K^2)f_\epsilon(Z)$. Its stochastic integrand is bounded by $K/(4\epsilon)$, making [expectation](probability-theory.md#expected-value) legitimate on finite horizons. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) and the value $f_\epsilon(0)=1/\epsilon$ then exclude finite-time contact from a strictly positive starting difference.

### Global existence theorem for stochastic differential equations with Lipschitz coefficients

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

Globally Lipschitz drift and diffusion coefficients have linear growth and give a nonexplosive [strong stochastic solution](#strong-solution-of-a-stochastic-differential-equation) for a prescribed initial state and [Brownian motion](brownian-motion.md). The solution satisfies [pathwise uniqueness](#pathwise-uniqueness). Local versions apply after stopping inside compact regions.

### Tanaka equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tanaka_equation)

With $s(x)=1$ for $x\geq0$ and $s(x)=-1$ for $x<0$, the equation starting at zero has [uniqueness in law](#uniqueness-in-law) but not [pathwise uniqueness](#pathwise-uniqueness). For existence, take a [Brownian motion](brownian-motion.md) $W$ and set $B=\int s(W)dW$; the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion) and [associativity of stochastic integration](#associativity-of-stochastic-integration) give $W=\int s(W)dB$. Every solution has [quadratic variation](#quadratic-variation) $t$ and hence the [Brownian motion](brownian-motion.md) law. Both $W$ and $-W$ are solutions driven by the same $B$, since the time spent at zero is zero and $s(-W)=-s(W)$ away from zero. Using $s(0)=0$ instead would allow the constant solution and invalidate this uniqueness-in-law example.

<h3 id="ito-diffusion">Itô diffusion</h3>

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Itô_diffusion)

An Itô diffusion solves a stochastic differential equation $dX_t=b(X_t)dt+\sigma(X_t)dB_t$ driven by [Brownian motion](brownian-motion.md).

#### Exponential small-noise concentration for a Lipschitz diffusion

↑ **Parent:** [Itô diffusion](#ito-diffusion)

Couple $dX_t^\varepsilon=b(X_t^\varepsilon)dt+\varepsilon dW_t$ with $\dot x_t=b(x_t)$ and the same initial value. If $b$ has Lipschitz constant $L$, the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) gives $\sup_{s\le t}|X_s^\varepsilon-x_s|\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|$. Applying the [Gaussian maximal bound for Brownian motion](brownian-motion.md#gaussian-maximal-bound-for-brownian-motion) coordinatewise in dimension $d$ bounds the deviation [probability](probability-theory.md#probability) by $2d\exp[-\delta^2e^{-2Lt}/(2dt\varepsilon^2)]$ for $t>0$. Matching initial values is essential.

#### Generator of an SDE diffusion

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The Itô formula identifies the operator of an SDE with drift $b$ and noise vector fields $\sigma_k$ as the displayed second-order operator. With bounded measurable coefficients, every solution satisfies the true martingale identity for $C_b^2$ test functions, hence is an [L-diffusion](#diffusion-martingale-problem) in the martingale-problem sense.

// Target: probability-and-statistics.bigb

<h4 id="initial-mean-and-variance-derivatives-of-an-ito-diffusion">Initial mean and variance derivatives of an Itô diffusion</h4>

↑ **Parent:** [Itô diffusion](#ito-diffusion)

For deterministic $X_0=x$ and bounded continuous drift and volatility, the initial right derivative of the mean is $b(x)$ and that of the variance is $\sigma(x)^2$. The stochastic integral has mean zero and second moment $\int_0^t\mathbb E\sigma(X_s)^2ds$; the bounded drift contributes only higher-order terms to the variance.

// Target: probability-and-statistics.bigb

<h4 id="wright-fisher-diffusion">Wright–Fisher diffusion</h4>

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The neutral one-dimensional Wright–Fisher diffusion records a proportion in $[0,1]$, with absorbing endpoints, zero drift and generator $Lf(x)=x(1-x)f''(x)/2$. Its conditional variance rate is largest near one-half and vanishes at fixation. Mutation or selection variants add drift and must be specified separately.

<h5 id="wright-fisher-binomial-sampling-chain">Wright–Fisher binomial sampling chain</h5>

↑ **Parent:** [Wright–Fisher diffusion](#wright-fisher-diffusion)

An urn with $j$ red balls among $n$ is sampled independently $n$ times with replacement, and the next generation's red count is the number of red draws. Its proportion is a bounded discrete-time [martingale](martingale.md). Accelerating generation time by $n$ gives a [Wright–Fisher diffusion](#wright-fisher-diffusion) limit: the one-step variance of the proportion is $x(1-x)/n$, and the higher moments make Taylor remainders negligible.

#### Diffusion with hyperbolic tangent drift

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The scalar [stochastic differential equation](#stochastic-differential-equation) $dX_t=\tanh X_t\,dt+dW_t$ has a pathwise unique global strong solution, since its coefficients are globally Lipschitz. The positive martingale $e^{t/2}/\cosh X_t$ gives a [Girsanov theorem](#girsanov-theorem) change of measure under which $X_t-X_0$ is [Brownian motion](brownian-motion.md). For $X_0=x$, its transition density is

$$
p_t(x,z)=e^{-t/2}\frac{\cosh z}{\cosh x}(2\pi t)^{-1/2}e^{-(z-x)^2/(2t)}.
$$

This is a [Doob h-transform](markov-process.md#doob-h-transform) with $h=\cosh$, and a mixture of $N(x+t,t)$ and $N(x-t,t)$ with weights $e^x/(2\cosh x)$ and $e^{-x}/(2\cosh x)$.

#### Diffusion amplitude

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The coefficient $\sigma$ multiplying the [Brownian motion](brownian-motion.md) increment in a scalar [stochastic differential equation](#stochastic-differential-equation). The local variance rate is $\sigma^2$, and the second-order coefficient in the backward [Kolmogorov backward equation](#kolmogorov-backward-equation) is $\sigma^2/2$. This distinguishes the amplitude from the physical [diffusion coefficient](brownian-motion.md#diffusion-coefficient) convention $D=\sigma^2/2$.

#### Diffusion occupation time

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The time spent by a [Itô diffusion](#ito-diffusion) in a measurable set $I$ up to time $T$ is $A_T(I)=\int_0^T\mathbf1_I(X_t)\,dt$. Under [stationarity](time-series.md#stationary-process) its [expected value](probability-theory.md#expected-value) is $T\mu(I)$, where $\mu$ is the [Invariant distribution of an Itô diffusion](#invariant-distribution-of-an-ito-diffusion). Occupation times form the denominator of a local [drift estimator](#drift-estimator).

#### Power diffusion

↑ **Parent:** [Itô diffusion](#ito-diffusion)

A power diffusion has a power of its positive state as noise coefficient. Here the normalized zero-drift family is considered on $U=(0,\infty)$ with $X_0>0$. Its coefficients are locally [Lipschitz continuous](real-analysis.md#lipschitz-continuity) on that domain, so a [maximal local solution of a stochastic differential equation](#maximal-local-solution-of-a-stochastic-differential-equation) is pathwise unique before its lifetime. The [Lamperti transform](#lamperti-transform-diffusion) reduces its noise coefficient to a constant; the case $\alpha=1$ is [geometric Brownian motion](#geometric-brownian-motion). This normalized family is part of the constant-elasticity-of-variance models, but is not the whole model with arbitrary drift and scale.

##### Finite lifetime threshold for a power diffusion

↑ **Parent:** [Power diffusion](#power-diffusion)

For the positive-domain [power diffusion](#power-diffusion) with $0<\alpha\leq1$, assuming the lifetime is the limit of the hitting times of $1/n$, it is finite [almost surely](convergence-of-random-variables.md#almost-sure-convergence) exactly when $\alpha<1$. For $\alpha<1$, the [Itô formula](#ito-s-lemma) gives

$$
d(X^{1-\alpha})=(1-\alpha)dB-\frac{\alpha(1-\alpha)}{2X^{1-\alpha}}dt.
$$

The negative drift bounds this positive process above by $X_0^{1-\alpha}+(1-\alpha)B$, whose first hit of zero is finite by [recurrence of one-dimensional Brownian motion](brownian-motion.md#recurrence-of-one-dimensional-brownian-motion). The lifetime must precede that hit. At $\alpha=1$, $X_t=X_0e^{B_t-t/2}$ is positive and finite on every compact time interval, so the lifetime is infinite. Approaching zero only as $t\to\infty$ is not a finite boundary lifetime.

#### Lamperti transform (diffusion)

↑ **Parent:** [Itô diffusion](#ito-diffusion)

On an interval where $\sigma>0$ is continuously differentiable, define $F(x)=\int^x\sigma(y)^{-1}dy$. The [Itô formula](#ito-s-lemma) transforms $dX=b(X)dt+\sigma(X)dB$ into

$$
dF(X_t)=dB_t+\left(\frac{b(X_t)}{\sigma(X_t)}-\frac12\sigma'(X_t)\right)dt.
$$

The transformed [Itô diffusion](#ito-diffusion) has constant noise coefficient. For a [power diffusion](#power-diffusion) $\sigma(x)=x^\alpha$, $F(x)=x^{1-\alpha}/(1-\alpha)$ when $\alpha\ne1$, and $F(x)=\log x$ when $\alpha=1$. This simplifies comparison with [Brownian motion](brownian-motion.md) and exposes the boundary drift.

#### Drift coefficient

↑ **Parent:** [Itô diffusion](#ito-diffusion)

The drift coefficient is the coefficient $b$ of $dt$ in a [stochastic differential equation](#stochastic-differential-equation). It describes the local deterministic tendency of the process.

##### Drift estimator

↑ **Parent:** [Drift coefficient](#drift-coefficient)

From a continuously observed [Itô diffusion](#ito-diffusion), a local drift estimator divides $\int_0^T\mathbf1_{[x-h,x+h]}(X_t)\,dX_t$ by the corresponding [diffusion occupation time](#diffusion-occupation-time). Its error separates into a local [Hölder continuity](sobolev-space.md#holder-condition) bias and an [Itô integral](#ito-integral) divided by occupation time. The [Itô isometry](#ito-isometry) gives a pointwise noise scale $(Th)^{-1/2}$ when the invariant density is locally positive.

#### Geometric Brownian motion

↑ **Parent:** [Itô diffusion](#ito-diffusion)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_Brownian_motion)

Geometric Brownian motion has the explicit strong solution

$$
X_t=X_0\exp\left(\sigma B_t+
\left(\mu-\frac12\sigma^2\right)t\right).
$$

##### Killed geometric Brownian heat kernel

↑ **Parent:** [Geometric Brownian motion](#geometric-brownian-motion)

The [differential operator](analysis.md#differential-operator) $L=\tfrac12x^2\partial_{xx}+\tfrac12x\partial_x-\tfrac12$ has solution operator $P_tg(x)=e^{-t/2}\mathbb E[g(xe^{B_t})]$. For $x\ne0$ its [integral kernel](functional-analysis.md#integral-kernel) with respect to [Lebesgue measure](measure-theory.md#lebesgue-measure) is $p(t,x,y)=e^{-t/2}(|y|\sqrt{2\pi t})^{-1}\exp[-\log^2(|y/x|)/(2t)]$ when $xy>0$, and zero otherwise. For $x=0$ the kernel is the [measure](measure-theory.md#measure) $e^{-t/2}\delta_0$, not a density. The [Itô formula](#ito-s-lemma) applied to $e^{-s/2}u(t-s,X_s)$ proves this [Feynman-Kac formula](#feynman-kac-formula).

<h3 id="invariant-distribution-of-an-ito-diffusion">Invariant distribution of an Itô diffusion</h3>

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

For $D=\sigma\sigma^T/2$, a density $\pi$ is invariant for $dX=b\,dt+\sigma\,dB$ exactly when the stationary Fokker-Planck equation $\nabla\cdot(b\pi-\nabla\cdot(D\pi))=0$ holds with suitable boundary decay.

### Underdamped Langevin dynamics

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Underdamped_Langevin_dynamics)

Underdamped Langevin dynamics augments position by momentum and combines Hamiltonian transport with friction and matching Gaussian noise. For potential $U$, momentum variance $\eta$, and friction $\gamma$, its invariant density is proportional to $\exp[-U(x)-|p|^2/(2\eta)]$.

#### Inertial Brownian displacement with zero initial velocity

↑ **Parent:** [Underdamped Langevin dynamics](#underdamped-langevin-dynamics)

A free particle following [Langevin dynamics](stochastic-process.md#langevin-dynamics) initialized at zero position and velocity has relaxation time $\tau=m/\zeta$ and thermal [diffusivity](brownian-motion.md#diffusion-coefficient) $D=k_BT/\zeta$. Its position is the convolution of the random force with $[1-e^{-t/\tau}]/\zeta$. The [fluctuation-dissipation relation for a Langevin particle](thermodynamics.md#fluctuation-dissipation-relation-for-a-langevin-particle) gives force covariance amplitude $2\zeta k_BT$, and integrating the squared kernel yields the displayed [variance](variance.md). At short times it grows as $2Dt^3/(3\tau^2)$ because the initial velocity is cold; at long times it grows as $2Dt$. A Maxwellian initial velocity produces a different short-time transient.

### Overdamped Langevin dynamics

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

Neglecting inertia in [Langevin dynamics](stochastic-process.md#langevin-dynamics) gives the overdamped limit.

For potential $F$ and mobility $\mathcal M$, overdamped Langevin dynamics is

$$
dX_t=-\mathcal M\nabla F(X_t)dt+\sqrt{2k_BT\mathcal M}\,dW_t.
$$

The matching noise amplitude is the fluctuation-dissipation relation that makes the Boltzmann density proportional to $e^{-F/(k_BT)}$ invariant.

#### Isothermal diffusion with position-dependent drag

↑ **Parent:** [Overdamped Langevin dynamics](#overdamped-langevin-dynamics)

With local thermal noise matched to spatially varying drag, the overdamped probability density obeys the displayed [diffusion equation](diffusion-equation.md). Its equivalent [Itô diffusion](#ito-diffusion) is $dX=D'(X)dt+\sqrt{2D(X)}\,dW$, since the two terms in the [Fokker-Planck equation](probability-theory.md#fokker-planck-equation) combine to $\partial_x(DP_x)$. Thus $d\langle X\rangle/dt=\langle D'(X)\rangle$, even with no applied force. The [drift](#drift-coefficient) points toward greater [diffusivity](brownian-motion.md#diffusion-coefficient), but a uniform density has zero flux: the drift is balanced by the spatial variation of the noise. Holding the force-noise amplitude fixed instead would not produce this isothermal Fickian equation.

#### Tilted washboard potential

↑ **Parent:** [Overdamped Langevin dynamics](#overdamped-langevin-dynamics)

A periodic corrugation plus a uniform tilt. For the [Adler phase equation](dynamical-systems.md#adler-phase-equation), $V(\theta)=-\omega\theta-\epsilon\cos\theta$ gives force $-V'=\omega-\epsilon\sin\theta$ and $V(\theta+2\pi)-V(\theta)=-2\pi\omega$. It has wells when $|\omega|<\epsilon$ and no extrema when $|\omega|>\epsilon$. It is a potential on the unwrapped phase, not a single-valued periodic potential on the circle.

#### Kramers escape rate

↑ **Parent:** [Overdamped Langevin dynamics](#overdamped-langevin-dynamics)

For weak noise $D$ in a one-dimensional potential $\phi$, escape from a minimum $m$ across a neighboring maximum $M$ occurs at leading rate

$$
k=\frac{\sqrt{|\phi''(m)\phi''(M)|}}{2\pi}
e^{-[\phi(M)-\phi(m)]/D}.
$$

### Euler-Maruyama method

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler–Maruyama_method)

For $dX_t=a(X_t)dt+\sigma(X_t)dW_t$, the Euler-Maruyama method advances

$$
X_{n+1}=X_n+a(X_n)\Delta t+\sigma(X_n)\Delta W_n,
$$

where $\Delta W_n\sim N(0,\Delta t)$.

#### Milstein method

↑ **Parent:** [Euler-Maruyama method](#euler-maruyama-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Milstein_method)

For a scalar [stochastic differential equation](#stochastic-differential-equation), the Milstein method adds the quadratic-variation correction

$$
X_{n+1}=X_n+a(X_n)\Delta t+\sigma(X_n)\Delta W_n
+\frac12\sigma(X_n)\sigma'(X_n)
\left((\Delta W_n)^2-\Delta t\right).
$$

Under standard smoothness assumptions it has [strong order of convergence](#strong-convergence-of-a-stochastic-numerical-method) one and [weak order of convergence](#weak-convergence-of-a-stochastic-numerical-method) one.

### Strong convergence of a stochastic numerical method

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A stochastic numerical method has strong order $p$ when, under a coupling using the same driving noise, its expected pathwise error is $O(\!\Delta t^p)$. Strong convergence measures approximation of individual sample paths.

### Weak convergence of a stochastic numerical method

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A stochastic numerical method has weak order $p$ when its error in expected sufficiently smooth observables is $O(\!\Delta t^p)$. Weak convergence measures approximation of distributions rather than individual sample paths.

### Markov diffusion

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A Markov diffusion is a continuous-path [Markov process](markov-process.md) whose local evolution is described by a drift vector and diffusion matrix. For sufficiently regular coefficients, its [infinitesimal generator](stochastic-process.md#infinitesimal-generator-stochastic-processes) is a second-order differential operator and its conditional expectations satisfy a [Kolmogorov backward equation](#kolmogorov-backward-equation).

#### Driftless square-root diffusion

↑ **Parent:** [Markov diffusion](#markov-diffusion)

A driftless square-root [diffusion process](#markov-diffusion) is the nonnegative solution of $dX_t=\sqrt{X_t}\,dW_t$, with zero an absorbing boundary. For elapsed time $h>0$, starting from $x\geq0$, its [Laplace transform](analysis.md#laplace-transform) is

$$
\mathbb E_x[e^{-uX_h}]=\exp\left(-\frac{xu}{1+uh/2}\right),\qquad u\geq0.
$$

To prove this, fix the final time $h$ and set $F(t,x)=\exp[-xu/(1+u(h-t)/2)]$. Differentiation gives $F_t+\tfrac12xF_{xx}=0$, while $F(h,x)=e^{-ux}$. By [Itô formula](#ito-s-lemma), $F(t,X_t)$ is a [local martingale](martingale.md#local-martingale); it takes values in $[0,1]$, so localization and bounded convergence make it a true [martingale](martingale.md). Taking expectations at the two endpoints proves the formula. The [Markov property](markov-process.md#markov-property) gives the same formula conditionally at any starting time.

##### Compound Poisson transition law of a driftless square-root diffusion

↑ **Parent:** [Driftless square-root diffusion](#driftless-square-root-diffusion)

The elapsed-time $h>0$ transition distribution of a [driftless square-root diffusion](#driftless-square-root-diffusion) starting at $x$ is the [compound Poisson distribution](actuarial-statistics.md#compound-poisson-distribution)

$$
X_h\ \stackrel{d}{=}\ \sum_{j=1}^{N}Y_j,\qquad N\sim\operatorname{Poisson}(2x/h),\quad Y_j\sim\operatorname{Exp}(2/h),
$$

where all variables on the right are independent and the empty sum is zero. Here the [exponential distribution](continuous-probability-distribution.md#exponential-distribution) parameter is its rate. The [Laplace transform](analysis.md#laplace-transform) of this sum is

$$
\exp\left[\frac{2x}{h}\left(\frac{2/h}{2/h+u}-1\right)\right]=\exp\left(-\frac{xu}{1+uh/2}\right),
$$

which is the [Laplace transform](analysis.md#laplace-transform) of the [driftless square-root diffusion](#driftless-square-root-diffusion); uniqueness of the [Laplace transform](analysis.md#laplace-transform) proves the distributional identity. In particular, for $0\leq v<2/h$, the [exponential moment](probability-theory.md#exponential-moment) is

$$
\mathbb E_x[e^{vX_h}]=\exp\left(\frac{xv}{1-vh/2}\right).
$$

For $x>0$ this [exponential moment](probability-theory.md#exponential-moment) is infinite when $v\geq2/h$, since the event $N=1$ has positive probability and one exponential jump already has an infinite moment there. At $x=0$ the process remains zero and every such moment is one.

#### Diffusion limit

↑ **Parent:** [Markov diffusion](#markov-diffusion)

A diffusion limit rescales a sequence of stochastic processes so that its limit is a [diffusion process](#markov-diffusion). For suitably rescaled independent small jumps, the first two jump moments determine the limiting drift and diffusion coefficient. [Brownian motion](brownian-motion.md) arises when the limiting drift is zero and the variance grows linearly in time.

#### Speed density of a one-dimensional diffusion

↑ **Parent:** [Markov diffusion](#markov-diffusion)

For a diffusion with generator $(\sigma^2/2)\partial_{xx}+b\partial_x$ and increasing [scale function of a one-dimensional diffusion](#scale-function-stochastic-processes) $s$, its speed density is $m=2/(\sigma^2s')$. Scale records hitting probabilities; speed records expected occupation and exit times. Multiplying scale by a positive constant divides speed by the same constant, leaving their Green-kernel product unchanged.

##### Finite-interval diffusion exit Green kernel

↑ **Parent:** [Speed density of a one-dimensional diffusion](#speed-density-of-a-one-dimensional-diffusion)

The expected exit time from $(\ell,r)$ for a one-dimensional diffusion is $\int_\ell^rK(x,v)m(v)dv$ when finite. Differentiating this expression on each side of $v=x$ gives the equation $\mathcal Lu=-1$ with zero endpoint values. For the [SLE two-boundary-point ratio diffusion](stochastic-process.md#sle-two-boundary-point-ratio-diffusion), $s(v)-s(1)$ behaves as $(v-1)^{1-4/\kappa}$ and the [speed density](#speed-density-of-a-one-dimensional-diffusion) behaves as $(v-1)^{4/\kappa}$, so the product is integrable at $1$ for $\kappa>4$.

### Maximal local solution of a stochastic differential equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A maximal local solution solves a stochastic differential equation until its lifetime, usually the first exit from every compact subset of the region where its coefficients are locally Lipschitz. If the lifetime is finite, the path approaches the boundary of that region or becomes unbounded.

#### Existence and pathwise uniqueness theorem for a stochastic differential equation

↑ **Parent:** [Maximal local solution of a stochastic differential equation](#maximal-local-solution-of-a-stochastic-differential-equation)

If the drift and diffusion coefficients are locally Lipschitz on an open domain, then for every initial point there is a pathwise unique strong solution up to a maximal lifetime. That lifetime is the limit of the exit times from an increasing sequence of compact subsets of the domain.

##### Linear growth condition for an SDE

↑ **Parent:** [Existence and pathwise uniqueness theorem for a stochastic differential equation](#existence-and-pathwise-uniqueness-theorem-for-a-stochastic-differential-equation)

The linear growth condition bounds the drift norm and diffusion-matrix norm by $C(1+|x|)$ for one constant $C$. Together with globally Lipschitz coefficients it gives global strong existence and pathwise uniqueness, preventing finite-time explosion. Linear coefficient maps satisfy it even when they are not bounded.

###### Maximal second-moment bound under linear growth

↑ **Parent:** [Linear growth condition for an SDE](#linear-growth-condition-for-an-sde)

For $dX=\sigma(X)dB+b(X)dt$, $X_0=0$, and $\sigma^2+b^2\leq A(1+X^2)$, the [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) imply, for $t\leq1$, $F(t)\leq8A\int_0^t(1+F(s))ds$, where $F(t)=\mathbb E\sup_{s\leq t}|X_s|^2$. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) yields $F(t)\leq e^{8At}-1$. Apply the calculation first to stopped paths; truncating [locally Lipschitz functions](real-analysis.md#locally-lipschitz-function) and using this uniform bound gives exit probabilities at most $(e^{8A}-1)/n^2$, proving nonexplosion on the unit time interval.

### Scale function (stochastic processes)

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Scale_function_(stochastic_processes))

For the one-dimensional diffusion

$$
dX_t=b(X_t)dt+\sigma(X_t)dB_t,
$$

a scale function is a strictly increasing function $s$ satisfying

$$
\frac12\sigma^2s''+bs'=0.
$$

The [Itô formula](#ito-s-lemma) then makes $s(X_t)$ a local martingale before the diffusion reaches a boundary.

#### Arctangent transform of a two-noise affine diffusion

↑ **Parent:** [Scale function (stochastic processes)](#scale-function-stochastic-processes)

For independent [Brownian motions](brownian-motion.md) $W,B$, the [Itô formula](#ito-s-lemma) cancels the drift after the arctangent transform. Normalizing the two noise coefficients gives a [continuous local martingale](martingale.md#continuous-local-martingale) $Z$ with [quadratic variation](#quadratic-variation) $t$, hence another [Brownian motion](brownian-motion.md) by the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion).

##### Endpoint convergence of a bounded angle diffusion

↑ **Parent:** [Arctangent transform of a two-noise affine diffusion](#arctangent-transform-of-a-two-noise-affine-diffusion)

A diffusion remaining in $(-\pi/2,\pi/2)$ with the displayed equation is a bounded [martingale](martingale.md) and has a terminal limit. Its expected total [quadratic variation](#quadratic-variation) is finite by its bounded second moments. An interior limit would leave its squared diffusion coefficient bounded away from zero and force infinite [quadratic variation](#quadratic-variation). Thus it converges to an endpoint, and the preserved mean determines the two endpoint probabilities.

#### Scale transform for an additive-noise diffusion

↑ **Parent:** [Scale function (stochastic processes)](#scale-function-stochastic-processes)

For $dX=b(X)\,dt+dW$ with continuous drift, integrate the positive derivative displayed above. The resulting [scale function of a one-dimensional diffusion](#scale-function-stochastic-processes) solves $g''=-2bg'$. The [Itô formula](#ito-s-lemma) removes the drift of $g(X)$, giving $dY=h(Y)\,dW$, where $h=g'\circ g^{-1}$ on the interval $g(\mathbb R)$. If the drift is bounded, $h'=-2b\circ g^{-1}$ is bounded, so $h$ is Lipschitz on that interval.

##### Strong well-posedness of additive-noise equations with bounded continuous drift

↑ **Parent:** [Scale transform for an additive-noise diffusion](#scale-transform-for-an-additive-noise-diffusion)

The [zero extension of a scale diffusion coefficient at finite endpoints](#zero-extension-of-a-scale-diffusion-coefficient-at-finite-endpoints) makes the transformed equation globally Lipschitz. Inverting its solution gives the original additive-noise equation. The pathwise bound $|X_t|\leq|x|+\sup_{s\leq T}|W_s|+\|b\|_\infty T$ prevents the inverse scale from reaching infinity at any finite time. This proves global strong existence and [pathwise uniqueness](#pathwise-uniqueness) even when the original drift is not Lipschitz.

##### Zero extension of a scale diffusion coefficient at finite endpoints

↑ **Parent:** [Scale transform for an additive-noise diffusion](#scale-transform-for-an-additive-noise-diffusion)

The diffusion coefficient obtained from a [scale transform for an additive-noise diffusion](#scale-transform-for-an-additive-noise-diffusion) need only be defined on an open interval. If it is Lipschitz, its limit at a finite endpoint is zero: a positive limit would bound the derivative $1/h$ of the inverse scale and prevent the inverse from diverging. Extending it by zero beyond finite endpoints therefore preserves global [Lipschitz continuity](real-analysis.md#lipschitz-continuity).

#### Boundary hitting probability from a diffusion scale function

↑ **Parent:** [Scale function (stochastic processes)](#scale-function-stochastic-processes)

If $a<x<b$ and the diffusion exits $(a,b)$ almost surely, optional stopping of the bounded local martingale $s(X_{t\wedge\tau})$ gives

$$
\mathbb P_x(X_\tau=a)=\frac{s(b)-s(x)}{s(b)-s(a)},
\qquad
\mathbb P_x(X_\tau=b)=\frac{s(x)-s(a)}{s(b)-s(a)}.
$$

##### Hypotheses for a diffusion scale hitting formula

↑ **Parent:** [Boundary hitting probability from a diffusion scale function](#boundary-hitting-probability-from-a-diffusion-scale-function)

The equation $\frac12\sigma^2s''+bs'=0$ makes the scale transform a [local martingale](martingale.md#local-martingale) but does not alone prove the usual two-boundary hitting ratio. Stopped on $[a,b]$, it is bounded, so optional stopping gives that ratio when exit is almost surely finite and the endpoint scale values differ. If exit can be infinite, the terminal [martingale](martingale.md) has a further contribution on the non-exit event. For example, $\sigma=b=0$, $X_t=x\in(a,b)$ and $s(y)=y$ satisfy the differential equation but never hit either endpoint; the claimed ratio would nevertheless be positive. A constant solution for $s$ also gives an undefined denominator and is excluded by the usual strict-monotonicity convention for scale.

### Weak solution of a stochastic differential equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A weak solution may choose its probability space and driving Brownian motion as part of the solution. It is weaker than a strong solution, which must be adapted to a prescribed Brownian motion.

#### Weak existence and uniqueness in law for an additive-noise SDE with bounded drift

↑ **Parent:** [Weak solution of a stochastic differential equation](#weak-solution-of-a-stochastic-differential-equation)

If $b:\mathbb R\to\mathbb R$ is bounded and measurable, then on every finite time interval

$$
dX_t=b(X_t)dt+dW_t
$$

has a weak solution and [uniqueness in law](#uniqueness-in-law). Starting with [Wiener measure](brownian-motion.md#wiener-measure), the [Novikov condition](#novikov-s-condition) and [Girsanov theorem](#girsanov-theorem) add the drift. Applying the inverse change of measure to any weak solution recovers Wiener measure and identifies its law by the same pathwise density.

### Strong solution of a stochastic differential equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

A strong solution is adapted to the filtration of a prescribed driving [Brownian motion](brownian-motion.md) on a prescribed probability space and satisfies the stochastic integral equation almost surely.

#### Strong existence

↑ **Parent:** [Strong solution of a stochastic differential equation](#strong-solution-of-a-stochastic-differential-equation)

A [stochastic differential equation](#stochastic-differential-equation) has strong existence for specified coefficients and initial data if a [strong stochastic solution](#strong-solution-of-a-stochastic-differential-equation) can be constructed on every prescribed stochastic basis carrying the required initial variable and driving [Brownian motion](brownian-motion.md). This existence assertion is distinct from [pathwise uniqueness](#pathwise-uniqueness) and from a definition of the solution itself.

#### Strong existence theorem for additive-noise SDEs with bounded measurable drift

↑ **Parent:** [Strong solution of a stochastic differential equation](#strong-solution-of-a-stochastic-differential-equation)

For bounded Borel $b:\mathbb R^d\to\mathbb R^d$, the [stochastic differential equation](#stochastic-differential-equation) $dX_t=b(X_t)dt+dB_t$ has [strong existence](#strong-existence) and [pathwise uniqueness](#pathwise-uniqueness). The identity diffusion matrix is nondegenerate. A [Girsanov theorem](#girsanov-theorem) argument alone establishes weak existence and [uniqueness in law](#uniqueness-in-law); the strong conclusion requires an additional theorem. This statement does not extend without further hypotheses to arbitrary path-dependent drift or arbitrary diffusion matrices. See [the primary bounded-drift strong-solution theorem](https://www.mathnet.ru/php/archive.phtml?jrnid=sm&option_lang=eng&paperid=2601&wshow=paper).

### Pathwise uniqueness

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pathwise_uniqueness)

Pathwise uniqueness holds when any two solutions with the same initial value and driven by the same Brownian motion on the same filtered probability space are indistinguishable.

### Uniqueness in law

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)

Uniqueness in law holds when any two weak solutions with the same initial distribution have the same distribution on path space, even though they may live on different probability spaces.

### Kolmogorov backward equation

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov_backward_equation)

For a diffusion with [infinitesimal generator](stochastic-process.md#infinitesimal-generator-stochastic-processes) $L$, the Kolmogorov backward equation is $\partial_tu=Lu$. Its solutions propagate terminal observables backward through the transition semigroup.

#### Bounded backward-equation stochastic representation

↑ **Parent:** [Kolmogorov backward equation](#kolmogorov-backward-equation)

For a bounded smooth solution of $u_t=Lu$ with initial function $f$, apply the [Itô formula](#ito-s-lemma) to $u(t-s,X_s)$. Its drift vanishes and its boundedness upgrades the localized stochastic integral to a true martingale. Taking endpoint expectations yields $u(t,x)=\mathbb E_xf(X_t)$ without a global bound on $u_x$.

#### Feynman-Kac formula

↑ **Parent:** [Kolmogorov backward equation](#kolmogorov-backward-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feynman-Kac_formula)

The Feynman-Kac formula represents solutions of certain parabolic [partial differential equations](partial-differential-equation.md) as conditional expectations of functionals of a diffusion. It follows by applying [Itô formula](#ito-s-lemma) to the solution along the diffusion and taking expectations.

##### Critical quadratic potential for the Ornstein-Uhlenbeck generator

↑ **Parent:** [Feynman-Kac formula](#feynman-kac-formula)

For $\mathcal L=\tfrac12\Delta-\lambda x\cdot\nabla$ and potential $V=\lambda^2|x|^2/2$, the [Feynman-Kac formula](#feynman-kac-formula) with initial value one gives $u=\mathbb E_x^{OU}e^{\int_0^tV(X_s)ds}$. The [Ornstein-Uhlenbeck likelihood relative to Wiener measure](#ornstein-uhlenbeck-likelihood-relative-to-wiener-measure) cancels the quadratic time integral, leaving a Gaussian endpoint integral. Completing the square gives the displayed answer for $1+\lambda t>0$. It is finite for all nonnegative times when $\lambda\ge0$; when $\lambda<0$ the path expectation diverges at and beyond $t=-1/\lambda$.

##### Elliptic Feynman-Kac formula

↑ **Parent:** [Feynman-Kac formula](#feynman-kac-formula)

For a bounded domain, a bounded [classical solution](partial-differential-equation.md#classical-solution) with boundary data $g$, nonnegative bounded $V$, bounded $f$ and integrable diffusion exit time $\tau$ satisfies

$$
u(x)=\mathbb E_x\left[e^{-\int_0^\tau V(X_r)dr}g(X_\tau)+\int_0^\tau e^{-\int_0^sV(X_r)dr}f(X_s)ds\right].
$$

Apply the [Itô product rule](#ito-product-rule) to the discounted stopped solution and add its source integral. The stopped martingale is dominated by $\|u\|_\infty+\|f\|_\infty\tau$, so [dominated convergence](measure-theory.md#dominated-convergence-theorem) permits passage to the exit. For $V=f=0$, this is a boundary-value averaging principle for functions harmonic under $L$.

##### Parabolic Feynman-Kac formula with a source

↑ **Parent:** [Feynman-Kac formula](#feynman-kac-formula)

For a nonexplosive [diffusion process](#markov-diffusion), bounded source $f$, terminal data $g$ and nonnegative bounded potential $V$, a bounded [classical solution](partial-differential-equation.md#classical-solution) with $u(T,x)=g(x)$ is

$$
u(t,x)=\mathbb E_{t,x}\left[e^{-\int_t^TV(X_r)dr}g(X_T)+\int_t^Te^{-\int_t^sV(X_r)dr}f(s,X_s)ds\right].
$$

The [Itô product rule](#ito-product-rule) shows that the discounted solution plus its accumulated discounted source is a local martingale. Its deterministic finite-horizon bound upgrades it to a true martingale, giving the formula and uniqueness without a global derivative bound.

##### Discounted boundary-hitting representation

↑ **Parent:** [Feynman-Kac formula](#feynman-kac-formula)

For a continuous [Itô diffusion](#ito-diffusion) with [diffusion generator](stochastic-process.md#diffusion-generator) $\mathcal L$, let $u$ solve $\mathcal Lu=\lambda u$ with $\lambda>0$, be bounded on an open domain and its boundary, and equal $g$ on the boundary. Stop at the first boundary hit $\tau$. The [Itô formula](#ito-s-lemma) makes $e^{-\lambda(t\wedge\tau)}u(X_{t\wedge\tau})$ a bounded martingale. Its limit is zero on $\{\tau=\infty\}$ and equals $e^{-\lambda\tau}g(X_\tau)$ on $\{\tau<\infty\}$. Thus

$$
u(x)=\mathbb E_x[e^{-\lambda\tau}g(X_\tau)\mathbf1_{\{\tau<\infty\}}].
$$

Boundedness justifies passage to the terminal expectation even if hitting is not almost surely finite.

##### Feynman-Kac formula with a bounded potential

↑ **Parent:** [Feynman-Kac formula](#feynman-kac-formula)

For bounded $V$ and bounded initial data $f$, a sufficiently regular [classical solution](partial-differential-equation.md#classical-solution) bounded on every finite time slab satisfies

$$
u(t,x)=\mathbb E_x\left[f(B_t)\exp\!\left(\int_0^tV(B_s)ds\right)\right].
$$

To prove this, the [Itô formula](#ito-s-lemma) and [Itô product rule](#ito-product-rule) make $u(T-t,B_t)e^{\int_0^tV(B_s)ds}$ a [local martingale](martingale.md#local-martingale). Its deterministic bound on $[0,T]$ makes it a true [martingale](martingale.md); taking [expectations](probability-theory.md#expected-value) at the two endpoints gives the formula. This also gives uniqueness in the finite-horizon bounded class. The exponent has the same sign as the potential in the equation.

###### Soft killing limit for Brownian nonnegative survival

↑ **Parent:** [Feynman-Kac formula with a bounded potential](#feynman-kac-formula-with-a-bounded-potential)

Let $\phi$ be continuous, nonnegative, zero on $[0,\infty)$, and strictly positive on $(-\infty,0)$. By continuity of Brownian paths, its occupation integral vanishes exactly on nonnegative paths. [Dominated convergence](measure-theory.md#dominated-convergence-theorem) gives the displayed limit. The [Brownian reflection principle](brownian-motion.md#reflection-principle-wiener-process) makes it $1-2\mathbb P_x(B_t\leq0)$ for $x\geq0$ and zero for $x<0$. In particular the limit at $x=0$ is zero for every positive time. The choice $\phi(x)=\min(1,\max(0,-x))$ is a bounded soft killing potential.

###### Zero-noise limit with a bounded potential

↑ **Parent:** [Feynman-Kac formula with a bounded potential](#feynman-kac-formula-with-a-bounded-potential)

For globally Lipschitz drift $b$, couple $dX^\varepsilon=b(X^\varepsilon)dt+\varepsilon dW$ and $\dot x=b(x)$ from the same point. The [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) gives $\sup_{s\le t}|X_s^\varepsilon-x_s|\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|$. Thus convergence is uniform on each finite horizon. The [Feynman-Kac formula](#feynman-kac-formula) for generator $\varepsilon^2\Delta/2+b\cdot\nabla+c$ has weight $\exp\int c$, with a positive sign. Bounded continuous $c$ is uniformly continuous on a compact neighbourhood of the deterministic trajectory, and bounded continuous $f$ supplies a deterministic integrable bound. The [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) proves the displayed limit without requiring global uniform continuity of $c$.

###### Positive-potential growth from Brownian recurrence

↑ **Parent:** [Feynman-Kac formula with a bounded potential](#feynman-kac-formula-with-a-bounded-potential)

Suppose bounded $V\geq0$ is bounded below by a positive constant on some nonempty open interval, and $f\geq C>0$. The [Feynman-Kac formula with a bounded potential](#feynman-kac-formula-with-a-bounded-potential) gives $u(t,x)\geq C\mathbb E_x e^{\int_0^tV(B_s)ds}$. [Infinite occupation time of one-dimensional Brownian motion](brownian-motion.md#infinite-occupation-time-of-one-dimensional-brownian-motion) makes that integral tend to infinity [almost surely](convergence-of-random-variables.md#almost-sure-convergence). The [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) then gives $u(t,x)\to\infty$ for every fixed $x$. Thus no globally bounded [classical solution](partial-differential-equation.md#classical-solution) exists under these hypotheses, although boundedness on every finite time slab is compatible with the conclusion.

### Martingale problem

↑ **Parent:** [Stochastic differential equation](#stochastic-differential-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Martingale_problem)

For a differential operator $L$, the martingale problem asks for a process $X$ such that

$$
f(X_t)-f(X_0)-\int_0^tLf(X_s)\,ds
$$

is a local martingale for every test function $f$ in a suitable domain.

#### Martingale problem for Brownian motion

↑ **Parent:** [Martingale problem](#martingale-problem)

A continuous adapted process started at a fixed point is [Brownian motion](brownian-motion.md) exactly when $f(X_t)-f(X_0)-\frac12\int_0^t\Delta f(X_s)ds$ is a [martingale](martingale.md) for every $f\in C_c^\infty(\mathbb R^d)$. Cutoff coordinate and coordinate-product tests give continuous [local martingales](martingale.md#local-martingale) with [quadratic covariations](#quadratic-covariation) $[X^i,X^j]_t=\delta_{ij}t$. The [Itô formula](#ito-s-lemma) makes $\exp(iu\cdot(X_t-X_0)+|u|^2t/2)$ a local martingale, whose deterministic modulus bound on bounded horizons makes it a true martingale. Its conditional expectation identifies every increment as centered Gaussian with covariance $(t-s)I$, independent of the past. This proves the converse via the [Lévy characterization of multidimensional Brownian motion](brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion). The forward implication is the [Itô formula](#ito-s-lemma).

#### Diffusion approximation theorem

↑ **Parent:** [Martingale problem](#martingale-problem)

For discrete-time Markov chains run at time step $1/n$, suppose the displayed conditional moments converge uniformly on compact sets to continuous coefficients, the local conditional large-jump second moments vanish, initial laws converge, and [compact containment](convergence-of-random-variables.md#compact-containment) holds on each finite horizon. If the limiting diffusion [martingale problem](#martingale-problem) is well-posed and nonexplosive, the chain laws converge to its solution. Vanishing jumps give a continuous limit; linearly interpolated paths converge in the uniform path topology and step paths in [Skorokhod J1 topology](convergence-of-random-variables.md#skorokhod-j1-topology). Local moment bounds give tightness after exit-time localization. Taylor expansion identifies the limiting test-function martingales, and uniqueness of the [martingale problem](#martingale-problem) makes every subsequential limit the same. The [diffusion approximation of a birth-death process](markov-process.md#diffusion-approximation-of-a-birth-death-process) is an important example.

#### Well-posed martingale problem

↑ **Parent:** [Martingale problem](#martingale-problem)

A [martingale](martingale.md) problem is well-posed for a specified test domain and class of paths if it admits a solution for every specified starting point and that solution is unique in law. Existence on one fixed probability space is not required. Test-domain and true-versus-local conventions must be stated. For bounded diffusion coefficients and $C_b^2$ test functions, boundedness on every finite horizon upgrades the local identities to true [martingale](martingale.md) identities.

#### Diffusion martingale problem

↑ **Parent:** [Martingale problem](#martingale-problem)

For bounded measurable $a,b$, with $a$ symmetric positive semidefinite, an [L-diffusion](#diffusion-martingale-problem) is a continuous [adapted process](stochastic-process.md#adapted-process) $X$ such that $g(X_t)-g(X_0)-\int_0^t Lg(X_s)ds$ is a true [martingale](martingale.md) for every $g\in C_b^2$. The general local [martingale problem](#martingale-problem) may instead use compactly supported test functions and require only a [local martingale](martingale.md#local-martingale). Specify the test class and the true or local convention when coefficients are unbounded.

##### Bounded-domain harmonic uniqueness for a diffusion

↑ **Parent:** [Diffusion martingale problem](#diffusion-martingale-problem)

For a bounded-domain diffusion with almost surely finite exit time $\tau_D$, bounded $L$-harmonic functions continuous up to the boundary satisfy $u(x)=\mathbb E_xu(X_{\tau_D})$. Stop the test-function martingale and use bounded convergence. Identical boundary values therefore imply identical harmonic functions. Uniform ellipticity and bounded SDE coefficients ensure finite exit by the projection argument.

// Target: probability-and-statistics.bigb

##### Projection unboundedness of a uniformly elliptic diffusion

↑ **Parent:** [Diffusion martingale problem](#diffusion-martingale-problem)

For an SDE with bounded drift and diffusion coefficients and $\sum_k\langle\xi,\sigma_k(x)\rangle^2\ge\lambda|\xi|^2$, each fixed nonzero scalar projection of a solution is unbounded in absolute value almost surely. Rescale a slab to $(-1,1)$; its projected drift is controlled by its uniformly positive bracket density. The [exit with drift controlled by quadratic variation](martingale.md#exit-with-drift-controlled-by-quadratic-variation) then forces exit from every slab in a countable exhaustion.

// Target: probability-and-statistics.bigb

##### Time-dependent test functions for a diffusion martingale problem

↑ **Parent:** [Diffusion martingale problem](#diffusion-martingale-problem)

For an [L-diffusion](#diffusion-martingale-problem) with bounded coefficients and $f\in C_b^{1,2}$, $M^f$ is a continuous [martingale](martingale.md). Freeze the time argument along a deterministic partition, apply the spatial [martingale problem](#martingale-problem) on each interval, and pass to the limit by the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem). The same proof works if the absolute drift coefficients and the trace of the diffusivity have integrable time integrals along the path on every finite horizon. Local hypotheses alone give a [local martingale](martingale.md#local-martingale) conclusion.

<h2 id="doleans-dade-exponential">Doléans-Dade exponential</h2>

↑ **Parent:** [Stochastic calculus](stochastic-calculus.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doléans-Dade_exponential)

For a continuous semimartingale $X$, its Doléans-Dade exponential is

$$
\mathcal E(X)_t=\exp\!\left(X_t-X_0-\frac12[X]_t\right).
$$

It solves $dZ_t=Z_t\,dX_t$ with $Z_0=1$.

### Pathwise uniqueness for a multiplicative martingale equation

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)

The [Itô formula](#ito-s-lemma) gives $d\log Z=dM-\frac12d[M]$ for a strictly positive solution. Therefore equal initial values give indistinguishable solutions. Conversely the displayed exponential satisfies the equation. This is uniqueness for a fixed continuous local martingale driver and does not require the exponential to be a true martingale.

### Stochastic logarithm

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)

For a strictly positive continuous semimartingale $Z$, its stochastic logarithm is $\int Z^{-1}\,dZ$. When $Z$ is a continuous local martingale starting at one, this is a local martingale $L$ and the [Itô formula](#ito-s-lemma) gives $Z=\exp(L-\langle L\rangle/2)$. Unlike the ordinary logarithm, it has no compensating finite-variation term.

#### Divergent logarithmic clock for a positive local martingale tending to zero

↑ **Parent:** [Stochastic logarithm](#stochastic-logarithm)

Write a positive continuous local martingale as $M=\exp(X-\langle X\rangle/2)$ using its [stochastic logarithm](#stochastic-logarithm). If $M_t\to0$, its logarithmic bracket must diverge. Otherwise the [finite-bracket convergence lemma](martingale.md#finite-bracket-convergence-lemma) makes $X$ converge finitely and the exponential has a positive limit.

<h3 id="kazamaki-s-condition">Kazamaki's condition</h3>

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kazamaki's_condition)

This is an exponential-moment criterion for the [stochastic exponential](#doleans-dade-exponential) to be a true [martingale](martingale.md). In the infinite-horizon stopped-moment form, a zero-starting convergent [continuous local martingale](martingale.md#continuous-local-martingale) satisfying $\sup_T\mathbb Ee^{M_T/2}<\infty$ has a [uniformly integrable martingale](martingale.md#uniformly-integrable-martingale) $\mathcal E(M)$. The [half-threshold for the exponential-martingale Hölder bound](#half-threshold-for-the-exponential-martingale-holder-bound) first controls strict scalings. The [terminal scaling inequality for stochastic exponentials](#terminal-scaling-inequality-for-stochastic-exponentials) and [terminal expectation criterion for a nonnegative local martingale](martingale.md#terminal-expectation-criterion-for-a-nonnegative-local-martingale) then include the endpoint scaling.

### Terminal scaling inequality for stochastic exponentials

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)

For a convergent [continuous local martingale](martingale.md#continuous-local-martingale) and $r>1$, factor $\mathcal E(X)$ into $\mathcal E(rX)^{1/r^2}$ and an ordinary exponential. Apply the [Holder inequality](functional-analysis.md#holder-inequality) and then the concave [Jensen inequality](real-analysis.md#jensen-s-inequality) to the fractional power $2/(r+1)$. The displayed lower bound is informative when the terminal exponential moment is finite.

<h3 id="holder-factorization-of-stochastic-exponentials">Hölder factorization of stochastic exponentials</h3>

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)

For a zero-starting [continuous local martingale](martingale.md#continuous-local-martingale) $X$, the [stochastic exponential](#doleans-dade-exponential) satisfies

$$
\mathcal E(X)^p=\mathcal E(\sqrt{pq}X)^{1/q}
\bigl(e^{C(p,q)X}\bigr)^{(q-1)/q}.
$$

The [Holder inequality](functional-analysis.md#holder-inequality) and the [supermartingale](martingale.md#supermartingale) property of the first exponential bound its stopped $p$th moment by $(\mathbb Ee^{C(p,q)X_T})^{(q-1)/q}$. The subtraction in the coefficient is $\sqrt{pq}-1$, not a square root of $pq-1$.

<h4 id="half-threshold-for-the-exponential-martingale-holder-bound">Half-threshold for the exponential-martingale Hölder bound</h4>

↑ **Parent:** [Hölder factorization of stochastic exponentials](#holder-factorization-of-stochastic-exponentials)

For fixed $q>1$, the coefficient in the [Hölder factorization of stochastic exponentials](#holder-factorization-of-stochastic-exponentials) exceeds $\sqrt q/(\sqrt q+1)>1/2$. Taking $q=1+\varepsilon$ and $p=1+\varepsilon^2$ approaches one-half. Thus a uniform stopped exponential moment at coefficient one-half bounds some $p$th moment of each strict scaling $\mathcal E(aM)$, $0<a<1$.

<h3 id="novikov-s-condition">Novikov's condition</h3>

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Novikov's_condition)

If a continuous local martingale $M$ satisfies

$$
\mathbb E\exp\!\left(\frac12[M]_T\right)<\infty,
$$

then its [stochastic exponential](#doleans-dade-exponential) is a true martingale through time $T$.

#### Bounded-bracket criterion for a stochastic exponential

↑ **Parent:** [Novikov's condition](#novikov-s-condition)

For a zero-start [continuous local martingale](martingale.md#continuous-local-martingale) $M$ with $[M]_\infty\leq C$ deterministically, its [stochastic exponential](#doleans-dade-exponential) is a [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) [martingale](martingale.md). For each $p>1$, $\sup_t\mathbb E\mathcal E(M)_t^p\leq e^{p(p-1)C/2}$. Its terminal value is strictly positive, so it defines an equivalent infinite-horizon [change of measure](measure-theory.md#change-of-measure) by the [Girsanov theorem](#girsanov-theorem).

#### Dambis-Dubins-Schwarz proof of the Novikov condition

↑ **Parent:** [Novikov's condition](#novikov-s-condition)

Write $M_t=B_{[M]_t}$ by the [Dambis-Dubins-Schwarz theorem](martingale.md#dambis-dubins-schwarz-theorem) and stop the exponential Brownian martingale when $B_s-s$ first reaches $b<0$. The stopped exponential has mean one. Its boundary contribution before $[M]_T$ is at most

$$
e^b\mathbb E e^{[M]_T/2},
$$

which vanishes as $b\to-\infty$. The remaining term converges monotonically to $\mathcal E(M)_t$, proving that its expectation is one.

### Girsanov theorem

↑ **Parent:** [Doléans-Dade exponential](#doleans-dade-exponential)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Girsanov_theorem)

Girsanov's theorem describes how a change of probability measure changes the drift of a semimartingale. If the appropriate [stochastic exponential](#doleans-dade-exponential) is a true martingale, weighting by it turns $W_t+\int_0^t\theta_sds$ into a Brownian motion under the new measure.

#### Ornstein-Uhlenbeck likelihood relative to Wiener measure

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

On each finite horizon the displayed [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative) changes [Wiener measure](brownian-motion.md#wiener-measure) into the law of $dX=dB-\mu Xdt$. Stop at coordinate magnitude n so the [Novikov condition](#novikov-s-condition) applies. Under each stopped tilted measure the coordinate solves the drifted equation, and the [Gronwall inequality](probability-and-statistics.md#gronwall-inequality) with the [Doob L2 maximal inequality](martingale.md#doob-l2-maximal-inequality) bounds its maximal second moment uniformly in n. The probability of reaching n therefore tends to zero; this proves that the unstopped density has expectation one. No unrestricted large-time Novikov estimate is needed.

#### Bounded Girsanov density for exit of an unstable linear diffusion

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

Under a reference measure where $X$ is [Brownian motion](brownian-motion.md) started at zero, let $T$ be its exit time from $(-1,1)$. The displayed density is the stochastic exponential with integrand $X\mathbf1_{[0,T]}$, by the [Itô formula](#ito-s-lemma). It is bounded by $e^{1/2}$, hence defines a uniformly integrable density process with terminal density $Z_T$. Under that measure change, $X_t-\int_0^{t\wedge T}X_sds$ is [Brownian motion](brownian-motion.md). At exit, $Z_T\ge e^{1/2-T}$, implying $\mathbb P(T\le t)\ge e^{1/2-t}\widetilde{\mathbb P}(T\le t)$. This is a terminal density on the whole probability space, not merely an unspecified finite-horizon change of measure.

#### Semimartingale invariance under equivalent measures

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

On a fixed finite horizon, equivalent probability measures have the same [semimartingales](#semimartingale). For a strictly positive continuous [Radon-Nikodym density martingale](measure-theory.md#radon-nikodym-density-martingale) $Z$ and a continuous local martingale $L$ under the original measure, $L-\int Z^{-1}d[L,Z]$ is a local martingale under the new one, by the [Girsanov theorem](#girsanov-theorem). Thus the finite-variation part of a continuous [semimartingale decomposition](#semimartingale-decomposition) changes by the opposite covariation correction.

#### Finite-horizon drift replacement by a change of measure

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

For $dX=\mu\,dt+\sigma\,dB$ on $[0,T]$, take $\theta=(\nu-\mu)/\sigma$ and use density $\mathcal E(\int\theta\,dB)_T$. If $\mu,\nu$ are bounded and $\sigma$ is continuous and bounded below by a positive constant, the exponential has bounded bracket and defines an equivalent measure. Under it, $\widetilde B=B-\int\theta\,dt$ is Brownian and $dX=\nu\,dt+\sigma\,d\widetilde B$. Set $\theta=0$ after $T$ to define the density on the entire original sigma-algebra and the new [Brownian motion](brownian-motion.md) on the whole time axis.

#### Girsanov density for a stopped Bessel process

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

For reference [Brownian motion](brownian-motion.md) $R=x+W$, stopped at $T=t\wedge\tau_{(a,b)}$ with $0<a<x<b$, this expression is the [Radon-Nikodym derivative](measure-theory.md#radon-nikodym-derivative) of the stopped [Bessel process](brownian-motion.md#bessel-process) law of dimension $\delta$. The bounded stopped drift verifies the [Novikov condition](#novikov-s-condition). The comparison laws must have the same initial value and the same stopping rule.

##### Brownian conditioning by a stopped Bessel density

↑ **Parent:** [Girsanov density for a stopped Bessel process](#girsanov-density-for-a-stopped-bessel-process)

For $0<x<M$, a [three-dimensional Bessel process](brownian-motion.md#three-dimensional-bessel-process) stopped at $M$ has the law of [Brownian motion](brownian-motion.md) conditioned to hit $M$ before zero and stopped at $M$. On $(\varepsilon,M)$, the [Girsanov theorem](#girsanov-theorem) and the [Itô formula](#ito-s-lemma) give terminal density $X_\tau/x$. Its value is $M/x$ at the upper exit and $\varepsilon/x$ at the lower exit. Letting $\varepsilon\downarrow0$ in bounded stopped-path functionals gives density $(M/x)\mathbf1_{\{T_M<T_0\}}$ relative to the corresponding stopped [Wiener measure](brownian-motion.md#wiener-measure). The exit probability is $x/M$ by the [optional stopping theorem](martingale.md#optional-sampling-theorem-for-a-supermartingale), so the density is normalized. On the unstopped full path space the same density defines the conditioned Brownian law; pushing it forward by the stopping map gives the stopped Bessel law. The already-stopped law is not absolutely continuous relative to unstopped Wiener measure, since eventually constant paths have Wiener probability zero.

#### Martingale transfer under a density process

↑ **Parent:** [Girsanov theorem](#girsanov-theorem)

Let $Z$ be a positive uniformly integrable martingale defining $d\widetilde{\mathbb P}=Z_\infty\,d\mathbb P$. If $Y$ is bounded and $ZY$ is a true $\mathbb P$-martingale, then $Y$ is a $\widetilde{\mathbb P}$-martingale. This follows from the conditional-expectation change-of-measure identity.

##### Initial integrability under a density change

↑ **Parent:** [Martingale transfer under a density process](#martingale-transfer-under-a-density-process)

The density-product proof of the [Girsanov theorem](#girsanov-theorem) makes drift-corrected zero-starting increments a [local martingale](martingale.md#local-martingale) under the new measure. Adding the initial random variable requires its integrability under that measure. This is automatic if the density is one at time zero, because the measures agree on the initial [sigma-algebra](measure-theory.md#sigma-algebra). Without this normalization it can fail: take $P(n)=2^{-n}$, $Q(n)=c/n^2$, constant $M_t=\log(Q(n)/P(n))$ and constant $X_t=n$. These are P-martingales and the prescribed exponential density is valid, but $X_0$ is not Q-integrable.

##### Bounded-process density-product criterion

↑ **Parent:** [Martingale transfer under a density process](#martingale-transfer-under-a-density-process)

Let $Z$ be a positive uniformly integrable density martingale. If $Y$ is bounded and $ZY$ is a local martingale under the original measure, the product is a true martingale: its stopped absolute values are dominated by a fixed multiple of the uniformly integrable stopped density. Bayes then makes $Y$ a martingale under the new measure. Stop a locally bounded continuous $Y$ at absolute-value levels to obtain the local version.

## ↑ Ancestors (6)

1. [Stochastic process](stochastic-process.md)
2. [Probability theory](probability-theory.md)
3. [Probability and statistics](probability-and-statistics.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#6/iii/solution)
