# Ergodic theory

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ergodic_theory)

Ergodic theory studies the long-time statistical behaviour of [measure-preserving transformations](#measure-preserving-transformation).

**Table of contents**

- [Generic point for an invariant measure](#generic-point-for-an-invariant-measure)
- [Invariant measure](#invariant-measure)
  - [Invariant probability measure for a semigroup](#invariant-probability-measure-for-a-semigroup)
    - [Krylov–Bogolyubov theorem](#krylov-bogolyubov-theorem)
- [Cutting and stacking](#cutting-and-stacking)
  - [Chacon transformation](#chacon-transformation)
- [Unique ergodicity](#unique-ergodicity)
  - [Uniform ergodic convergence for uniquely ergodic systems](#uniform-ergodic-convergence-for-uniquely-ergodic-systems)
- [Van der Corput lemma (Hilbert space sequences)](#van-der-corput-lemma-hilbert-space-sequences)
  - [Van der Corput inequality for finite scalar sequences](#van-der-corput-inequality-for-finite-scalar-sequences)
- [Equidistributed sequence](#equidistributed-sequence)
  - [Equidistribution criterion for a torus translation](#equidistribution-criterion-for-a-torus-translation)
  - [Interval discrepancy](#interval-discrepancy)
  - [Weyl criterion](#weyl-criterion)
    - [Differencing obstruction to equidistribution](#differencing-obstruction-to-equidistribution)
    - [Equidistribution of a quadratic polynomial with irrational leading coefficient](#equidistribution-of-a-quadratic-polynomial-with-irrational-leading-coefficient)
      - [Uniform square recurrence on the circle](#uniform-square-recurrence-on-the-circle)
- [Nonsingular transformation](#nonsingular-transformation)
- [Koopman operator](#koopman-operator)
  - [Spectral measure of a Koopman observable](#spectral-measure-of-a-koopman-observable)
  - [Almost periodic observable](#almost-periodic-observable)
    - [Syndetic near returns of an almost periodic observable](#syndetic-near-returns-of-an-almost-periodic-observable)
    - [Compact measure-preserving system](#compact-measure-preserving-system)
  - [Decay of autocorrelation implies weak convergence of an observable](#decay-of-autocorrelation-implies-weak-convergence-of-an-observable)
  - [Bounded Koopman operator criterion](#bounded-koopman-operator-criterion)
- [Measure-preserving transformation](#measure-preserving-transformation)
  - [Lebesgue-measure-preserving map](#lebesgue-measure-preserving-map)
  - [Integer multiplication map on the circle](#integer-multiplication-map-on-the-circle)
    - [Ergodicity of integer multiplication on the circle](#ergodicity-of-integer-multiplication-on-the-circle)
  - [Measure-preserving system](#measure-preserving-system)
    - [Factor of a measure-preserving system](#factor-of-a-measure-preserving-system)
      - [Factor map between measure-preserving systems](#factor-map-between-measure-preserving-systems)
        - [Compact extension of a measure-preserving system](#compact-extension-of-a-measure-preserving-system)
          - [Finite-fiber compact extension](#finite-fiber-compact-extension)
          - [Positive-measure almost periodic indicator in a compact extension](#positive-measure-almost-periodic-indicator-in-a-compact-extension)
        - [Relatively almost periodic observable](#relatively-almost-periodic-observable)
          - [Localization of relative almost periodicity to base sets](#localization-of-relative-almost-periodicity-to-base-sets)
  - [Finite full-support measure-preserving map is bijective](#finite-full-support-measure-preserving-map-is-bijective)
  - [Invertible measure-preserving system](#invertible-measure-preserving-system)
  - [Invariant sigma-algebra](#invariant-sigma-algebra)
    - [Invariant set of a measure-preserving transformation](#invariant-set-of-a-measure-preserving-transformation)
  - [Ergodicity](#ergodicity)
    - [Strong mixing](#strong-mixing)
      - [Diagonal set-correlation criterion for mixing](#diagonal-set-correlation-criterion-for-mixing)
    - [Ergodic decomposition](#ergodic-decomposition)
      - [Ergodic components of a rational circle rotation](#ergodic-components-of-a-rational-circle-rotation)
      - [Ergodic component](#ergodic-component)
        - [Countable-test proof of ergodicity of conditional components](#countable-test-proof-of-ergodicity-of-conditional-components)
      - [Affinity of entropy under ergodic decomposition](#affinity-of-entropy-under-ergodic-decomposition)
    - [Ergodic invariant probability on a countable state space has finite cyclic support](#ergodic-invariant-probability-on-a-countable-state-space-has-finite-cyclic-support)
    - [Invariant-function characterization of ergodicity](#invariant-function-characterization-of-ergodicity)
    - [Bernoulli shift](#bernoulli-shift)
      - [Bernoulli coordinate observable is not almost periodic](#bernoulli-coordinate-observable-is-not-almost-periodic)
      - [Cantor Bernoulli measure](#cantor-bernoulli-measure)
    - [Irrational rotation](#irrational-rotation)
      - [Ergodicity criterion for a circle rotation](#ergodicity-criterion-for-a-circle-rotation)
      - [Everywhere interval frequency under an irrational rotation](#everywhere-interval-frequency-under-an-irrational-rotation)
    - [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)
      - [Arithmetic-progression multiple averages under weak mixing](#arithmetic-progression-multiple-averages-under-weak-mixing)
        - [Density convergence of multiple weak-mixing correlations](#density-convergence-of-multiple-weak-mixing-correlations)
      - [Stability of weak mixing under powers and products](#stability-of-weak-mixing-under-powers-and-products)
      - [Product characterization of weak mixing](#product-characterization-of-weak-mixing)
        - [Square-correlation proof of weak mixing from product ergodicity](#square-correlation-proof-of-weak-mixing-from-product-ergodicity)
      - [Koopman eigenfunction obstruction to weak mixing](#koopman-eigenfunction-obstruction-to-weak-mixing)
      - [Simultaneous hitting characterization of weak mixing](#simultaneous-hitting-characterization-of-weak-mixing)
  - [Poincaré recurrence theorem](#poincare-recurrence-theorem)
    - [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem)
      - [SZ property](#sz-property)
      - [Multiple recurrence for circle rotations](#multiple-recurrence-for-circle-rotations)
- [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)
  - [Nonnegative ergodic averages with infinite integral](#nonnegative-ergodic-averages-with-infinite-integral)
  - [Maximal ergodic lemma](#maximal-ergodic-lemma)
  - [Triangular ergodic averaging lemma](#triangular-ergodic-averaging-lemma)
  - [Linear growth bound for integrable observables](#linear-growth-bound-for-integrable-observables)
    - [Sharpness of the linear growth bound for integrable observables](#sharpness-of-the-linear-growth-bound-for-integrable-observables)
  - [L1 convergence in the Birkhoff ergodic theorem on a finite measure space](#l1-convergence-in-the-birkhoff-ergodic-theorem-on-a-finite-measure-space)
- [Upper Banach density](#upper-banach-density)
  - [Furstenberg correspondence principle](#furstenberg-correspondence-principle)
- [Convergence in density of a sequence](#convergence-in-density-of-a-sequence)
  - [Mean-square criterion for convergence in density](#mean-square-criterion-for-convergence-in-density)
  - [Cesaro convergence of a sequence](#cesaro-convergence-of-a-sequence)
- [Entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition)
  - [Conditional entropy of finite measurable partitions](#conditional-entropy-of-finite-measurable-partitions)
  - [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)
    - [Infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate)
      - [Block conditional entropy given the infinite future](#block-conditional-entropy-given-the-infinite-future)
    - [Shannon-McMillan-Breiman theorem](#shannon-mcmillan-breiman-theorem)
    - [Monotonicity of normalized block entropy](#monotonicity-of-normalized-block-entropy)
    - [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)
      - [Completely positive entropy](#completely-positive-entropy)
      - [Generating measurable partition](#generating-measurable-partition)
        - [One-sided generator](#one-sided-generator)
          - [Finite one-sided generator of an invertible system forces zero entropy](#finite-one-sided-generator-of-an-invertible-system-forces-zero-entropy)
        - [Kolmogorov-Sinai generator theorem](#kolmogorov-sinai-generator-theorem)
      - [Host equidistribution theorem](#host-equidistribution-theorem)
        - [Rudolph measure rigidity theorem](#rudolph-measure-rigidity-theorem)
      - [Entropy preservation under a finite-to-one factor](#entropy-preservation-under-a-finite-to-one-factor)
      - [Pinsker sigma-algebra](#pinsker-sigma-algebra)
        - [Tail characterization of the Pinsker sigma-algebra](#tail-characterization-of-the-pinsker-sigma-algebra)
    - [Infimum rule for partition entropy rate](#infimum-rule-for-partition-entropy-rate)
- [K-mixing](#k-mixing)
  - [Tail sigma-algebra of a measurable partition](#tail-sigma-algebra-of-a-measurable-partition)
    - [Finite partitions measurable in a partition tail have zero entropy rate](#finite-partitions-measurable-in-a-partition-tail-have-zero-entropy-rate)

## Generic point for an invariant measure

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

A point is generic for an [invariant measure](#invariant-measure) $\mu$ of a [continuous map](topology.md#continuous-map) on a [compact metric space](topological-analysis.md#compact-metric-space) if the displayed convergence holds for every [continuous function](calculus.md#continuous-function) $\varphi$. Its empirical [probability measures](probability-space.md#probability-measure) converge against continuous test functions to $\mu$. The same test-function condition may be used before invariance is known: the telescoping identity for $\varphi\circ f-\varphi$ then proves that the limiting [Borel probability measure](measure.md#borel-probability-measure) must be invariant. If almost every point is generic for the same measure, continuous approximation of invariant-set indicators proves that this measure is [ergodic](#ergodicity).

## Invariant measure

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

For a measurable transformation $T$, a [measure](measure.md) is invariant if the [pushforward measure](measure.md#pushforward-measure) equals the original [measure](measure.md), or equivalently $\mu(T^{-1}A)=\mu(A)$ for every measurable $A$. This is the [measure](measure.md) used in a [measure-preserving system](#measure-preserving-system).

### Invariant probability measure for a semigroup

↑ **Parent:** [Invariant measure](#invariant-measure)

A [Borel probability measure](measure.md#borel-probability-measure) is invariant for a [Markov kernel](markov-chain.md#markov-kernel) semigroup if every transition preserves it. For a [Feller semigroup](functional-analysis.md#feller-semigroup) on a compact metric space, it suffices to test the displayed identity on [continuous functions](calculus.md#continuous-function). Kernel [Jensen inequality](real-analysis.md#jensen-s-inequality) gives contraction on $L^p(\mu)$, and sup-norm strong continuity followed by density gives [strong continuity](functional-analysis.md#strong-continuity) there for $1\leq p<\infty$.

<h4 id="krylov-bogolyubov-theorem">Krylov–Bogolyubov theorem</h4>

↑ **Parent:** [Invariant probability measure for a semigroup](#invariant-probability-measure-for-a-semigroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krylov–Bogolyubov_theorem)

For a [Feller semigroup](functional-analysis.md#feller-semigroup) on a compact [metric space](topological-analysis.md#metric-space), time-averaged transition laws have weakly convergent subsequences by [compactness of probability measures on a compact metric space](convergence-of-random-variables.md#compactness-of-probability-measures-on-a-compact-metric-space). Shifting a time interval of length $n$ by $t$ changes a bounded test-function average by at most $2t\|f\|_\infty/n$. A weak subsequential limit is therefore an [invariant probability measure for a semigroup](#invariant-probability-measure-for-a-semigroup). More generally, tightness of the time averages supplies the required compactness.

## Cutting and stacking

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

Cutting and stacking constructs [measure-preserving transformations](#measure-preserving-transformation) from towers of equal-measure levels. Cut a tower into equal-width subcolumns, add new spacer levels, and stack the resulting columns. Map each level to the one above by a measure-preserving identification; subsequent stages extend the partial map. When uncovered and top-level measures tend to zero, the limiting map is defined modulo null sets.

### Chacon transformation

↑ **Parent:** [Cutting and stacking](#cutting-and-stacking)

The standard three-cut Chacon transformation is an invertible [measure-preserving transformation](#measure-preserving-transformation) built by [cutting and stacking](#cutting-and-stacking) with spacer vector $(0,1,0)$ at every stage. Cut the current tower into three equal subcolumns, place one spacer above the middle, and stack left to right. With initial width $2/3$ and height one on a unit interval, level counts and widths are $h_j=(3^{j+1}-1)/2$ and $w_j=2/3^{j+1}$. Tower measure tends to one, using total spacer measure $1/3$. Tower words obey $W_{j+1}=W_jW_j1W_j$.

## Unique ergodicity

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

A continuous self-map of a compact [metric space](topological-analysis.md#metric-space) is uniquely ergodic when it has exactly one invariant [Borel probability measure](measure.md#borel-probability-measure). An [irrational rotation of the circle](#irrational-rotation) is uniquely ergodic: invariance multiplies its nonzero-index [Fourier coefficients](fourier-series.md#fourier-coefficient) by nontrivial phases, forcing those coefficients to vanish. The [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) then identifies the invariant measure as normalized [Lebesgue measure](measure-theory.md#lebesgue-measure).

### Uniform ergodic convergence for uniquely ergodic systems

↑ **Parent:** [Unique ergodicity](#unique-ergodicity)

For a [uniquely ergodic](#unique-ergodicity) continuous map $T$ of a compact [metric space](topological-analysis.md#metric-space), every continuous $f$ satisfies $N^{-1}\sum_{j=0}^{N-1}f(T^jx)\to\int f\,d\mu$ uniformly in $x$. Otherwise choose increasingly long orbit [empirical measures](probability-space.md#empirical-measure) with a fixed discrepancy. Compactness provides a weak limit; the telescoping identity makes it invariant, so it must be the unique measure $\mu$, contradicting that discrepancy. Compactness and continuity are essential hypotheses.

## Van der Corput lemma (Hilbert space sequences)

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

For a bounded sequence $(u_n)$ in a [Hilbert space](hilbert-space.md), put $c_h=\limsup_{N\to\infty}|N^{-1}\sum_{n=0}^{N-h-1}\langle u_{n+h},u_n\rangle|$. If $H^{-1}\sum_{h=1}^Hc_h\to0$, then $N^{-1}\sum_{n=0}^{N-1}u_n\to0$ in norm. Since the $c_h$ are bounded, it suffices that $(c_h)$ has [convergence in density of a sequence](#convergence-in-density-of-a-sequence) to zero. The proof applies the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to an average of shifted sums.

### Van der Corput inequality for finite scalar sequences

↑ **Parent:** [Van der Corput lemma (Hilbert space sequences)](#van-der-corput-lemma-hilbert-space-sequences)

For complex numbers $|u_n|\leq1$, $0\leq n<N$, and $1\leq H\leq N$, put $C_h=\sum_{n=0}^{N-h-1}u_{n+h}\overline{u_n}$. Then

$$
\left|\frac1N\sum_{n=0}^{N-1}u_n\right|^2
\leq\frac{N+H-1}{NH}\left(1+2\sum_{h=1}^{H-1}\left(1-\frac hH\right)\frac{|C_h|}{N}\right).
$$

Extend the sequence by zero, count each summand in $H$ consecutive windows, and apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to their sum. Expansion of the squared window sums gives the stated coefficients. Fixing $H$ and making each normalized correlation tend to zero bounds the limiting squared average by $1/H$; then let $H$ tend to infinity. This is the scalar finite form underlying the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences).

## Equidistributed sequence

↑ **Parent:** [Ergodic theory](ergodic-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equidistributed_sequence)

A sequence $(x_n)$ in $\mathbb R/\mathbb Z$ is equidistributed if the limiting frequency in every half-open interval equals that interval's length. Equivalently, its empirical probability measures converge to normalized [Lebesgue measure](measure-theory.md#lebesgue-measure) when tested against every continuous function.

### Equidistribution criterion for a torus translation

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

The sequence $r(u,v)$ is equidistributed in $\mathbb T^2$ precisely when $ku+\ell v\notin2\pi\mathbb Z$ for every nonzero integer pair $(k,\ell)$. Equivalently $1,u/(2\pi),v/(2\pi)$ are rationally independent. Under that condition, nonconstant character averages tend to zero by the geometric-series formula. Uniform approximation by [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) gives convergence for continuous functions, and continuous upper and lower bounds give convergence for rectangles. If a character is resonant, the orbit lies in its proper closed kernel and misses a positive-area rectangle, so equidistribution fails.

### Interval discrepancy

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

Interval discrepancy measures the difference between empirical counts and the expected count for normalized [Lebesgue measure](measure-theory.md#lebesgue-measure). Convolving an enlarged interval [indicator function](measure-theory.md#indicator-function) with a narrow unit-integral [indicator function](measure-theory.md#indicator-function) gives a continuous majorant. Its [Fourier coefficients](fourier-series.md#fourier-coefficient) decay as $O(1/(\delta k^2))$, converting the count into a constant term, finite exponential sums and a controlled absolute tail.

### Weyl criterion

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

A sequence $(x_n)$ in $\mathbb R/\mathbb Z$ is an [equidistributed sequence](#equidistributed-sequence) if and only if $N^{-1}\sum_{n=0}^{N-1}e^{2\pi i m x_n}\to0$ for every nonzero integer $m$. Approximation of continuous functions by [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) proves the criterion.

#### Differencing obstruction to equidistribution

↑ **Parent:** [Weyl criterion](#weyl-criterion)

If a circle-valued sequence is not an [equidistributed sequence](#equidistributed-sequence), some positive-shift difference is not equidistributed either. The contrapositive follows by applying the [Van der Corput inequality for finite scalar sequences](#van-der-corput-inequality-for-finite-scalar-sequences) to every nonzero integer [exponential sum](analytic-number-theory.md#exponential-sum). Thus cancellation for all fixed nonzero differences implies [equidistribution](#equidistributed-sequence) of the original sequence.

#### Equidistribution of a quadratic polynomial with irrational leading coefficient

↑ **Parent:** [Weyl criterion](#weyl-criterion)

If $a$ is irrational and $b,c$ are real, the fractional parts of $an^2+bn+c$ form an [equidistributed sequence](#equidistributed-sequence). In the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences), every nonzero-lag correlation of $e^{2\pi im(an^2+bn+c)}$ is a [geometric series](sequence-and-series.md#geometric-series) with irrational frequency $2mah$ and tends to zero. The [Weyl criterion](#weyl-criterion) then applies.

##### Uniform square recurrence on the circle

↑ **Parent:** [Equidistribution of a quadratic polynomial with irrational leading coefficient](#equidistribution-of-a-quadratic-polynomial-with-irrational-leading-coefficient)

For rational $a$, a multiple of its denominator gives exact integer recurrence. For irrational $a$, [Weyl differencing](analytic-number-theory.md#weyl-differencing) and the [Weyl criterion](#weyl-criterion) give an [equidistributed sequence](#equidistributed-sequence) $am^2$ modulo one. Thus every parameter belongs to one of the open sets $\{a:\|am^2\|<\epsilon\}$. Compactness of the [circle group](lie-theory.md#circle-group) gives a finite subcover, hence a bound $N$ uniform in $a$; no explicit rate follows from this compactness step.

## Nonsingular transformation

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

A measurable transformation $T:X\to X$ is nonsingular with respect to $\mu$ when $\mu(T^{-1}N)=0$ for every $\mu$-null set $N$, equivalently when the [pushforward measure](measure.md#pushforward-measure) $T_*\mu$ is [absolutely continuous](measure-theory.md#absolute-continuity-of-measures) with respect to $\mu$.

## Koopman operator

↑ **Parent:** [Ergodic theory](ergodic-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koopman_operator)

For a measurable dynamical map $F$, the Koopman operator acts on observables by $K_Fg=g\circ F$. If $F$ is nonsingular, it defines an operator on equivalence classes of measurable functions.

### Spectral measure of a Koopman observable

↑ **Parent:** [Koopman operator](#koopman-operator)

The finite positive measure representing an observable's autocorrelation sequence by the [Bochner–Herglotz theorem](harmonic-analysis.md#bochner-herglotz-theorem). For a probability [measure-preserving system](#measure-preserving-system), the [Koopman operator](#koopman-operator) is an [isometry](riemannian-geometry.md#isometry), so its forward autocorrelations, extended by complex conjugation to negative indices, form a [positive-definite function](harmonic-analysis.md#positive-definite-function) on $\mathbb Z$. The measure has mass $\|f\|_2^2$, and its atoms are squared norms of projections onto [Koopman operator](#koopman-operator) eigenspaces, including for noninvertible transformations.

### Almost periodic observable

↑ **Parent:** [Koopman operator](#koopman-operator)

An $L^2$ observable of an invertible probability [measure-preserving system](#measure-preserving-system) is almost periodic when its [Koopman operator](#koopman-operator) orbit is totally bounded in the global $L^2$ norm. A noninvertible system uses its forward orbit. This is the Hilbert-space dynamical definition, distinguished from uniform almost periodicity for continuous functions of a real variable.

#### Syndetic near returns of an almost periodic observable

↑ **Parent:** [Almost periodic observable](#almost-periodic-observable)

If the forward orbit of $f$ under an [isometry](riemannian-geometry.md#isometry) $U$ is totally bounded, choose a finite net whose centers are $U^{n_j}f$ and let $M=\max_jn_j$. For every sufficiently large $n$, some center is within $\varepsilon$ of $U^nf$, so cancellation gives $n-n_j\in R_\varepsilon$. Thus $R_\varepsilon$ is a [syndetic set](dynamical-systems.md#syndetic-set). Telescoping also gives $\|U^{kn}f-f\|_2\leq k\|U^nf-f\|_2$.

#### Compact measure-preserving system

↑ **Parent:** [Almost periodic observable](#almost-periodic-observable)

A probability [measure-preserving system](#measure-preserving-system) is compact if every $L^2$ observable has a relatively compact [Koopman operator](#koopman-operator) orbit in the global $L^2$ norm. For an invertible system one may use all integer times; for a general transformation use nonnegative times. This is a measure-theoretic definition, stronger than compactness of the underlying topological space.

### Decay of autocorrelation implies weak convergence of an observable

↑ **Parent:** [Koopman operator](#koopman-operator)

For a probability [measure-preserving system](#measure-preserving-system), if $\langle U_T^nf,f\rangle\to|\int f\,d\mu|^2$, then $U_T^nf$ converges weakly in $L^2$ to $(\int f\,d\mu)\mathbf1$. Centre $v=f-(\int f)\mathbf1$; its autocorrelations tend to zero. The [isometry](riemannian-geometry.md#isometry) identity gives the same decay against each $U_T^kv$, hence by approximation against their closed forward span. Against its orthogonal complement the correlations are exactly zero. [Orthogonal decomposition by a closed subspace](hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) finishes the proof without invertibility.

### Bounded Koopman operator criterion

↑ **Parent:** [Koopman operator](#koopman-operator)

For a nonsingular map $F$ on a probability space, $K_F$ extends boundedly to $L^2$ exactly when $d(F_*\mu)/d\mu\in L^\infty$. In that case

$$
\|K_F\|^2=\left\|\frac{d(F_*\mu)}{d\mu}\right\|_\infty.
$$

## Measure-preserving transformation

↑ **Parent:** [Ergodic theory](ergodic-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measure-preserving_transformation)

A measurable transformation $T:X\to X$ preserves a measure $\mu$ when $\mu(T^{-1}A)=\mu(A)$ for every measurable set $A$.

### Lebesgue-measure-preserving map

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

Such a measurable self-map preserves [Lebesgue measure](measure-theory.md#lebesgue-measure). On the unit interval examples include the identity, reflection $t\mapsto1-t$, and $t\mapsto2t\pmod1$. Invertibility is not required.

### Integer multiplication map on the circle

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

For an integer $K\geq2$, multiplication by $K$ on the [circle group](lie-theory.md#circle-group) preserves normalized [Lebesgue measure](measure-theory.md#lebesgue-measure). Each inverse image consists of $K$ branches, each scaling lengths by $1/K$.

#### Ergodicity of integer multiplication on the circle

↑ **Parent:** [Integer multiplication map on the circle](#integer-multiplication-map-on-the-circle)

The [integer multiplication map on the circle](#integer-multiplication-map-on-the-circle) is an [ergodic transformation](#ergodicity) for [Lebesgue measure](measure-theory.md#lebesgue-measure). In the [Fourier basis](fourier-series.md#fourier-basis), an invariant function has coefficients $c_j=0$ when $K$ does not divide $j$, and $c_j=c_{j/K}$ otherwise. Every nonzero index eventually reduces to the first case, so only the constant coefficient remains.

### Measure-preserving system

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

A measure-preserving system is a measure space $(X,\mathcal B,\mu)$ together with a [measure-preserving transformation](#measure-preserving-transformation) $T$. In ergodic theory the measure is commonly a probability measure.

#### Factor of a measure-preserving system

↑ **Parent:** [Measure-preserving system](#measure-preserving-system)

A factor map $\pi$ is a measurable map satisfying $\pi\circ T=S\circ\pi$ and $\pi_*\mu=\nu$, from one [measure-preserving system](#measure-preserving-system) to another. The target system is the factor; its observable functions pull back to observable functions of the source.

##### Factor map between measure-preserving systems

↑ **Parent:** [Factor of a measure-preserving system](#factor-of-a-measure-preserving-system)

A measurable measure-preserving map intertwining the transformations of two probability [measure-preserving systems](#measure-preserving-system). The equalities may be imposed on invariant full-measure domains. It represents the target's observable information inside the source. The [conditional measures of a factor](probability-theory.md#conditional-measures-of-a-factor) describe the information remaining on each fiber.

###### Compact extension of a measure-preserving system

↑ **Parent:** [Factor map between measure-preserving systems](#factor-map-between-measure-preserving-systems)

An extension for which the [relatively almost periodic observables](#relatively-almost-periodic-observable) are dense in global $L^2$. Density does not assert that every $L^2$ function already meets the uniform finite-net condition on fibers. Localization yields the [positive-measure almost periodic indicator in a compact extension](#positive-measure-almost-periodic-indicator-in-a-compact-extension).

###### Finite-fiber compact extension

↑ **Parent:** [Compact extension of a measure-preserving system](#compact-extension-of-a-measure-preserving-system)

For a skew-product extension with finitely many labeled fibers, the orbit of a bounded observable on each fiber lies in a fixed bounded subset of a finite-dimensional vector space. A finite net there supplies global centers constant in the base coordinate. Bounded observables are dense in $L^2$, so this is a [compact extension](#compact-extension-of-a-measure-preserving-system). Global almost periodicity can still fail because the base can be weakly mixing.

###### Positive-measure almost periodic indicator in a compact extension

↑ **Parent:** [Compact extension of a measure-preserving system](#compact-extension-of-a-measure-preserving-system)

Approximate $\mathbf1_A$ by relative almost periodic functions with summable squared global errors. [Tonelli theorem](measure-theory.md#tonelli-theorem) makes their conditional errors tend to zero almost everywhere. Choose a positive base set on which the conditional mass of $A$ is bounded below, then use the [Egorov theorem](sequence-and-series.md#egorov-s-theorem) to make those errors uniform on a smaller positive set $C$. [Localization of relative almost periodicity to base sets](#localization-of-relative-almost-periodicity-to-base-sets) and conditional-norm closure prove $\mathbf1_B$ is relatively almost periodic and $\mu(B)>0$.

###### Relatively almost periodic observable

↑ **Parent:** [Factor map between measure-preserving systems](#factor-map-between-measure-preserving-systems)

For every positive $\varepsilon$, require finitely many global $L^2$ centers $g_j$ such that the displayed inequality holds for every integer $n$ on almost every fiber of the [factor map](#factor-map-between-measure-preserving-systems). A center can depend on the fiber and time; its finite list is fixed. This is weaker than [almost periodic observable](#almost-periodic-observable) in global norm. For noninvertible systems use nonnegative times.

###### Localization of relative almost periodicity to base sets

↑ **Parent:** [Relatively almost periodic observable](#relatively-almost-periodic-observable)

Multiplying a [relatively almost periodic observable](#relatively-almost-periodic-observable) by a base-set indicator preserves [relative almost periodicity](#relatively-almost-periodic-observable): on each fiber an orbit value is either unchanged or zero, so add zero to the finite list of centers. [Conditional norm covariance under a factor map](measure-theory.md#conditional-norm-covariance-under-a-factor-map) also proves closure under convergence in the [uniform conditional L2 norm](measure-theory.md#uniform-conditional-l2-norm).

### Finite full-support measure-preserving map is bijective

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

Let $X$ be a [finite set](set.md#finite-set), let every singleton have positive probability, and let $T:X\to X$ preserve that probability measure. For every $x\in X$,

$$
\mu(T^{-1}\{x\})=\mu(\{x\})>0,
$$

so every $x$ has a preimage. Thus $T$ is a [surjection](algebra.md#surjective-function), and every surjection from a finite set to itself is a [bijection](function.md#bijection).

### Invertible measure-preserving system

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

An invertible measure-preserving system has a measurable inverse modulo null sets and preserves its measure in both time directions. Its [Koopman operator](#koopman-operator) on $L^2$ is unitary.

### Invariant sigma-algebra

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

The invariant sigma-algebra of $T$ consists, modulo null sets, of measurable sets $A$ satisfying $T^{-1}A=A$.

#### Invariant set of a measure-preserving transformation

↑ **Parent:** [Invariant sigma-algebra](#invariant-sigma-algebra)

A measurable set $A$ satisfying $T^{-1}A=A$, or equality modulo null sets in the measure-theoretic convention. These sets form a $\sigma$-algebra, and an [ergodic measure-preserving transformation](#ergodicity) gives each invariant set probability zero or one.

### Ergodicity

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ergodicity)

A [measure-preserving transformation](#measure-preserving-transformation) is ergodic when every set in its [invariant sigma-algebra](#invariant-sigma-algebra) has measure zero or full measure. Equivalently, every integrable invariant function is almost everywhere constant.

#### Strong mixing

↑ **Parent:** [Ergodicity](#ergodicity)

A probability [measure-preserving transformation](#measure-preserving-transformation) is strongly mixing when $\mu(T^{-n}A\cap B)\to\mu(A)\mu(B)$ for every pair of measurable sets $A,B$. Unlike weak mixing, this is an ordinary limit along all sufficiently large times.

##### Diagonal set-correlation criterion for mixing

↑ **Parent:** [Strong mixing](#strong-mixing)

A probability [measure-preserving transformation](#measure-preserving-transformation) is [strong mixing](#strong-mixing) exactly when $\mu(T^{-n}A\cap A)\to\mu(A)^2$ for every measurable $A$. The converse follows by applying [decay of autocorrelation implies weak convergence of an observable](#decay-of-autocorrelation-implies-weak-convergence-of-an-observable) to $f=\mathbf1_A$ and then testing against $\mathbf1_B$. Diagonal polarization alone controls a sum of the two directed cross-correlations and does not suffice as a proof.

#### Ergodic decomposition

↑ **Parent:** [Ergodicity](#ergodicity)

For a [measure-preserving system](#measure-preserving-system) on a standard probability space, an invariant probability measure is an integral of ergodic invariant probability measures. Its conditional measures given the [invariant sigma-algebra](#invariant-sigma-algebra) are the ergodic components.

##### Ergodic components of a rational circle rotation

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

For rotation by $p/q$ with coprime integers and Haar probability on the circle, components are the equal measures on the $q$-point orbits. The quotient map is $x\mapsto qx\pmod1$. Integration over the quotient recovers Haar measure, and the rotation permutes each orbit transitively, making its [probability measure](probability-space.md#probability-measure) [ergodic](#ergodicity).

##### Ergodic component

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

A conditional probability of an invariant [probability measure](probability-space.md#probability-measure) given its [invariant sigma-algebra](#invariant-sigma-algebra). In a standard Borel probability system, almost every such probability is invariant and [ergodic](#ergodicity). Their integral recovers the original measure. The [countable-test proof of ergodicity of conditional components](#countable-test-proof-of-ergodicity-of-conditional-components) explains why invariance alone is not the whole conclusion.

###### Countable-test proof of ergodicity of conditional components

↑ **Parent:** [Ergodic component](#ergodic-component)

Apply the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) to a countable generating algebra, and disintegrate the resulting common full-measure convergence set over the [invariant sigma-algebra](#invariant-sigma-algebra). The orbit limits on a fiber are its conditional masses. Applying the theorem to that invariant component shows its invariant projection is constant on all generating indicators, hence on all $L^2$ functions by density. This proves [ergodicity](#ergodicity) without an uncountable intersection of null sets.

##### Affinity of entropy under ergodic decomposition

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

If $\mu=\int\nu\,d\tau(\nu)$ is an [ergodic decomposition](#ergodic-decomposition), then the [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy) satisfies $h_\mu(T)=\int h_\nu(T)\,d\tau(\nu)$.

#### Ergodic invariant probability on a countable state space has finite cyclic support

↑ **Parent:** [Ergodicity](#ergodicity)

Let $T$ be an [ergodic transformation](#ergodicity) preserving a probability measure $\mu$ on a [countable set](cardinal-number.md#countable-set). Some state $x$ has $\mu(\{x\})>0$. Along its forward orbit,

$$
\mu(\{T^{n+1}x\})
=\mu(T^{-1}\{T^{n+1}x\})
\geq\mu(\{T^nx\}).
$$

An infinite sequence of distinct states with masses bounded below by $\mu(\{x\})$ is impossible, so the orbit eventually reaches a finite cycle $Y$. Since $Y\subseteq T^{-1}Y$ and invariance gives $\mu(T^{-1}Y)=\mu(Y)>0$, the difference is null. The cycle is invariant modulo null sets, and ergodicity therefore gives $\mu(Y)=1$.

#### Invariant-function characterization of ergodicity

↑ **Parent:** [Ergodicity](#ergodicity)

An invertible measure-preserving system is ergodic exactly when the fixed space of its [Koopman operator](#koopman-operator) on $L^2$ consists only of almost-everywhere constant functions. One direction applies invariance to level sets; the other applies it to indicator functions of invariant sets.

#### Bernoulli shift

↑ **Parent:** [Ergodicity](#ergodicity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_shift)

On a one-sided sequence space $E^{\mathbb N}$ with [product measure](probability-theory.md#product-measure), the Bernoulli shift is

$$
S(x_0,x_1,x_2,\ldots)=(x_1,x_2,x_3,\ldots).
$$

It preserves the product measure. Every invariant event lies in the [tail sigma-algebra](probability-theory.md#tail-sigma-algebra) of the coordinate process, so the [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law) makes the shift an [ergodic transformation](#ergodicity).

##### Bernoulli coordinate observable is not almost periodic

↑ **Parent:** [Bernoulli shift](#bernoulli-shift)

For independent fair signs on a two-sided [Bernoulli shift](#bernoulli-shift), the coordinate observable $f(y)=y_0$ has unit norm and pairwise orthogonal orbit values. Their pairwise squared distance is two, excluding a finite small net in global $L^2$. Its pullback along a [factor map](#factor-map-between-measure-preserving-systems) can nevertheless be a [relatively almost periodic observable](#relatively-almost-periodic-observable), since it is fiber-constant and takes only two values.

##### Cantor Bernoulli measure

↑ **Parent:** [Bernoulli shift](#bernoulli-shift)

The law of $\sum_{j\geq1}2\omega_j3^{-j}$, for independent fair binary digits $\omega_j$, is supported on the [Cantor set](geometry-and-topology.md#cantor-set). It is invariant and ergodic under $T_3$, as the image of a [Bernoulli shift](#bernoulli-shift). Each permitted ternary cylinder of length $n$ has measure $2^{-n}$, giving entropy rate $\log2$. The [Host equidistribution theorem](#host-equidistribution-theorem) makes almost every point a [normal number](number-theory.md#normal-number) in base $2$, while its ternary digits omit $1$.

#### Irrational rotation

↑ **Parent:** [Ergodicity](#ergodicity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irrational_rotation)

For irrational $\alpha$, the circle rotation $T(x)=x+\alpha\pmod1$ preserves [Lebesgue measure](measure-theory.md#lebesgue-measure) and is an [ergodic transformation](#ergodicity).

##### Ergodicity criterion for a circle rotation

↑ **Parent:** [Irrational rotation](#irrational-rotation)

The rotation $x\mapsto x+a$ of a circle of circumference $2\pi$ is ergodic exactly when $a/\pi$ is irrational. In the [Fourier basis](fourier-series.md#fourier-basis), an invariant function can have a nonzero $k$th coefficient only when $e^{ika}=1$.

##### Everywhere interval frequency under an irrational rotation

↑ **Parent:** [Irrational rotation](#irrational-rotation)

Every orbit of an [irrational rotation of the circle](#irrational-rotation) visits a half-open interval $I$ with limiting frequency equal to its length. One proof sandwiches the orbit of an arbitrary point between inner and outer intervals along a nearby orbit for which the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) holds.

#### Weakly mixing measure-preserving transformation

↑ **Parent:** [Ergodicity](#ergodicity)

A probability [measure-preserving transformation](#measure-preserving-transformation) $T$ is weakly mixing when, for every pair of measurable sets $A,B$, the average absolute correlation discrepancy tends to zero:

$$
\frac1N\sum_{n=0}^{N-1}|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Equivalently, the correlations converge to their products in [convergence in density of a sequence](#convergence-in-density-of-a-sequence), its [Cartesian product](set-theory.md#cartesian-product) with itself is an [ergodic transformation](#ergodicity), or its product with every [ergodic transformation](#ergodicity) is ergodic. The absolute values are essential: signed [Cesaro convergence of a sequence](#cesaro-convergence-of-a-sequence) of the correlations to their products characterizes [ergodic transformations](#ergodicity) and does not imply weak mixing. For example, the transformation interchanging two equally weighted points has discrepancy $(-1)^n/4$ for a singleton $A=B$: its signed average tends to zero while its average absolute discrepancy stays $1/4$.

##### Arithmetic-progression multiple averages under weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

For bounded observables of a probability [weak mixing](#weakly-mixing-measure-preserving-transformation) system, the displayed convergence holds in $L^2$. Induct on $k$: center the final observable, compute the lagged Hilbert-space correlations, apply the induction hypothesis to the $k-1$ remaining factors, and use [weak mixing](#weakly-mixing-measure-preserving-transformation) of $T^k$ with the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences) to obtain zero. Adding back the final mean completes the induction.

###### Density convergence of multiple weak-mixing correlations

↑ **Parent:** [Arithmetic-progression multiple averages under weak mixing](#arithmetic-progression-multiple-averages-under-weak-mixing)

For real bounded observables, the [Cesaro limit](#cesaro-convergence-of-a-sequence) of the correlation comes from [arithmetic-progression multiple averages under weak mixing](#arithmetic-progression-multiple-averages-under-weak-mixing). Apply the same result on the weakly mixing product system to $f_j\otimes f_j$ to obtain its second moment. The averaged squared error tends to zero, so the [mean-square criterion for convergence in density](#mean-square-criterion-for-convergence-in-density) gives the displayed density limit.

##### Stability of weak mixing under powers and products

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

Every positive power of a [weak mixing](#weakly-mixing-measure-preserving-transformation) transformation is weakly mixing: its nonnegative discrepancies are a subsequence whose average is bounded by $r$ times the full average. Products are weakly mixing because correlations of simple tensors factor; the absolute product discrepancy is bounded by the sum of bounded multiples of the single-system discrepancies. Density of finite tensor sums gives the full $L^2$ assertion.

##### Product characterization of weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

If $T$ is weakly mixing, then $T\times S$ is ergodic exactly when $S$ is ergodic. In particular, ergodicity of $T\times T$ is equivalent to weak mixing of $T$.

###### Square-correlation proof of weak mixing from product ergodicity

↑ **Parent:** [Product characterization of weak mixing](#product-characterization-of-weak-mixing)

For mean-zero $f$, apply the [mean ergodic theorem](vector-space.md#von-neumann-mean-ergodic-theorem) on an ergodic product system to $f\otimes\overline f$, paired with $g\otimes\overline g$. Its correlation is $|\langle U^nf,g\rangle|^2$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) then gives averaged absolute correlation decay, the definition of [weak mixing](#weakly-mixing-measure-preserving-transformation).

##### Koopman eigenfunction obstruction to weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

A weakly mixing system has no nonconstant [Koopman operator](#koopman-operator) eigenfunction. If $U_Tf=\lambda f$, then $f(x)\overline{f(y)}$ is invariant under $T\times T$, contradicting the [product characterization of weak mixing](#product-characterization-of-weak-mixing) unless $f$ is constant.

##### Simultaneous hitting characterization of weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

A system is weakly mixing exactly when, for every positive-measure $A,B,C$, some $n\geq1$ makes both $T^{-n}A\cap B$ and $T^{-n}A\cap C$ have positive measure. This is the finite simultaneous-hitting form of the density-one correlation characterization.

<h3 id="poincare-recurrence-theorem">Poincaré recurrence theorem</h3>

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_recurrence_theorem)

In a finite [measure-preserving system](#measure-preserving-system), almost every point of every measurable set $A$ returns to $A$ infinitely often. The points of $A$ that never return form a wandering set: all its inverse images are pairwise disjoint and have equal measure, so that set must be null.

#### Furstenberg multiple recurrence theorem

↑ **Parent:** [Poincaré recurrence theorem](#poincare-recurrence-theorem)

For a probability [measure-preserving system](#measure-preserving-system), every measurable $B$ of positive measure and every integer $k\geq2$ admit an integer $n\geq1$ with $\mu(\bigcap_{j=0}^{k-1}T^{-jn}B)>0$. The sets are preimages; neither invertibility nor an [ergodic transformation](#ergodicity) is required. The [Furstenberg correspondence principle](#furstenberg-correspondence-principle) converts this simultaneous return into [arithmetic progressions](arithmetic.md#arithmetic-progression) and yields the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem). The case $k=2$ follows from the [Poincaré recurrence theorem](#poincare-recurrence-theorem).

##### SZ property

↑ **Parent:** [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem)

A probability [measure-preserving system](#measure-preserving-system) has the SZ property at level $k$ if the displayed lower limit is positive for every measurable set $A$ of positive measure. This convention counts $k$ nonzero shifts, hence progressions of length $k+1$. The [Furstenberg correspondence principle](#furstenberg-correspondence-principle) turns this property at all levels into the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem). A [compact measure-preserving system](#compact-measure-preserving-system) has the property because [syndetic near returns of an almost periodic observable](#syndetic-near-returns-of-an-almost-periodic-observable) applied to an indicator give uniformly positive multiple intersections at bounded-gap times.

##### Multiple recurrence for circle rotations

↑ **Parent:** [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem)

Every circle rotation has the [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem) property for normalized [Lebesgue measure](measure-theory.md#lebesgue-measure). For a rational angle, use a period. For an irrational angle, choose a positive return time with angle close to zero; [translation continuity in L1 on the circle](measure-theory.md#translation-continuity-in-l1-on-the-circle) then makes finitely many translates of a given positive-measure set simultaneously close to that set, and the [union bound](probability-inequality.md#boole-s-inequality) leaves a positive-measure intersection.

## Birkhoff ergodic theorem

↑ **Parent:** [Ergodic theory](ergodic-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birkhoff_ergodic_theorem)

For a [measure-preserving transformation](#measure-preserving-transformation) $T$ and $f\in L^1(\mu)$, the ergodic averages

$$
A_nf=\frac1n\sum_{j=0}^{n-1}f\circ T^j
$$

converge almost everywhere to $\mathbb E[f\mid\mathcal I]$, the [conditional expectation](measure-theory.md#conditional-expectation) on the [invariant sigma-algebra](#invariant-sigma-algebra). The limit has the same integral as $f$.

### Nonnegative ergodic averages with infinite integral

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

In a probability [measure-preserving system](#measure-preserving-system) whose transformation is an [ergodic transformation](#ergodicity), a nonnegative measurable $f$ with $\int f\,d\mu=+\infty$ has $N^{-1}\sum_{j=0}^{N-1}f(T^jx)\to+\infty$ [almost everywhere](measure-theory.md#almost-everywhere). Apply the [pointwise ergodic theorem](#birkhoff-ergodic-theorem) to $\min(f,K)$ on a common full-measure set for integer $K$, then bound the lower limit by each truncated integral. The [monotone convergence theorem](measure-theory.md#monotone-convergence-theorem) sends those integrals to infinity. The finite-integral case is the ordinary [pointwise ergodic theorem](#birkhoff-ergodic-theorem).

### Maximal ergodic lemma

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

For a [measure-preserving transformation](#measure-preserving-transformation) and real integrable $f$, let $S_kf=\sum_{j<k}f\circ T^j$. For $E_N=\{\max_{1\leq k\leq N}S_kf>0\}$ the lemma asserts $\int_{E_N}f\,d\mu\geq0$. Passing to the increasing [union](set.md#set-union) gives the corresponding infinite-supremum inequality.

### Triangular ergodic averaging lemma

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

Suppose $f_k\to f$ [almost everywhere](measure-theory.md#almost-everywhere) and $\sup_k|f_k|\in L^1$ in a probability [measure-preserving system](#measure-preserving-system). Then

$$
\frac1n\sum_{j=0}^{n-1}f_{n-1-j}(T^jx)
\longrightarrow\mathbb E[f\mid\mathcal I]
$$

[almost everywhere](measure-theory.md#almost-everywhere) and in $L^1$, where $\mathcal I$ is the [invariant sigma-algebra](#invariant-sigma-algebra). For the almost-everywhere assertion, bound the terms with index at least $M$ by $\sup_{k\geq M}|f_k-f|$, apply the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem), and then let $M\to\infty$. The finitely many remaining end terms vanish by the [linear growth bound for integrable observables](#linear-growth-bound-for-integrable-observables).

### Linear growth bound for integrable observables

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

In a probability [measure-preserving system](#measure-preserving-system), $f\in L^1$ implies $f(T^nx)/n\to0$ [almost everywhere](measure-theory.md#almost-everywhere). For every $\varepsilon>0$, the [tail integral formula for moments](expected-value.md#tail-integral-formula-for-moments) gives $\sum_{n\geq1}\mu(|f|>\varepsilon n)\leq\|f\|_1/\varepsilon$. Invariance and the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) finish the proof. Consequently division by $n^a$ also gives zero for every $a\geq1$.

#### Sharpness of the linear growth bound for integrable observables

↑ **Parent:** [Linear growth bound for integrable observables](#linear-growth-bound-for-integrable-observables)

For every $0<a<1$, choose $1<p<1/a$. On the [Bernoulli shift](#bernoulli-shift) over independent uniform coordinates in $(0,1)$, the observable $f(x)=x_0^{-1/p}$ is integrable, but $\mu(f(T^nx)>n^a)=n^{-ap}$. The events are independent and their probabilities have divergent sum, so the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) implies that $f(T^nx)/n^a>1$ infinitely often [almost surely](convergence-of-random-variables.md#almost-sure-convergence). No exponent below one gives a universal bound for all integrable observables.

### L1 convergence in the Birkhoff ergodic theorem on a finite measure space

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

On a [finite measure](measure.md#finite-measure) space, the convergence in the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) also holds in $L^1$. Prove it first for bounded truncations by the [dominated convergence theorem](measure-theory.md#dominated-convergence-theorem), then use the $L^1$ contraction $\|A_nh\|_1\leq\|h\|_1$ and [Fatou lemma](measure-theory.md#fatou-s-lemma) to remove the truncation.

## Upper Banach density

↑ **Parent:** [Ergodic theory](ergodic-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_Banach_density)

For $S\subseteq\mathbb Z$, its upper Banach density is

$$
d^*(S)=\limsup_{N\to\infty}\sup_{m\in\mathbb Z}\frac{|S\cap[m,m+N-1]|}{N}.
$$

### Furstenberg correspondence principle

↑ **Parent:** [Upper Banach density](#upper-banach-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Furstenberg_correspondence_principle)

The Furstenberg correspondence principle turns a subset $S\subseteq\mathbb Z$ of positive [upper Banach density](#upper-banach-density) into a shift-invariant probability system and a positive-measure cylinder $A$ such that recurrence times of $A$ produce differences of elements of $S$.

## Convergence in density of a sequence

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

A sequence $a_n$ converges in density to $a$ when, for every $\varepsilon>0$,

$$
\frac1N\left|\{1\leq n\leq N:|a_n-a|\geq\varepsilon\}\right|\longrightarrow0.
$$

### Mean-square criterion for convergence in density

↑ **Parent:** [Convergence in density of a sequence](#convergence-in-density-of-a-sequence)

The displayed condition implies [convergence in density of a sequence](#convergence-in-density-of-a-sequence) to $\ell$, since the fraction of indices with $|a_n-\ell|\geq\varepsilon$ is at most $\varepsilon^{-2}$ times the averaged squared error. A signed [Cesaro limit](#cesaro-convergence-of-a-sequence) alone is insufficient: $a_n=(-1)^n$ has zero signed average but no density limit.

### Cesaro convergence of a sequence

↑ **Parent:** [Convergence in density of a sequence](#convergence-in-density-of-a-sequence)

A sequence $a_n$ converges in the Cesaro sense to $a$ when $N^{-1}\sum_{n=1}^Na_n\to a$. For bounded sequences, convergence in density to $a$ is equivalent to Cesaro convergence of $|a_n-a|$ to zero.

## Entropy of a finite measurable partition

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

For a finite measurable partition $\xi$, its entropy is

$$
H_\mu(\xi)=-\sum_{A\in\xi}\mu(A)\log\mu(A),
$$

with $0\log0=0$.

### Conditional entropy of finite measurable partitions

↑ **Parent:** [Entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition)

For finite partitions $\xi,\eta$,

$$
H_\mu(\xi\mid\eta)
=\sum_{B\in\eta}\mu(B)H_\mu(\xi\mid B)
=H_\mu(\xi\vee\eta)-H_\mu(\eta).
$$

[Conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy), so $H_\mu(\xi\mid\eta)\leq H_\mu(\xi)$.

### Entropy rate of a measurable partition

↑ **Parent:** [Entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition)

The entropy rate of $\xi$ is

$$
h_\mu(T,\xi)=\lim_{N\to\infty}\frac1N
H_\mu\left(\bigvee_{n=0}^{N-1}T^{-n}\xi\right).
$$

The numerator is a [subadditive sequence](sequence-and-series.md#subadditive-sequence), so the limit exists and equals the infimum of the displayed ratios.

#### Infinite-future formula for partition entropy rate

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a finite [measurable partition](measure-theory.md#measurable-partition) $\xi$, put $\mathcal F_1=\sigma(\bigvee_{j\ge1}T^{-j}\xi)$. Then $h_\mu(T,\xi)=H_\mu(\xi\mid\mathcal F_1)=\lim_{n\to\infty}H_\mu(\xi\mid\xi_1^n)$. The backward entropy chain rule writes $H_\mu(\xi_0^{N-1})$ as the sum of the first $N$ decreasing finite-future conditional entropies. Their averages have the same limit. Increasing conditioning fields converge by the [martingale convergence theorem](martingale.md#martingale-convergence-theorem).

##### Block conditional entropy given the infinite future

↑ **Parent:** [Infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate)

For $\mathcal F_L=\sigma(\bigvee_{j\ge L}T^{-j}\xi)$ and a finite [measurable partition](measure-theory.md#measurable-partition) $\xi$, $H_\mu(\xi_0^{L-1}\mid\mathcal F_L)=Lh_\mu(T,\xi)$. The backward conditional entropy chain rule expresses the left side as $\sum_{j=0}^{L-1}H_\mu(T^{-j}\xi\mid\mathcal F_{j+1})$. Each term equals $h_\mu(T,\xi)$ by measure preservation and the [infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate). No invertibility is needed.

#### Shannon-McMillan-Breiman theorem

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a probability [measure-preserving system](#measure-preserving-system) and a countable [measurable partition](measure-theory.md#measurable-partition) $\xi$ of finite entropy, $-n^{-1}\log\mu(\xi_0^{n-1}(x))$ converges [almost everywhere](measure-theory.md#almost-everywhere) and in $L^1$ to an invariant function whose integral is $h_\mu(T,\xi)$. For an [ergodic transformation](#ergodicity), the limit is the constant $h_\mu(T,\xi)$. In general it is $\mathbb E[I_\mu(\xi\mid\bigvee_{j=1}^\infty T^{-j}\xi)\mid\mathcal I]$. The [martingale convergence theorem](martingale.md#martingale-convergence-theorem), [maximal inequality for conditional information functions](measure-theory.md#maximal-inequality-for-conditional-information-functions), and [triangular ergodic averaging lemma](#triangular-ergodic-averaging-lemma) prove this directly, without invertibility.

#### Monotonicity of normalized block entropy

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a stationary process associated with a finite-entropy [measurable partition](measure-theory.md#measurable-partition), $H_\mu(\xi_0^{n-1})/n$ is non-increasing. The increments $c_k=H_\mu(\xi\mid\bigvee_{j=1}^kT^{-j}\xi)$ are non-increasing by [conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy), and the chain rule gives $H_\mu(\xi_0^{n-1})=\sum_{k=0}^{n-1}c_k$. Averages of a decreasing sequence are decreasing.

#### Kolmogorov-Sinai entropy

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov-Sinai_entropy)

The Kolmogorov-Sinai entropy is $h_\mu(T)=\sup_\xi h_\mu(T,\xi)$ over finite measurable partitions.

##### Completely positive entropy

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

A probability [measure-preserving system](#measure-preserving-system) has completely positive entropy if $h_\mu(T,\xi)>0$ for every finite [measurable partition](measure-theory.md#measurable-partition) with $H_\mu(\xi)>0$. Equivalently, its [Pinsker sigma-algebra](#pinsker-sigma-algebra) is trivial. Since [finite partitions measurable in a partition tail have zero entropy rate](#finite-partitions-measurable-in-a-partition-tail-have-zero-entropy-rate), this property forces every finite-partition [tail sigma-algebra of a measurable partition](#tail-sigma-algebra-of-a-measurable-partition) to be trivial.

##### Generating measurable partition

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

For an invertible [measure-preserving system](#measure-preserving-system), a generating measurable partition $\xi$ has $\sigma(\bigvee_{j\in\mathbb Z}T^{-j}\xi)=\mathcal B$ modulo null sets. Thus knowing the entire two-sided itinerary determines all measurable observations. A finite or countable finite-entropy generating partition computes the system entropy through the [Kolmogorov-Sinai generator theorem](#kolmogorov-sinai-generator-theorem).

###### One-sided generator

↑ **Parent:** [Generating measurable partition](#generating-measurable-partition)

A one-sided generator is a [measurable partition](measure-theory.md#measurable-partition) $\xi$ with $\sigma(\bigvee_{j\ge0}T^{-j}\xi)=\mathcal B$ modulo null sets. Equivalently, every measurable set can be approximated in measure by unions of atoms of finite forward-name blocks. A one-sided coordinate partition generates a one-sided [Bernoulli shift](#bernoulli-shift); for a nontrivial base distribution, it does not generate the two-sided version, whose negative coordinates are independent of the nonnegative ones.

###### Finite one-sided generator of an invertible system forces zero entropy

↑ **Parent:** [One-sided generator](#one-sided-generator)

If an invertible probability [measure-preserving system](#measure-preserving-system) has a finite [one-sided generator](#one-sided-generator) $\xi$, then its future sigma-algebra $\mathcal F_1=T^{-1}\mathcal B$ equals $\mathcal B$ modulo null sets. Hence $H_\mu(\xi\mid\mathcal F_1)=0$, and the [infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate) and [Kolmogorov-Sinai generator theorem](#kolmogorov-sinai-generator-theorem) give $h_\mu(T)=0$. Invertibility matters: a fair binary one-sided [Bernoulli shift](#bernoulli-shift) has entropy $\log2$ and a finite one-sided generator.

###### Kolmogorov-Sinai generator theorem

↑ **Parent:** [Generating measurable partition](#generating-measurable-partition)

For an invertible probability [measure-preserving system](#measure-preserving-system) with a finite or countable finite-entropy [generating measurable partition](#generating-measurable-partition) $\xi$, $h_\mu(T)=h_\mu(T,\xi)$. For a noninvertible system the same conclusion holds for a finite-entropy [one-sided generator](#one-sided-generator). The finite-entropy hypothesis is part of this form of the theorem.

##### Host equidistribution theorem

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

Let $p,q\geq2$ be relatively prime integers. If $\nu$ is invariant and ergodic for the [integer multiplication map on the circle](#integer-multiplication-map-on-the-circle) $T_p$ and $h_\nu(T_p)>0$, then for $\nu$-almost every $x$ the sequence $(T_q^nx)$ is an [equidistributed sequence](#equidistributed-sequence) for [Lebesgue measure](measure-theory.md#lebesgue-measure). For a non-ergodic $T_p$ invariant measure, the same conclusion holds if almost every measure in its [ergodic decomposition](#ergodic-decomposition) has positive entropy. Positive entropy of the whole measure alone does not suffice.

###### Rudolph measure rigidity theorem

↑ **Parent:** [Host equidistribution theorem](#host-equidistribution-theorem)

A probability measure on the circle invariant under $T_2$ and $T_3$ and ergodic for their jointly generated semigroup is [Lebesgue measure](measure-theory.md#lebesgue-measure) if either transformation has positive [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy). Without joint ergodicity, a mixture of [Lebesgue measure](measure-theory.md#lebesgue-measure) and an atomic invariant measure shows why positive entropy alone is insufficient.

##### Entropy preservation under a finite-to-one factor

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

For standard probability systems, a [factor of a measure-preserving system](#factor-of-a-measure-preserving-system) with at most $q$ points in every fibre preserves [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy). Conditional on the complete factor point, every finite orbit name has at most $q$ possibilities, so its conditional entropy is at most $\log q$. Dividing by the orbit length gives zero relative entropy.

##### Pinsker sigma-algebra

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

The Pinsker sigma-algebra consists of the measurable sets $A$ whose binary partition $\{A,X\setminus A\}$ has entropy rate zero. It is a sigma-algebra and is the largest invariant factor with zero [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy).

###### Tail characterization of the Pinsker sigma-algebra

↑ **Parent:** [Pinsker sigma-algebra](#pinsker-sigma-algebra)

A set belongs to the [Pinsker sigma-algebra](#pinsker-sigma-algebra) exactly when, modulo a null set, it belongs to $\mathcal T(\xi)$ for some finite measurable partition $\xi$. For a zero-entropy binary partition one may take that partition itself: zero conditional entropy makes its present atom measurable from every remote future.

#### Infimum rule for partition entropy rate

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a measure-preserving action of $\mathbb Z$ and a finite partition $\xi$,

$$
h_\mu(T,\xi)=\inf_{\varnothing\ne F\subseteq\mathbb Z_{\geq0}\text{ finite}}
\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).
$$

The reverse inequality to the interval formula follows from [Shearer's inequality](information-theory.md#shearer-s-inequality) applied to translates of $F$ along long intervals; the uncovered boundary has sublinear size.

## K-mixing

↑ **Parent:** [Ergodic theory](ergodic-theory.md)

A system is K-mixing when every finite partition becomes asymptotically independent of every event in its remote future: if $\mathcal F_n(\xi)=\bigvee_{k=n}^\infty T^{-k}\xi$, then

$$
\sup_{B\in\mathcal F_n(\xi)}|\mu(A\cap B)-\mu(A)\mu(B)|\longrightarrow0
$$

for every measurable $A$ and every finite $\xi$.

### Tail sigma-algebra of a measurable partition

↑ **Parent:** [K-mixing](#k-mixing)

The tail sigma-algebra of a finite partition $\xi$ is

$$
\mathcal T(\xi)=\bigcap_{n\geq0}\bigvee_{k=n}^\infty T^{-k}\xi.
$$

By the [reverse martingale convergence theorem](martingale.md#reverse-martingale-convergence-theorem), K-mixing is equivalent to triviality of $\mathcal T(\xi)$ for every finite partition $\xi$.

#### Finite partitions measurable in a partition tail have zero entropy rate

↑ **Parent:** [Tail sigma-algebra of a measurable partition](#tail-sigma-algebra-of-a-measurable-partition)

Let $\alpha$ be finite and measurable in $\mathcal T(\xi)$ for a finite [measurable partition](measure-theory.md#measurable-partition) $\xi$, and put $h=h_\mu(T,\xi)$. Choose $r$ with $H(\alpha\mid\xi_0^r)<\varepsilon$. For $\gamma=\alpha_0^{n-1}$ and $\beta=\xi_0^{n+r-1}$, conditional subadditivity gives $H(\gamma\mid\beta)<n\varepsilon$. Tail measurability and [block conditional entropy given the infinite future](#block-conditional-entropy-given-the-infinite-future) give $H(\beta\mid\gamma)\ge(n+r)h$. Thus $H(\gamma)\le H(\beta)-(n+r)h+n\varepsilon$. Divide by $n$, then let $n\to\infty$ and $\varepsilon\downarrow0$, proving $h_\mu(T,\alpha)=0$. The proof also works for noninvertible transformations.

## ↑ Ancestors (6)

1. [Measure theory](measure-theory.md)
2. [Real analysis](real-analysis.md)
3. [Analysis](analysis.md)
4. [Area of mathematics](mathematics.md#area-of-mathematics)
5. [Mathematics](mathematics.md)
6. [Codex Wiki](README.md)
