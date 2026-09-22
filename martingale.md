# Martingale

↑ **Parent:** [Probability theory](probability-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Martingale)

An integrable adapted process $(M_n)$ is a martingale when $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$.

**Table of contents**

- [Positive random-environment path-weight martingale](#positive-random-environment-path-weight-martingale)
  - [Tail event for a vanishing positive path-weight limit](#tail-event-for-a-vanishing-positive-path-weight-limit)
  - [Collision-count second moment for independent path weights](#collision-count-second-moment-for-independent-path-weights)
- [Bernstein bound for bounded-jump martingales](#bernstein-bound-for-bounded-jump-martingales)
- [Ville inequality](#ville-inequality)
- [Finite voter-model consensus probability](#finite-voter-model-consensus-probability)
- [Unchanging betting probability under sampling without replacement](#unchanging-betting-probability-under-sampling-without-replacement)
- [Nonnegative martingale](#nonnegative-martingale)
- [Doob exposure martingale](#doob-exposure-martingale)
- [Rare-jump martingale divergence](#rare-jump-martingale-divergence)
- [Characterization of a martingale by bounded continuous-time stopped expectations](#characterization-of-a-martingale-by-bounded-continuous-time-stopped-expectations)
- [Azuma's inequality](#azuma-s-inequality)
  - [Two-sided Azuma-Hoeffding inequality](#two-sided-azuma-hoeffding-inequality)
- [Martingale increments obstruct finite convergence](#martingale-increments-obstruct-finite-convergence)
- [Absorption at zero of a nonnegative martingale](#absorption-at-zero-of-a-nonnegative-martingale)
  - [Absorption-time bound from conditional variance and overshoot](#absorption-time-bound-from-conditional-variance-and-overshoot)
    - [Square-root tail bound for martingale absorption](#square-root-tail-bound-for-martingale-absorption)
- [Martingale difference sequence](#martingale-difference-sequence)
  - [Martingale difference](#martingale-difference)
  - [Strong law for martingales with bounded increments](#strong-law-for-martingales-with-bounded-increments)
- [Dyadic slope martingale](#dyadic-slope-martingale)
- [Fair-coin doubling martingale](#fair-coin-doubling-martingale)
- [Martingale-difference orthogonality](#martingale-difference-orthogonality)
- [Submartingale](#submartingale)
  - [Positive martingale majorant of an L1-bounded submartingale](#positive-martingale-majorant-of-an-l1-bounded-submartingale)
  - [Doob-Meyer decomposition theorem](#doob-meyer-decomposition-theorem)
  - [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)
    - [Truncated layer-cake proof of the L2 maximal inequality](#truncated-layer-cake-proof-of-the-l2-maximal-inequality)
    - [One-sided martingale maximal inequality](#one-sided-martingale-maximal-inequality)
    - [Kolmogorov maximal inequality](#kolmogorov-maximal-inequality)
    - [One-sided maximal inequality for a centered square-integrable martingale](#one-sided-maximal-inequality-for-a-centered-square-integrable-martingale)
    - [Maximal bound for a nonnegative martingale](#maximal-bound-for-a-nonnegative-martingale)
    - [One-sided maximal inequality for independent centered sums](#one-sided-maximal-inequality-for-independent-centered-sums)
- [Square martingale for independent centered sums](#square-martingale-for-independent-centered-sums)
  - [Small-ball maximal bound for sums with bounded increments](#small-ball-maximal-bound-for-sums-with-bounded-increments)
- [Conditional-expectation martingale](#conditional-expectation-martingale)
  - [Edge-exposure martingale](#edge-exposure-martingale)
- [Product martingale from independent mean-one factors](#product-martingale-from-independent-mean-one-factors)
- [Continuous-time martingale](#continuous-time-martingale)
  - [Uniform-arrival residual mass martingale](#uniform-arrival-residual-mass-martingale)
    - [Finite-jump boundary crossing identity](#finite-jump-boundary-crossing-identity)
  - [Uniformly integrable martingale](#uniformly-integrable-martingale)
  - [Càdlàg martingale](#cadlag-martingale)
  - [Continuous martingale](#continuous-martingale)
  - [L2-bounded continuous martingale](#l2-bounded-continuous-martingale)
    - [Integrable terminal bracket criterion](#integrable-terminal-bracket-criterion)
    - [Equivalent terminal and maximal norms for L2-bounded continuous martingales](#equivalent-terminal-and-maximal-norms-for-l2-bounded-continuous-martingales)
  - [Local martingale](#local-martingale)
    - [Bounded local martingale criterion](#bounded-local-martingale-criterion)
    - [Integrable discrete-time local martingale is a martingale](#integrable-discrete-time-local-martingale-is-a-martingale)
      - [Nonnegative discrete-time local martingale is a martingale](#nonnegative-discrete-time-local-martingale-is-a-martingale)
    - [Strict local martingale](#strict-local-martingale)
      - [Logarithm of planar Brownian radius](#logarithm-of-planar-brownian-radius)
    - [Localizing sequence](#localizing-sequence)
    - [Continuous local martingale](#continuous-local-martingale)
      - [Finite-variation smooth transform of a continuous local martingale](#finite-variation-smooth-transform-of-a-continuous-local-martingale)
      - [Exponential criterion for a continuous local martingale and its bracket](#exponential-criterion-for-a-continuous-local-martingale-and-its-bracket)
      - [Conditionally symmetric increments](#conditionally-symmetric-increments)
        - [Characteristic function under conditionally symmetric martingale increments](#characteristic-function-under-conditionally-symmetric-martingale-increments)
      - [Finite-bracket convergence lemma](#finite-bracket-convergence-lemma)
      - [Fourth-moment deficit and bracket variance identity](#fourth-moment-deficit-and-bracket-variance-identity)
      - [Integrable-supremum martingale criterion](#integrable-supremum-martingale-criterion)
      - [Continuous local martingale with bounded quadratic variation](#continuous-local-martingale-with-bounded-quadratic-variation)
      - [Continuous finite-variation local martingale is constant](#continuous-finite-variation-local-martingale-is-constant)
      - [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)
        - [Cosine-exponential Brownian local martingale](#cosine-exponential-brownian-local-martingale)
        - [Gaussian terminal value at a deterministic bracket level](#gaussian-terminal-value-at-a-deterministic-bracket-level)
        - [Exit with drift controlled by quadratic variation](#exit-with-drift-controlled-by-quadratic-variation)
        - [Common-clock time change of orthogonal local martingales](#common-clock-time-change-of-orthogonal-local-martingales)
        - [One-sided bound criterion for a martingale clock](#one-sided-bound-criterion-for-a-martingale-clock)
        - [Finite-lifetime extension of the Dambis-Dubins-Schwarz theorem](#finite-lifetime-extension-of-the-dambis-dubins-schwarz-theorem)
        - [Inverse-clock proof of the Dambis-Dubins-Schwarz theorem](#inverse-clock-proof-of-the-dambis-dubins-schwarz-theorem)
        - [Stochastic-integral representation from absolutely continuous quadratic variation](#stochastic-integral-representation-from-absolutely-continuous-quadratic-variation)
        - [Brownian motion produced by the Dambis-Dubins-Schwarz theorem need not be independent of its clock](#brownian-motion-produced-by-the-dambis-dubins-schwarz-theorem-need-not-be-independent-of-its-clock)
      - [Burkholder-Davis-Gundy inequalities](#burkholder-davis-gundy-inequalities)
        - [Upper maximal moment bound for a continuous local martingale](#upper-maximal-moment-bound-for-a-continuous-local-martingale)
    - [Nonnegative local martingale](#nonnegative-local-martingale)
      - [Maximal identity for a continuous nonnegative local martingale tending to zero](#maximal-identity-for-a-continuous-nonnegative-local-martingale-tending-to-zero)
      - [Terminal expectation criterion for a nonnegative local martingale](#terminal-expectation-criterion-for-a-nonnegative-local-martingale)
- [Doob L2 maximal inequality](#doob-l2-maximal-inequality)
- [Doob Lp maximal inequality](#doob-lp-maximal-inequality)
- [L2 martingale convergence theorem](#l2-martingale-convergence-theorem)
- [Symmetric signs forced by the martingale property](#symmetric-signs-forced-by-the-martingale-property)
- [Doob upcrossing inequality](#doob-upcrossing-inequality)
  - [Dubins upcrossing inequality](#dubins-upcrossing-inequality)
    - [Multiplicative upcrossing supermartingale](#multiplicative-upcrossing-supermartingale)
  - [Upcrossing](#upcrossing)
    - [Upcrossing count](#upcrossing-count)
  - [Martingale convergence theorem](#martingale-convergence-theorem)
    - [Almost-sure martingale convergence to a nonintegrable limit](#almost-sure-martingale-convergence-to-a-nonintegrable-limit)
    - [L2-bounded martingale convergence theorem](#l2-bounded-martingale-convergence-theorem)
    - [Coin-doubling martingale](#coin-doubling-martingale)
    - [Almost sure submartingale convergence theorem](#almost-sure-submartingale-convergence-theorem)
    - [Lp martingale convergence theorem](#lp-martingale-convergence-theorem)
    - [Uniformly integrable martingale convergence theorem](#uniformly-integrable-martingale-convergence-theorem)
      - [Uniform integrability of a stopped uniformly integrable martingale](#uniform-integrability-of-a-stopped-uniformly-integrable-martingale)
    - [Reverse martingale convergence theorem](#reverse-martingale-convergence-theorem)
    - [Almost sure supermartingale convergence theorem](#almost-sure-supermartingale-convergence-theorem)
      - [Multiplicative correction for summable adapted drift](#multiplicative-correction-for-summable-adapted-drift)
      - [Supermartingale convergence with summable adapted drift](#supermartingale-convergence-with-summable-adapted-drift)
        - [Deterministic summable drift correction](#deterministic-summable-drift-correction)
    - [Conditional-expectation convergence along a filtration](#conditional-expectation-convergence-along-a-filtration)
      - [Moving-variable conditional-expectation convergence](#moving-variable-conditional-expectation-convergence)
    - [Continuous-time martingale convergence theorem](#continuous-time-martingale-convergence-theorem)
- [Supermartingale](#supermartingale)
  - [Pasting supermartingales with downward jumps](#pasting-supermartingales-with-downward-jumps)
  - [Terminal decomposition of an L1-bounded supermartingale](#terminal-decomposition-of-an-l1-bounded-supermartingale)
  - [Stopping preserves supermartingales in discrete time](#stopping-preserves-supermartingales-in-discrete-time)
  - [Local supermartingale](#local-supermartingale)
  - [Square-root stock supermartingale](#square-root-stock-supermartingale)
  - [Maximal inequality for a nonnegative supermartingale](#maximal-inequality-for-a-nonnegative-supermartingale)
  - [Zero is absorbing for a nonnegative supermartingale](#zero-is-absorbing-for-a-nonnegative-supermartingale)
  - [Constant-expectation supermartingale is a martingale](#constant-expectation-supermartingale-is-a-martingale)
  - [Supermartingale majorant bound](#supermartingale-majorant-bound)
- [Stopping time](#stopping-time)
  - [Closed-level hitting times of continuous adapted processes](#closed-level-hitting-times-of-continuous-adapted-processes)
  - [Waiting time for two consecutive successes](#waiting-time-for-two-consecutive-successes)
  - [Stopped process](#stopped-process)
    - [Stopped predictable budget for adapted increments](#stopped-predictable-budget-for-adapted-increments)
  - [Integrability of a stopped random-walk increment](#integrability-of-a-stopped-random-walk-increment)
  - [Stopping-time sigma-algebra](#stopping-time-sigma-algebra)
    - [Pasting ordered stopping times](#pasting-ordered-stopping-times)
  - [Announcing sequence for a stopping time](#announcing-sequence-for-a-stopping-time)
  - [Bounded stopping time](#bounded-stopping-time)
  - [Geometric tail bound from a uniform escape probability](#geometric-tail-bound-from-a-uniform-escape-probability)
    - [Random-walk exit bound from a positive-increment block](#random-walk-exit-bound-from-a-positive-increment-block)
  - [Waiting time for a word in independent uniform symbols](#waiting-time-for-a-word-in-independent-uniform-symbols)
  - [Skorokhod embedding theorem](#skorokhod-embedding-theorem)
    - [Skorokhod embedding of a centered random walk](#skorokhod-embedding-of-a-centered-random-walk)
      - [Central limit theorem from the Skorokhod embedding](#central-limit-theorem-from-the-skorokhod-embedding)
  - [Stopped martingale in discrete time](#stopped-martingale-in-discrete-time)
    - [Integrable overshoot of a stopped L1-bounded martingale](#integrable-overshoot-of-a-stopped-l1-bounded-martingale)
    - [Stopped-martingale uniform integrability criterion](#stopped-martingale-uniform-integrability-criterion)
    - [Characterization of a martingale by stopped expectations](#characterization-of-a-martingale-by-stopped-expectations)
    - [Discounted symmetric random-walk exit transform](#discounted-symmetric-random-walk-exit-transform)
  - [Optional sampling theorem for a supermartingale](#optional-sampling-theorem-for-a-supermartingale)
    - [Bounded-increment optional stopping with integrable time](#bounded-increment-optional-stopping-with-integrable-time)
    - [Bounded-stopping-time characterization of a martingale](#bounded-stopping-time-characterization-of-a-martingale)
    - [Exponential-supermartingale escape bound](#exponential-supermartingale-escape-bound)
- [Predictable process](#predictable-process)
  - [Martingale transform](#martingale-transform)
    - [Terminal nonnegativity criterion for a finite-horizon martingale transform](#terminal-nonnegativity-criterion-for-a-finite-horizon-martingale-transform)
    - [Predictable-coefficient localization of a martingale transform](#predictable-coefficient-localization-of-a-martingale-transform)
    - [Recovery of a martingale-transform integrand by conditional covariance](#recovery-of-a-martingale-transform-integrand-by-conditional-covariance)
    - [Stopped martingale](#stopped-martingale)
      - [Stopped-walk martingale with almost sure but not L1 convergence](#stopped-walk-martingale-with-almost-sure-but-not-l1-convergence)
    - [Reflection principle for simple symmetric random walk](#reflection-principle-for-simple-symmetric-random-walk)
      - [Point probability for the maximum of simple symmetric random walk](#point-probability-for-the-maximum-of-simple-symmetric-random-walk)
    - [Predictable representation in a Rademacher filtration](#predictable-representation-in-a-rademacher-filtration)
      - [Stopped martingale isometry in a Rademacher filtration](#stopped-martingale-isometry-in-a-rademacher-filtration)
  - [Predictable compensator of a discrete supermartingale](#predictable-compensator-of-a-discrete-supermartingale)
  - [Predictable sigma-algebra](#predictable-sigma-algebra)
    - [Predictable rectangle](#predictable-rectangle)
    - [Survival-observation predictable sigma-algebra](#survival-observation-predictable-sigma-algebra)
    - [Predictable sections at deterministic times](#predictable-sections-at-deterministic-times)
    - [Elementary predictable process with stopping-time intervals](#elementary-predictable-process-with-stopping-time-intervals)
    - [Simple predictable process](#simple-predictable-process)
      - [Density of simple predictable processes for finite measures](#density-of-simple-predictable-processes-for-finite-measures)
    - [Deterministic càdlàg process is predictable](#deterministic-cadlag-process-is-predictable)
- [Doob decomposition theorem](#doob-decomposition-theorem)
  - [Strong law for submartingales with bounded increments](#strong-law-for-submartingales-with-bounded-increments)
  - [Doob decomposition of an adapted integrable process](#doob-decomposition-of-an-adapted-integrable-process)
- [Snell envelope](#snell-envelope)
  - [Snell envelope of a multiplicative process](#snell-envelope-of-a-multiplicative-process)
  - [Optimal stopping](#optimal-stopping)
    - [Uniform-offer stopping recursion](#uniform-offer-stopping-recursion)
    - [Smooth pasting](#smooth-pasting)
    - [Optimal stopping value function](#optimal-stopping-value-function)
      - [Convexity of a random-walk Snell value function](#convexity-of-a-random-walk-snell-value-function)
      - [Integrability of translated convex random-walk rewards](#integrability-of-translated-convex-random-walk-rewards)
  - [Optimal stopping time](#optimal-stopping-time)
  - [Complementarity for the Snell envelope compensator](#complementarity-for-the-snell-envelope-compensator)
  - [Optimal stopping time from the compensator](#optimal-stopping-time-from-the-compensator)
- [Doob's martingale inequality](#doob-s-martingale-inequality)
- [Doob's martingale convergence theorems](#doob-s-martingale-convergence-theorems)

## Positive random-environment path-weight martingale

↑ **Parent:** [Martingale](martingale.md)

Let $\xi$ be a [random walk](markov-process.md#random-walk), [independent](random-variable.md#independent-random-variables) of centered, [independent](random-variable.md#independent-random-variables) time-space signs $h$, and let $0<\varepsilon<1$. Averaging over the walk gives a positive [martingale](martingale.md) in the environment [filtration](stochastic-process.md#filtration-probability-theory): each new time layer has conditional mean-one weight. Hence $\mathbb EZ_t=1$ and the [martingale convergence theorem](#martingale-convergence-theorem) gives a finite nonnegative almost-sure limit. Preserving its [mean](probability-theory.md#expected-value) requires an additional condition such as bounded [second moments](probability-theory.md#second-moment); positivity of finite-time weights alone does not suffice.

### Tail event for a vanishing positive path-weight limit

↑ **Parent:** [Positive random-environment path-weight martingale](#positive-random-environment-path-weight-martingale)

Delete the first $m$ environment factors from the path-weight expectation and call the result $Z_T^{(m)}$. Pointwise, $(1-\varepsilon)^mZ_T^{(m)}\le Z_T\le(1+\varepsilon)^mZ_T^{(m)}$. Thus $\{\liminf_TZ_T=0\}$ equals $\{\liminf_TZ_T^{(m)}=0\}$ and belongs to every future-time environment sigma-algebra. The [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law) makes its probability zero or one. If the nonnegative [martingale](martingale.md) limit has [mean](probability-theory.md#expected-value) one, the probability cannot be one, so its limit is strictly positive almost surely. The pointwise comparison establishes a genuine [tail event](probability-theory.md#tail-event), rather than merely invariance outside an unspecified exceptional set.

### Collision-count second moment for independent path weights

↑ **Parent:** [Positive random-environment path-weight martingale](#positive-random-environment-path-weight-martingale)

Here $I_t=\sum_{j=1}^t\mathbf1_{\{\xi_j^{(1)}=\xi_j^{(2)}\}}$ counts simultaneous collisions of two [independent](random-variable.md#independent-random-variables) walks. A shared environment sign contributes $\mathbb E(1+\varepsilon h)^2=1+\varepsilon^2$; distinct signs contribute one. If the difference walk returns to zero with probability $\rho<1$, its total number of positive-time returns has law $\mathbb P(I_\infty=k)=(1-\rho)\rho^k$. Therefore the [second moments](probability-theory.md#second-moment) are bounded by $(1-\rho)/(1-\rho(1+\varepsilon^2))$ whenever $\rho(1+\varepsilon^2)<1$. [Convergence in L2](convergence-of-random-variables.md#convergence-in-l2) then preserves the limit's [mean](probability-theory.md#expected-value) one.

## Bernstein bound for bounded-jump martingales

↑ **Parent:** [Martingale](martingale.md)

For a compensated jump [martingale](martingale.md) starting at zero, with jumps bounded in absolute value by $c$ and [predictable quadratic variation](stochastic-calculus.md#predictable-quadratic-variation) at most $v$ on the interval, the displayed maximal bound holds. For $0<\theta c<3$, the elementary exponential bound

$$
e^{\theta h}-1-\theta h\le\frac{\theta^2h^2}{2(1-\theta c/3)}\qquad(|h|\le c)
$$

makes the exponential of $\theta M$ minus that multiple of its predictable bracket a nonnegative supermartingale. Stop at the first crossing of $\eta$ and use its mean bound. Taking $\theta=\eta/(v+c\eta/3)$ yields the one-sided bound; apply the same argument to $-M$ and use the [union bound](probability-inequality.md#boole-s-inequality) for the displayed two-sided version. The elementary estimate follows from the exponential series and $k!\ge2\,3^{k-2}$ for $k\ge2$. If $v=0$, the compensated martingale is constant and the crossing probability is zero; the parameter choice above is needed only for $v>0$.

## Ville inequality

↑ **Parent:** [Martingale](martingale.md)

For a nonnegative [martingale](martingale.md), the displayed maximal probability bound follows by stopping at the first crossing of $a$. The stopped expectation is at most its initial expectation, and on the crossing event its value is at least $a$. Bound the stopping time first and pass to the limit using nonnegativity. This form is useful for the [Poisson maximal concentration bound](probability-theory.md#poisson-maximal-concentration-bound).

## Finite voter-model consensus probability

↑ **Parent:** [Martingale](martingale.md)

In a finite population that repeatedly lets one uniformly chosen individual copy a uniformly chosen distinct individual, the fraction of either type is a bounded [martingale](martingale.md). Conditional probabilities of an increase and decrease coincide. Absorption at one of the two unanimous states occurs almost surely, since from every state there is a uniformly positive probability of reaching unanimity in a fixed finite block of updates. Bounded convergence implies that the probability of eventual unanimity of one type equals its initial fraction.

## Unchanging betting probability under sampling without replacement

↑ **Parent:** [Martingale](martingale.md)

In a uniformly shuffled deck with $r$ red and $b$ black cards remaining, the conditional probability that the next two are red is $q(r,b)$. If at least three cards remain, $q(r,b)$ is the weighted average of $q(r-1,b)$ and $q(r,b-1)$ after one reveal. Hence these probabilities form a bounded [martingale](martingale.md) until only two cards remain. Any adapted choice of exactly one betting time before that deadline has the same winning probability by bounded [optional stopping](#optional-sampling-theorem-for-a-supermartingale). Waiting creates no advantage when a bet must eventually be made.

## Nonnegative martingale

↑ **Parent:** [Martingale](martingale.md)

A nonnegative [martingale](martingale.md) takes nonnegative values [almost surely](convergence-of-random-variables.md#almost-sure-convergence) at each time. In discrete time its [expectations](probability-theory.md#expected-value) are constant, so it is bounded in $L^1$ and the [martingale convergence theorem](#martingale-convergence-theorem) gives a finite integrable almost sure limit. Its [expectations](probability-theory.md#expected-value) need not converge to the [expectation](probability-theory.md#expected-value) of that limit; [uniform integrability](convergence-of-random-variables.md#uniform-integrability) is needed for [convergence in L1](convergence-of-random-variables.md#convergence-in-l1).

## Doob exposure martingale

↑ **Parent:** [Martingale](martingale.md)

Expose independent coordinates successively and take the conditional mean of a function after each exposure. These conditional means form a [martingale](martingale.md) from $\mathbb Ef$ to $f$. A coordinate oscillation bound $c_i$ gives a conditional interval of length $c_i$ for the corresponding increment, by coupling the unexposed coordinates. Applying the [Hoeffding lemma](probability-inequality.md#hoeffding-lemma) to these conditional ranges proves the [McDiarmid inequality](probability-inequality.md#mcdiarmid-s-inequality).

## Rare-jump martingale divergence

↑ **Parent:** [Martingale](martingale.md)

A [martingale](martingale.md) can diverge to $+\infty$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence) when its increments are finite but not uniformly bounded. For independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) with $\mathbb P(Y_n=1)=2^{-n}$,

$$
X_n=\sum_{k=1}^n(1-2^kY_k)
$$

has centered integrable increments. The [First Borel-Cantelli lemma](probability-theory.md#borel-cantelli-first-lemma) makes the rare negative jumps occur only finitely often, after which every increment equals one. The expectation remains zero at every finite time despite this pathwise divergence.

## Characterization of a martingale by bounded continuous-time stopped expectations

↑ **Parent:** [Martingale](martingale.md)

An integrable [adapted process](stochastic-process.md#adapted-process) is a [martingale](martingale.md) if all its values at [bounded stopping times](#bounded-stopping-time) are integrable with the same [expectation](probability-theory.md#expected-value) as $X_0$. For the converse, compare deterministic $t$ with $U=s\mathbf1_A+t\mathbf1_{A^c}$, where $s<t$ and $A\in\mathcal F_s$. The resulting identity $\mathbb E[(X_t-X_s)\mathbf1_A]=0$ is precisely the defining test for [conditional expectation](measure-theory.md#conditional-expectation). In the forward direction, use the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) for a [càdlàg martingale](#cadlag-martingale) under the [usual conditions for a filtration](stochastic-process.md#usual-conditions-for-a-filtration).

<h2 id="azuma-s-inequality">Azuma's inequality</h2>

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Azuma's_inequality)

If a [martingale](martingale.md) has increments with $|M_i-M_{i-1}|\leq c_i$ almost surely for deterministic $c_i$, then each one-sided deviation of magnitude $t>0$ from $M_0$ has [probability](probability-theory.md#probability) at most $\exp(-t^2/(2\sum_i c_i^2))$. If all $c_i$ vanish, the [martingale](martingale.md) is constant. The inequality gives concentration from bounded increments without requiring independent increments.

### Two-sided Azuma-Hoeffding inequality

↑ **Parent:** [Azuma's inequality](#azuma-s-inequality)

For deterministic bounds $|M_k-M_{k-1}|\le c_k$, the conditional mean-zero increment has exponential moment at most $e^{\theta^2c_k^2/2}$. Iteration, the [Markov inequality](probability-inequality.md#markov-inequality) and optimization at $\theta=x/\sum c_k^2$ give each one-sided tail, and the [union bound](probability-inequality.md#boole-s-inequality) gives the displayed inequality. The factor two in the exponent denominator cannot be omitted: a single symmetric increment of size one has absolute deviation one with probability one.

## Martingale increments obstruct finite convergence

↑ **Parent:** [Martingale](martingale.md)

If a real sequence converges finitely, its successive increments tend to zero. A [martingale](martingale.md) whose increments stay bounded away from zero on every sample path cannot have a finite almost-sure limit, regardless of its zero conditional mean increments.

## Absorption at zero of a nonnegative martingale

↑ **Parent:** [Martingale](martingale.md)

Once a nonnegative [martingale](martingale.md) hits zero, it stays zero almost surely. [Conditional expectation](measure-theory.md#conditional-expectation) on $\{M_n=0\}$ gives $\mathbb E[M_{n+1}\mathbf1_{\{M_n=0\}}]=0$; nonnegativity forces the next value to vanish there. A countable intersection makes these assertions simultaneous for all times, proving absorption at the first zero.

### Absorption-time bound from conditional variance and overshoot

↑ **Parent:** [Absorption at zero of a nonnegative martingale](#absorption-at-zero-of-a-nonnegative-martingale)

Let a nonnegative [martingale](martingale.md) start at one, let $T$ be its first zero, and let $T_R$ be its first hit of $[R,\infty)$. Suppose $\mathbb E[(M_{n+1}-M_n)^2\mid\mathcal F_n]\geq\sigma^2\mathbf1_{\{T>n\}}$ and $M_{T_R}\leq\tau R$ on finite hits, for thresholds $R\geq1$. Then $M_{T\wedge T_R\wedge n}^2-\sigma^2(T\wedge T_R\wedge n)$ is a [submartingale](#submartingale). The bounded stopped values have mean one, so their second moment is at most $\tau R$. Consequently $\mathbb E(T\wedge T_R)\leq(\tau R-1)/\sigma^2$. For $\tau\geq1$ this implies the weaker bound $\tau^2R/\sigma^2$. The threshold restriction prevents an impossible overshoot requirement below the starting value.

#### Square-root tail bound for martingale absorption

↑ **Parent:** [Absorption-time bound from conditional variance and overshoot](#absorption-time-bound-from-conditional-variance-and-overshoot)

Under the conditional-[variance](variance.md) and overshoot assumptions of the [absorption-time bound from conditional variance and overshoot](#absorption-time-bound-from-conditional-variance-and-overshoot), $\mathbb P(T>n)\leq2\tau/(\sigma\sqrt n)$. Bound the probability by $\mathbb P(T_R<\infty)+\mathbb E(T\wedge T_R)/n$ and optimize $1/R+\tau^2R/(\sigma^2n)$. If the resulting bound is below one, its minimizing threshold is greater than one; otherwise the probability bound is trivial.

## Martingale difference sequence

↑ **Parent:** [Martingale](martingale.md)

A martingale difference sequence is an [adapted](stochastic-process.md#adapted-process) sequence of integrable random variables $D_n$, $n\geq1$, with $\mathbb E[D_n\mid\mathcal F_{n-1}]=0$. Its partial sums are a [martingale](martingale.md), and martingale increments give such sequences. If the differences are square-integrable, they are [uncorrelated random variables](variance.md#uncorrelated-random-variables): for $j<k$, conditioning on $\mathcal F_{k-1}$ gives $\mathbb E D_jD_k=0$.

### Martingale difference

↑ **Parent:** [Martingale difference sequence](#martingale-difference-sequence)

A time-indexed increment $D_j$ with $\mathbb E(D_j\mid\mathcal F_{j-1})=0$ is a martingale difference relative to its history. Square-integrable differences at different indices are orthogonal, allowing their conditional variances to accumulate. They need not be independent.

### Strong law for martingales with bounded increments

↑ **Parent:** [Martingale difference sequence](#martingale-difference-sequence)

If a [martingale](martingale.md) has increments bounded by a single deterministic constant, then $M_n/n\to0$ almost surely. Its increments form a uniformly $L^2$-bounded [martingale difference sequence](#martingale-difference-sequence); apply the [strong law for uniformly L2-bounded uncorrelated random variables](convergence-of-random-variables.md#strong-law-for-uniformly-l2-bounded-uncorrelated-random-variables) to their partial sums and note $M_0/n\to0$. No square-integrability of the initial value is needed beyond the usual martingale integrability.

## Dyadic slope martingale

↑ **Parent:** [Martingale](martingale.md)

For a real [continuous function](calculus.md#continuous-function) $f$ on $[0,1]$, let $G_n$ be its secant slope on each length-$2^{-n}$ dyadic cell. Regard $([0,1],\mathcal B,dt)$ as a [probability space](probability-theory.md#probability-space) and use the [filtration](stochastic-process.md#filtration-probability-theory) of half-open dyadic cells with the endpoint $\{1\}$ as a separate null cell. The mean of the two child slopes equals the parent slope, so $(G_n)$ is a [martingale](martingale.md). Its [integral](calculus.md#integral) gives the [linear interpolation](function.md#linear-interpolation) of $f$ on that grid. If $f$ is [Lipschitz continuous](real-analysis.md#lipschitz-continuity), these slopes are bounded by its [Lipschitz constant](real-analysis.md#lipschitz-constant); the [Lp martingale convergence theorem](#lp-martingale-convergence-theorem) then supplies a bounded [integral](calculus.md#integral) density for $f$.

## Fair-coin doubling martingale

↑ **Parent:** [Martingale](martingale.md)

For fair [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $\xi_j$ with the [Bernoulli distribution](discrete-probability-distribution.md#bernoulli-distribution), $M_n=2^n\mathbf1_{\{\xi_1=\cdots=\xi_n=1\}}$ is a nonnegative [martingale](martingale.md). It has [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) to zero but $\mathbb E M_n=1$, so it lacks [convergence in L1](convergence-of-random-variables.md#convergence-in-l1).

## Martingale-difference orthogonality

↑ **Parent:** [Martingale](martingale.md)

If $(M_n)$ is a square-integrable [martingale](martingale.md), then its increments are orthogonal in $L^2$: for $i<j$,

$$
\mathbb E[(M_i-M_{i-1})(M_j-M_{j-1})]=0.
$$

More generally, multiplying the later increment by any square-integrable quantity measurable before it still gives expectation zero whenever the product is integrable.

## Submartingale

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Submartingale)

An integrable adapted process $(X_n)$ is a submartingale when

$$
\mathbb E[X_{n+1}\mid\mathcal F_n]\geq X_n.
$$

### Positive martingale majorant of an L1-bounded submartingale

↑ **Parent:** [Submartingale](#submartingale)

For a [submartingale](#submartingale) with $\sup_n\mathbb E|X_n|=C<\infty$, its [positive part](function.md#positive-part-of-a-real-valued-function) is a [submartingale](#submartingale) by the [conditional Jensen inequality](measure-theory.md#conditional-jensen-inequality). Thus the displayed [conditional expectations](measure-theory.md#conditional-expectation) increase in $p$. Their limits are finite [almost surely](convergence-of-random-variables.md#almost-sure-convergence) and have [expectations](probability-theory.md#expected-value) at most $C$, by the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem). Conditional monotone convergence and the [tower property of conditional expectation](measure-theory.md#law-of-total-expectation) give $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$. Moreover $M_n\geq X_n^+$. Consequently $Y_n=M_n-X_n$ is a nonnegative [supermartingale](#supermartingale), $\sup_n\mathbb E Y_n\leq2C$, and $X=M-Y$. The resulting [martingale](martingale.md) need not have [uniform integrability](convergence-of-random-variables.md#uniform-integrability).

### Doob-Meyer decomposition theorem

↑ **Parent:** [Submartingale](#submartingale)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doob–Meyer_decomposition_theorem)

Under the usual filtration conditions, a càdlàg submartingale of [Class D](convergence-of-random-variables.md#class-d-process) on a finite horizon has a unique decomposition into a uniformly integrable martingale and a predictable integrable nondecreasing process starting at zero. A general [continuous semimartingale decomposition](stochastic-calculus.md#continuous-semimartingale-decomposition) instead allows an arbitrary continuous finite-variation drift. A convex function of a semimartingale need not be a submartingale when that drift has unrestricted sign.

### Doob maximal inequality for a nonnegative submartingale

↑ **Parent:** [Submartingale](#submartingale)

If $(X_m)_{m\leq n}$ is a nonnegative [submartingale](#submartingale), then for every $a>0$,

$$
a\,\mathbb P\left(\max_{m\leq n}X_m\geq a\right)
\leq\mathbb E[X_n].
$$

Stop at the first crossing of $a$ and use the submartingale property on that event.

#### Truncated layer-cake proof of the L2 maximal inequality

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For a nonnegative [submartingale](#submartingale) with maximum $M_t$, the first-moment maximal estimate is $\lambda\mathbb P(M_t\geq\lambda)\leq\mathbb E[X_t\mathbf1_{\{M_t\geq\lambda\}}]$. Integrate $2\lambda$ times the tail probability only up to $R$, obtaining $\mathbb E(M_t\wedge R)^2\leq2\mathbb E[X_t(M_t\wedge R)]$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $\|M_t\wedge R\|_2\leq2\|X_t\|_2$, and [monotone convergence](measure-theory.md#monotone-convergence-theorem) gives the result as $R\to\infty$. Truncation avoids assuming beforehand that the maximum has a finite second moment.

// Target: brownian-motion.bigb

#### One-sided martingale maximal inequality

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For a [square-integrable](measure-theory.md#square-integrable-function) [martingale](martingale.md) with $M_0=0$ and $V=\mathbb EM_n^2$, apply the [Doob maximal inequality](#doob-maximal-inequality-for-a-nonnegative-submartingale) to $(M_k+c)^2$ for $c\geq0$. An upper crossing of $x$ implies a square crossing of $(x+c)^2$, giving $(V+c^2)/(x+c)^2$. Minimization at $c=V/x$ gives the displayed bound. A one-step [martingale](martingale.md) taking $x$ with probability $V/(V+x^2)$ and $-V/x$ otherwise attains equality when $V>0$.

#### Kolmogorov maximal inequality

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For [independent](random-variable.md#independent-random-variables) zero-mean [square-integrable](measure-theory.md#square-integrable-function) increments, their partial sums form a [martingale](martingale.md), and their squares form a nonnegative [submartingale](#submartingale). Apply the [Doob maximal inequality](#doob-maximal-inequality-for-a-nonnegative-submartingale) to the squared process at threshold $x^2$. [Independence](random-variable.md#independent-random-variables) and zero [means](probability-theory.md#expected-value) make its terminal [second moment](probability-theory.md#second-moment) the sum of the increment [variances](variance.md). Identical distributions are not required.

#### One-sided maximal inequality for a centered square-integrable martingale

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For a centered square-integrable [martingale](martingale.md) with $v=\mathbb E M_n^2$ and $\lambda>0$, apply the [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale) to $(M_k+c)^2$ for $c\geq0$. [Conditional Jensen inequality](measure-theory.md#conditional-jensen-inequality) gives the [submartingale](#submartingale) property, and crossing $\lambda$ forces its square above $(\lambda+c)^2$. The bound $(v+c^2)/(\lambda+c)^2$ is minimized by $c=v/\lambda$. This extends the [Cantelli inequality](probability-inequality.md#cantelli-inequality) from one [random variable](random-variable.md) to a [martingale](martingale.md) maximum, without requiring [independent increments](stochastic-process.md#independent-increments).

#### Maximal bound for a nonnegative martingale

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For a nonnegative [martingale](martingale.md), $T_R=\inf\{n:M_n\geq R\}$ satisfies $\mathbb P(T_R<\infty)\leq\mathbb E M_0/R$. Stop at $T_R\wedge n$ and use nonnegativity before passing to the increasing event. A limit of thresholds from below also gives the bound for $\{\sup_nM_n\geq R\}$ even when the supremum is not attained.

#### One-sided maximal inequality for independent centered sums

↑ **Parent:** [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale)

For independent centered random variables and $S_m=\sum_{j\leq m}X_j$,

$$
\mathbb P\left(\max_{m\leq n}S_m\geq x\right)
\leq\frac{\operatorname{Var}(S_n)}
{\operatorname{Var}(S_n)+x^2}.
$$

Apply the [Doob maximal inequality for a nonnegative submartingale](#doob-maximal-inequality-for-a-nonnegative-submartingale) to $(S_m+c)^2$ and optimize at $c=\operatorname{Var}(S_n)/x$.

## Square martingale for independent centered sums

↑ **Parent:** [Martingale](martingale.md)

For independent centered square-integrable variables, if $S_n=\sum_{m\leq n}X_m$ and $V_n=\operatorname{Var}(S_n)$, then

$$
S_n^2-V_n
$$

is a [martingale](martingale.md).

### Small-ball maximal bound for sums with bounded increments

↑ **Parent:** [Square martingale for independent centered sums](#square-martingale-for-independent-centered-sums)

If additionally $|X_m|\leq K$, then

$$
\mathbb P\left(\max_{m\leq n}|S_m|\leq x\right)
\leq\frac{(x+K)^2}{\operatorname{Var}(S_n)}.
$$

Stop the [square martingale for independent centered sums](#square-martingale-for-independent-centered-sums) at the first exit from $[-x,x]$ or at time $n$.

## Conditional-expectation martingale

↑ **Parent:** [Martingale](martingale.md)

For an integrable random variable $Z$ and an increasing [filtration](stochastic-process.md#filtration-probability-theory) $(\mathcal F_n)$, the process $M_n=\mathbb E[Z\mid\mathcal F_n]$ is a [martingale](martingale.md). The [tower property of conditional expectation](measure-theory.md#law-of-total-expectation) gives the martingale identity.

### Edge-exposure martingale

↑ **Parent:** [Conditional-expectation martingale](#conditional-expectation-martingale)

Expose the independent [edge](graph-theory.md#edge-of-a-graph) indicators of a [binomial random graph](graph-theory.md#binomial-random-graph) in a fixed order, and set $M_i=\mathbb E[Z\mid\text{the first }i\text{ indicators}]$ for an integrable statistic $Z$. This is a [martingale](martingale.md) from $\mathbb EZ$ to $Z$. If changing one [edge](graph-theory.md#edge-of-a-graph) changes $Z$ by at most $c$, coupling the unexposed indicators gives $|M_i-M_{i-1}|\leq c$, permitting the [Azuma-Hoeffding inequality](#azuma-s-inequality).

## Product martingale from independent mean-one factors

↑ **Parent:** [Martingale](martingale.md)

If $Y_1,Y_2,\ldots$ are independent integrable random variables with $\mathbb E[Y_i]=1$, then

$$
M_n=\prod_{i=1}^nY_i
$$

is a martingale for $\mathcal F_n=\sigma(Y_1,\ldots,Y_n)$, because independence gives $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n\mathbb E[Y_{n+1}]=M_n$.

## Continuous-time martingale

↑ **Parent:** [Martingale](martingale.md)

An adapted integrable process $(M_t)_{t\geq0}$ is a continuous-time martingale when $\mathbb E[M_t\mid\mathcal F_s]=M_s$ for every $s\leq t$.

### Uniform-arrival residual mass martingale

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)

For finitely many independent uniform arrival times on $[0,1]$, and fixed positive weights, normalize the unarrived mass by the remaining time. Conditional on not having arrived by $s$, each arrival remains uniform on $(s,1)$, giving the [martingale](martingale.md) identity. The process is [càdlàg](calculus.md#cadlag), nonnegative, and has constant mean equal to the total weight. It vanishes eventually before time one on each typical path, so it is not [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) when the total weight is positive.

#### Finite-jump boundary crossing identity

↑ **Parent:** [Uniform-arrival residual mass martingale](#uniform-arrival-residual-mass-martingale)

For the [uniform-arrival residual mass martingale](#uniform-arrival-residual-mass-martingale) with total weight $0<S<1$, the first crossing of level one happens continuously: its only jumps are downward, and an arrival almost surely misses the finitely many deterministic possible crossing times. Stop at that crossing or at $r<1$. The stopped values lie between zero and one, and their limit as $r\uparrow1$ is the crossing indicator. [Optional stopping](#optional-sampling-theorem-for-a-supermartingale) and [dominated convergence](measure-theory.md#dominated-convergence-theorem) identify its [probability](probability-theory.md#probability) as $S$. At $S=1$ the strict boundary inequality already fails at time zero.

### Uniformly integrable martingale

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)

A [martingale](martingale.md) whose values over its whole time interval form a [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) family has an integrable terminal limit and is closed by that limit. Conversely, conditional expectations of an integrable terminal variable form a [uniformly integrable martingale](#uniformly-integrable-martingale), by [uniform integrability of conditional expectations](convergence-of-random-variables.md#uniform-integrability-of-conditional-expectations). For [continuous martingales](#continuous-martingale), one may equivalently use [uniform integrability](convergence-of-random-variables.md#uniform-integrability) of the family stopped at finite stopping times.

<h3 id="cadlag-martingale">Càdlàg martingale</h3>

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)

A [càdlàg martingale](#cadlag-martingale) is a continuous-time [martingale](martingale.md) represented by a [càdlàg process](stochastic-process.md#cadlag-process): its paths are right-continuous and have finite left limits at positive times, on one common probability-one event. This path regularity permits approximation of [stopping times](#stopping-time) from above.

### Continuous martingale

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)

A [continuous martingale](#continuous-martingale) is a [continuous-time martingale](#continuous-time-martingale) whose paths are continuous outside one null event. Continuity does not remove the integrability or conditional-expectation requirements in the [martingale](martingale.md) definition.

### L2-bounded continuous martingale

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)

A continuous [martingale](martingale.md) $M$ is L2-bounded when $\sup_{t\geq0}\mathbb E|M_t|^2<\infty$. The [L2 martingale convergence theorem](#l2-martingale-convergence-theorem) gives a terminal value $M_\infty$ with convergence in $L^2$ and [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence). The resulting [conditional expectation](measure-theory.md#conditional-expectation) identity is $M_t=\mathbb E[M_\infty\mid\mathcal F_t]$. Boundedness on each separate finite horizon is a weaker condition. The subspace with $M_0=0$ is commonly denoted $\mathcal M_0^2$.

#### Integrable terminal bracket criterion

↑ **Parent:** [L2-bounded continuous martingale](#l2-bounded-continuous-martingale)

For a [continuous local martingale](#continuous-local-martingale) starting at zero, finite expected terminal [quadratic variation](stochastic-calculus.md#quadratic-variation) is equivalent to being an [L2-bounded continuous martingale](#l2-bounded-continuous-martingale). Stop at bounded path and bracket levels and use $\mathbb E(M_t^\tau)^2=\mathbb E[M]_{t\wedge\tau}$. Uniform integrability removes the localization; [Doob L2 maximal inequality](#doob-l2-maximal-inequality) justifies convergence of squares. The terminal identity is $\mathbb E M_\infty^2=\mathbb E[M]_\infty$. For nonzero initial values one must additionally assume $M_0\in L^2$.

#### Equivalent terminal and maximal norms for L2-bounded continuous martingales

↑ **Parent:** [L2-bounded continuous martingale](#l2-bounded-continuous-martingale)

For a [L2-bounded continuous martingale](#l2-bounded-continuous-martingale), the terminal and maximal [norms](functional-analysis.md#norm) satisfy

$$
\|M_\infty\|_2\leq\left\|\sup_{t\geq0}|M_t|\right\|_2\leq2\|M_\infty\|_2.
$$

The first inequality follows from [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence). Apply the [Doob L2 maximal inequality](#doob-l2-maximal-inequality) on $[0,T]$ and then the [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) as $T\to\infty$ for the second. These are [equivalent norms](functional-analysis.md#equivalent-norms) on the space modulo [indistinguishability of stochastic processes](stochastic-process.md#indistinguishability-of-stochastic-processes); neither inequality needs a zero initial value.

### Local martingale

↑ **Parent:** [Continuous-time martingale](#continuous-time-martingale)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Local_martingale)

An adapted process $M$ is a local martingale when there are stopping times $T_n\uparrow\infty$ almost surely such that each stopped process $M_{t\wedge T_n}$ is a martingale. Every martingale is local, while a positive local martingale is a supermartingale.

#### Bounded local martingale criterion

↑ **Parent:** [Local martingale](#local-martingale)

A uniformly bounded [local martingale](#local-martingale) is a true [uniformly integrable martingale](#uniformly-integrable-martingale): a [localizing sequence](#localizing-sequence) gives uniformly dominated stopped values, so their conditional identities pass to the limit. A deterministic bound on each compact time interval gives a true [martingale](martingale.md) on each such interval, even when the bound grows with time.

#### Integrable discrete-time local martingale is a martingale

↑ **Parent:** [Local martingale](#local-martingale)

An integrable discrete-time [local martingale](#local-martingale) is a true [martingale](martingale.md). Its stopped increments have the form $\mathbf1_{\{\tau\geq t\}}(X_t-X_{t-1})$, and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) removes a [localizing sequence](#localizing-sequence) from the conditional increment identity.

##### Nonnegative discrete-time local martingale is a martingale

↑ **Parent:** [Integrable discrete-time local martingale is a martingale](#integrable-discrete-time-local-martingale-is-a-martingale)

The [Fatou lemma](measure-theory.md#fatou-s-lemma) makes every time value of a nonnegative discrete-time [local martingale](#local-martingale) integrable, assuming the usual integrable initial value. The integrable discrete-time result then makes it a true [martingale](martingale.md).

#### Strict local martingale

↑ **Parent:** [Local martingale](#local-martingale)

A strict local martingale is a [local martingale](#local-martingale) that is not a true [martingale](martingale.md). The reciprocal of a three-dimensional [Bessel process](brownian-motion.md#bessel-process) is an example: it is a nonnegative [continuous local martingale](#continuous-local-martingale) whose [expectation](probability-theory.md#expected-value) decreases strictly.

##### Logarithm of planar Brownian radius

↑ **Parent:** [Strict local martingale](#strict-local-martingale)

For planar Brownian motion started at zero, $\log|B_t|$, considered from time one onward, is a local martingale because $\log|x|$ is harmonic off the polar point zero. Every fixed-time absolute moment is finite, but $\mathbb EX_t=\frac12\log t+\mathbb E\log|B_1|$ increases. It is therefore not a true martingale. Finite moments at individual times do not establish class DL.

// Target: probability-and-statistics.bigb

#### Localizing sequence

↑ **Parent:** [Local martingale](#local-martingale)

A localizing sequence for a [local martingale](#local-martingale) $M$ is an increasing sequence of [stopping times](#stopping-time) $T_n\uparrow\infty$ almost surely such that every stopped process $M^{T_n}$ is a true martingale. One can often choose the times so that the stopped processes are bounded.

#### Continuous local martingale

↑ **Parent:** [Local martingale](#local-martingale)

A continuous local martingale is a [local martingale](#local-martingale) whose sample paths are continuous almost surely. Its [quadratic variation](stochastic-calculus.md#quadratic-variation) determines much of its pathwise behaviour.

##### Finite-variation smooth transform of a continuous local martingale

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

If $M$ is a [continuous local martingale](#continuous-local-martingale) and $f\in C^2(\mathbb R)$, then [finite variation](real-analysis.md#total-variation-of-a-function) of $f(M)$ forces $f(M_t)=f(M_0)$. The [Itô formula](stochastic-calculus.md#ito-s-lemma) and the [quadratic variation of a stochastic integral](stochastic-calculus.md#quadratic-variation-of-a-stochastic-integral) give $\int_0^t f'(M_s)^2d[M]_s=0$. The [occupation-times formula](brownian-motion.md#occupation-times-formula) implies that $L_t^a(M)=0$ almost everywhere where $f'(a)\ne0$. On the zero set of $f'$, its derivative $f''$ vanishes almost everywhere: zeros at which $f''\ne0$ are isolated and hence countable. Thus $\int_0^t|f''(M_s)|d[M]_s=\int |f''(a)|L_t^a(M)da=0$. Both terms in the [Itô formula](stochastic-calculus.md#ito-s-lemma) vanish.

##### Exponential criterion for a continuous local martingale and its bracket

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

Suppose $X,A$ are continuous, start at zero, and $A$ is increasing. If $e^{X-A/2}$ and $e^{-X-A/2}$ are [local martingales](#local-martingale), their logarithms first recover adaptation of $X,A$ and the [semimartingale](stochastic-calculus.md#semimartingale) property of $X$. In the decomposition $X=N+V$, the two Itô drift measures give $dV+(d[N]-dA)/2=0$ and $-dV+(d[N]-dA)/2=0$. Thus $V=0$ and $[X]=A$. All real exponential parameters may be assumed, but these two suffice.

##### Conditionally symmetric increments

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

A process has conditionally symmetric increments if, for all deterministic $s\le t$ and bounded measurable $g$,

$$
\mathbb E[g(X_t-X_s)\mid\mathcal F_s]=\mathbb E[g(X_s-X_t)\mid\mathcal F_s].
$$

Equivalently, the [conditional characteristic function](probability-theory.md#conditional-characteristic-function) of every increment is invariant under changing the sign of its argument. This property is stronger than unconditional symmetry and is different from [independent increments](stochastic-process.md#independent-increments). It supplies identities between positive and negative exponential terminal martingales.

###### Characteristic function under conditionally symmetric martingale increments

↑ **Parent:** [Conditionally symmetric increments](#conditionally-symmetric-increments)

Suppose $X$ is a continuous local martingale starting at zero, with [conditionally symmetric increments](#conditionally-symmetric-increments), and terminal conditional expectations have continuous martingale versions. Then

$$
\mathbb E e^{i\theta X_T}=\mathbb E e^{-\theta^2\langle X\rangle_T/2}.
$$

To prove this, set $M_t=\mathbb E[e^{i\theta X_T}\mid\mathcal F_t]$. Symmetry makes $e^{-2i\theta X_t}M_t$ a martingale, and the [Itô product rule](stochastic-calculus.md#ito-product-rule) gives $d\langle M,X\rangle=i\theta M\,d\langle X\rangle$. Consequently $e^{-i\theta X_t-\theta^2\langle X\rangle_t/2}M_t$ is a bounded local martingale, hence a martingale. Evaluating at the endpoints proves the formula. If also $X_T\sim N(0,T)$ for all $T$, the values of the bracket [Laplace transform](analysis.md#laplace-transform) at $1$ and $2$ force $\langle X\rangle_T=T$ almost surely. Continuity and the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion) then identify $X$ as [Brownian motion](brownian-motion.md).

##### Finite-bracket convergence lemma

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

A continuous local martingale converges to a finite limit on the event that its terminal bracket is finite. Stopping at each integer bracket level gives an L2-bounded martingale and its almost sure limit. On the finite-bracket event, some such stopped process coincides with the original process forever. This supplies terminal values for a finite DDS lifetime.

##### Fourth-moment deficit and bracket variance identity

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

The polynomial $X^4-6X^2\langle X\rangle+3\langle X\rangle^2$ has zero Itô drift. Finite fourth maximal and second bracket moments make it a true martingale. If $\mathbb EX_t^2=t$ and $\operatorname{Cov}(X_t^2,\langle X\rangle_t)=0$, then $\mathbb EX_t^4=3t^2-3\operatorname{Var}(\langle X\rangle_t)$. Equality at every time forces a deterministic clock and hence [Brownian motion](brownian-motion.md) by the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion).

##### Integrable-supremum martingale criterion

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

If a [local martingale](#local-martingale) has an integrable running absolute supremum on each fixed finite horizon, localization and conditional dominated convergence make it a true [martingale](martingale.md). This upgrades polynomial Itô local martingales when maximal moments and bracket moments control all terms.

##### Continuous local martingale with bounded quadratic variation

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

A [continuous local martingale](#continuous-local-martingale) $M$ with $M_0=0$ and deterministically bounded [quadratic variation](stochastic-calculus.md#quadratic-variation) on every finite horizon is a [square-integrable](measure-theory.md#square-integrable-function) [martingale](martingale.md), with $\mathbb EM_t^2=\mathbb E[M]_t$. Localization, the [Doob L2 maximal inequality](#doob-l2-maximal-inequality), and the resulting integrable bound on the squared supremum justify removing the [localizing sequence](#localizing-sequence).

##### Continuous finite-variation local martingale is constant

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)

A continuous [local martingale](#local-martingale) with [finite variation](real-analysis.md#total-variation-of-a-function) is almost surely constant. After localization, its [quadratic variation](stochastic-calculus.md#quadratic-variation) is both zero, because it has finite variation, and the quantity controlling its $L^2$ increments, because it is a martingale.

##### Dambis-Dubins-Schwarz theorem

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dambis-Dubins-Schwarz_theorem)

Let $M$ be a continuous local martingale with $M_0=0$ and $[M]_\infty=\infty$. For

$$
\tau_s=\inf\{t\geq0:[M]_t>s\},
$$

the process $B_s=M_{\tau_s}$ is [Brownian motion](brownian-motion.md) and

$$
M_t=B_{[M]_t}.
$$

When $[M]_\infty<\infty$, one can enlarge the probability space and continue $B$ independently beyond that time.

###### Cosine-exponential Brownian local martingale

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

For independent standard [Brownian motions](brownian-motion.md) $B,W$, [Itô formula](stochastic-calculus.md#ito-s-lemma) gives $dY=e^W\cos B\,dW-e^W\sin B\,dB$: the two second-order drifts cancel. Independence gives zero cross [quadratic covariation](stochastic-calculus.md#quadratic-covariation), so the displayed bracket follows. The process itself is not Brownian because its bracket is random. Its inverse-bracket time change is Brownian motion starting at one, in the time-changed [filtration](stochastic-process.md#filtration-probability-theory); subtracting one gives standard Brownian motion. The [Divergence of a driftless Brownian exponential clock](brownian-motion.md#divergence-of-a-driftless-brownian-exponential-clock) guarantees that the inverse is finite at every new time.

###### Gaussian terminal value at a deterministic bracket level

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

Let $M$ be a zero-starting [continuous local martingale](#continuous-local-martingale) and let $T<\infty$ be a [stopping time](#stopping-time) with $[M]_{t\wedge T}\le a$ and $[M]_T=a$ for a deterministic $a$. The complex exponential $\exp(iuM_{t\wedge T}+u^2[M]_{t\wedge T}/2)$ is a bounded [local martingale](#local-martingale), hence a true [martingale](martingale.md). Its terminal expectation is one, giving the [characteristic function](probability-theory.md#characteristic-function) $\mathbb E e^{iuM_T}=e^{-u^2a/2}$. Conditional optional sampling between two bracket levels also gives independent Gaussian increments in inverse-bracket time; Gaussian one-time marginals alone do not establish that independence.

###### Exit with drift controlled by quadratic variation

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

For a continuous local martingale $M$ with divergent bracket $K$ and a continuous drift $D$ satisfying $|D_t-D_s|\le C(K_t-K_s)$, the process $y+M+D$, $|y|<1$, exits $(-1,1)$ almost surely. In unit bracket time a Brownian increment of absolute size greater than $C+2$ forces exit within one unit, giving a geometric survival bound. The inverse bracket clock transfers this finite exit to ordinary time.

// Target: probability-and-statistics.bigb

###### Common-clock time change of orthogonal local martingales

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

If a continuous vector local martingale has bracket matrix $A_tI$ with $A_\infty=\infty$, inverse-clock time change gives bracket matrix $rI$. The [Lévy characterization of multidimensional Brownian motion](brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion) then gives Brownian motion in the common time-changed filtration. A continuous local martingale is constant on flat intervals of its bracket, so inverses using $A_t\geq r$ and $A_t>r$ give the same martingale values. The filtration at the earlier inverse is smaller; adaptation and independence from the larger past transfer the Brownian property to it. Nonzero initial values are retained by adding the initial vector back.

###### One-sided bound criterion for a martingale clock

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

A continuous [local martingale](#local-martingale) bounded above pathwise throughout a stochastic time interval cannot have infinite [quadratic variation](stochastic-calculus.md#quadratic-variation) at that interval's endpoint. The [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem) represents it as Brownian motion at its quadratic-variation clock; an infinite clock would force unbounded oscillations. Its clock therefore has a finite limit, and so does the martingale. A bound below gives the same conclusion by changing sign. The bound may be random; it must hold over the entire interval.

###### Finite-lifetime extension of the Dambis-Dubins-Schwarz theorem

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

Strict increase of a bracket does not force an infinite terminal value. Up to $L=\langle M\rangle_\infty$, the inverse-clock martingale continues at a finite lifetime by its terminal limit, with bracket $u\wedge L$. On an independent product extension, add $\int_0^u\mathbf1_{\{s>L\}}\,d\beta_s$. Its bracket fills $(u-L)^+$ and its cross variation with the original part vanishes. The result is Brownian for all clock times and still represents $M_t$.

###### Inverse-clock proof of the Dambis-Dubins-Schwarz theorem

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

For a continuous strictly increasing unbounded bracket $V$, the inverse times $T_u=\inf\{t:V_t>u\}$ satisfy $V_{T_u}=u$ and $T_{V_t}=t$. Optional sampling of the original martingale stopped at bounded bracket levels makes $M_{T_u}$ a continuous local martingale in $\mathcal F_{T_u}$. Time-changing the square-minus-bracket martingale gives its bracket $u$; the [Lévy characterization of Brownian motion](brownian-motion.md#levy-characterization-of-brownian-motion) identifies it as Brownian.

###### Stochastic-integral representation from absolutely continuous quadratic variation

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

If a continuous local martingale satisfies

$$
[M]_t=\int_0^tA_s\,ds
$$

for a nonnegative predictable process $A$, then, after enlarging the probability space if necessary, there is a Brownian motion $B$ such that

$$
M_t-M_0=\int_0^t\sqrt{A_s}\,dB_s.
$$

An independent Brownian motion supplies noise on the set where $A=0$.

###### Brownian motion produced by the Dambis-Dubins-Schwarz theorem need not be independent of its clock

↑ **Parent:** [Dambis-Dubins-Schwarz theorem](#dambis-dubins-schwarz-theorem)

The Brownian motion $B$ in $M_t=B_{[M]_t}$ is generally constructed from $M$, so it need not be independent of the [quadratic variation](stochastic-calculus.md#quadratic-variation) $[M]$. For example, $M_t=(W_t^2-t)/2=\int_0^tW_s\,dW_s$ has clock $\int_0^tW_s^2ds$, and their dependence can be detected by a nonzero mixed moment.

##### Burkholder-Davis-Gundy inequalities

↑ **Parent:** [Continuous local martingale](#continuous-local-martingale)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Burkholder-Davis-Gundy_inequalities)

For every $p>0$ there are constants $c_p,C_p>0$ such that a continuous local martingale $M$ with $M_0=0$ satisfies

$$
c_p\mathbb E[M]_T^{p/2}\leq\mathbb E\!\left[\sup_{t\leq T}|M_t|^p\right]\leq C_p\mathbb E[M]_T^{p/2}
$$

for every [stopping time](#stopping-time) $T$ for which the quantities are finite.

###### Upper maximal moment bound for a continuous local martingale

↑ **Parent:** [Burkholder-Davis-Gundy inequalities](#burkholder-davis-gundy-inequalities)

For $p\geq2$ and a continuous local martingale starting at zero, the [Itô formula](stochastic-calculus.md#ito-s-lemma) for $|X|^p$, the [Doob Lp maximal inequality](#doob-lp-maximal-inequality) and [Hölder's inequality](real-analysis.md#holder-s-inequality) yield $\mathbb E\sup_{s\leq t}|X_s|^p\leq C_p\mathbb E\langle X\rangle_t^{p/2}$. One possible constant is $C_p=[p(p-1)(p/(p-1))^p/2]^{p/2}$. Stop at increasing absolute-value levels to remove an initial boundedness assumption. This proves the upper half of the [Burkholder-Davis-Gundy inequalities](#burkholder-davis-gundy-inequalities) in this range.

#### Nonnegative local martingale

↑ **Parent:** [Local martingale](#local-martingale)

Every nonnegative [local martingale](#local-martingale) is a [supermartingale](#supermartingale). In particular, one that starts from zero is identically zero: its nonnegative value at every time has expectation at most zero.

##### Maximal identity for a continuous nonnegative local martingale tending to zero

↑ **Parent:** [Nonnegative local martingale](#nonnegative-local-martingale)

For $M_0=1$ and $M_t\to0$, stop at the infimum of strict crossings above $a>1$. Continuity bounds the stopped process by $a$ and makes its value at a finite crossing time exactly $a$. Its expectation remains one, and bounded convergence at infinity yields $\mathbb P(\sup M>a)=1/a$. The maximum has density $m^{-2}$ on $m>1$, with no endpoint atom.

##### Terminal expectation criterion for a nonnegative local martingale

↑ **Parent:** [Nonnegative local martingale](#nonnegative-local-martingale)

A [nonnegative local martingale](#nonnegative-local-martingale) is a [supermartingale](#supermartingale). If its integrable terminal limit has the same expectation as its initial value, conditional [Fatou lemma](measure-theory.md#fatou-s-lemma) gives $\mathbb E[Z_\infty\mid\mathcal F_t]\leq Z_t$, and equality of expectations makes this an equality. It is therefore a [uniformly integrable martingale](#uniformly-integrable-martingale).

## Doob L2 maximal inequality

↑ **Parent:** [Martingale](martingale.md)

For a square-integrable martingale starting at zero,

$$
\mathbb E\sup_{s\leq t}|M_s|^2\leq4\mathbb E|M_t|^2.
$$

For a continuous local martingale stopped so that its quadratic variation is integrable, the [Itô isometry](stochastic-calculus.md#ito-isometry) makes the right-hand side $4\mathbb E[M]_t$.

This is the $p=2$ specialization of [Doob's martingale inequality](#doob-s-martingale-inequality).

## Doob Lp maximal inequality

↑ **Parent:** [Martingale](martingale.md)

For $p>1$ and a martingale $(M_k)_{k\leq n}$,

$$
\left\|\max_{k\leq n}|M_k|\right\|_p
\leq\frac p{p-1}\|M_n\|_p.
$$

This strong $L^p$ bound is one form of [Doob's martingale inequality](#doob-s-martingale-inequality).

## L2 martingale convergence theorem

↑ **Parent:** [Martingale](martingale.md)

A martingale bounded in $L^2$ converges almost surely and in $L^2$ to a square-integrable limit. Orthogonality of its increments makes their squared $L^2$ norms summable.

## Symmetric signs forced by the martingale property

↑ **Parent:** [Martingale](martingale.md)

If every increment $\xi_n=M_n-M_{n-1}$ of a discrete martingale takes values in $\{-1,1\}$, then

$$
\mathbb P(\xi_n=1\mid\mathcal F_{n-1})
=\mathbb P(\xi_n=-1\mid\mathcal F_{n-1})=\frac12.
$$

Iterated conditioning shows that the increments are independent symmetric signs, so $M_n-M_0$ is a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk).

## Doob upcrossing inequality

↑ **Parent:** [Martingale](martingale.md)

If $(M_n)$ is a martingale and $U_N[a,b]$ counts its completed upcrossings of $[a,b]$ by time $N$, then

$$
(b-a)\mathbb E U_N[a,b]\leq\mathbb E(M_N-a)^-.
$$

Equivalent conventions may add an initial endpoint term.

### Dubins upcrossing inequality

↑ **Parent:** [Doob upcrossing inequality](#doob-upcrossing-inequality)

For a nonnegative [supermartingale](#supermartingale) and $0<a<b$, let $U$ count completed [upcrossings](#upcrossing) of $[a,b]$, allowing the first entry at time zero. The displayed bound holds for every integer $k\geq1$. Construct the [multiplicative upcrossing supermartingale](#multiplicative-upcrossing-supermartingale), stop at the $k$th completed crossing, and use its initial [expected value](probability-theory.md#expected-value) and nonnegativity. The bound is exponential in the number of crossings, and complements the first-moment [Doob upcrossing inequality](#doob-upcrossing-inequality).

#### Multiplicative upcrossing supermartingale

↑ **Parent:** [Dubins upcrossing inequality](#dubins-upcrossing-inequality)

Start with cash one, switch to $X/a$ when a nonnegative [supermartingale](#supermartingale) first reaches at most $a$, and switch to cash $q=b/a$ when it next reaches at least $b$. Repeat with coefficients multiplied by $q$ after every completed [upcrossing](#upcrossing). At each switch the new value is at most the old one, so [pasting supermartingales with downward jumps](#pasting-supermartingales-with-downward-jumps) gives a [supermartingale](#supermartingale) when stopped after any fixed number of switches. Its initial value is $\min(X_0/a,1)$, and its value at the $k$th completed crossing is exactly $q^k$. Applying its [expected value](probability-theory.md#expected-value) bound proves the [Dubins upcrossing inequality](#dubins-upcrossing-inequality).

### Upcrossing

↑ **Parent:** [Doob upcrossing inequality](#doob-upcrossing-inequality)

An [upcrossing](#upcrossing) of an interval $[a,b]$ consists of an observation at or below $a$ followed by a later observation at or above $b$. Successive completed [upcrossings](#upcrossing) use disjoint buy-sell pairs.

#### Upcrossing count

↑ **Parent:** [Upcrossing](#upcrossing)

The [upcrossing count](#upcrossing-count) $U_N[a,b]$ counts completed [upcrossings](#upcrossing) by time $N$, allowing the first purchase at time zero. For a [martingale](martingale.md), the [Doob upcrossing inequality](#doob-upcrossing-inequality) bounds its [expected value](probability-theory.md#expected-value) by $\mathbb E(M_N-a)^-/(b-a)$.

### Martingale convergence theorem

↑ **Parent:** [Doob upcrossing inequality](#doob-upcrossing-inequality)

A discrete-time martingale with $\sup_n\mathbb E|M_n|<\infty$ converges almost surely to an integrable random variable. If the martingale is [uniformly integrable](convergence-of-random-variables.md#uniform-integrability), convergence also holds in $L^1$.

This is one of [Doob's martingale convergence theorems](#doob-s-martingale-convergence-theorems); uniform integrability upgrades almost-sure convergence to convergence in mean.

#### Almost-sure martingale convergence to a nonintegrable limit

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

Let independent increments $\xi_k$ equal $4^k$ or $-4^k$ with probabilities $2^{-k-1}$ each, and zero otherwise. Every partial sum $M_n=\sum_{k\leq n}\xi_k$ is integrable and is a [martingale](martingale.md). The [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) makes only finitely many increments nonzero almost surely, so $M_n$ has a finite almost-sure limit $Y$. Yet $\mathbb E|Y|=\infty$: the disjoint events that only the $k$th increment is nonzero have probabilities at least $c2^{-k}$ for $c=\prod_j(1-2^{-j})>0$, and contribute at least $c2^k$ each. This does not contradict the [martingale convergence theorem](#martingale-convergence-theorem), whose integrability conclusion requires a uniform first-moment bound.

// Target: markov-process.bigb

#### L2-bounded martingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

An $L^2$-bounded real [martingale](martingale.md) has a square-integrable terminal value, converges to it almost surely and in $L^2$, and satisfies $M_t=\mathbb E[M_\infty\mid\mathcal F_t]$. The $L^2$ Cauchy property follows from orthogonality of increments and monotonicity of $\mathbb EM_t^2$. This terminal representation permits optional sampling at finite unbounded [stopping times](#stopping-time) and uniform-integrability control of stopped squares by conditional Jensen.

#### Coin-doubling martingale

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

For independent fair Bernoulli variables, this [nonnegative martingale](#nonnegative-martingale) starts at one, doubles on every success, and becomes zero permanently on the first failure. Its [expectation](probability-theory.md#expected-value) is always one, but it tends to zero [almost surely](convergence-of-random-variables.md#almost-sure-convergence) because the probability of success forever is zero. Thus it satisfies the [martingale convergence theorem](#martingale-convergence-theorem) while failing [convergence in L1](convergence-of-random-variables.md#convergence-in-l1). This illustrates how rare large values obstruct [uniform integrability](convergence-of-random-variables.md#uniform-integrability).

#### Almost sure submartingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

A [submartingale](#submartingale) with $\sup_n\mathbb E Y_n^+<\infty$ converges almost surely to a finite [integrable random variable](probability-theory.md#integrable-random-variable). The positive-part bound also bounds negative parts because $\mathbb E Y_n\geq\mathbb E Y_0$. The result specializes to an $L^1$-bounded [martingale](martingale.md), and hence to every nonnegative [martingale](martingale.md). It does not by itself give [convergence in L1](convergence-of-random-variables.md#convergence-in-l1); [uniform integrability](convergence-of-random-variables.md#uniform-integrability) supplies that stronger conclusion.

#### Lp martingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

A [martingale](martingale.md) satisfying $\sup_n\mathbb E|M_n|^p<\infty$, for $1<p<\infty$, has [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) and [convergence in Lp](convergence-of-random-variables.md#convergence-in-lp) to a limit $M_\infty\in L^p$. Also $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$. The [Doob Lp maximal inequality](#doob-lp-maximal-inequality) makes $\sup_n|M_n|$ integrable to the power $p$; the [martingale convergence theorem](#martingale-convergence-theorem) gives the almost-sure limit, and the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem) gives convergence in the [Lp norm](real-analysis.md#lp-norm). Boundedness in $L^1$ alone does not imply [convergence in L1](convergence-of-random-variables.md#convergence-in-l1).

#### Uniformly integrable martingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

A [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) [martingale](martingale.md) $M_n$ has [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) and [convergence in L1](convergence-of-random-variables.md#convergence-in-l1) to an [integrable random variable](probability-theory.md#integrable-random-variable) $M_\infty$, and $M_n=\mathbb E[M_\infty\mid\mathcal F_n]$.

##### Uniform integrability of a stopped uniformly integrable martingale

↑ **Parent:** [Uniformly integrable martingale convergence theorem](#uniformly-integrable-martingale-convergence-theorem)

Stopping a [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) discrete-time [martingale](martingale.md) at any [stopping time](#stopping-time) preserves [uniform integrability](convergence-of-random-variables.md#uniform-integrability), including when the [stopping time](#stopping-time) can be infinite. For $C=\sup_n\mathbb E|X_n|$, the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) and the [Markov inequality](probability-inequality.md#markov-inequality) give

$$
\mathbb E[|X_{n\wedge T}|\mathbf1_{\{|X_{n\wedge T}|>K\}}]\leq\sup_j\mathbb E[|X_j|\mathbf1_{\{|X_j|>R\}}]+RC/K.
$$

Choose $R$ first, then $K$, to make this uniformly small.

#### Reverse martingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reverse_martingale_convergence_theorem)

For a decreasing sequence of sigma-algebras $\mathcal F_n$ and an integrable random variable $X$,

$$
\mathbb E[X\mid\mathcal F_n]
\longrightarrow
\mathbb E[X\mid\bigcap_n\mathcal F_n]
$$

almost surely and in $L^1$.

#### Almost sure supermartingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

A nonnegative [supermartingale](#supermartingale), or more generally a supermartingale whose negative parts have uniformly bounded expectations, converges almost surely to a finite integrable random variable.

##### Multiplicative correction for summable adapted drift

↑ **Parent:** [Almost sure supermartingale convergence theorem](#almost-sure-supermartingale-convergence-theorem)

Suppose $X_n\geq0$ is an [integrable](measure-theory.md#integrability) [adapted process](stochastic-process.md#adapted-process), $Y_n\geq0$ is finite and adapted, and $\mathbb E[X_{n+1}\mid\mathcal F_n]\leq(1+Y_n)X_n$. The displayed correction is a nonnegative [supermartingale](#supermartingale): its next denominator is [measurable](measure-theory.md#measurability) at time $n$, and its reciprocal is at most one. If $\sum_nY_n<\infty$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), the denominators converge to a finite positive limit since $\log(1+y)\leq y$. The [almost sure supermartingale convergence theorem](#almost-sure-supermartingale-convergence-theorem) then gives finite [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) of $X_n$. No [integrability](measure-theory.md#integrability) of the infinite product or of $\sum_nY_n$ is needed.

##### Supermartingale convergence with summable adapted drift

↑ **Parent:** [Almost sure supermartingale convergence theorem](#almost-sure-supermartingale-convergence-theorem)

Suppose $X_n\geq0$ is [integrable](measure-theory.md#integrability) and adapted, and $Y_n\geq0$ is finite and adapted. Use the [stopped predictable budget for adapted increments](#stopped-predictable-budget-for-adapted-increments) with an integer budget $a$. The process $X_{n\wedge\tau_a}+a-U_{n\wedge\tau_a}$ is an [integrable](measure-theory.md#integrability) nonnegative [supermartingale](#supermartingale), because its budget decrement cancels the localized drift. It has a finite almost-sure limit. On the event that the total drift is smaller than $a$, the [stopping time](#stopping-time) is infinite, so $X_n$ itself converges. Taking the [countable](set-theory.md#countable-set) union over integer budgets proves finite [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence). No [expectation](probability-theory.md#expected-value) of the total drift is needed.

###### Deterministic summable drift correction

↑ **Parent:** [Supermartingale convergence with summable adapted drift](#supermartingale-convergence-with-summable-adapted-drift)

When the drift bound is a deterministic summable sequence $\delta_n\geq0$, the displayed correction is a nonnegative [supermartingale](#supermartingale). Its added tail tends to zero, so the [almost sure supermartingale convergence theorem](#almost-sure-supermartingale-convergence-theorem) directly implies finite [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) of $X_n$. This simpler tail correction requires deterministic bounds; an arbitrary future random drift tail is not generally [measurable](measure-theory.md#measurability) at the current time.

#### Conditional-expectation convergence along a filtration

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

If $\mathcal F_\infty=\sigma(\bigcup_n\mathcal F_n)$ and $Z$ is bounded, then

$$
\mathbb E[Z\mid\mathcal F_n]
\longrightarrow
\mathbb E[Z\mid\mathcal F_\infty]
$$

almost surely and in $L^1$. Testing the almost-sure martingale limit on the algebra $\bigcup_n\mathcal F_n$ identifies it with the terminal conditional expectation.

##### Moving-variable conditional-expectation convergence

↑ **Parent:** [Conditional-expectation convergence along a filtration](#conditional-expectation-convergence-along-a-filtration)

If bounded random variables $X_n$ converge almost surely to $X$, then

$$
\mathbb E[X_n\mid\mathcal F_n]
\longrightarrow
\mathbb E[X\mid\mathcal F_\infty]
$$

almost surely and in $L^1$. For $Z_n=\sup_{m\geq n}|X_m-X|$, the variables $\mathbb E[Z_n\mid\mathcal F_n]$ form a nonnegative supermartingale with expectations tending to zero.

#### Continuous-time martingale convergence theorem

↑ **Parent:** [Martingale convergence theorem](#martingale-convergence-theorem)

A right-continuous continuous-time martingale with $\sup_{t\geq0}\mathbb E|M_t|<\infty$ has an almost-sure finite limit as $t\to\infty$.

## Supermartingale

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Supermartingale)

An integrable adapted process $(V_n)$ is a supermartingale when $\mathbb E[V_{n+1}\mid\mathcal F_n]\leq V_n$.

### Pasting supermartingales with downward jumps

↑ **Parent:** [Supermartingale](#supermartingale)

If two [supermartingales](#supermartingale) satisfy $X_N^1\geq X_N^2$ on the event that the [stopping time](#stopping-time) $N$ is finite, the displayed pasted [adapted process](stochastic-process.md#adapted-process) is a [supermartingale](#supermartingale). On $\{N>n\}$ its next value is at most $X_{n+1}^1$, because a possible switch at $n+1$ only decreases it. On $\{N\leq n\}$ it follows the second [supermartingale](#supermartingale). Conditioning these inequalities proves the assertion. Finite repeated pastings inherit the same property, allowing a multiplicative trading construction for [upcrossings](#upcrossing).

### Terminal decomposition of an L1-bounded supermartingale

↑ **Parent:** [Supermartingale](#supermartingale)

An $L^1$-bounded [supermartingale](#supermartingale) has an [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) limit $X_\infty$ in $L^1$. The [conditional-expectation martingale](#conditional-expectation-martingale) $M_n=\mathbb E[X_\infty\mid\mathcal F_n]$ has [uniform integrability](convergence-of-random-variables.md#uniform-integrability) and converges to $X_\infty$ both [almost surely](convergence-of-random-variables.md#almost-sure-convergence) and in $L^1$. To identify its limit, test against every event in every finite-time [sigma-algebra](measure-theory.md#sigma-algebra) and use uniqueness on their generated [sigma-algebra](measure-theory.md#sigma-algebra). Then $Y=X-M$ is a [supermartingale](#supermartingale) tending to zero [almost surely](convergence-of-random-variables.md#almost-sure-convergence). There is no general nonnegativity conclusion for $Y$, nor general [convergence in L1](convergence-of-random-variables.md#convergence-in-l1) to zero: the negative of the [fair-coin doubling martingale](#fair-coin-doubling-martingale) is a counterexample to both stronger assertions.

### Stopping preserves supermartingales in discrete time

↑ **Parent:** [Supermartingale](#supermartingale)

If $U_t$ is a [supermartingale](#supermartingale) and $\tau$ is a [stopping time](#stopping-time), then $U_{t\wedge\tau}$ is a supermartingale. Adaptedness follows from the stopping-time events, and integrability follows from $|U_{t\wedge\tau}|\leq\sum_{j=0}^t|U_j|$. Its increment is $\mathbf1_{\{\tau>t\}}(U_{t+1}-U_t)$. Since $\{\tau>t\}\in\mathcal F_t$, conditioning gives a nonpositive conditional mean. No integrability assumption on the possibly unbounded stopping time is required for this stopped-process assertion at each fixed finite $t$.

### Local supermartingale

↑ **Parent:** [Supermartingale](#supermartingale)

A [local supermartingale](#local-supermartingale) becomes a [supermartingale](#supermartingale) after stopping along an increasing sequence of [stopping times](#stopping-time) tending to infinity. Localization allows an [Itô formula](stochastic-calculus.md#ito-s-lemma) comparison before global integrability is established. Additional lower bounds or uniform integrability are needed to pass from the local comparison to an unrestricted expectation inequality.

### Square-root stock supermartingale

↑ **Parent:** [Supermartingale](#supermartingale)

For a positive stock satisfying $dS=S\sigma\,dW$, the [Itô formula](stochastic-calculus.md#ito-s-lemma) gives $d\sqrt S=\tfrac12\sqrt S\sigma dW-\tfrac18\sqrt S\sigma^2dt$. Localization and the conditional [Fatou lemma](measure-theory.md#fatou-s-lemma) make this nonnegative local supermartingale a true [supermartingale](#supermartingale).

### Maximal inequality for a nonnegative supermartingale

↑ **Parent:** [Supermartingale](#supermartingale)

For a right-continuous nonnegative [supermartingale](#supermartingale) $M$ and $R>0$, the first level-hit time $\sigma$ and the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) give $R\mathbb P(\sigma\leq T)\leq\mathbb E[M_{\sigma\wedge T}]\leq\mathbb E[M_0]$. Let $T\to\infty$ and first use levels $R-\varepsilon$, then $\varepsilon\downarrow0$, to include a supremum not attained. For a continuous [nonnegative local martingale](#nonnegative-local-martingale) on a stochastic interval, apply the argument on increasing localized compact subintervals, then pass to their limit. Letting $R\to\infty$ shows that its running supremum is finite almost surely.

### Zero is absorbing for a nonnegative supermartingale

↑ **Parent:** [Supermartingale](#supermartingale)

If a nonnegative [supermartingale](#supermartingale) reaches zero at a discrete [stopping time](#stopping-time), its later nonnegative values have conditional [expectation](probability-theory.md#expected-value) at most zero and must also be zero [almost surely](convergence-of-random-variables.md#almost-sure-convergence).

### Constant-expectation supermartingale is a martingale

↑ **Parent:** [Supermartingale](#supermartingale)

A discrete-time supermartingale $X$ is a martingale exactly when $\mathbb E[X_n]=\mathbb E[X_0]$ for every $n$. If expectations are constant, the nonnegative variable

$$
X_n-\mathbb E[X_{n+1}\mid\mathcal F_n]
$$

has expectation zero and therefore vanishes almost surely.

### Supermartingale majorant bound

↑ **Parent:** [Supermartingale](#supermartingale)

If a supermartingale $V$ dominates an adapted reward process $Z$, optional sampling gives $\mathbb E Z_\tau\leq V_0$ for every bounded stopping time $\tau$.

## Stopping time

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stopping_time)

A random time $\tau$ is a stopping time when $\{\tau\leq n\}\in\mathcal F_n$ for every $n$.

### Closed-level hitting times of continuous adapted processes

↑ **Parent:** [Stopping time](#stopping-time)

For a continuous [adapted process](stochastic-process.md#adapted-process) $X$ and $T=\inf\{s\geq0:X_s\geq\lambda\}$,

$$
\{T\leq t\}=\bigcap_{m\geq1}\bigcup_{r\in(\mathbb Q\cap[0,t])\cup\{t\}}\{X_r>\lambda-1/m\}.
$$

Continuity makes the supremum on $[0,t]$ attained and equals its supremum on this countable dense set. Each displayed event belongs to $\mathcal F_t$, so $T$ is a [stopping time](#stopping-time) without requiring right-continuity of the filtration.

// Target: martingale.bigb

### Waiting time for two consecutive successes

↑ **Parent:** [Stopping time](#stopping-time)

For [independent](random-variable.md#independent-random-variables) trials of success [probability](probability-theory.md#probability) $p\in(0,1]$, let $T$ be the first index completing two consecutive successes. If $e_0,e_1$ are the mean remaining times with no trailing success and with one trailing success, conditioning gives $e_0=1+(1-p)e_0+pe_1$ and $e_1=1+(1-p)e_0$. Solving yields $e_0=(1+p)/p^2$, so fair trials have mean waiting time six. Disjoint pairs give a geometric tail bound and justify finiteness before solving the equations. Overlapping pairs are not [independent](random-variable.md#independent-random-variables) trials.

### Stopped process

↑ **Parent:** [Stopping time](#stopping-time)

The stopped [stochastic process](stochastic-process.md) follows $X$ until the [stopping time](#stopping-time) $\tau$ and thereafter keeps the value $X_\tau$ when $\tau$ is finite. For a pathwise [right-continuous](calculus.md#right-continuous-function) [adapted process](stochastic-process.md#adapted-process), the [stopped process](#stopped-process) is adapted, by [progressive measurability](stochastic-process.md#progressive-measurability) and measurable evaluation at $t\wedge\tau$. When $X$ is a [martingale](martingale.md), further stopping and integrability conditions determine whether its [stopped process](#stopped-process) is a [martingale](martingale.md).

#### Stopped predictable budget for adapted increments

↑ **Parent:** [Stopped process](#stopped-process)

For finite nonnegative [adapted processes](stochastic-process.md#adapted-process) $Y_j$, set $\tau_a=\inf\{n:\sum_{j\leq n}Y_j>a\}$ and $U_n=\sum_{j<n}Y_j$. Stopping this one-step-lagged sum gives $A_n=a-U_{n\wedge\tau_a}\in[0,a]$, with $A_{n+1}-A_n=-Y_n\mathbf1_{\{\tau_a>n\}}$. The latter is nonpositive and [measurable](measure-theory.md#measurability) at time $n$, so $A$ is a nonnegative [supermartingale](#supermartingale). The overshooting increment is excluded, which is essential to nonnegativity.

### Integrability of a stopped random-walk increment

↑ **Parent:** [Stopping time](#stopping-time)

Let $X_n$ be integrable [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables), and let $T\geq1$ be a [stopping time](#stopping-time) for their [natural filtration](stochastic-process.md#natural-filtration), with $\mathbb ET<\infty$. Since $\{T\geq n\}$ is measurable before $X_n$ is observed, [independence](random-variable.md#independent-random-variables) and the [Tonelli theorem](measure-theory.md#tonelli-theorem) give $\mathbb E|X_T|\leq\sum_n\mathbb E[|X_n|\mathbf1_{\{T\geq n\}}]=\mathbb E|X_1|\mathbb ET$. The event $T=n$ need not be independent of $X_n$, so the selected increment can be biased.

### Stopping-time sigma-algebra

↑ **Parent:** [Stopping time](#stopping-time)

The information available at a [stopping time](#stopping-time) $T$ is the [sigma-algebra](measure-theory.md#sigma-algebra)

$$
\mathcal F_T=\{A\in\mathcal F:A\cap\{T\leq t\}\in\mathcal F_t\text{ for every }t\geq0\}.
$$

In discrete time, $A\cap\{T=k\}\in\mathcal F_k$ for $A\in\mathcal F_T$. A [bounded stopping time](#bounded-stopping-time) permits conditional forms of the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) with respect to this [sigma-algebra](measure-theory.md#sigma-algebra).

#### Pasting ordered stopping times

↑ **Parent:** [Stopping-time sigma-algebra](#stopping-time-sigma-algebra)

If $S\leq T$ are [stopping times](#stopping-time) and $A\in\mathcal F_S$, then $U=S\mathbf1_A+T\mathbf1_{A^c}$ is a [stopping time](#stopping-time). The key identity is

$$
A^c\cap\{T\leq t\}=\{T\leq t\}\setminus(A\cap\{S\leq t\}).
$$

This uses the ordering $S\leq T$: without it, $A$ need not be known when $T$ occurs. Such pastings test the [martingale](martingale.md) identity through [expectations](probability-theory.md#expected-value) at [bounded stopping times](#bounded-stopping-time).

### Announcing sequence for a stopping time

↑ **Parent:** [Stopping time](#stopping-time)

An announcing sequence consists of [stopping times](#stopping-time) increasing to $T$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), strictly smaller than $T$ on $\{T>0\}$. Such a lifetime can be approached through stopped intervals on which a [locally defined stochastic process](stochastic-process.md#locally-defined-stochastic-process) is an ordinary [adapted process](stochastic-process.md#adapted-process). For the usual [maximal local solution of a stochastic differential equation](stochastic-calculus.md#maximal-local-solution-of-a-stochastic-differential-equation), the exit times $\tau_n$ from a nested [compact exhaustion](topology.md#compact-exhaustion) of the open domain, capped as $T_n=\tau_n\wedge n$, supply this sequence. The existence of such a sequence is an extra lifetime convention; arbitrary [stopping times](#stopping-time) need not admit one.

### Bounded stopping time

↑ **Parent:** [Stopping time](#stopping-time)

A [bounded stopping time](#bounded-stopping-time) is a [stopping time](#stopping-time) bounded [almost surely](convergence-of-random-variables.md#almost-sure-convergence) by a deterministic finite constant. In discrete time, a bound $T\leq N$ makes $M_T$ integrable whenever $M_0,\ldots,M_N$ are [integrable random variables](probability-theory.md#integrable-random-variable), and the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) applies to a [martingale](martingale.md) without additional limiting hypotheses. Almost-sure finiteness alone is weaker than boundedness.

### Geometric tail bound from a uniform escape probability

↑ **Parent:** [Stopping time](#stopping-time)

Suppose a nonnegative [stopping time](#stopping-time) $T$ and constants $L>0$, $0<q\leq1$ satisfy $\mathbb P(T\leq nL+L\mid\mathcal F_{nL})\geq q$ on $\{T>nL\}$. Take $L$ to be a positive integer in discrete time. Then

$$
\mathbb P(T>nL)\leq(1-q)^n,\qquad \mathbb ET\leq L/q.
$$

On the surviving [event](probability-theory.md#event), conditional survival is at most $1-q$. The [tower property of conditional expectation](measure-theory.md#law-of-total-expectation) therefore gives

$$
\mathbb P(T>(n+1)L)\leq(1-q)\mathbb P(T>nL).
$$

Induction proves the geometric bound. Partitioning the tail [integral](calculus.md#integral) into intervals of length $L$ then gives $\mathbb ET\leq L\sum_{n\geq0}\mathbb P(T>nL)\leq L/q$; in discrete time, group the tail sum into $L$ successive integer indices instead. This proves finite [expected hitting times](markov-process.md#expected-hitting-time) when every surviving state has a uniform positive chance of escaping within a fixed time. It works in discrete or continuous time without assuming [independence](random-variable.md#independent-random-variables) of successive survival [events](probability-theory.md#event).

#### Random-walk exit bound from a positive-increment block

↑ **Parent:** [Geometric tail bound from a uniform escape probability](#geometric-tail-bound-from-a-uniform-escape-probability)

For a [random walk](markov-process.md#random-walk) with [independent and identically distributed](random-variable.md#independent-and-identically-distributed-random-variables) increments and an exit time from $(0,r)$, suppose $p=\mathbb P(X_1>r/m)>0$ for some integer $m\geq1$. A block of $m$ such positive increments forces an exit. Conditional on survival, every successive block has success probability at least $p^m$, so $\mathbb P(T>km)\leq(1-p^m)^k$ and $\mathbb ET\leq m/p^m$. This is an instance of the [geometric tail bound from a uniform escape probability](#geometric-tail-bound-from-a-uniform-escape-probability); centering of the increments is not required.

### Waiting time for a word in independent uniform symbols

↑ **Parent:** [Stopping time](#stopping-time)

Let a fixed word $w$ be sampled from an alphabet of $q$ symbols by independent uniform draws, and let $\tau_w$ count draws through its first occurrence. If $B(w)$ is the set of lengths of the [borders of a word](foundations-of-mathematics.md#border-of-a-word), including the full length, then

$$
\mathbb E\tau_w=\sum_{k\in B(w)}q^k.
$$

Shorter borders contribute because a failed or completed match can retain a suffix that is already a prefix of the next match.

### Skorokhod embedding theorem

↑ **Parent:** [Stopping time](#stopping-time)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Skorokhod_embedding_theorem)

The Skorokhod embedding theorem represents a centered [probability distribution](probability-theory.md#probability-distribution) $\mu$ on the [real numbers](arithmetic.md#real-number) with finite [variance](variance.md) as $B_T\sim\mu$ for a [stopping time](#stopping-time) $T$ of [Brownian motion](brownian-motion.md). One may choose $T$ so that the stopped process $(B_{t\wedge T})$ is [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) and $\mathbb ET=\int x^2\mu(dx)$.

#### Skorokhod embedding of a centered random walk

↑ **Parent:** [Skorokhod embedding theorem](#skorokhod-embedding-theorem)

If a random walk has independent identically distributed centered steps of variance $\sigma^2<\infty$, there are increasing Brownian stopping times $T_n$ such that

$$
(B_{T_n})_{n\geq0}\overset d=(S_n)_{n\geq0},
$$

and the increments $T_n-T_{n-1}$ are independent and identically distributed with mean $\sigma^2$. Apply the one-step embedding repeatedly using the strong Markov property.

##### Central limit theorem from the Skorokhod embedding

↑ **Parent:** [Skorokhod embedding of a centered random walk](#skorokhod-embedding-of-a-centered-random-walk)

The law of large numbers gives $T_n/n\to\sigma^2$. Brownian maximal estimates then show

$$
\frac{B_{T_n}-B_{n\sigma^2}}{\sqrt n}\longrightarrow0
$$

in probability. Since $B_{n\sigma^2}/\sqrt n\sim N(0,\sigma^2)$, the embedded random walk satisfies the central limit theorem.

### Stopped martingale in discrete time

↑ **Parent:** [Stopping time](#stopping-time)

For a discrete martingale and stopping time $T$,

$$
M_{(n+1)\wedge T}-M_{n\wedge T}
=\mathbf1_{\{T>n\}}(M_{n+1}-M_n).
$$

The indicator is measurable at time $n$, so the stopped process is a martingale. If it is uniformly bounded and $T<\infty$ almost surely, bounded convergence gives $\mathbb E M_T=\mathbb E M_0$ directly.

#### Integrable overshoot of a stopped L1-bounded martingale

↑ **Parent:** [Stopped martingale in discrete time](#stopped-martingale-in-discrete-time)

For an integrable discrete-time [martingale](martingale.md), stop at the first time $|f_n|\geq N$. For any deterministic $m$, conditioning the terminal value $f_m$ on each event $\{\tau=j\}$ gives $\mathbb E|f_{\tau\wedge m}|\leq\mathbb E|f_m|$. [Monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) therefore proves the displayed overshoot bound. The maximum of the [stopped martingale](#stopped-martingale) is at most $N\vee |f_\tau|\mathbf1_{\{\tau<\infty\}}$, an integrable variable. This permits a convergence proof without assuming bounded overshoots.

#### Stopped-martingale uniform integrability criterion

↑ **Parent:** [Stopped martingale in discrete time](#stopped-martingale-in-discrete-time)

For an [almost surely](convergence-of-random-variables.md#almost-sure-convergence) finite [stopping time](#stopping-time) $T$, if $\mathbb E|M_T|<\infty$ and $\mathbb E[|M_n|\mathbf1_{\{T>n\}}]\to0$, then $M_{n\wedge T}\to M_T$ with [convergence in L1](convergence-of-random-variables.md#convergence-in-l1). Thus [L1 convergence implies uniform integrability](convergence-of-random-variables.md#l1-convergence-implies-uniform-integrability) makes the [stopped martingale](#stopped-martingale) [uniformly integrable](convergence-of-random-variables.md#uniform-integrability).

#### Characterization of a martingale by stopped expectations

↑ **Parent:** [Stopped martingale in discrete time](#stopped-martingale-in-discrete-time)

Let an integrable process $(M_n)$ be [adapted](stochastic-process.md#adapted-process) to $(\mathcal F_n)$. It is a [martingale](martingale.md) if and only if $\mathbb E[M_{n\wedge\tau}]=\mathbb E[M_0]$ for every $n$ and every [stopping time](#stopping-time) $\tau$. For the reverse implication, fix $A\in\mathcal F_n$ and take $\tau=n$ on $A$ and $\tau=n+1$ on $A^c$. Comparing its stopped expectation at $n+1$ with the expectation obtained from the deterministic stopping time $n+1$ gives $\mathbb E[\mathbf1_A(M_{n+1}-M_n)]=0$. Since this holds for every $A\in\mathcal F_n$, it is exactly $\mathbb E[M_{n+1}\mid\mathcal F_n]=M_n$.

#### Discounted symmetric random-walk exit transform

↑ **Parent:** [Stopped martingale in discrete time](#stopped-martingale-in-discrete-time)

For simple symmetric random walk stopped on hitting $-a$ or $b$ and $0<z<1$, choose $w>1$ by

$$
z=\frac2{w+w^{-1}},
\qquad
w=\frac{1+\sqrt{1-z^2}}z.
$$

Then $z^nw^{\pm X_n}$ are martingales. Solving the two boundary equations gives

$$
\mathbb E_0z^T
=\frac{w^a+w^b-w^{-a}-w^{-b}}
{w^{a+b}-w^{-(a+b)}}.
$$

### Optional sampling theorem for a supermartingale

↑ **Parent:** [Stopping time](#stopping-time)

For bounded stopping times $\sigma\leq\tau$, a supermartingale satisfies $\mathbb E[V_\tau\mid\mathcal F_\sigma]\leq V_\sigma$; equality holds for a martingale.

#### Bounded-increment optional stopping with integrable time

↑ **Parent:** [Optional sampling theorem for a supermartingale](#optional-sampling-theorem-for-a-supermartingale)

For an integrable [supermartingale](#supermartingale) with the displayed increment bound, $|X_{T\wedge n}|\le|X_0|+KT$. Thus the stopped values are dominated by one [integrable random variable](probability-theory.md#integrable-random-variable), including $X_T$. Apply [optional stopping](#optional-sampling-theorem-for-a-supermartingale) at the bounded times $T\wedge n$ and then the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem). For a [martingale](martingale.md) the same proof gives equality.

#### Bounded-stopping-time characterization of a martingale

↑ **Parent:** [Optional sampling theorem for a supermartingale](#optional-sampling-theorem-for-a-supermartingale)

An [adapted process](stochastic-process.md#adapted-process) with integrable coordinates is a [martingale](martingale.md) exactly when the displayed equality holds for every bounded [stopping time](#stopping-time). For the forward implication, expand $M_T-M_0=\sum_{k=1}^N\mathbf1_{\{T\geq k\}}(M_k-M_{k-1})$ and condition each term on $\mathcal F_{k-1}$. Conversely, for $A\in\mathcal F_n$ choose $T=n+1$ on $A$ and $T=n$ elsewhere. Subtract the equality for the constant [stopping time](#stopping-time) $n$ to obtain $\mathbb E[\mathbf1_A(M_{n+1}-M_n)]=0$, which is the defining [conditional expectation](measure-theory.md#conditional-expectation) identity.

#### Exponential-supermartingale escape bound

↑ **Parent:** [Optional sampling theorem for a supermartingale](#optional-sampling-theorem-for-a-supermartingale)

If $e^{-\theta N_{t\wedge\sigma_K}}$ is a nonnegative [supermartingale](#supermartingale), with $\sigma_K$ the first time $N_t\leq K$, the [optional stopping theorem](#optional-sampling-theorem-for-a-supermartingale) yields $\mathbb P_N(\sigma_K<\infty)\leq e^{-\theta(N-K)}$. Such a bound can prove escape of a backlog independently of heuristic [fluid models](queueing-theory.md#fluid-model).

## Predictable process

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Predictable_process)

In discrete time, a process $A_n$ is predictable or previsible when $A_n$ is $\mathcal F_{n-1}$-measurable for every $n\geq1$. In continuous time, predictability means measurability with respect to the [predictable sigma-algebra](#predictable-sigma-algebra).

### Martingale transform

↑ **Parent:** [Predictable process](#predictable-process)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Martingale_transform)

If $M$ is a martingale and $A$ is predictable, then, subject to integrability,

$$
X_n=X_0+\sum_{k=1}^nA_k(M_k-M_{k-1})
$$

is a martingale.

#### Terminal nonnegativity criterion for a finite-horizon martingale transform

↑ **Parent:** [Martingale transform](#martingale-transform)

For $Y_t=\sum_{s\leq t}K_s(M_s-M_{s-1})$ and fixed finite deterministic $T$, bounded events in $\mathcal F_{t-1}$ restricting both $Y_{t-1}$ and $K_t$ show that nonnegativity of $Y_t$ forces nonnegativity of $Y_{t-1}$. Induction makes the entire stopped process nonnegative. The [nonnegative discrete-time local martingale is a martingale](#nonnegative-discrete-time-local-martingale-is-a-martingale) criterion then gives $\mathbb E Y_T=Y_0=0$. Nonnegative terminal gain is therefore zero almost surely, even without an intermediate wealth bound.

#### Predictable-coefficient localization of a martingale transform

↑ **Parent:** [Martingale transform](#martingale-transform)

For a finite-valued [predictable process](#predictable-process) $K$, this is a [stopping time](#stopping-time) and increases to infinity. The stopped [martingale transform](#martingale-transform) uses coefficients $K_s\mathbf1_{\{s\leq\sigma_j\}}$, which are [predictable](#predictable-process) and bounded by $j$. Thus a transform of a discrete-time [martingale](martingale.md) is a [local martingale](#local-martingale) without a global boundedness assumption. The stop is before, not after, the first large coefficient is used.

#### Recovery of a martingale-transform integrand by conditional covariance

↑ **Parent:** [Martingale transform](#martingale-transform)

For a square-integrable martingale transform and positive conditional increment variance,

$$
A_n=\frac{\operatorname{Cov}(X_n,M_n\mid\mathcal F_{n-1})}
{\operatorname{Var}(M_n\mid\mathcal F_{n-1})}.
$$

#### Stopped martingale

↑ **Parent:** [Martingale transform](#martingale-transform)

For a stopping time $T$,

$$
M_{n\wedge T}-M_{(n-1)\wedge T}
=\mathbf1_{\{T\geq n\}}(M_n-M_{n-1}).
$$

The indicator is predictable, so a stopped integrable martingale is a martingale.

##### Stopped-walk martingale with almost sure but not L1 convergence

↑ **Parent:** [Stopped martingale](#stopped-martingale)

For a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk), the [infinite mean first passage of a simple symmetric random walk](probability-theory.md#infinite-mean-first-passage-of-a-simple-symmetric-random-walk) gives a finite almost sure first passage $T_1$ to $1$. The [stopped martingale](#stopped-martingale) $M_n=1-S_{n\wedge T_1}$ is nonnegative and eventually zero almost surely. Nevertheless $\mathbb EM_n=1$ for every $n$, so it has [almost sure convergence](convergence-of-random-variables.md#almost-sure-convergence) but no [convergence in L1](convergence-of-random-variables.md#convergence-in-l1). It is therefore not [uniformly integrable](convergence-of-random-variables.md#uniform-integrability). Before absorption the nearest-neighbour walk is at most zero, ensuring nonnegativity.

#### Reflection principle for simple symmetric random walk

↑ **Parent:** [Martingale transform](#martingale-transform)

Let $S_0=0$ be a [simple symmetric random walk](probability-theory.md#simple-symmetric-random-walk), let $T_a$ be its first hitting time of the positive integer $a$, and reverse every increment after $T_a$. The resulting path is again a simple symmetric random walk. Consequently,

$$
\mathbb P\left(\max_{k\leq n}S_k\geq a\right)
=\mathbb P(S_n\geq a)+\mathbb P(S_n\geq a+1).
$$

The continuous analogue is the existing [Reflection principle (Wiener process)](brownian-motion.md#reflection-principle-wiener-process); its tail formula has no discrete one-unit lattice correction.

##### Point probability for the maximum of simple symmetric random walk

↑ **Parent:** [Reflection principle for simple symmetric random walk](#reflection-principle-for-simple-symmetric-random-walk)

For $M_n=\max_{0\leq k\leq n}S_k$ and a positive integer $a$,

$$
\mathbb P(M_n=a)
=\mathbb P(S_n=a)+\mathbb P(S_n=a+1).
$$

Exactly one term can be nonzero because $S_n$ has the parity of $n$.

#### Predictable representation in a Rademacher filtration

↑ **Parent:** [Martingale transform](#martingale-transform)

If $\mathcal F_n$ is generated by independent symmetric signs $\xi_1,\ldots,\xi_n$, every martingale has predictable coefficients $B_n$ such that

$$
M_n=M_0+\sum_{k=1}^nB_k\xi_k.
$$

One may take $B_n=\mathbb E[M_n\xi_n\mid\mathcal F_{n-1}]$.

##### Stopped martingale isometry in a Rademacher filtration

↑ **Parent:** [Predictable representation in a Rademacher filtration](#predictable-representation-in-a-rademacher-filtration)

For a bounded stopping time $T$ and a square-integrable representation $M_n=M_0+\sum_{k\leq n}B_k\xi_k$,

$$
\mathbb E[M_T^2]=M_0^2+\mathbb E\sum_{k=1}^TB_k^2.
$$

The cross terms vanish because predictable multiples of distinct independent signs are orthogonal martingale differences.

### Predictable compensator of a discrete supermartingale

↑ **Parent:** [Predictable process](#predictable-process)

The increments $\Delta A_{n+1}=V_n-\mathbb E[V_{n+1}\mid\mathcal F_n]$ of a supermartingale are predictable and nonnegative.

### Predictable sigma-algebra

↑ **Parent:** [Predictable process](#predictable-process)

The predictable sigma-algebra on $\Omega\times[0,\infty)$ is generated by $A\times\{0\}$ for $A\in\mathcal F_0$ and by $A\times(s,t]$ for $A\in\mathcal F_s$. Equivalently, it is the smallest sigma-algebra making every left-continuous [adapted process](stochastic-process.md#adapted-process) measurable.

#### Predictable rectangle

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

A predictable rectangle has the displayed form for $0\leq s<t$. Its indicator is a left-continuous [adapted process](stochastic-process.md#adapted-process), and these rectangles generate the [predictable sigma-algebra](#predictable-sigma-algebra) on positive times. If the time-zero slice is included, also use $B\times\{0\}$ with $B\in\mathcal F_0$.

#### Survival-observation predictable sigma-algebra

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

On $\Omega=(0,\infty)$, observe only $X_t(\omega)=\mathbf1_{\{t\leq\omega\}}$. Before and at the observed lifetime, the [natural filtration](stochastic-process.md#natural-filtration) cannot distinguish any two surviving outcomes. The [predictable sigma-algebra](#predictable-sigma-algebra) on positive times therefore consists exactly of sets whose trace on $D=\{\omega\geq t\}$ is $D\cap(\Omega\times T)$ for a [Borel set](measure-theory.md#borel-set) $T$, and whose trace on $D^c$ is arbitrary product-Borel. To prove sufficiency, $D$ is predictable because $X$ is left-continuous and adapted; on $D^c$, insert a rational $s$ with $\omega<s<t$ and use the predictable rectangles $(E\cap(0,s))\times(s,\infty)$.

#### Predictable sections at deterministic times

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

For a [predictable process](#predictable-process) $H$ and deterministic $t>0$, $H_t$ is measurable for the [left-limit sigma-algebra](stochastic-process.md#left-limit-sigma-algebra) $\mathcal F_{t-}$. This follows by taking sections of the generating predictable rectangles. At time zero use $\mathcal F_{0-}=\mathcal F_0$.

#### Elementary predictable process with stopping-time intervals

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

An elementary [predictable process](#predictable-process) may use finitely many ordered [stopping times](#stopping-time) $\tau_j$, with bounded $\mathcal F_{\tau_j}$-measurable coefficients $h_j$ on $(\tau_j,\tau_{j+1}]$. Its elementary [stochastic integral](stochastic-calculus.md#stochastic-integral) is $\sum_jh_j(X_{t\wedge\tau_{j+1}}-X_{t\wedge\tau_j})$. The stopped indicators are left-continuous and adapted, so the process is [predictable](#predictable-process); common refinement shows the sum is independent of its representation. Deterministic endpoints recover the usual [simple predictable process](#simple-predictable-process). These integrands give the precise good-integrator test in the [Bichteler-Dellacherie theorem](stochastic-calculus.md#bichteler-dellacherie-theorem).

#### Simple predictable process

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

A simple predictable process is constant on finitely many deterministic time intervals $(t_k,t_{k+1}]$, and its value there is $\mathcal F_{t_k}$-measurable. Such processes generate the predictable sigma-algebra and are dense in the corresponding $L^p$ spaces for finite measures.

##### Density of simple predictable processes for finite measures

↑ **Parent:** [Simple predictable process](#simple-predictable-process)

For every [finite measure](measure-theory.md#finite-measure) $\mu$ on the [predictable sigma-algebra](#predictable-sigma-algebra), bounded [simple predictable processes](#simple-predictable-process) are dense in $L^2(\mu)$. Include a bounded $\mathcal F_0$-measurable value supported at time zero when $\mu$ may charge that slice. Indicators of the generating rectangles and the [Pi-lambda theorem](probability-theory.md#pi-lambda-theorem) prove density. This gives the completion step in the [Itô isometry](stochastic-calculus.md#ito-isometry) construction.

<h4 id="deterministic-cadlag-process-is-predictable">Deterministic càdlàg process is predictable</h4>

↑ **Parent:** [Predictable sigma-algebra](#predictable-sigma-algebra)

Every deterministic [càdlàg function](calculus.md#cadlag) is Borel measurable in time. Since the predictable sigma-algebra contains every set $\Omega\times A$ with $A$ Borel, the corresponding deterministic process is predictable.

## Doob decomposition theorem

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doob_decomposition_theorem)

Every integrable discrete-time supermartingale has the form $V=M-A$, where $M$ is a martingale and $A$ is predictable, integrable, nondecreasing, and starts at zero.

More generally, an integrable adapted process $X_n$ decomposes as $X_n=M_n+A_n$ with $A_0=0$ and $A_n-A_{n-1}=\mathbb E[X_n-X_{n-1}\mid\mathcal F_{n-1}]$. For a supermartingale this drift is nonincreasing, so writing it as $-A$ yields the nondecreasing convention above.

### Strong law for submartingales with bounded increments

↑ **Parent:** [Doob decomposition theorem](#doob-decomposition-theorem)

If a [submartingale](#submartingale) has uniformly [bounded increments](stochastic-process.md#bounded-increments), then $\liminf_n Y_n/n\geq0$ almost surely. In its [Doob decomposition in discrete time](#doob-decomposition-theorem), the predictable compensator is nondecreasing, while the martingale part has [bounded increments](stochastic-process.md#bounded-increments). The [strong law for martingales with bounded increments](#strong-law-for-martingales-with-bounded-increments) makes the latter negligible on the linear scale.

### Doob decomposition of an adapted integrable process

↑ **Parent:** [Doob decomposition theorem](#doob-decomposition-theorem)

Every adapted integrable process $X$ has a unique decomposition $X=M+A$, where $M$ is a martingale, $A_0=0$, and $A$ is predictable. Its increments are

$$
A_{n+1}-A_n
=\mathbb E[X_{n+1}-X_n\mid\mathcal F_n].
$$

For a supermartingale these increments are nonpositive; changing the sign of $A$ gives the usual nondecreasing compensator convention.

## Snell envelope

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Snell_envelope)

The finite-horizon Snell envelope of rewards $Z_n$ is defined backward by $V_N=Z_N$ and $V_n=\max\{Z_n,\mathbb E[V_{n+1}\mid\mathcal F_n]\}$. It is the least supermartingale dominating $Z$.

### Snell envelope of a multiplicative process

↑ **Parent:** [Snell envelope](#snell-envelope)

Let $Y_t=Y_0\prod_{j=1}^tZ_j$, where $Y_0>0$ is deterministic and the positive factors are independent and integrable. Use the natural filtration. Its finite-horizon [Snell envelope](#snell-envelope) is

$$
U_t=Y_tc_t,\qquad c_T=1,\qquad c_t=\max\{1,c_{t+1}\mathbb E Z_{t+1}\}.
$$

Indeed, backward induction and [independence of random variables](random-variable.md#independent-random-variables) give $\mathbb E[U_{t+1}\mid\mathcal F_t]=Y_tc_{t+1}\mathbb E Z_{t+1}$; take the maximum with immediate exercise $Y_t$. The constants are finite and at least one. Equivalently, $c_t$ is the maximum of $1$ and the successive products $\prod_{j=t+1}^u\mathbb E Z_j$ for $t<u\le T$. If the factors have a common mean $\lambda>1$, waiting until maturity is optimal and $c_t=\lambda^{T-t}$. Integrability and [independence of random variables](random-variable.md#independent-random-variables) from the current information are essential to the finite deterministic coefficient conclusion.

### Optimal stopping

↑ **Parent:** [Snell envelope](#snell-envelope)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Optimal_stopping)

Choosing a [stopping time](#stopping-time) to maximize an expected reward. For an adapted integrable reward process over a finite discrete horizon, the [Snell envelope](#snell-envelope) computes the conditional optimal reward by comparing immediate exercise with continuation.

#### Uniform-offer stopping recursion

↑ **Parent:** [Optimal stopping](#optimal-stopping)

With independent [uniform distributions](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$ as sequential offers and a finite number of rounds, the continuation value with $j-1$ offers remaining is $v_{j-1}$. Accept the current offer when it reaches that threshold. Integrating the maximum of the offer and continuation value gives the recursion, by the [Snell envelope](#snell-envelope) principle.

#### Smooth pasting

↑ **Parent:** [Optimal stopping](#optimal-stopping)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smooth_pasting)

At a regular exercise boundary for a diffusion [optimal stopping](#optimal-stopping) problem, value matching is commonly accompanied by matching first derivatives. This makes the value $C^1$ across the boundary and eliminates a derivative-jump [local time of a semimartingale](stochastic-calculus.md#local-time-of-a-semimartingale) term in the generalized [Itô formula](stochastic-calculus.md#ito-s-lemma). It does not assert that second derivatives agree, or that smooth fit holds for every possible stopping problem.

#### Optimal stopping value function

↑ **Parent:** [Optimal stopping](#optimal-stopping)

For a [Markov process](markov-process.md) with reward $f$, the value starting at time $t$ in state $s$ is the supremum of expected rewards over admissible [stopping times](#stopping-time). In finite discrete time it obeys $V(T,s)=f(s)$ and $V(t,s)=\max\{f(s),PV(t+1,\cdot)(s)\}$ for the [transition operator](markov-process.md#transition-operator) $P$, wherever expectations are well-defined. Statewise absolute integrability of every remaining-horizon reward makes these values finite.

##### Convexity of a random-walk Snell value function

↑ **Parent:** [Optimal stopping value function](#optimal-stopping-value-function)

The [transition operator](markov-process.md#transition-operator) of an additive [random walk](markov-process.md#random-walk) preserves [convex functions](real-analysis.md#convex-function): apply their convexity inequality to $x+\xi$ and $y+\xi$, then integrate. The [pointwise maximum of convex functions](real-analysis.md#pointwise-maximum-of-convex-functions) preserves convexity too, so induction proves convexity of the [Snell envelope](#snell-envelope) Bellman functions. Expectations are allowed to be extended-valued until finiteness is justified. Integrability of rewards on a finite horizon implies finiteness of these functions at every state for $t\geq1$, by [integrability of translated convex random-walk rewards](#integrability-of-translated-convex-random-walk-rewards) and the bound $W_t(x)\leq\sum_{j=0}^{T-t}\mathbb E[f(x+Z_j)^+]$. At time zero only $X_0=0$ is observed; if $W_0$ is infinite elsewhere, its finite value at zero has a constant convex extension representing the same Snell envelope. Full statewise Bellman recursion at time zero requires an additional translated-integrability hypothesis.

##### Integrability of translated convex random-walk rewards

↑ **Parent:** [Optimal stopping value function](#optimal-stopping-value-function)

Let $Z_j$ be the sum of $j$ independent identically distributed real increments. For a finite [convex function](real-analysis.md#convex-function) $f$, integrability of $f(Z_j)$ and $f(Z_{j+1})$ implies integrability of $f(Z_j+x)$ for every fixed $x$. Its negative part is controlled by [negative part of a finite convex function is Lipschitz](real-analysis.md#negative-part-of-a-finite-convex-function-is-lipschitz). For $x>0$, if the increment law is unbounded above, take an independent increment $\eta$ with $p=\mathbb P(\eta\geq x)>0$. On this event convexity gives $f(Z_j+x)^+\leq f(Z_j)^++f(Z_j+\eta)^+$, so the expectation is bounded by $\mathbb E f(Z_j)^++p^{-1}\mathbb E f(Z_{j+1})^+$. If increments are bounded above by $M$, use $Z_j\leq jM$ and bound the positive part by $f(Z_j)^++f(jM+x)^+$. For $x<0$, use the symmetric lower-tail argument. This supplies translated integrability without assuming integrable increments or a growth bound on $f$.

### Optimal stopping time

↑ **Parent:** [Snell envelope](#snell-envelope)

An optimal stopping time attains the supremum of the expected reward over an admissible class of [stopping times](#stopping-time). For a finite-horizon [Snell envelope](#snell-envelope), the first time at which its value equals the current reward is optimal.

### Complementarity for the Snell envelope compensator

↑ **Parent:** [Snell envelope](#snell-envelope)

For the Doob compensator of a Snell envelope, $(V_n-Z_n)(A_{n+1}-A_n)=0$: compensation grows only on the stopping region $V_n=Z_n$.

### Optimal stopping time from the compensator

↑ **Parent:** [Snell envelope](#snell-envelope)

The first time the Snell-envelope compensator is about to become positive is an optimal stopping time; before it the martingale part equals both value and reward at stopping.

<h2 id="doob-s-martingale-inequality">Doob's martingale inequality</h2>

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doob's_martingale_inequality)

For a nonnegative submartingale $X$, the maximal tail bound is $\lambda\mathbb P(\max_{k\leq n}X_k\geq\lambda)\leq\mathbb E[X_n;\max_{k\leq n}X_k\geq\lambda]$. Applied to the absolute value of a martingale and integrated over $\lambda$, it gives the [Doob Lp maximal inequality](#doob-lp-maximal-inequality); at $p=2$ this is the [Doob L2 maximal inequality](#doob-l2-maximal-inequality).

<h2 id="doob-s-martingale-convergence-theorems">Doob's martingale convergence theorems</h2>

↑ **Parent:** [Martingale](martingale.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Doob's_martingale_convergence_theorems)

These are convergence results for martingales and submartingales under appropriate one-sided or absolute-integrability bounds. They distinguish almost-sure convergence from convergence in mean: uniform integrability gives the latter. The [martingale convergence theorem](#martingale-convergence-theorem) stated for an L1-bounded martingale is one standard member of the family.

## ↑ Ancestors (5)

1. [Probability theory](probability-theory.md)
2. [Probability and statistics](probability-and-statistics.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (565)

- [Absorption at zero of a nonnegative martingale](#absorption-at-zero-of-a-nonnegative-martingale)
- [Absorption-time bound from conditional variance and overshoot](#absorption-time-bound-from-conditional-variance-and-overshoot)
- [Adaptedness of a stopped right-continuous process](stochastic-process.md#adaptedness-of-a-stopped-right-continuous-process)
- [Almost sure convergence criterion for an independent Gaussian series](probability-theory.md#almost-sure-convergence-criterion-for-an-independent-gaussian-series)
- [Almost-sure martingale convergence to a nonintegrable limit](#almost-sure-martingale-convergence-to-a-nonintegrable-limit)
- [Almost sure submartingale convergence theorem](#almost-sure-submartingale-convergence-theorem)
- [Azuma's inequality](#azuma-s-inequality)
- [Barely-supercritical largest-component expectation](graph-theory.md#barely-supercritical-largest-component-expectation)
- [Bernstein bound for bounded-jump martingales](#bernstein-bound-for-bounded-jump-martingales)
- [Binary Brownian drift filter](time-series.md#binary-brownian-drift-filter)
- [Binomial-market probability density](mathematical-finance.md#binomial-market-probability-density)
- [Bounded-bracket criterion for a stochastic exponential](stochastic-calculus.md#bounded-bracket-criterion-for-a-stochastic-exponential)
- [Bounded-coefficient asset deflator](mathematical-finance.md#bounded-coefficient-asset-deflator)
- [Bounded diffusion coefficient gives square martingales](stochastic-calculus.md#bounded-diffusion-coefficient-gives-square-martingales)
- [Bounded harmonic function theorem on a recurrent graph](partial-differential-equation.md#bounded-harmonic-function-theorem-on-a-recurrent-graph)
- [Bounded harmonic representation with almost sure Brownian exit](analysis.md#bounded-harmonic-representation-with-almost-sure-brownian-exit)
- [Bounded-increment martingale convergence-or-oscillation dichotomy](stochastic-process.md#bounded-increment-martingale-convergence-or-oscillation-dichotomy)
- [Bounded-increment optional stopping with integrable time](#bounded-increment-optional-stopping-with-integrable-time)
- [Bounded local martingale criterion](#bounded-local-martingale-criterion)
- [Bounded stopping time](#bounded-stopping-time)
- [Bounded-stopping-time characterization of a martingale](#bounded-stopping-time-characterization-of-a-martingale)
- [Breadth-first exploration of a binomial random graph](graph-theory.md#breadth-first-exploration-of-a-binomial-random-graph)
- [Brownian martingale proof of Gaussian concentration](stochastic-process.md#brownian-martingale-proof-of-gaussian-concentration)
- [Brownian proof of the fundamental theorem of algebra](algebra.md#brownian-proof-of-the-fundamental-theorem-of-algebra)
- [Càdlàg martingale](#cadlag-martingale)
- [Centered finite-rate jump kernel gives square martingales](markov-process.md#centered-finite-rate-jump-kernel-gives-square-martingales)
- [Characterization of a martingale by bounded continuous-time stopped expectations](#characterization-of-a-martingale-by-bounded-continuous-time-stopped-expectations)
- [Characterization of a martingale by stopped expectations](#characterization-of-a-martingale-by-stopped-expectations)
- [Compensated jump-measure local martingale](markov-process.md#compensated-jump-measure-local-martingale)
- [Conditional-expectation martingale](#conditional-expectation-martingale)
- [Continuous local martingale with bounded quadratic variation](#continuous-local-martingale-with-bounded-quadratic-variation)
- [Continuous martingale](#continuous-martingale)
- [Continuous semimartingale](stochastic-calculus.md#continuous-semimartingale)
- [Counting-process martingale](stochastic-process.md#counting-process-martingale)
- [Cox-Ross short-rate pricing equation](mathematical-finance.md#cox-ross-short-rate-pricing-equation)
- [Density process](measure-theory.md#density-process)
- [Derivative-weighted call delta martingale](mathematical-finance.md#derivative-weighted-call-delta-martingale)
- [Diffusion martingale problem](stochastic-calculus.md#diffusion-martingale-problem)
- [Discount factor](mathematical-finance.md#discount-factor)
- [Discounted bond price martingale](mathematical-finance.md#discounted-bond-price-martingale)
- [Discounted dividend gains](mathematical-finance.md#discounted-dividend-gains)
- [Discounted wealth martingale integrability condition](mathematical-finance.md#discounted-wealth-martingale-integrability-condition)
- [Discrete Dupire equation](mathematical-finance.md#discrete-dupire-equation)
- [Discrete Tanaka formula](stochastic-calculus.md#discrete-tanaka-formula)
- [Discrete-time Markov chain martingale characterization](markov-process.md#discrete-time-markov-chain-martingale-characterization)
- [Doob exposure martingale](#doob-exposure-martingale)
- [Driftless square-root diffusion](stochastic-calculus.md#driftless-square-root-diffusion)
- [Dyadic conditional averages recover integrable functions](measure-theory.md#dyadic-conditional-averages-recover-integrable-functions)
- [Dyadic density martingale](measure-theory.md#dyadic-density-martingale)
- [Dyadic slope martingale](#dyadic-slope-martingale)
- [Dynkin's formula](stochastic-process.md#dynkin-s-formula)
- [Edge-exposure martingale](#edge-exposure-martingale)
- [Endpoint convergence of a bounded angle diffusion](stochastic-calculus.md#endpoint-convergence-of-a-bounded-angle-diffusion)
- [Equivalent local martingale measures exclude admissible arbitrage](mathematical-finance.md#equivalent-local-martingale-measures-exclude-admissible-arbitrage)
- [Exponential first-passage transform for an upward skip-free random walk](markov-process.md#exponential-first-passage-transform-for-an-upward-skip-free-random-walk)
- [Exponential Laplace martingale of a compound Poisson process](stochastic-process.md#exponential-laplace-martingale-of-a-compound-poisson-process)
- [Exponential martingale from a jump generator](markov-process.md#exponential-martingale-from-a-jump-generator)
- [Exponential martingale of a Lévy process](stochastic-process.md#exponential-martingale-of-a-levy-process)
- [Exponential martingale of a random walk](markov-process.md#exponential-martingale-of-a-random-walk)
- [Exponential moment bound for a Gaussian random-walk maximum](markov-process.md#exponential-moment-bound-for-a-gaussian-random-walk-maximum)
- [Exponential surplus martingale](actuarial-statistics.md#exponential-surplus-martingale)
- [Fair-coin doubling martingale](#fair-coin-doubling-martingale)
- [Fair-game gambling induced by an incentive fee](utility-function.md#fair-game-gambling-induced-by-an-incentive-fee)
- [Feynman-Kac formula with a bounded potential](stochastic-calculus.md#feynman-kac-formula-with-a-bounded-potential)
- [Finite-horizon pricing density for Gaussian drift learning](time-series.md#finite-horizon-pricing-density-for-gaussian-drift-learning)
- [Finite-variation terms do not change quadratic variation](stochastic-calculus.md#finite-variation-terms-do-not-change-quadratic-variation)
- [Finite voter-model consensus probability](#finite-voter-model-consensus-probability)
- [Forward-measure terminal rate in a linear bond model](mathematical-finance.md#forward-measure-terminal-rate-in-a-linear-bond-model)
- [Futures contract](mathematical-finance.md#futures-contract)
- [Futures pricing](mathematical-finance.md#futures-pricing)
- [Gaussian characteristic-function martingale from covariance loss](stochastic-process.md#gaussian-characteristic-function-martingale-from-covariance-loss)
- [Gaussian exponential martingale with deterministic variance](stochastic-process.md#gaussian-exponential-martingale-with-deterministic-variance)
- [Gaussian forward-rate covariance drift restriction](mathematical-finance.md#gaussian-forward-rate-covariance-drift-restriction)
- [Gaussian terminal value at a deterministic bracket level](#gaussian-terminal-value-at-a-deterministic-bracket-level)
- [Half-volatility measure for a square-root stock claim](mathematical-finance.md#half-volatility-measure-for-a-square-root-stock-claim)
- [Harmonic function for a Markov chain](markov-process.md#harmonic-function-for-a-markov-chain)
- [Harmonic functions of Brownian motion](partial-differential-equation.md#harmonic-functions-of-brownian-motion)
- [Heath-Jarrow-Morton model](mathematical-finance.md#heath-jarrow-morton-model)
- [High-level escape representation of a mapping-out height](stochastic-process.md#high-level-escape-representation-of-a-mapping-out-height)
- [Hypotheses for a diffusion scale hitting formula](stochastic-calculus.md#hypotheses-for-a-diffusion-scale-hitting-formula)
- [Independent increments of a Gaussian martingale](stochastic-process.md#independent-increments-of-a-gaussian-martingale)
- [Initial-value integrability in normalized semimartingale decompositions](stochastic-calculus.md#initial-value-integrability-in-normalized-semimartingale-decompositions)
- [Integrable discrete-time local martingale is a martingale](#integrable-discrete-time-local-martingale-is-a-martingale)
- [Integrable overshoot of a stopped L1-bounded martingale](#integrable-overshoot-of-a-stopped-l1-bounded-martingale)
- [Integrable-supremum martingale criterion](#integrable-supremum-martingale-criterion)
- [Kazamaki's condition](stochastic-calculus.md#kazamaki-s-condition)
- [Kolmogorov maximal inequality](#kolmogorov-maximal-inequality)
- [L2-bounded continuous martingale](#l2-bounded-continuous-martingale)
- [L2-bounded martingale convergence theorem](#l2-bounded-martingale-convergence-theorem)
- [L2 construction of compensated Poisson integrals](probability-theory.md#l2-construction-of-compensated-poisson-integrals)
- [Laplace transform of symmetric Brownian interval-exit time](brownian-motion.md#laplace-transform-of-symmetric-brownian-interval-exit-time)
- [Law of one price](mathematical-finance.md#law-of-one-price)
- [Lévy characterization of multidimensional Brownian motion](brownian-motion.md#levy-characterization-of-multidimensional-brownian-motion)
- [Localization and patching of quadratic variation](stochastic-calculus.md#localization-and-patching-of-quadratic-variation)
- [Lp martingale convergence theorem](#lp-martingale-convergence-theorem)
- [Martingale compound Poisson process](stochastic-process.md#martingale-compound-poisson-process)
- [Martingale construction of Lebesgue decomposition](measure-theory.md#martingale-construction-of-lebesgue-decomposition)
- [Martingale decomposition of a density-dependent jump process](markov-process.md#martingale-decomposition-of-a-density-dependent-jump-process)
- [Martingale-difference orthogonality](#martingale-difference-orthogonality)
- [Martingale difference sequence](#martingale-difference-sequence)
- [Martingale increments obstruct finite convergence](#martingale-increments-obstruct-finite-convergence)
- [Martingale problem for Brownian motion](stochastic-calculus.md#martingale-problem-for-brownian-motion)
- [Maturity monotonicity of calls with nonnegative strikes](mathematical-finance.md#maturity-monotonicity-of-calls-with-nonnegative-strikes)
- [Maximal bound for a nonnegative martingale](#maximal-bound-for-a-nonnegative-martingale)
- [Multi-period dividend pricing identity](mathematical-finance.md#multi-period-dividend-pricing-identity)
- [Nested polygonal approximation of Brownian rough paths](analysis.md#nested-polygonal-approximation-of-brownian-rough-paths)
- [Nonnegative discrete-time local martingale is a martingale](#nonnegative-discrete-time-local-martingale-is-a-martingale)
- [Nonnegative martingale](#nonnegative-martingale)
- [One-sided martingale maximal inequality](#one-sided-martingale-maximal-inequality)
- [One-sided maximal inequality for a centered square-integrable martingale](#one-sided-maximal-inequality-for-a-centered-square-integrable-martingale)
- [Parameter derivative of the exponential Brownian martingale](brownian-motion.md#parameter-derivative-of-the-exponential-brownian-martingale)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-21.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-22.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-24.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-27.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-29.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-31.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-32.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-29.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#6/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-32.md#6/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-33.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-39.md#3/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-28.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-30.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-31.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-34.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-35.md#5/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-7.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2.md#29i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-12.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#1/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-34.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-35.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/a/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-38.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-48.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-1.md#28i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#27i/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-3.md#27i/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4.md#28i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-14.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-31.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#1/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-32.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-35.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-39.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-40.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-43.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1.md#28j/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2.md#28j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#27j/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-3.md#28i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-33.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-36.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-37.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-39.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-41.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-42.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#28j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#28j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-2.md#28j/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-34.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-36.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-37.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#1/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-39.md#5/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-2.md#30j/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-101.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-29.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-31.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#5/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-32.md#6/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-39.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-2.md#30i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-27.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#1/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#1/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#5/b/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-28.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-29.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-38.md#3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#2/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-39.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-33.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-34.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#1/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#1/d/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-35.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-43.md#6/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-44.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-9.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-24.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-25.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-27.md#2/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-39.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#1/3/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-26.md#2/2/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#5/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-27.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#3/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-29.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-38.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#26k/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#26k/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1.md#26k/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-13.md#3/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#1/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#1/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#2/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-29.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#4/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-30.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-40.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-201.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#4/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#4/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-202.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-211.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#29j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#29j/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1.md#29j/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3.md#27j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4.md#28j/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#2/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#2/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#1/e/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#3/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-202.md#6/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-1.md#30k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3.md#29k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#1/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#1/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-201.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#1/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/iii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#2/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#4/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#5/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#5/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#5/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-202.md#6/iv/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-207.md#5/b/v/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#2/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#2/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#2/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#4/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#5/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#6/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-211.md#6/d/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#30k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#30k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1.md#30k/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-4.md#29k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-202.md#1/1/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4.md#29k/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1.md#19h/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1.md#30k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#29k/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-3.md#29k/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-201.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4.md#29k/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-201.md#1/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-201.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-207.md#4/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-201.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#2/c/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#2/c/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/a/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/a/ii/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/b/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#3/d/i/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-202.md#6/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-203.md#3/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#1/c/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#3/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#5/a/solution)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-201.md#5/b/solution)
- [Pasting ordered stopping times](#pasting-ordered-stopping-times)
- [Period-two martingale corrector for a birth-death chain](markov-process.md#period-two-martingale-corrector-for-a-birth-death-chain)
- [Poisson exponential martingale](probability-theory.md#poisson-exponential-martingale)
- [Positive martingale majorant of an L1-bounded submartingale](#positive-martingale-majorant-of-an-l1-bounded-submartingale)
- [Positive random-environment path-weight martingale](#positive-random-environment-path-weight-martingale)
- [Positive regression deflator in a complete finite market](mathematical-finance.md#positive-regression-deflator-in-a-complete-finite-market)
- [Predictable-coefficient localization of a martingale transform](#predictable-coefficient-localization-of-a-martingale-transform)
- [Predictable compensator of a jump measure](markov-process.md#predictable-compensator-of-a-jump-measure)
- [Pricing equation for a local volatility model](mathematical-finance.md#pricing-equation-for-a-local-volatility-model)
- [Radon-Nikodym density martingale](measure-theory.md#radon-nikodym-density-martingale)
- [Rare-jump martingale divergence](#rare-jump-martingale-divergence)
- [Risk-neutral measure for the Black-Scholes model](mathematical-finance.md#risk-neutral-measure-for-the-black-scholes-model)
- [Risk-neutral probability](mathematical-finance.md#risk-neutral-probability)
- [Risk-neutral probability in the Cox--Ross--Rubinstein model](probability-theory.md#risk-neutral-probability-in-the-cox-ross-rubinstein-model)
- [Short-rate bond pricing equation](mathematical-finance.md#short-rate-bond-pricing-equation)
- [Single marked exponential jump process](markov-process.md#single-marked-exponential-jump-process)
- [SLE4 angle martingale](stochastic-process.md#sle4-angle-martingale)
- [Space-time Hermite polynomial](numerical-analysis.md#space-time-hermite-polynomial)
- [Square martingale for independent centered sums](#square-martingale-for-independent-centered-sums)
- [Squared-population near-invariant for stochastic attrition](markov-process.md#squared-population-near-invariant-for-stochastic-attrition)
- [Stopped inverse radial power martingale classification](brownian-motion.md#stopped-inverse-radial-power-martingale-classification)
- [Stopped likelihood ratio under exponential tilting](markov-process.md#stopped-likelihood-ratio-under-exponential-tilting)
- [Stopped process](#stopped-process)
- [Stopping-time shift of a stochastic integral](stochastic-calculus.md#stopping-time-shift-of-a-stochastic-integral)
- [Strict local martingale](#strict-local-martingale)
- [Strict local martingale failure of the law of one price](mathematical-finance.md#strict-local-martingale-failure-of-the-law-of-one-price)
- [Strong law for martingales with bounded increments](#strong-law-for-martingales-with-bounded-increments)
- [Tail event for a vanishing positive path-weight limit](#tail-event-for-a-vanishing-positive-path-weight-limit)
- [Terminal correlation does not identify adapted stock volatility](variance.md#terminal-correlation-does-not-identify-adapted-stock-volatility)
- [Terminal proportionality identifies bounded stock volatility](variance.md#terminal-proportionality-identifies-bounded-stock-volatility)
- [Time-dependent test functions for a diffusion martingale problem](stochastic-calculus.md#time-dependent-test-functions-for-a-diffusion-martingale-problem)
- [Transversality and fundamental dividend prices](mathematical-finance.md#transversality-and-fundamental-dividend-prices)
- [Unchanging betting probability under sampling without replacement](#unchanging-betting-probability-under-sampling-without-replacement)
- [Uniform-arrival residual mass martingale](#uniform-arrival-residual-mass-martingale)
- [Uniform integrability of a stopped uniformly integrable martingale](#uniform-integrability-of-a-stopped-uniformly-integrable-martingale)
- [Uniformly integrable martingale](#uniformly-integrable-martingale)
- [Uniformly integrable martingale convergence theorem](#uniformly-integrable-martingale-convergence-theorem)
- [Upcrossing count](#upcrossing-count)
- [Usual conditions for a filtration](stochastic-process.md#usual-conditions-for-a-filtration)
- [Verification by a nonnegative control supermartingale](mathematical-optimization.md#verification-by-a-nonnegative-control-supermartingale)
- [Ville inequality](#ville-inequality)
- [Waiting time for a word in independent nonuniform symbols](mathematics.md#waiting-time-for-a-word-in-independent-nonuniform-symbols)
- [Well-posed martingale problem](stochastic-calculus.md#well-posed-martingale-problem)
- [Wright–Fisher binomial sampling chain](stochastic-calculus.md#wright-fisher-binomial-sampling-chain)
- [Zero-recovery default model](mathematical-finance.md#zero-recovery-default-model)
