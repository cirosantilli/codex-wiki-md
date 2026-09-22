# Measure theory

↑ **Parent:** [Real analysis](real-analysis.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measure_theory)

Measure theory studies [measures](#measure), which assign sizes to [measurable sets](#measurable-set), and the [Lebesgue integral](#lebesgue-integral), which accumulates values weighted by those sizes. The same framework describes [Lebesgue measure](#lebesgue-measure) on the [real numbers](arithmetic.md#real-number), [counting measure](#counting-measure) on discrete collections, and [probability measures](probability-theory.md#probability-measure) on possible outcomes. The choice of [measure](#measure) determines what counts as large; the choice of [sigma-algebra](#sigma-algebra) determines what can be measured.

A striking example separates size from proximity: the [rational numbers](number-theory.md#rational-number) in $[0,1]$ form a [dense set](topology.md#dense-set) with [Lebesgue measure](#lebesgue-measure) zero, although the whole interval has [Lebesgue measure](#lebesgue-measure) one. This distinction makes [almost everywhere](#almost-everywhere) statements useful: exceptional [null sets](#null-set) can be ignored in a [Lebesgue integral](#lebesgue-integral) even when they meet every open subinterval. The [monotone convergence theorem](#monotone-convergence-theorem) and [dominated convergence theorem](#dominated-convergence-theorem) then give precise conditions for passing a [limit](calculus.md#limit-of-a-function) through an [integral](calculus.md#integral).

A historical starting point is Lebesgue's 1902 thesis, [Intégrale, Longueur, Aire (original title page reproduced in USP lecture notes)](https://www.ime.usp.br/~glaucio/mat5798/textos/aula1.pdf#page=2). Its title connects [integration](calculus.md#integral) with the geometric task of assigning sizes.

**Table of contents**

- [Wiener covering lemma](#wiener-covering-lemma)
  - [Disjoint ball decomposition modulo null sets](#disjoint-ball-decomposition-modulo-null-sets)
- [Geometric measure theory](#geometric-measure-theory)
  - [Hausdorff measure](#hausdorff-measure)
    - [Scale-restricted Hausdorff content](#scale-restricted-hausdorff-content)
    - [Hausdorff dimension](#hausdorff-dimension)
      - [Mass distribution principle](#mass-distribution-principle)
      - [Hausdorff dimension of the Cantor set](#hausdorff-dimension-of-the-cantor-set)
      - [Pressure upper bound for Hausdorff dimension](#pressure-upper-bound-for-hausdorff-dimension)
      - [Hausdorff dimension of a connected set](#hausdorff-dimension-of-a-connected-set)
- [Vector measure](#vector-measure)
  - [Vector Radon measure](#vector-radon-measure)
    - [Polar decomposition of a vector measure](#polar-decomposition-of-a-vector-measure)
- [Standard Borel probability space](#standard-borel-probability-space)
- [Measurable space](#measurable-space)
  - [Standard Borel space](#standard-borel-space)
- [Null set](#null-set)
  - [Lebesgue null set](#lebesgue-null-set)
  - [Borel null set](#borel-null-set)
- [Random measure](#random-measure)
- [Measurable partition](#measurable-partition)
  - [Partition atom](#partition-atom)
  - [Entropy of a countable measurable partition](#entropy-of-a-countable-measurable-partition)
    - [Conditional information function](#conditional-information-function)
      - [Maximal inequality for conditional information functions](#maximal-inequality-for-conditional-information-functions)
      - [Conditional entropy of a countable measurable partition](#conditional-entropy-of-a-countable-measurable-partition)
  - [Join of measurable partitions](#join-of-measurable-partitions)
- [Field of sets](#field-of-sets)
- [Semiring of sets](#semiring-of-sets)
- [Monotone class](#monotone-class)
  - [Monotone class theorem](#monotone-class-theorem)
    - [Functional monotone-class theorem](#functional-monotone-class-theorem)
- [Measurable function](#measurable-function)
  - [Essential range](#essential-range)
  - [Measurability](#measurability)
  - [Borel measurable function](#borel-measurable-function)
  - [Composition of measurable functions](#composition-of-measurable-functions)
- [Measure density](#measure-density)
  - [Spherical derivative of a measure](#spherical-derivative-of-a-measure)
    - [Spherical derivative of a singular measure vanishes](#spherical-derivative-of-a-singular-measure-vanishes)
  - [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem)
    - [Oscillating annuli obstruct differentiation at a point](#oscillating-annuli-obstruct-differentiation-at-a-point)
    - [Lebesgue point](#lebesgue-point)
    - [Differentiation of an indefinite Lebesgue integral](#differentiation-of-an-indefinite-lebesgue-integral)
  - [Lebesgue's density theorem](#lebesgue-s-density-theorem)
    - [Density point](#density-point)
    - [High-density interval in a positive-measure subset of the real line](#high-density-interval-in-a-positive-measure-subset-of-the-real-line)
- [Lebesgue measurable set](#lebesgue-measurable-set)
  - [Regularity of Lebesgue measure](#regularity-of-lebesgue-measure)
- [Almost everywhere](#almost-everywhere)
- [Lebesgue integrable function](#lebesgue-integrable-function)
  - [Integrability](#integrability)
- [Conditional expectation](#conditional-expectation)
  - [Conditional expectation preserving a distribution](#conditional-expectation-preserving-a-distribution)
  - [Dyadic conditional averages recover integrable functions](#dyadic-conditional-averages-recover-integrable-functions)
  - [Symmetrization as conditional expectation](#symmetrization-as-conditional-expectation)
    - [Sampling with and without replacement comparison for bounded products](#sampling-with-and-without-replacement-comparison-for-bounded-products)
  - [Conditional expectation from finite-measure densities](#conditional-expectation-from-finite-measure-densities)
  - [Equality case for conditional second moments](#equality-case-for-conditional-second-moments)
  - [Conditional L2 norm](#conditional-l2-norm)
    - [Conditional norm covariance under a factor map](#conditional-norm-covariance-under-a-factor-map)
    - [Uniform conditional L2 norm](#uniform-conditional-l2-norm)
  - [Conditional Jensen inequality](#conditional-jensen-inequality)
  - [L1 contraction of conditional expectation](#l1-contraction-of-conditional-expectation)
  - [Conditional expectation of a summand given future partial sums](#conditional-expectation-of-a-summand-given-future-partial-sums)
  - [Law of total expectation](#law-of-total-expectation)
    - [Nested conditioning keeps the coarser information](#nested-conditioning-keeps-the-coarser-information)
  - [Independent sigma-algebras have trivial intersection](#independent-sigma-algebras-have-trivial-intersection)
  - [Iterated conditional expectation over nonnested sigma-algebras](#iterated-conditional-expectation-over-nonnested-sigma-algebras)
  - [Conditional Fatou lemma](#conditional-fatou-lemma)
- [Fatou's lemma](#fatou-s-lemma)
  - [Fatou lemma for series](#fatou-lemma-for-series)
  - [Proof of Fatou lemma](#proof-of-fatou-lemma)
  - [Strict inequality in Fatou lemma](#strict-inequality-in-fatou-lemma)
- [Ergodic theory](#ergodic-theory)
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
- [Outer measure](#outer-measure)
  - [Carathéodory's criterion](#caratheodory-s-criterion)
  - [Lebesgue outer measure](#lebesgue-outer-measure)
- [Measure](#measure)
  - [Inner regular measure](#inner-regular-measure)
  - [p-adic measure](#p-adic-measure)
    - [Mahler expansion of continuous p-adic functions](#mahler-expansion-of-continuous-p-adic-functions)
    - [Amice transform](#amice-transform)
    - [Convolution of p-adic measures](#convolution-of-p-adic-measures)
  - [Stieltjes transform of a measure](#stieltjes-transform-of-a-measure)
  - [Outer regular measure](#outer-regular-measure)
  - [Complex measure](#complex-measure)
  - [Countable subadditivity of a measure](#countable-subadditivity-of-a-measure)
  - [Complete measure](#complete-measure)
    - [Completion of a measure](#completion-of-a-measure)
  - [Variation measure](#variation-measure)
    - [Total variation norm of a measure](#total-variation-norm-of-a-measure)
  - [Signed measure](#signed-measure)
  - [Dirac measure](#dirac-measure)
  - [Atom (measure theory)](#atom-measure-theory)
    - [Non-atomic measure](#non-atomic-measure)
      - [Lyapunov convexity theorem](#lyapunov-convexity-theorem)
  - [Counting measure](#counting-measure)
    - [Series as a Lebesgue integral against counting measure](#series-as-a-lebesgue-integral-against-counting-measure)
  - [Premeasure](#premeasure)
    - [Cylinder premeasure from a positive functional](#cylinder-premeasure-from-a-positive-functional)
    - [Carathéodory's extension theorem](#caratheodory-s-extension-theorem)
  - [Positive measure](#positive-measure)
  - [Borel measure](#borel-measure)
    - [Support of a measure](#support-of-a-measure)
      - [Support under a continuous map](#support-under-a-continuous-map)
    - [Borel probability measure](#borel-probability-measure)
      - [Continuous approximation of Borel indicators on a compact metric space](#continuous-approximation-of-borel-indicators-on-a-compact-metric-space)
    - [Regular Borel measure](#regular-borel-measure)
    - [Radon measure](#radon-measure)
      - [Regularity of finite Borel measures on Euclidean space](#regularity-of-finite-borel-measures-on-euclidean-space)
  - [Measure space](#measure-space)
  - [Pushforward measure](#pushforward-measure)
    - [Probability pushforward embedding theorem](#probability-pushforward-embedding-theorem)
  - [Change of measure](#change-of-measure)
    - [Density process](#density-process)
  - [Haar measure](#haar-measure)
    - [Haar measure from a left-invariant coframe](#haar-measure-from-a-left-invariant-coframe)
    - [Haar measure from normalized covering functionals](#haar-measure-from-normalized-covering-functionals)
    - [Compact-group invariant probability by finite averaging](#compact-group-invariant-probability-by-finite-averaging)
    - [Haar integral](#haar-integral)
    - [Weyl integration formula for SU(2)](#weyl-integration-formula-for-su-2)
    - [Pauli-coordinate Haar measure on SU(2)](#pauli-coordinate-haar-measure-on-su-2)
    - [Minimal left covering net of a compact group](#minimal-left-covering-net-of-a-compact-group)
      - [Matching minimal covering nets of a compact group](#matching-minimal-covering-nets-of-a-compact-group)
  - [Countable additivity](#countable-additivity)
    - [Continuity from below of a measure](#continuity-from-below-of-a-measure)
    - [Continuity from above of a measure](#continuity-from-above-of-a-measure)
  - [Finite measure](#finite-measure)
    - [Finite-measure set](#finite-measure-set)
  - [Sigma-finite measure](#sigma-finite-measure)
- [Step function](#step-function)
- [Lebesgue integral](#lebesgue-integral)
  - [Integral average](#integral-average)
    - [Volume average](#volume-average)
  - [Simple function](#simple-function)
- [Indicator function](#indicator-function)
  - [Indicator vector](#indicator-vector)
- [Sigma-algebra](#sigma-algebra)
  - [Algebra of sets](#algebra-of-sets)
    - [Countable generating algebra](#countable-generating-algebra)
  - [Measurable set](#measurable-set)
  - [Atom of a sigma-algebra](#atom-of-a-sigma-algebra)
  - [Borel set](#borel-set)
    - [Borel hierarchy](#borel-hierarchy)
    - [Borel sigma-algebra](#borel-sigma-algebra)
      - [Borel sigma-algebra of a discrete space](#borel-sigma-algebra-of-a-discrete-space)
  - [Pi-system](#pi-system)
  - [Dynkin system](#dynkin-system)
    - [Dynkin lemma](#dynkin-lemma)
- [Fubini's theorem](#fubini-s-theorem)
  - [Frullani integral](#frullani-integral)
- [Sigma-finite uniqueness theorem for measures](#sigma-finite-uniqueness-theorem-for-measures)
  - [Lebesgue measure](#lebesgue-measure)
    - [Null-set limsup cover by finite arc families](#null-set-limsup-cover-by-finite-arc-families)
    - [Compact batching of a small open set](#compact-batching-of-a-small-open-set)
    - [Inner regularity of Lebesgue measure](#inner-regularity-of-lebesgue-measure)
    - [Sierpiński set](#sierpinski-set)
    - [Divisibility of Lebesgue measure](#divisibility-of-lebesgue-measure)
    - [Completeness of Lebesgue measure](#completeness-of-lebesgue-measure)
- [Bochner integral](#bochner-integral)
  - [Mean-square integral](#mean-square-integral)
  - [Barycenter of a measure on a Banach space](#barycenter-of-a-measure-on-a-banach-space)
  - [Strongly measurable function](#strongly-measurable-function)
- [Essential supremum](#essential-supremum)
- [Lp space](#lp-space)
  - [L1 space](#l1-space)
  - [Sum of Lp spaces](#sum-of-lp-spaces)
    - [Threshold decomposition between Lp spaces](#threshold-decomposition-between-lp-spaces)
  - [Sine sequence is not Cauchy in the integral norm](#sine-sequence-is-not-cauchy-in-the-integral-norm)
  - [Translation continuity in Lp on a locally compact group](#translation-continuity-in-lp-on-a-locally-compact-group)
  - [Derivative of a power of the Lp norm](#derivative-of-a-power-of-the-lp-norm)
  - [Closest point theorem for a closed convex subset of Lp](#closest-point-theorem-for-a-closed-convex-subset-of-lp)
  - [Completeness of Lp spaces](#completeness-of-lp-spaces)
  - [Weak Lq space](#weak-lq-space)
    - [Integral norm for weak Lq](#integral-norm-for-weak-lq)
  - [Mixed Lebesgue norm](#mixed-lebesgue-norm)
  - [Locally square-integrable function](#locally-square-integrable-function)
  - [Translation continuity in Lp](#translation-continuity-in-lp)
  - [Translation continuity in L1 on the circle](#translation-continuity-in-l1-on-the-circle)
  - [Lp norms converge to the supremum norm](#lp-norms-converge-to-the-supremum-norm)
    - [Moment ratios converge to the essential supremum](#moment-ratios-converge-to-the-essential-supremum)
  - [Lp interpolation inequality](#lp-interpolation-inequality)
    - [Nonvanishing level-set bound between three Lp norms](#nonvanishing-level-set-bound-between-three-lp-norms)
  - [Square-integrable function](#square-integrable-function)
  - [L2 space is a Hilbert space](#l2-space-is-a-hilbert-space)
    - [Exponentially weighted L2 space](#exponentially-weighted-l2-space)
      - [Weighted essential spectrum of a Fisher travelling front](#weighted-essential-spectrum-of-a-fisher-travelling-front)
    - [Mean-zero L2 space](#mean-zero-l2-space)
    - [L2 inner product](#l2-inner-product)
  - [Riesz-Fischer theorem](#riesz-fischer-theorem)
  - [Banach intersection of L1 and L2](#banach-intersection-of-l1-and-l2)
- [Approximation by nonnegative simple functions](#approximation-by-nonnegative-simple-functions)
- [Monotone convergence theorem](#monotone-convergence-theorem)
  - [Moving-spike obstruction to interchanging a limit and an infinite sum](#moving-spike-obstruction-to-interchanging-a-limit-and-an-infinite-sum)
- [Dominated convergence theorem](#dominated-convergence-theorem)
- [Bounded convergence theorem](#bounded-convergence-theorem)
- [Tonelli theorem](#tonelli-theorem)
- [Mutually singular measures](#mutually-singular-measures)
  - [Density level sets separate a singular measure](#density-level-sets-separate-a-singular-measure)
- [Absolute continuity of measures](#absolute-continuity-of-measures)
  - [Dominating measure](#dominating-measure)
  - [Lusin condition N](#lusin-condition-n)
  - [Image-length measure of a strictly increasing continuous function](#image-length-measure-of-a-strictly-increasing-continuous-function)
  - [Uniform absolute continuity for a finite measure](#uniform-absolute-continuity-for-a-finite-measure)
  - [Mutually absolutely continuous measures](#mutually-absolutely-continuous-measures)
    - [Equivalent probability measure](#equivalent-probability-measure)
  - [Radon-Nikodym theorem](#radon-nikodym-theorem)
    - [Hilbert-space construction of dominated measure densities](#hilbert-space-construction-of-dominated-measure-densities)
    - [Radon-Nikodym derivative](#radon-nikodym-derivative)
      - [Radon-Nikodym density martingale](#radon-nikodym-density-martingale)
    - [Positive Radon-Nikodym derivative](#positive-radon-nikodym-derivative)
  - [Lebesgue decomposition theorem](#lebesgue-decomposition-theorem)
    - [Dyadic density martingale](#dyadic-density-martingale)
      - [Martingale construction of Lebesgue decomposition](#martingale-construction-of-lebesgue-decomposition)
    - [Lebesgue decomposition from a sum-measure density](#lebesgue-decomposition-from-a-sum-measure-density)
  - [Dominating mixture measure](#dominating-mixture-measure)
- [Lebesgue-Stieltjes measure](#lebesgue-stieltjes-measure)
  - [Lebesgue–Stieltjes integration](#lebesgue-stieltjes-integration)
- [Lp inclusion on a finite measure space](#lp-inclusion-on-a-finite-measure-space)
  - [Almost-everywhere convergent subsequence from Lp convergence](#almost-everywhere-convergent-subsequence-from-lp-convergence)
  - [Lq inclusion implies finite measure on a Euclidean Borel subset](#lq-inclusion-implies-finite-measure-on-a-euclidean-borel-subset)
  - [Power singularity integrability](#power-singularity-integrability)

## Wiener covering lemma

↑ **Parent:** [Measure theory](measure-theory.md)

A finite collection of Euclidean open balls has a disjoint subcollection whose concentric triples cover the original union. Greedily retain a largest remaining ball and discard all intersecting ones. Each discarded ball has radius no greater than the retained one and lies in its triple. [Lebesgue measure](#lebesgue-measure) consequently bounds the original union by $3^d$ times the sum of the retained volumes. This covering lemma is distinct from inverse-closedness results for the [Wiener algebra](fourier-series.md#wiener-algebra).

### Disjoint ball decomposition modulo null sets

↑ **Parent:** [Wiener covering lemma](#wiener-covering-lemma)

Every open set of finite [Lebesgue measure](#lebesgue-measure) in Euclidean space is covered, up to a [null set](#null-set), by countably many pairwise disjoint open balls contained in it. At each stage cover a compact subset of the open remainder, choose a packing with the [Wiener covering lemma](#wiener-covering-lemma), and remove its closed balls. A fixed positive fraction of the remaining measure is removed each time, while sphere boundaries are null.

## Geometric measure theory

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Geometric_measure_theory)

Geometric measure theory uses [measures](#measure) and [analysis](analysis.md) to study geometric objects that need not be smooth. Its measuring rules can distinguish a [curve](topology.md#curve) from its surrounding plane or capture the fine structure of a [fractal](geometry-and-topology.md#fractal). [Hausdorff measure](#hausdorff-measure) supplies size adapted to an exponent, while [Hausdorff dimension](#hausdorff-dimension) identifies the exponent at which that size changes character.

The [Cantor set](geometry-and-topology.md#cantor-set) is an elementary starting point: it has zero [Lebesgue measure](#lebesgue-measure) but positive [Hausdorff dimension](#hausdorff-dimension). In [Hausdorff dimension of the Cantor set](#hausdorff-dimension-of-the-cantor-set), explicit small [covers](set.md#cover-topology) give an upper bound and a distributed [probability measure](probability-theory.md#probability-measure) supplies the matching lower bound. This combination of geometric coverings and analytic control is useful even before more advanced tools for irregular surfaces are introduced.

### Hausdorff measure

↑ **Parent:** [Geometric measure theory](#geometric-measure-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_measure)

Hausdorff measure measures the geometric size of a [set](set.md) using [covers](set.md#cover-topology) by increasingly small pieces. The exponent $s$ chooses the measuring scale: $s=1$ is length-like, $s=2$ is area-like, and noninteger exponents can measure [fractals](geometry-and-topology.md#fractal). Unlike a count of occupied grid cells, the construction allows pieces of different sizes and considers every admissible [cover](set.md#cover-topology).

For $s>0$ and a [subset](set.md#subset) $E$ of a [metric space](topological-analysis.md#metric-space), use the diameter-cost convention

$$
\mathcal H_\delta^s(E)=\inf\left\{
\sum_{j=1}^\infty(\operatorname{diam}U_j)^s:
E\subseteq\bigcup_jU_j,\quad\operatorname{diam}U_j\leq\delta
\right\},\qquad
\mathcal H^s(E)=\lim_{\delta\downarrow0}\mathcal H_\delta^s(E).
$$

The first quantity is [scale-restricted Hausdorff content](#scale-restricted-hausdorff-content). Shrinking $\delta$ removes options from the [infimum](real-analysis.md#infimum), so these contents increase to a [limit](calculus.md#limit-of-a-function), possibly infinite. The resulting [outer measure](#outer-measure) restricts to a [measure](#measure) on the [Borel sets](#borel-set). For $s=0$, counting each nonempty covering piece with cost one gives [counting measure](#counting-measure).

A different common convention multiplies these quantities by $c_s=\pi^{s/2}/(2^s\Gamma(1+s/2))$, using the [Gamma function](complex-analysis.md#gamma-function). At integer $s$, that normalization agrees with ordinary Euclidean $s$-dimensional volume. Here $c_1=1$, so both conventions make $\mathcal H^1$ agree with [arc length](riemannian-geometry.md#arc-length) on [smooth curves](differential-geometry.md#smooth-curve) in [Euclidean space](functional-analysis.md#euclidean-norm). Positive normalization constants never change [Hausdorff dimension](#hausdorff-dimension). A definition must specify this constant when numerical values of [Hausdorff measure](#hausdorff-measure) matter.

For a line segment of [length](physics.md#length) $L$, splitting it into $n$ equal pieces gives the [cover](set.md#cover-topology) cost

$$
n(L/n)^s=L^s n^{1-s}.
$$

It tends to zero for $s>1$, stays at $L$ for $s=1$, and grows for $s<1$. The matching lower bound comes from the fact that any interval [cover](set.md#cover-topology) must have total [length](physics.md#length) at least $L$. The exponent one is therefore the transition between a measuring rule too coarse to see the segment and one that assigns it infinite size. For a [Cantor set](geometry-and-topology.md#cantor-set), the transition is instead at $\log2/\log3$, as shown in [Hausdorff dimension of the Cantor set](#hausdorff-dimension-of-the-cantor-set).

This makes [Hausdorff measure](#hausdorff-measure) useful when ordinary [Lebesgue measure](#lebesgue-measure) sees too little: a [curve](topology.md#curve) in the plane has zero planar area but can have positive [arc length](riemannian-geometry.md#arc-length), and the [Cantor set](geometry-and-topology.md#cantor-set) has zero line [length](physics.md#length) but positive geometric size at its own dimension. It also separates local covering estimates from global cardinality: a [countable](set-theory.md#countable-set) dense [set](set.md) has zero [Hausdorff dimension](#hausdorff-dimension), despite meeting every open region of its closure.

An original source for the construction is Felix Hausdorff's [Dimension und äußeres Maß, Mathematische Annalen 79, pp. 157–179](https://link.springer.com/article/10.1007/BF01457179). The modern covering and [Hausdorff dimension](#hausdorff-dimension) framework is developed in [Bishop and Peres, Fractals in Probability and Analysis, §1.2](https://www.math.stonybrook.edu/~bishop/fractalbook.pdf).

#### Scale-restricted Hausdorff content

↑ **Parent:** [Hausdorff measure](#hausdorff-measure)

For $\delta>0$, [scale-restricted Hausdorff content](#scale-restricted-hausdorff-content) is the [infimum](real-analysis.md#infimum) of $\sum_j(\operatorname{diam}U_j)^s$ over [countable](set-theory.md#countable-set) [covers](set.md#cover-topology) of $F$ by [sets](set.md) of [diameter](topological-analysis.md#diameter) at most $\delta$, using the convention in [Hausdorff measure](#hausdorff-measure). It increases as $\delta$ decreases; its [limit](calculus.md#limit-of-a-function) is [Hausdorff measure](#hausdorff-measure). Unrestricted Hausdorff content imposes no [diameter](topological-analysis.md#diameter) bound and can behave differently.

Any explicit [cover](set.md#cover-topology) supplies an upper bound on [scale-restricted Hausdorff content](#scale-restricted-hausdorff-content), rather than its exact value. The level-$n$ intervals of the [Cantor set](geometry-and-topology.md#cantor-set), for example, give

$$
\mathcal H_{3^{-n}}^s(C)\leq2^n3^{-ns}.
$$

If this right-hand side tends to zero, then $\mathcal H^s(C)=0$. If it grows, that alone proves no positive lower bound: a different [cover](set.md#cover-topology) might be cheaper. The [mass distribution principle](#mass-distribution-principle) addresses precisely this gap by bounding the cost of every sufficiently small [cover](set.md#cover-topology).

#### Hausdorff dimension

↑ **Parent:** [Hausdorff measure](#hausdorff-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hausdorff_dimension)

The Hausdorff dimension is the critical exponent at which [Hausdorff measure](#hausdorff-measure) changes from infinite to zero:

$$
\dim_HE=\inf\{s\geq0:\mathcal H^s(E)=0\}
=\sup\{s\geq0:\mathcal H^s(E)=\infty\},
$$

with the standard endpoint convention for an empty supremum. This measures fine-scale geometric size rather than the number of coordinates used to describe the [set](set.md). A line segment has [Hausdorff dimension](#hausdorff-dimension) one; a square has dimension two; the middle-third [Cantor set](geometry-and-topology.md#cantor-set) has dimension $\log2/\log3\approx0.63093$.

Why can a dimension be fractional? At a scale reduced by a factor of three, the [Cantor set](geometry-and-topology.md#cantor-set) needs twice as many construction intervals. The balance $2(1/3)^d=1$ gives $d=\log2/\log3$, between the growth rates of finitely many points and a whole interval. Making this argument rigorous requires a [cover](set.md#cover-topology) upper bound and the [mass distribution principle](#mass-distribution-principle) lower bound, as in [Hausdorff dimension of the Cantor set](#hausdorff-dimension-of-the-cantor-set).

At the critical exponent itself, [Hausdorff measure](#hausdorff-measure) can be zero, finite and positive, or infinite; dimension does not specify that endpoint value. For example, [finite sets](set.md#finite-set) and [countably infinite sets](set-theory.md#countably-infinite-set) both have dimension zero, although their [counting measures](#counting-measure) differ. Dimension is also different from a finite-resolution estimate: [box-counting dimension](geometry-and-topology.md#box-counting-dimension) is another asymptotic definition, and fitting a scaling slope over a handful of observed scales does not establish either dimension.

The metric matters. Multiplying every distance by a fixed positive constant multiplies $\mathcal H^s$ by that constant to the power $s$ and preserves [Hausdorff dimension](#hausdorff-dimension). A [Lipschitz map](real-analysis.md#lipschitz-continuity) cannot increase it, because mapped [cover](set.md#cover-topology) [diameters](topological-analysis.md#diameter) increase by at most a fixed factor. A [bi-Lipschitz map](real-analysis.md#bi-lipschitz-map) therefore preserves it by applying this fact in both directions. These properties make [Hausdorff dimension](#hausdorff-dimension) useful for comparing geometric models while controlling how their measurements change.

##### Mass distribution principle

↑ **Parent:** [Hausdorff dimension](#hausdorff-dimension)

The mass distribution principle converts a diffuse [measure](#measure) into a lower bound on [Hausdorff dimension](#hausdorff-dimension). Let $s>0$ and let a [Borel probability measure](#borel-probability-measure) $\mu$ give a [Borel set](#borel-set) $E$ full mass. If, for some $C,r_0>0$, every [ball](topological-analysis.md#ball-mathematics) centered in $E$ satisfies

$$
\mu(B(x,r))\leq Cr^s\qquad(0<r<r_0),
$$

then $\mathcal H^s(E)\geq1/C>0$ in the diameter-cost convention, and consequently $\dim_HE\geq s$.

The idea is to keep unit mass from being crowded into cheap covering pieces. For a piece $U$ of positive [diameter](topological-analysis.md#diameter) $r$ meeting $E$, choose $x\in U\cap E$. A ball of radius $r+\varepsilon$ contains $U$; letting $\varepsilon\downarrow0$ gives $\mu^*(U)\leq Cr^s$, where $\mu^*$ is the associated [outer measure](#outer-measure). Zero-diameter pieces have zero mass by the same estimate. For any sufficiently small [cover](set.md#cover-topology),

$$
1=\mu(E)\leq\sum_j\mu^*(U_j)\leq C\sum_j(\operatorname{diam}U_j)^s.
$$

Thus every cover costs at least $1/C$. This is the lower-bound counterpart to the explicit covers in [scale-restricted Hausdorff content](#scale-restricted-hausdorff-content). The [Cantor distribution](continuous-probability-distribution.md#cantor-distribution) supplies the needed mass in [Hausdorff dimension of the Cantor set](#hausdorff-dimension-of-the-cantor-set). [Bishop and Peres, §1.2: the mass distribution principle](https://www.math.stonybrook.edu/~bishop/fractalbook.pdf).

##### Hausdorff dimension of the Cantor set

↑ **Parent:** [Hausdorff dimension](#hausdorff-dimension)

The middle-third [Cantor set](geometry-and-topology.md#cantor-set) has [Hausdorff dimension](#hausdorff-dimension)

$$
d=\frac{\log2}{\log3}\approx0.63093.
$$

Its [Lebesgue measure](#lebesgue-measure) is zero, yet $0<\mathcal H^d(C)<\infty$. These assertions measure different aspects of size: interval [length](physics.md#length) is too coarse to distinguish this set from a [null set](#null-set), while the critical fractional measuring rule captures its remaining structure.

At level $n$, the construction [covers](set.md#cover-topology) $C$ by $2^n$ intervals of [diameter](topological-analysis.md#diameter) $3^{-n}$. Their total $s$-cost is

$$
2^n(3^{-n})^s=(2\,3^{-s})^n.
$$

For $s>d$ it tends to zero, proving the upper dimension bound. At $s=d$ it equals one, giving $\mathcal H^d(C)\leq1$. For $s<d$ this particular [cover](set.md#cover-topology)'s cost grows, but that alone would not prove a lower bound on [Hausdorff measure](#hausdorff-measure).

<a id="image-cantor-cover-costs-change-trend-at-the-critical-exponent-and-distributed-mass-supplies-the-lower-bound"></a>
![](hausdorff-cover-cost-threshold.png)

**[Figure 1](#image-cantor-cover-costs-change-trend-at-the-critical-exponent-and-distributed-mass-supplies-the-lower-bound). Cantor cover costs change trend at the critical exponent, and distributed mass supplies the lower bound**.

For the matching lower bound, use the [Cantor distribution](continuous-probability-distribution.md#cantor-distribution), which assigns mass $2^{-n}$ to each level-$n$ [Cantor cylinder](geometry-and-topology.md#cantor-cylinder). An interval of length $r$ with $3^{-(n+1)}<r\leq3^{-n}$ meets at most two level-$n$ construction intervals, since their gaps are at least $3^{-n}$. Its mass is therefore at most

$$
2\,2^{-n}=2(3^{-n})^d<2\,3^d r^d=4r^d.
$$

Every covering [set](set.md) of [diameter](topological-analysis.md#diameter) $r$ in the line lies in an interval of length $r$, so any small [cover](set.md#cover-topology) must have total $d$-cost at least $1/4$. This is the [mass distribution principle](#mass-distribution-principle) in its interval form: $1/4\leq\mathcal H^d(C)\leq1$, sufficient to prove the claimed dimension. The constants are convenient bounds, rather than an assertion of the exact critical [Hausdorff measure](#hausdorff-measure). In the diagram, the right panel is a finite-stage approximation to the [Cantor function](mathematics.md#cantor-function), showing how probability is shared while the middle third receives none.

The reusable pattern is to obtain an upper bound by constructing [covers](set.md#cover-topology) and a lower bound by distributing mass. The same strategy underlies [Cartesian powers of the Cantor set](geometry-and-topology.md#cartesian-powers-of-the-cantor-set) and the dimension formula for a [finite similarity iterated function system](geometry-and-topology.md#finite-similarity-iterated-function-system) satisfying the [open set condition](geometry-and-topology.md#open-set-condition).

##### Pressure upper bound for Hausdorff dimension

↑ **Parent:** [Hausdorff dimension](#hausdorff-dimension)

Suppose shrinking interval covers of $F$ have length-power sums with logarithmic growth rate $P(\gamma)$, and $P$ is strictly decreasing with zero $\gamma_*$. For every $\gamma>\gamma_*$ those sums tend to zero exponentially. The definition of [Hausdorff measure](#hausdorff-measure) then gives $\mathcal H^\gamma(F)=0$, hence the displayed upper bound. A matching lower bound requires additional information and does not follow from this covering argument alone.

##### Hausdorff dimension of a connected set

↑ **Parent:** [Hausdorff dimension](#hausdorff-dimension)

A [connected](geometry-and-topology.md#connected-space) subset $C$ of [Euclidean space](functional-analysis.md#euclidean-norm) containing distinct points $a,b$ has [Hausdorff dimension](#hausdorff-dimension) at least one. The [Lipschitz](real-analysis.md#lipschitz-continuity) map $x\mapsto|x-a|$ maps $C$ onto a set containing $[0,|b-a|]$, since [continuous images of connected spaces](geometry-and-topology.md#continuous-image-of-a-connected-space) are [connected](geometry-and-topology.md#connected-space). A [Lipschitz map](real-analysis.md#lipschitz-continuity) cannot increase [Hausdorff dimension](#hausdorff-dimension), whereas an interval has [Hausdorff dimension](#hausdorff-dimension) one. Consequently any set of [Hausdorff dimension](#hausdorff-dimension) less than one is [totally disconnected](arithmetic.md#totally-disconnected-space).

## Vector measure

↑ **Parent:** [Measure theory](measure-theory.md)

A finite-dimensional [vector measure](#vector-measure) has scalar [measures](#measure) as components and a [total variation norm of a measure](#total-variation-norm-of-a-measure) defined using their joint vector [norm](functional-analysis.md#norm). Finite variation controls every pairing with a bounded continuous vector test. [Derivatives](calculus.md#derivative) in the [bounded-variation space](inverse-problem.md#function-of-bounded-variation-on-a-domain) are examples.

### Vector Radon measure

↑ **Parent:** [Vector measure](#vector-measure)

A vector [Radon measure](#radon-measure) has [Radon measures](#radon-measure) as components. The vector form of the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) identifies finite such [measures](#measure) with bounded functionals on $C_0(\Omega;\mathbb R^n)$.

#### Polar decomposition of a vector measure

↑ **Parent:** [Vector Radon measure](#vector-radon-measure)

Each component of a finite [vector measure](#vector-measure) is absolutely continuous with respect to its variation [measure](#measure). The [Radon-Nikodym theorem](#radon-nikodym-theorem) gives a vector density $\sigma$. Taking the [variation measure](#variation-measure) of this representation gives $|\mu|=|\sigma||\mu|$, hence the unit-length property. For a BV [derivative](calculus.md#derivative) this separates the magnitude of variation from its local direction.

## Standard Borel probability space

↑ **Parent:** [Measure theory](measure-theory.md)

A probability space whose measurable space is isomorphic to a Borel subset of a complete separable metric space with its Borel sigma-algebra. This supplies a [countable generating algebra](#countable-generating-algebra) and permits the [disintegration theorem for a probability measure](probability-theory.md#disintegration-theorem-for-a-probability-measure). Completions can be handled modulo null sets; conditional kernels are chosen on the underlying Borel model.

## Measurable space

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurable_space)

A measurable space is a set equipped with a [sigma-algebra](#sigma-algebra) of measurable subsets. A [measure space](#measure-space) additionally specifies a [measure](#measure) on that sigma-algebra.

### Standard Borel space

↑ **Parent:** [Measurable space](#measurable-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Standard_Borel_space)

A [standard Borel space](#standard-borel-space) is a [measurable space](#measurable-space) isomorphic to a [Borel set](#borel-set) of a [Polish space](topological-analysis.md#polish-space), with its Borel sigma-algebra. This measurable regularity permits the usual constructions of random samples and random counting measures, without requiring a particular compatible topology.

## Null set

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Null_set)

A [measurable set](#measurable-set) $N$ is a null set for a [measure](#measure) $\mu$ when $\mu(N)=0$. A property holds [almost everywhere](#almost-everywhere) when its exceptions lie in a null set. With a [complete measure](#complete-measure), every [subset](set.md#subset) of a null set is measurable and is itself a null set.

### Lebesgue null set

↑ **Parent:** [Null set](#null-set)

A Lebesgue null set has zero [Lebesgue measure](#lebesgue-measure). Since [Lebesgue measure](#lebesgue-measure) is complete, every [subset](set.md#subset) of one is also measurable and null. The [Cantor set](geometry-and-topology.md#cantor-set) is an [uncountable](set-theory.md#uncountable-set) example with positive [Hausdorff dimension](#hausdorff-dimension); the [rational numbers](number-theory.md#rational-number) form a [countable](set-theory.md#countable-set), [dense](topology.md#dense-set) example with [Hausdorff dimension](#hausdorff-dimension) zero. Being null does not imply being empty or having finitely many points.

### Borel null set

↑ **Parent:** [Null set](#null-set)

A [Borel set](#borel-set) of [Lebesgue measure](#lebesgue-measure) zero. Every Lebesgue-null [set](set.md) is contained in a Borel [null set](#null-set), by outer regularity; consequently testing all [Borel null sets](#borel-null-set) suffices in the definition of a [Sierpiński set](#sierpinski-set).

## Random measure

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Random_measure)

A random measure assigns a [measure](#measure) $\mu_\omega$ to each outcome so that $\omega\mapsto\mu_\omega(A)$ is a [random variable](random-variable.md) for every measurable $A$. A [finite-variation process](stochastic-calculus.md#finite-variation-process) gives pathwise signed random measures through [Lebesgue–Stieltjes integration](#lebesgue-stieltjes-integration).

## Measurable partition

↑ **Parent:** [Measure theory](measure-theory.md)

A countable measurable partition is a countable family of pairwise disjoint measurable sets whose union has full measure. Its members are its atoms; null atoms can be discarded in statements made [almost everywhere](#almost-everywhere).

### Partition atom

↑ **Parent:** [Measurable partition](#measurable-partition)

A partition atom is a member of a [measurable partition](#measurable-partition). For a finite or countable partition, each cell is an [atom of a sigma-algebra](#atom-of-a-sigma-algebra) generated by that partition, whose measurable sets are unions of cells. A partition atom need not be an [atom of a measure](#atom-measure-theory): an interval cell with positive [Lebesgue measure](#lebesgue-measure) can be split into smaller positive-measure sets that lie outside the generated partition sigma-algebra.

### Entropy of a countable measurable partition

↑ **Parent:** [Measurable partition](#measurable-partition)

For a countable [measurable partition](#measurable-partition), its entropy is $H_\mu(\xi)=-\sum_{A\in\xi}\mu(A)\log\mu(A)$, with $0\log0=0$. This extends [entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition) and is allowed to be infinite.

#### Conditional information function

↑ **Parent:** [Entropy of a countable measurable partition](#entropy-of-a-countable-measurable-partition)

For a [measurable partition](#measurable-partition) $\xi$ and a [sigma-algebra](#sigma-algebra) $\mathcal G$, the conditional information function is

$$
I_\mu(\xi\mid\mathcal G)
=-\sum_{A\in\xi}\mathbf1_A\log\mathbb E_\mu[\mathbf1_A\mid\mathcal G].
$$

The [conditional expectation](#conditional-expectation) in this formula is positive [almost everywhere](#almost-everywhere) on $A$. Without conditioning, the information is $I_\mu(\xi)(x)=-\log\mu(\xi(x))$.

##### Maximal inequality for conditional information functions

↑ **Parent:** [Conditional information function](#conditional-information-function)

For increasing [sigma-algebras](#sigma-algebra) $\mathcal G_n$, put $f_n=I_\mu(\xi\mid\mathcal G_n)$ and $F=\sup_n f_n$. For each atom $A\in\xi$ and $t\geq0$,

$$
\mu(A\cap\{F>t\})\leq e^{-t}.
$$

Together with the bound by $\mu(A)$ and the [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments), this yields $\int F\,d\mu\leq H_\mu(\xi)+1$. The inequality follows by stopping the [conditional-expectation martingale](martingale.md#conditional-expectation-martingale) $\mathbb E[\mathbf1_A\mid\mathcal G_n]$ the first time it falls below $e^{-t}$.

##### Conditional entropy of a countable measurable partition

↑ **Parent:** [Conditional information function](#conditional-information-function)

The conditional entropy is the integral of the [conditional information function](#conditional-information-function). Its chain rule expresses the entropy of a [join of measurable partitions](#join-of-measurable-partitions) as unconditional entropy plus conditional entropy. [Conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy), also for countable partitions of finite entropy.

### Join of measurable partitions

↑ **Parent:** [Measurable partition](#measurable-partition)

The join is the common refinement of two [measurable partitions](#measurable-partition), with atoms given by their nonempty intersections. For a [measure-preserving transformation](#measure-preserving-transformation), the block partition is $\xi_0^{n-1}=\bigvee_{j=0}^{n-1}T^{-j}\xi$.

## Field of sets

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Field_of_sets)

A Boolean algebra of subsets contains the empty set and is closed under finite unions and complements. It is consequently closed under finite intersections, differences, and symmetric differences.

## Semiring of sets

↑ **Parent:** [Measure theory](measure-theory.md)

A semiring of sets contains the empty set, is closed under intersections, and has the property that the difference of two members is a finite disjoint union of members. Predictable rectangles form a semiring generating the predictable sigma-algebra.

## Monotone class

↑ **Parent:** [Measure theory](measure-theory.md)

A monotone class of sets is closed under increasing countable unions and decreasing countable intersections.

### Monotone class theorem

↑ **Parent:** [Monotone class](#monotone-class)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monotone_class_theorem)

The monotone class theorem says that the smallest monotone class containing an algebra of sets equals the sigma-algebra generated by that algebra. It extends identities proved on a generating algebra to the full sigma-algebra.

#### Functional monotone-class theorem

↑ **Parent:** [Monotone class theorem](#monotone-class-theorem)

A vector space of bounded functions containing constants and indicators of a generating pi-system, and closed under uniformly bounded monotone pointwise limits, contains all bounded functions measurable for the generated sigma-algebra. This function version extends identities established on elementary integrands to every bounded measurable integrand.

// Target: probability-and-statistics.bigb

## Measurable function

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measurable_function)

A function $f:(X,\mathcal A)\to(Y,\mathcal B)$ between measurable spaces is measurable when $f^{-1}(B)\in\mathcal A$ for every $B\in\mathcal B$.

### Essential range

↑ **Parent:** [Measurable function](#measurable-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Essential_range)

The essential range of a real or complex [measurable function](#measurable-function) $m$ consists of the values $z$ whose every [neighborhood](topology.md#neighbourhood-mathematics) receives inputs of positive [measure](#measure):

$$
\operatorname{essran}_\mu m=\{z:\mu(\{x:|m(x)-z|<\varepsilon\})>0\text{ for every }\varepsilon>0\}.
$$

It depends on the [measure](#measure) as well as the [function](function.md). This definition concerns values arbitrarily near $z$, not necessarily inputs at which $m=z$ exactly. It therefore retains meaningful limiting values while ignoring values occurring only on [null sets](#null-set). [Teschl, Mathematical Methods in Quantum Mechanics, §2.4, equation (2.77): essential range](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe2.pdf).

For $m(x)=x$ on $(0,1)$ with [Lebesgue measure](#lebesgue-measure), **the ordinary [image of a function](set-theory.md#image-of-a-function) is $(0,1)$, but the [essential range](#essential-range) is $[0,1]$**. Neither endpoint is attained, yet inputs with $|m(x)|<\varepsilon$ or $|m(x)-1|<\varepsilon$ have positive [measure](#measure) for every $\varepsilon>0$. Every interior value also belongs to the [essential range](#essential-range), although its exact [fiber](function.md#fiber-of-a-function) is a [singleton](set.md#singleton-mathematics) of zero [measure](#measure). Positive [measure](#measure) of a fiber is sufficient, but is not necessary, for a value to belong to the [essential range](#essential-range).

The two-sided example $g$ from [essential infimum and essential supremum](real-analysis.md#essential-infimum-and-essential-supremum) illustrates what disappears. It follows $g(x)=x$ on $[0,1]$, except $g(1/4)=-3$ and $g(3/4)=4$. Its ordinary [image of a function](set-theory.md#image-of-a-function) is $([0,1]\setminus\{1/4,3/4\})\cup\{-3,4\}$, whereas its [essential range](#essential-range) remains $[0,1]$. The missing ordinary values $1/4$ and $3/4$ still have arbitrarily close neighbors with positive [measure](#measure); the exceptional values $-3$ and $4$ can each be isolated by a sufficiently small [neighborhood](topology.md#neighbourhood-mathematics) whose [preimage](set-theory.md#preimage) is a [null set](#null-set).

<a id="image-the-essential-range-of-the-modified-identity-function-remains-0-1-while-its-ordinary-image-of-a-function-includes-two-isolated-outliers"></a>
![](essential-upper-lower-bound-exceptions.png)

**[Figure 2](#image-the-essential-range-of-the-modified-identity-function-remains-0-1-while-its-ordinary-image-of-a-function-includes-two-isolated-outliers). The essential range of the modified identity function remains $[0,1]$, while its ordinary image of a function includes two isolated outliers**. For [Lebesgue measure](#lebesgue-measure), the filled outliers $-3$ and $4$ fail the criterion of positive [measure](#measure) in every [neighborhood](topology.md#neighbourhood-mathematics). The hollow values $1/4$ and $3/4$ still belong to the [essential range](#essential-range) because nearby outputs occur on [intervals](real-analysis.md#interval-mathematics) of positive [measure](#measure).

For the three-point example in [L-infinity norm](real-analysis.md#l-infinity-norm), the values are $1,3,10$. With weights $(0.5,0.5,0)$ the [essential range](#essential-range) is $\{1,3\}$; with weights $(0.499,0.5,0.001)$ it is $\{1,3,10\}$. A small but positive [probability](probability-theory.md#probability) retains ten, so an [essential range](#essential-range) does not discard a value merely because it is rare. For a real [function](function.md) on a space of positive total [measure](#measure), the [essential infimum](real-analysis.md#essential-infimum) and [essential supremum](#essential-supremum) are the lower and upper edges of its [essential range](#essential-range), allowing infinite bounds. The [L-infinity norm](real-analysis.md#l-infinity-norm) instead takes the upper edge of the [essential range](#essential-range) of $|m|$.

<a id="image-including-ten-in-the-essential-range-changes-the-limiting-lp-norm-even-when-its-probability-is-only-0-001"></a>
![](lp-norm-null-versus-rare-value.png)

**[Figure 3](#image-including-ten-in-the-essential-range-changes-the-limiting-lp-norm-even-when-its-probability-is-only-0-001). Including ten in the essential range changes the limiting Lp norm, even when its probability is only $0.001$**. The blue case has [essential range](#essential-range) $\{1,3\}$, while the red case has [essential range](#essential-range) $\{1,3,10\}$. These finite positive-valued examples make their largest essential values equal to their [L-infinity norms](real-analysis.md#l-infinity-norm).

A useful operator connection is the [spectrum of a real multiplication operator](vector-space.md#spectrum-of-a-real-multiplication-operator): on a nonzero [L2 space](#l2-space-is-a-hilbert-space) over a [sigma-finite measure](#sigma-finite-measure), multiplication by a real [measurable function](#measurable-function) $m$ has [spectrum](linear-operator-theory.md#spectrum-functional-analysis) equal to its [essential range](#essential-range), with the natural domain when $m$ is unbounded. Outside that range, $|m-z|$ has a positive lower bound [almost everywhere](#almost-everywhere), so multiplication by $1/(m-z)$ gives an [inverse function](function.md#inverse-function) that is a [bounded linear operator](topological-vector-space.md#continuous-linear-operator). Near an essential value, this lower bound fails. Thus discarding [null sets](#null-set) is precisely what makes the range match an operator acting on [almost everywhere](#almost-everywhere) [equivalence classes](set-theory.md#equivalence-class). [Teschl, Mathematical Methods in Quantum Mechanics, §2.4, equations (2.74)–(2.77): multiplication-operator spectrum](https://www.mat.univie.ac.at/~gerald/ftp/book-schroe/schroe2.pdf).

### Measurability

↑ **Parent:** [Measurable function](#measurable-function)

Measurability is the property that inverse images of measurable target sets are measurable in the source space. For a [stochastic process](stochastic-process.md), joint measurability in time and sample is a different condition from the separate adaptedness condition at each fixed time. The [predictable sigma-algebra](martingale.md#predictable-sigma-algebra) and [progressive measurability](stochastic-process.md#progressive-measurability) encode particular joint measurability requirements.

### Borel measurable function

↑ **Parent:** [Measurable function](#measurable-function)

A function into a topological space is Borel measurable when the inverse image of every [Borel set](#borel-set) is measurable. Equivalently, it is measurable when the target carries its Borel sigma-algebra.

### Composition of measurable functions

↑ **Parent:** [Measurable function](#measurable-function)

If $f:(X,\mathcal A)\to(Y,\mathcal B)$ and $g:(Y,\mathcal B)\to(Z,\mathcal C)$ are measurable, then $g\circ f$ is measurable because

$$
(g\circ f)^{-1}(C)=f^{-1}(g^{-1}(C)).
$$

## Measure density

↑ **Parent:** [Measure theory](measure-theory.md)

For a measurable set $A\subseteq\mathbb R^n$, its density at $x$ with respect to a locally finite measure $\mu$ is

$$
\rho_{\mu,A}(x)=\lim_{r\downarrow0}\frac{\mu(A\cap B_r(x))}{\mu(B_r(x))}
$$

when this [limit](calculus.md#limit-of-a-function) exists.

### Spherical derivative of a measure

↑ **Parent:** [Measure density](#measure-density)

The spherical [derivative](calculus.md#derivative) compares the mass of shrinking centered [open balls](topology.md#open-ball) with their [Lebesgue measure](#lebesgue-measure), when the limit exists. This is a density of one [measure](#measure) relative to Euclidean volume, rather than the relative density of a set within one fixed [measure](#measure). A singular finite [Borel measure](#borel-measure) has spherical [derivative](calculus.md#derivative) zero [Lebesgue almost everywhere](#almost-everywhere).

#### Spherical derivative of a singular measure vanishes

↑ **Parent:** [Spherical derivative of a measure](#spherical-derivative-of-a-measure)

For a finite singular [Borel measure](#borel-measure), choose [compact subsets](topology.md#compact-space) of a Lebesgue-null carrier whose omitted mass is arbitrarily small. Outside any such [compact subset](topology.md#compact-space), sufficiently small balls see only the omitted [measure](#measure). The [uncentered maximal weak-type inequality](analysis.md#uncentered-maximal-weak-type-inequality) bounds the volume of points where the omitted [measure](#measure) has large density. Letting its total mass tend to zero shows that the upper spherical density is zero almost everywhere. This argument does not require the null carrier itself to be closed or separated from every point outside it.

### Lebesgue differentiation theorem

↑ **Parent:** [Measure density](#measure-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_differentiation_theorem)

If $f$ is locally [Lebesgue integrable](#lebesgue-integrable-function) on $\mathbb R^n$, then for [Lebesgue almost every](#almost-everywhere) $x$,

$$
\lim_{r\downarrow0}\frac1{|B_r(x)|}\int_{B_r(x)}f(y)\,dy=f(x).
$$

#### Oscillating annuli obstruct differentiation at a point

↑ **Parent:** [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem)

Let $a_n=2^{-2^n}$ and, in angular coordinates near zero, take a bounded indicator alternating between one and zero on the rings $a_{n+1}<|t|\leq a_n$. Since $a_{n+1}/a_n\to0$, the mean over $[-a_n,a_n]$ approaches the value of the outermost ring. Its even and odd subsequences approach one and zero. Thus an integrable function can fail to have a limiting centered average at a specified point, although [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem) ensures convergence almost everywhere.

#### Lebesgue point

↑ **Parent:** [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_point)

A point $x\in\mathbb R^n$ is a Lebesgue point of a locally [Lebesgue integrable function](#lebesgue-integrable-function) $f$ when

$$
\lim_{r\downarrow0}\frac1{|B_r(x)|}
\int_{B_r(x)}|f(y)-f(x)|\,dy=0.
$$

The [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem) says that almost every point is a Lebesgue point.

#### Differentiation of an indefinite Lebesgue integral

↑ **Parent:** [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem)

If $g$ is locally [Lebesgue integrable](#lebesgue-integrable-function) and

$$
G(x)=\int_a^x g(t)\,dt,
$$

then $G'(x)=g(x)$ at every [Lebesgue point](#lebesgue-point) of $g$, and hence [almost everywhere](#almost-everywhere).

<h3 id="lebesgue-s-density-theorem">Lebesgue's density theorem</h3>

↑ **Parent:** [Measure density](#measure-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue's_density_theorem)

For every [Lebesgue measurable set](#lebesgue-measurable-set) $A\subseteq\mathbb R^n$, its [Lebesgue density](#measure-density) is $1$ at almost every point of $A$ and $0$ at almost every point of its complement.

#### Density point

↑ **Parent:** [Lebesgue's density theorem](#lebesgue-s-density-theorem)

A point at which a measurable set occupies an asymptotically full fraction of small balls, as expressed above with [Lebesgue measure](#lebesgue-measure). The [Lebesgue density theorem](#lebesgue-s-density-theorem) says that almost every point of a measurable set is a density point. On the real line, the same limiting conclusion holds for arbitrary shrinking intervals containing that point, since each interval lies in a centered interval of at most twice its length.

#### High-density interval in a positive-measure subset of the real line

↑ **Parent:** [Lebesgue's density theorem](#lebesgue-s-density-theorem)

If a measurable set $E\subseteq\mathbb R$ has positive measure, then for every $\varepsilon>0$ there is a bounded interval $I$ such that

$$
m(E\cap I)>(1-\varepsilon)m(I).
$$

Choose a density-one point of a finite positive-measure portion of $E$ using the [Lebesgue density theorem](#lebesgue-s-density-theorem), and take a sufficiently small interval centred there.

## Lebesgue measurable set

↑ **Parent:** [Measure theory](measure-theory.md)

A Lebesgue measurable set is a member of the completion of the Borel sigma-algebra with respect to [Lebesgue measure](#lebesgue-measure). In particular, it differs from a [Borel set](#borel-set) by a null set.

### Regularity of Lebesgue measure

↑ **Parent:** [Lebesgue measurable set](#lebesgue-measurable-set)

Every Lebesgue measurable set of finite measure can be approximated arbitrarily closely in measure from outside by an open set and from inside by a compact set. On a bounded interval it can consequently be approximated in symmetric-difference measure by a finite union of intervals.

## Almost everywhere

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Almost_everywhere)

A property holds almost everywhere with respect to a [measure](#measure) when the set of points where it fails has measure zero.

## Lebesgue integrable function

↑ **Parent:** [Measure theory](measure-theory.md)

A measurable function $f$ is Lebesgue integrable when $\int |f|\,d\lambda<\infty$.

### Integrability

↑ **Parent:** [Lebesgue integrable function](#lebesgue-integrable-function)

A real or complex [measurable function](#measurable-function) is integrable for a [measure](#measure) $\mu$ when its absolute value has finite integral. For a [random variable](random-variable.md), this is integrability with respect to its [probability measure](probability-theory.md#probability-measure), and makes its [expectation](probability-theory.md#expected-value) finite.

## Conditional expectation

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Conditional_expectation)

The conditional expectation is the average of a [random variable](random-variable.md) that can be predicted using specified information. It is itself a [random variable](random-variable.md): the average appropriate to one observed group may differ from that appropriate to another group. The [sigma-algebra](#sigma-algebra) $\mathcal G$ records which [events](probability-theory.md#event) can be distinguished with the available information.

For a real [integrable random variable](probability-theory.md#integrable-random-variable) $X$ on a [probability space](probability-theory.md#probability-space) $(\Omega,\mathcal F,\mathbb P)$ and a sub-[sigma-algebra](#sigma-algebra) $\mathcal G$, the conditional expectation $m=\mathbb E[X\mid\mathcal G]$ is the [almost surely](convergence-of-random-variables.md#almost-sure-convergence) unique [integrable random variable](probability-theory.md#integrable-random-variable) that is [measurable](#measurability) with respect to $\mathcal G$ and satisfies

$$
\int_A m\,d\mathbb P=\int_A X\,d\mathbb P\qquad\text{for every }A\in\mathcal G.
$$

Its average therefore agrees with that of $X$ on every distinguishable [event](probability-theory.md#event). The integral characterization handles discrete observations, continuous observations, and information that is not given by a single numerical value.[PDF pp. 4–8](mathematics-bibliography.md#18-175-lecture-16-conditional-expectation-random-walks-martingales-by-scott-sheffield)

If the information tells us which member of a finite [measurable partition](#measurable-partition) $A_1,\ldots,A_k$ contains the outcome, then on every member of positive [probability](probability-theory.md#probability),

$$
m=\frac{\mathbb E[X\mathbf1_{A_i}]}{\mathbb P(A_i)}\quad\text{on }A_i.
$$

Here $\mathbf1_{A_i}$ is an [indicator function](#indicator-function). Zero-probability members do not determine a unique value, which is why uniqueness is only [almost surely](convergence-of-random-variables.md#almost-sure-convergence). For [square-integrable](#square-integrable-function) $X$, this same [conditional mean](#conditional-expectation) is the best predictor among $\mathcal G$-measurable [random variables](random-variable.md) under [mean squared error](statistical-modelling.md#mean-squared-error); the [conditional variance](variance.md#conditional-variance) describes its remaining error. A [conditional mean](#conditional-expectation) is generally not the same as the actual observed value of $X$.[Theorem 4.1.15, p. 213](mathematics-bibliography.md#probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation)

### Conditional expectation preserving a distribution

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For a real [integrable random variable](probability-theory.md#integrable-random-variable) $X$, a [conditional expectation](#conditional-expectation) $Y=\mathbb E[X\mid\mathcal G]$ with the same [probability distribution](probability-theory.md#probability-distribution) as $X$ must equal $X$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence). No second moment is needed. For any real $c$, the nonnegative [random variable](random-variable.md) $D_c=|X-c|-\operatorname{sign}(Y-c)(X-c)$ has [expected value](probability-theory.md#expected-value) zero, by conditioning and equality of the two absolute moments. Thus $Y>c$ implies $X\geq c$, $Y<c$ implies $X\leq c$, and $Y=c$ implies $X=c$, outside a null set. Using a [countable](set-theory.md#countable-set) family of rational $c$ separates any unequal real values and proves the claim. Equality of the probabilities of $X=c$ and $Y=c$ also gives equality of their zero sets and hence equality of the two sign functions for every fixed $c$.

### Dyadic conditional averages recover integrable functions

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For an integrable [function](function.md) on $[0,1]$, average $f$ on each [dyadic interval](real-analysis.md#dyadic-interval) of length $2^{-n}$. The resulting [step function](#step-function) $f_n$ converges to $f$ [almost everywhere](#almost-everywhere) and in the [L1 norm](functional-analysis.md#l1-norm). If $U$ has the [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) on $[0,1]$, then $f_n(U)=\mathbb E[f(U)\mid\sigma(b_n(U))]$, where $b_n$ rounds down to a dyadic endpoint. Refinement makes these [conditional expectations](#conditional-expectation) a [uniformly integrable](convergence-of-random-variables.md#uniform-integrability) [martingale](martingale.md). The [uniformly integrable martingale convergence theorem](martingale.md#uniformly-integrable-martingale-convergence-theorem) gives almost-sure and [convergence in L1](convergence-of-random-variables.md#convergence-in-l1) to a limit $Y$.

Since $b_n(U)\to U$, the generated limiting [sigma-algebra](#sigma-algebra) contains $U$ up to null sets. For every [event](probability-theory.md#event) $A$ in any finite-stage [sigma-algebra](#sigma-algebra), convergence in the [L1 norm](functional-analysis.md#l1-norm) gives $\mathbb E[Y\mathbf1_A]=\mathbb E[f(U)\mathbf1_A]$. The [pi-lambda theorem](probability-theory.md#pi-lambda-theorem) extends this equality to the limiting [sigma-algebra](#sigma-algebra), identifying $Y=f(U)$. The [uniform distribution](continuous-probability-distribution.md#continuous-uniform-distribution) of $U$ translates the two convergence conclusions into the assertions for $f_n$. Choosing a Borel representative of $f$ and assigning arbitrary values at the endpoint one makes all random variables well defined without changing either conclusion.

### Symmetrization as conditional expectation

↑ **Parent:** [Conditional expectation](#conditional-expectation)

If a finite group $\Gamma$ acts by measure-preserving maps on a [probability space](probability-theory.md#probability-space), let $\mathcal I$ be its invariant [sigma-algebra](#sigma-algebra). For an integrable [random variable](random-variable.md) $Z$, the displayed group average is $\mathcal I$-measurable. For $A\in\mathcal I$, changing variables under each group element gives $\int_A Z\circ T_g\,d\mathbb P=\int_A Z\,d\mathbb P$. The average therefore satisfies the defining integral identity for [conditional expectation](#conditional-expectation). For permutations of $N$ exchangeable coordinates, averaging a product attached to $d$ distinct indices yields the sum over all ordered distinct $d$-tuples divided by the [falling factorial](combinatorics.md#falling-factorial) $(N)_d=N!/(N-d)!$.

#### Sampling with and without replacement comparison for bounded products

↑ **Parent:** [Symmetrization as conditional expectation](#symmetrization-as-conditional-expectation)

For arrays of values in $[0,1]$, let $U_N$ average a product of $d$ entries over all ordered index tuples from $N$ coordinates, and let $V_N$ average it over the tuples with distinct indices. Decompose the first average as $U_N=\alpha V_N+(1-\alpha)W_N$, where $\alpha=(N)_d/N^d$ and the repeated-index average $W_N$ lies in $[0,1]$. This gives $|U_N-V_N|\leq1-\alpha$. For uniformly sampled indices, a [union bound](probability-inequality.md#boole-s-inequality) over the $\binom d2$ pairs bounds the collision probability by $\binom d2/N$. This deterministic estimate is the bridge between empirical-product limits and the [De Finetti theorem](probability-theory.md#de-finetti-theorem).

### Conditional expectation from finite-measure densities

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For nonnegative [integrable](#integrability) $f$, the finite [measure](#measure) $A\mapsto\int_Af\,d\mu$ restricted to a sub-[sigma-algebra](#sigma-algebra) $\Sigma_0$ is [absolutely continuous with respect to](#absolute-continuity-of-measures) the restricted base [measure](#measure). Its [Radon-Nikodym derivative](#radon-nikodym-derivative) is $\Sigma_0$-measurable and has the required integral identities. Positive and negative parts extend the construction to real [integrable](#integrability) functions; real and imaginary parts extend it to complex functions. The result is unique [almost everywhere](#almost-everywhere).

### Equality case for conditional second moments

↑ **Parent:** [Conditional expectation](#conditional-expectation)

If $Y$ is a real square-integrable [random variable](random-variable.md) and $X=\mathbb E[Y\mid\mathcal G]$, then $\mathbb E[XY]=\mathbb EX^2$ and the displayed identity follows by expansion. Thus equality of the second moments forces $X=Y$ as an [almost sure equality](convergence-of-random-variables.md#almost-sure-equality). This is the equality case of the [conditional Jensen inequality](#conditional-jensen-inequality) for the strictly convex function $z\mapsto z^2$.

### Conditional L2 norm

↑ **Parent:** [Conditional expectation](#conditional-expectation)

Disintegrate over a [factor map](#factor-map-between-measure-preserving-systems) and take the $L^2$ norm using the conditional probability on each fiber. Its square integrates to the global squared norm. The [uniform conditional L2 norm](#uniform-conditional-l2-norm) takes the essential supremum of these fiber norms.

#### Conditional norm covariance under a factor map

↑ **Parent:** [Conditional L2 norm](#conditional-l2-norm)

For invertible probability systems linked by a [factor map](#factor-map-between-measure-preserving-systems), invariance and uniqueness of disintegration identify the pushforward of each conditional measure with the conditional measure on the transformed fiber. The displayed norm identity follows for all integer times on a common full-measure set. It transports uniform conditional error bounds along whole orbits.

#### Uniform conditional L2 norm

↑ **Parent:** [Conditional L2 norm](#conditional-l2-norm)

The essential supremum over the base of the [conditional L2 norm](#conditional-l2-norm). It may be infinite for a globally square-integrable function. For probability fibers, $\|f\|_2\leq\|f\|_{2,\infty\mid Y}$; the uniform norm controls all fibers outside a null set rather than only their average.

### Conditional Jensen inequality

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For an integrable [random variable](random-variable.md) $X$, a sub-[sigma-algebra](#sigma-algebra) $\mathcal G$, and a convex function $\phi$ with suitable integrability, $\phi(\mathbb E[X\mid\mathcal G])\le\mathbb E[\phi(X)\mid\mathcal G]$ almost surely. One proof writes $\phi$ as a supremum of supporting affine functions and applies monotonicity and [linearity](vector-space.md#linearity) of [conditional expectation](#conditional-expectation) to each. This proves the convex-loss form of the [Rao-Blackwell theorem](probability-and-statistics.md#rao-blackwell-theorem).

### L1 contraction of conditional expectation

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For an [integrable random variable](probability-theory.md#integrable-random-variable) $Y$, the [conditional expectation](#conditional-expectation) satisfies $|\mathbb E[Y\mid\mathcal G]|\leq\mathbb E[|Y|\mid\mathcal G]$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence). Taking [expected values](probability-theory.md#expected-value) gives the [L1 contraction of conditional expectation](#l1-contraction-of-conditional-expectation). Applying it to $Y_n-Y$ shows that [convergence in L1](convergence-of-random-variables.md#convergence-in-l1) is preserved by [conditional expectation](#conditional-expectation) with respect to any fixed [sigma-algebra](#sigma-algebra).

### Conditional expectation of a summand given future partial sums

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For [independent and identically distributed random variables](random-variable.md#independent-and-identically-distributed-random-variables) $X_j$ that are [integrable random variables](probability-theory.md#integrable-random-variable), with $S_n=\sum_{j=1}^nX_j$, symmetry gives $\mathbb E[X_1\mid S_n,S_{n+1},\ldots]=S_n/n$. The decreasing [sigma-algebras](#sigma-algebra) generated by these future sums permit application of the [reverse martingale convergence theorem](martingale.md#reverse-martingale-convergence-theorem).

### Law of total expectation

↑ **Parent:** [Conditional expectation](#conditional-expectation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Law_of_total_expectation)

The law of total expectation makes averaging in stages reliable, provided the outer stage uses the actual [probabilities](probability-theory.md#probability) of the groups. For an [integrable random variable](probability-theory.md#integrable-random-variable) $X$ and a sub-[sigma-algebra](#sigma-algebra) $\mathcal G$,

$$
\boxed{\mathbb E[\mathbb E[X\mid\mathcal G]]=\mathbb E[X].}
$$

Replacing each outcome by its group's [conditional mean](#conditional-expectation) preserves the overall [expected value](probability-theory.md#expected-value). In the definition of [conditional expectation](#conditional-expectation), take the [event](probability-theory.md#event) $A=\Omega$ to obtain this identity.[Equation (4.1.5), p. 212](mathematics-bibliography.md#probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation)

For a complete finite example, choose a group $Y=A$ with [probability](probability-theory.md#probability) $1/4$ and $Y=B$ with [probability](probability-theory.md#probability) $3/4$. Within group $A$, $X$ is $0$ or $4$ with equal [conditional probabilities](probability-theory.md#conditional-probability); within group $B$, it is $6$ or $10$ with equal [conditional probabilities](probability-theory.md#conditional-probability). Thus the [joint probability distribution](probability-theory.md#joint-probability-distribution) puts probabilities $1/8,1/8,3/8,3/8$ on $(A,0),(A,4),(B,6),(B,10)$. The [conditional means](#conditional-expectation) are two and eight. Consequently,

$$
\boxed{\mathbb E X=\frac14\cdot2+\frac34\cdot8=\frac{13}{2}.}
$$

Direct averaging of the four values gives the same $0/8+4/8+18/8+30/8=13/2$. Taking the unweighted average of the two group means instead gives five, which describes a different choice of group [probabilities](probability-theory.md#probability). This is why the outer weighting matters.

<a id="image-group-averages-preserve-the-overall-mean-when-weighted-by-group-probabilities"></a>
![](total-expectation-weighted-group-averages.png)

**[Figure 4](#image-group-averages-preserve-the-overall-mean-when-weighted-by-group-probabilities). Group averages preserve the overall mean when weighted by group probabilities**. The stipulated [joint probability distribution](probability-theory.md#joint-probability-distribution) assigns probabilities $1/8,1/8,3/8,3/8$ to values $0,4,6,10$ in groups $A,A,B,B$. The [conditional means](#conditional-expectation) are two and eight, occurring with probabilities $1/4$ and $3/4$. Both representations have [expected value](probability-theory.md#expected-value) $13/2$. The unweighted average of the group means, five, is shown separately as the result of different weighting. These are exact illustrative probabilities, not observations.

The formula is useful when conditioning on a first choice makes the remaining experiment simple. It can replace a large outcome enumeration by smaller calculations within groups. In a [mixture distribution](probability-theory.md#mixture-distribution), it combines component [means](probability-theory.md#expected-value) using mixture weights; in a [random sum of independent claims](actuarial-statistics.md#random-sum-of-independent-claims), it separates the number of summands from their individual [expected values](probability-theory.md#expected-value) under the stated [independence](random-variable.md#independent-random-variables) assumptions. The same averaging step appears in the [law of total variance](probability-theory.md#law-of-total-variance).

#### Nested conditioning keeps the coarser information

↑ **Parent:** [Law of total expectation](#law-of-total-expectation)

For [integrable random variable](probability-theory.md#integrable-random-variable) $X$ and nested sub-[sigma-algebras](#sigma-algebra) $\mathcal H\subseteq\mathcal G$, the [tower property](#law-of-total-expectation) says

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H].
$$

The finer-information [conditional mean](#conditional-expectation) can be averaged within each coarser group, recovering the coarser-information [conditional mean](#conditional-expectation). Conversely, conditioning an already $\mathcal H$-measurable [conditional mean](#conditional-expectation) on $\mathcal G$ leaves it unchanged. Both orders therefore recover $\mathbb E[X\mid\mathcal H]$ when the information is nested.[Theorem 4.1.13, p. 212](mathematics-bibliography.md#probability-theory-and-examples-fifth-edition-by-rick-durrett/4-1-conditional-expectation)

For the finite example in [law of total expectation](#law-of-total-expectation), exact knowledge of $X$ gives the finer mean $X$ itself. Averaging within the groups $A,B$ recovers two and eight. Forgetting the group then gives $13/2$. The nesting condition is essential; [iterated conditional expectation over nonnested sigma-algebras](#iterated-conditional-expectation-over-nonnested-sigma-algebras) describes why arbitrary successive conditioning cannot simply be replaced by conditioning on an intersection.

### Independent sigma-algebras have trivial intersection

↑ **Parent:** [Conditional expectation](#conditional-expectation)

If sub-sigma-algebras $\mathcal G$ and $\mathcal H$ are independent, every event in $\mathcal G\cap\mathcal H$ is independent of itself and consequently has probability zero or one. Thus

$$
\mathbb E[X\mid\mathcal G\cap\mathcal H]=\mathbb E[X]
$$

almost surely for every integrable random variable $X$.

### Iterated conditional expectation over nonnested sigma-algebras

↑ **Parent:** [Conditional expectation](#conditional-expectation)

In general,

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
\ne\mathbb E[X\mid\mathcal G\cap\mathcal H].
$$

Equality does hold when either sigma-algebra contains the other or when they are independent.

### Conditional Fatou lemma

↑ **Parent:** [Conditional expectation](#conditional-expectation)

For nonnegative random variables $X_n$ and a sigma-algebra $\mathcal G$,

$$
\mathbb E[\liminf_nX_n\mid\mathcal G]
\leq\liminf_n\mathbb E[X_n\mid\mathcal G]
$$

almost surely. It follows from the ordinary [Fatou lemma](#fatou-s-lemma) after testing both sides on every event in $\mathcal G$.

<h2 id="fatou-s-lemma">Fatou's lemma</h2>

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fatou's_lemma)

For nonnegative measurable functions,

$$
\int\liminf_nf_n\,d\mu\leq\liminf_n\int f_n\,d\mu.
$$

### Fatou lemma for series

↑ **Parent:** [Fatou's lemma](#fatou-s-lemma)

For nonnegative numbers $a_{n,k}$, [Fatou lemma](#fatou-s-lemma) applied to counting measure gives

$$
\sum_k\liminf_{n\to\infty}a_{n,k}
\leq\liminf_{n\to\infty}\sum_ka_{n,k}.
$$

### Proof of Fatou lemma

↑ **Parent:** [Fatou's lemma](#fatou-s-lemma)

Set

$$
g_n=\inf_{k\geq n}f_k.
$$

Then $0\leq g_n\uparrow\liminf_k f_k$. The [monotone convergence theorem](#monotone-convergence-theorem) and $g_n\leq f_k$ for every $k\geq n$ give

$$
\int\liminf_kf_k\,d\mu
=\lim_n\int g_n\,d\mu
\leq\lim_n\inf_{k\geq n}\int f_k\,d\mu
=\liminf_k\int f_k\,d\mu.
$$

### Strict inequality in Fatou lemma

↑ **Parent:** [Fatou's lemma](#fatou-s-lemma)

On $([0,1],\lambda)$, the functions

$$
f_n=n\mathbf1_{(0,1/n)}
$$

converge pointwise to zero but satisfy $\int f_n\,d\lambda=1$. Hence the two sides of [Fatou lemma](#fatou-s-lemma) can be zero and one.

## Ergodic theory

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ergodic_theory)

Ergodic theory studies the long-time statistical behaviour of [measure-preserving transformations](#measure-preserving-transformation).

### Generic point for an invariant measure

↑ **Parent:** [Ergodic theory](#ergodic-theory)

A point is generic for an [invariant measure](#invariant-measure) $\mu$ of a [continuous map](topology.md#continuous-map) on a [compact metric space](topological-analysis.md#compact-metric-space) if the displayed convergence holds for every [continuous function](calculus.md#continuous-function) $\varphi$. Its empirical [probability measures](probability-theory.md#probability-measure) converge against continuous test functions to $\mu$. The same test-function condition may be used before invariance is known: the telescoping identity for $\varphi\circ f-\varphi$ then proves that the limiting [Borel probability measure](#borel-probability-measure) must be invariant. If almost every point is generic for the same measure, continuous approximation of invariant-set indicators proves that this measure is [ergodic](#ergodicity).

### Invariant measure

↑ **Parent:** [Ergodic theory](#ergodic-theory)

For a measurable transformation $T$, a [measure](#measure) is invariant if the [pushforward measure](#pushforward-measure) equals the original [measure](#measure), or equivalently $\mu(T^{-1}A)=\mu(A)$ for every measurable $A$. This is the [measure](#measure) used in a [measure-preserving system](#measure-preserving-system).

#### Invariant probability measure for a semigroup

↑ **Parent:** [Invariant measure](#invariant-measure)

A [Borel probability measure](#borel-probability-measure) is invariant for a [Markov kernel](markov-process.md#markov-kernel) semigroup if every transition preserves it. For a [Feller semigroup](functional-analysis.md#feller-semigroup) on a compact metric space, it suffices to test the displayed identity on [continuous functions](calculus.md#continuous-function). Kernel [Jensen inequality](real-analysis.md#jensen-s-inequality) gives contraction on $L^p(\mu)$, and sup-norm strong continuity followed by density gives [strong continuity](functional-analysis.md#strong-continuity) there for $1\leq p<\infty$.

<h5 id="krylov-bogolyubov-theorem">Krylov–Bogolyubov theorem</h5>

↑ **Parent:** [Invariant probability measure for a semigroup](#invariant-probability-measure-for-a-semigroup)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Krylov–Bogolyubov_theorem)

For a [Feller semigroup](functional-analysis.md#feller-semigroup) on a compact [metric space](topological-analysis.md#metric-space), time-averaged transition laws have weakly convergent subsequences by [compactness of probability measures on a compact metric space](convergence-of-random-variables.md#compactness-of-probability-measures-on-a-compact-metric-space). Shifting a time interval of length $n$ by $t$ changes a bounded test-function average by at most $2t\|f\|_\infty/n$. A weak subsequential limit is therefore an [invariant probability measure for a semigroup](#invariant-probability-measure-for-a-semigroup). More generally, tightness of the time averages supplies the required compactness.

### Cutting and stacking

↑ **Parent:** [Ergodic theory](#ergodic-theory)

Cutting and stacking constructs [measure-preserving transformations](#measure-preserving-transformation) from towers of equal-measure levels. Cut a tower into equal-width subcolumns, add new spacer levels, and stack the resulting columns. Map each level to the one above by a measure-preserving identification; subsequent stages extend the partial map. When uncovered and top-level measures tend to zero, the limiting map is defined modulo null sets.

#### Chacon transformation

↑ **Parent:** [Cutting and stacking](#cutting-and-stacking)

The standard three-cut Chacon transformation is an invertible [measure-preserving transformation](#measure-preserving-transformation) built by [cutting and stacking](#cutting-and-stacking) with spacer vector $(0,1,0)$ at every stage. Cut the current tower into three equal subcolumns, place one spacer above the middle, and stack left to right. With initial width $2/3$ and height one on a unit interval, level counts and widths are $h_j=(3^{j+1}-1)/2$ and $w_j=2/3^{j+1}$. Tower measure tends to one, using total spacer measure $1/3$. Tower words obey $W_{j+1}=W_jW_j1W_j$.

### Unique ergodicity

↑ **Parent:** [Ergodic theory](#ergodic-theory)

A continuous self-map of a compact [metric space](topological-analysis.md#metric-space) is uniquely ergodic when it has exactly one invariant [Borel probability measure](#borel-probability-measure). An [irrational rotation of the circle](#irrational-rotation) is uniquely ergodic: invariance multiplies its nonzero-index [Fourier coefficients](fourier-series.md#fourier-coefficient) by nontrivial phases, forcing those coefficients to vanish. The [Stone-Weierstrass theorem](functional-analysis.md#stone-weierstrass-theorem) then identifies the invariant measure as normalized [Lebesgue measure](#lebesgue-measure).

#### Uniform ergodic convergence for uniquely ergodic systems

↑ **Parent:** [Unique ergodicity](#unique-ergodicity)

For a [uniquely ergodic](#unique-ergodicity) continuous map $T$ of a compact [metric space](topological-analysis.md#metric-space), every continuous $f$ satisfies $N^{-1}\sum_{j=0}^{N-1}f(T^jx)\to\int f\,d\mu$ uniformly in $x$. Otherwise choose increasingly long orbit [empirical measures](probability-theory.md#empirical-measure) with a fixed discrepancy. Compactness provides a weak limit; the telescoping identity makes it invariant, so it must be the unique measure $\mu$, contradicting that discrepancy. Compactness and continuity are essential hypotheses.

### Van der Corput lemma (Hilbert space sequences)

↑ **Parent:** [Ergodic theory](#ergodic-theory)

For a bounded sequence $(u_n)$ in a [Hilbert space](hilbert-space.md), put $c_h=\limsup_{N\to\infty}|N^{-1}\sum_{n=0}^{N-h-1}\langle u_{n+h},u_n\rangle|$. If $H^{-1}\sum_{h=1}^Hc_h\to0$, then $N^{-1}\sum_{n=0}^{N-1}u_n\to0$ in norm. Since the $c_h$ are bounded, it suffices that $(c_h)$ has [convergence in density of a sequence](#convergence-in-density-of-a-sequence) to zero. The proof applies the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to an average of shifted sums.

#### Van der Corput inequality for finite scalar sequences

↑ **Parent:** [Van der Corput lemma (Hilbert space sequences)](#van-der-corput-lemma-hilbert-space-sequences)

For complex numbers $|u_n|\leq1$, $0\leq n<N$, and $1\leq H\leq N$, put $C_h=\sum_{n=0}^{N-h-1}u_{n+h}\overline{u_n}$. Then

$$
\left|\frac1N\sum_{n=0}^{N-1}u_n\right|^2
\leq\frac{N+H-1}{NH}\left(1+2\sum_{h=1}^{H-1}\left(1-\frac hH\right)\frac{|C_h|}{N}\right).
$$

Extend the sequence by zero, count each summand in $H$ consecutive windows, and apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to their sum. Expansion of the squared window sums gives the stated coefficients. Fixing $H$ and making each normalized correlation tend to zero bounds the limiting squared average by $1/H$; then let $H$ tend to infinity. This is the scalar finite form underlying the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences).

### Equidistributed sequence

↑ **Parent:** [Ergodic theory](#ergodic-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Equidistributed_sequence)

A sequence $(x_n)$ in $\mathbb R/\mathbb Z$ is equidistributed if the limiting frequency in every half-open interval equals that interval's length. Equivalently, its empirical probability measures converge to normalized [Lebesgue measure](#lebesgue-measure) when tested against every continuous function.

#### Equidistribution criterion for a torus translation

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

The sequence $r(u,v)$ is equidistributed in $\mathbb T^2$ precisely when $ku+\ell v\notin2\pi\mathbb Z$ for every nonzero integer pair $(k,\ell)$. Equivalently $1,u/(2\pi),v/(2\pi)$ are rationally independent. Under that condition, nonconstant character averages tend to zero by the geometric-series formula. Uniform approximation by [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) gives convergence for continuous functions, and continuous upper and lower bounds give convergence for rectangles. If a character is resonant, the orbit lies in its proper closed kernel and misses a positive-area rectangle, so equidistribution fails.

#### Interval discrepancy

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

Interval discrepancy measures the difference between empirical counts and the expected count for normalized [Lebesgue measure](#lebesgue-measure). Convolving an enlarged interval [indicator function](#indicator-function) with a narrow unit-integral [indicator function](#indicator-function) gives a continuous majorant. Its [Fourier coefficients](fourier-series.md#fourier-coefficient) decay as $O(1/(\delta k^2))$, converting the count into a constant term, finite exponential sums and a controlled absolute tail.

#### Weyl criterion

↑ **Parent:** [Equidistributed sequence](#equidistributed-sequence)

A sequence $(x_n)$ in $\mathbb R/\mathbb Z$ is an [equidistributed sequence](#equidistributed-sequence) if and only if $N^{-1}\sum_{n=0}^{N-1}e^{2\pi i m x_n}\to0$ for every nonzero integer $m$. Approximation of continuous functions by [trigonometric polynomials](fourier-series.md#trigonometric-polynomial) proves the criterion.

##### Differencing obstruction to equidistribution

↑ **Parent:** [Weyl criterion](#weyl-criterion)

If a circle-valued sequence is not an [equidistributed sequence](#equidistributed-sequence), some positive-shift difference is not equidistributed either. The contrapositive follows by applying the [Van der Corput inequality for finite scalar sequences](#van-der-corput-inequality-for-finite-scalar-sequences) to every nonzero integer [exponential sum](analytic-number-theory.md#exponential-sum). Thus cancellation for all fixed nonzero differences implies [equidistribution](#equidistributed-sequence) of the original sequence.

##### Equidistribution of a quadratic polynomial with irrational leading coefficient

↑ **Parent:** [Weyl criterion](#weyl-criterion)

If $a$ is irrational and $b,c$ are real, the fractional parts of $an^2+bn+c$ form an [equidistributed sequence](#equidistributed-sequence). In the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences), every nonzero-lag correlation of $e^{2\pi im(an^2+bn+c)}$ is a [geometric series](real-analysis.md#geometric-series) with irrational frequency $2mah$ and tends to zero. The [Weyl criterion](#weyl-criterion) then applies.

###### Uniform square recurrence on the circle

↑ **Parent:** [Equidistribution of a quadratic polynomial with irrational leading coefficient](#equidistribution-of-a-quadratic-polynomial-with-irrational-leading-coefficient)

For rational $a$, a multiple of its denominator gives exact integer recurrence. For irrational $a$, [Weyl differencing](analytic-number-theory.md#weyl-differencing) and the [Weyl criterion](#weyl-criterion) give an [equidistributed sequence](#equidistributed-sequence) $am^2$ modulo one. Thus every parameter belongs to one of the open sets $\{a:\|am^2\|<\epsilon\}$. Compactness of the [circle group](lie-theory.md#circle-group) gives a finite subcover, hence a bound $N$ uniform in $a$; no explicit rate follows from this compactness step.

### Nonsingular transformation

↑ **Parent:** [Ergodic theory](#ergodic-theory)

A measurable transformation $T:X\to X$ is nonsingular with respect to $\mu$ when $\mu(T^{-1}N)=0$ for every $\mu$-null set $N$, equivalently when the [pushforward measure](#pushforward-measure) $T_*\mu$ is [absolutely continuous](#absolute-continuity-of-measures) with respect to $\mu$.

### Koopman operator

↑ **Parent:** [Ergodic theory](#ergodic-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Koopman_operator)

For a measurable dynamical map $F$, the Koopman operator acts on observables by $K_Fg=g\circ F$. If $F$ is nonsingular, it defines an operator on equivalence classes of measurable functions.

#### Spectral measure of a Koopman observable

↑ **Parent:** [Koopman operator](#koopman-operator)

The finite positive measure representing an observable's autocorrelation sequence by the [Bochner–Herglotz theorem](analysis.md#bochner-herglotz-theorem). For a probability [measure-preserving system](#measure-preserving-system), the [Koopman operator](#koopman-operator) is an [isometry](riemannian-geometry.md#isometry), so its forward autocorrelations, extended by complex conjugation to negative indices, form a [positive-definite function](analysis.md#positive-definite-function) on $\mathbb Z$. The measure has mass $\|f\|_2^2$, and its atoms are squared norms of projections onto [Koopman operator](#koopman-operator) eigenspaces, including for noninvertible transformations.

#### Almost periodic observable

↑ **Parent:** [Koopman operator](#koopman-operator)

An $L^2$ observable of an invertible probability [measure-preserving system](#measure-preserving-system) is almost periodic when its [Koopman operator](#koopman-operator) orbit is totally bounded in the global $L^2$ norm. A noninvertible system uses its forward orbit. This is the Hilbert-space dynamical definition, distinguished from uniform almost periodicity for continuous functions of a real variable.

##### Syndetic near returns of an almost periodic observable

↑ **Parent:** [Almost periodic observable](#almost-periodic-observable)

If the forward orbit of $f$ under an [isometry](riemannian-geometry.md#isometry) $U$ is totally bounded, choose a finite net whose centers are $U^{n_j}f$ and let $M=\max_jn_j$. For every sufficiently large $n$, some center is within $\varepsilon$ of $U^nf$, so cancellation gives $n-n_j\in R_\varepsilon$. Thus $R_\varepsilon$ is a [syndetic set](dynamical-systems.md#syndetic-set). Telescoping also gives $\|U^{kn}f-f\|_2\leq k\|U^nf-f\|_2$.

##### Compact measure-preserving system

↑ **Parent:** [Almost periodic observable](#almost-periodic-observable)

A probability [measure-preserving system](#measure-preserving-system) is compact if every $L^2$ observable has a relatively compact [Koopman operator](#koopman-operator) orbit in the global $L^2$ norm. For an invertible system one may use all integer times; for a general transformation use nonnegative times. This is a measure-theoretic definition, stronger than compactness of the underlying topological space.

#### Decay of autocorrelation implies weak convergence of an observable

↑ **Parent:** [Koopman operator](#koopman-operator)

For a probability [measure-preserving system](#measure-preserving-system), if $\langle U_T^nf,f\rangle\to|\int f\,d\mu|^2$, then $U_T^nf$ converges weakly in $L^2$ to $(\int f\,d\mu)\mathbf1$. Centre $v=f-(\int f)\mathbf1$; its autocorrelations tend to zero. The [isometry](riemannian-geometry.md#isometry) identity gives the same decay against each $U_T^kv$, hence by approximation against their closed forward span. Against its orthogonal complement the correlations are exactly zero. [Orthogonal decomposition by a closed subspace](hilbert-space.md#orthogonal-decomposition-by-a-closed-subspace) finishes the proof without invertibility.

#### Bounded Koopman operator criterion

↑ **Parent:** [Koopman operator](#koopman-operator)

For a nonsingular map $F$ on a probability space, $K_F$ extends boundedly to $L^2$ exactly when $d(F_*\mu)/d\mu\in L^\infty$. In that case

$$
\|K_F\|^2=\left\|\frac{d(F_*\mu)}{d\mu}\right\|_\infty.
$$

### Measure-preserving transformation

↑ **Parent:** [Ergodic theory](#ergodic-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measure-preserving_transformation)

A measurable transformation $T:X\to X$ preserves a measure $\mu$ when $\mu(T^{-1}A)=\mu(A)$ for every measurable set $A$.

#### Lebesgue-measure-preserving map

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

Such a measurable self-map preserves [Lebesgue measure](#lebesgue-measure). On the unit interval examples include the identity, reflection $t\mapsto1-t$, and $t\mapsto2t\pmod1$. Invertibility is not required.

#### Integer multiplication map on the circle

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

For an integer $K\geq2$, multiplication by $K$ on the [circle group](lie-theory.md#circle-group) preserves normalized [Lebesgue measure](#lebesgue-measure). Each inverse image consists of $K$ branches, each scaling lengths by $1/K$.

##### Ergodicity of integer multiplication on the circle

↑ **Parent:** [Integer multiplication map on the circle](#integer-multiplication-map-on-the-circle)

The [integer multiplication map on the circle](#integer-multiplication-map-on-the-circle) is an [ergodic transformation](#ergodicity) for [Lebesgue measure](#lebesgue-measure). In the [Fourier basis](fourier-series.md#fourier-basis), an invariant function has coefficients $c_j=0$ when $K$ does not divide $j$, and $c_j=c_{j/K}$ otherwise. Every nonzero index eventually reduces to the first case, so only the constant coefficient remains.

#### Measure-preserving system

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

A measure-preserving system is a measure space $(X,\mathcal B,\mu)$ together with a [measure-preserving transformation](#measure-preserving-transformation) $T$. In ergodic theory the measure is commonly a probability measure.

##### Factor of a measure-preserving system

↑ **Parent:** [Measure-preserving system](#measure-preserving-system)

A factor map $\pi$ is a measurable map satisfying $\pi\circ T=S\circ\pi$ and $\pi_*\mu=\nu$, from one [measure-preserving system](#measure-preserving-system) to another. The target system is the factor; its observable functions pull back to observable functions of the source.

###### Factor map between measure-preserving systems

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

Approximate $\mathbf1_A$ by relative almost periodic functions with summable squared global errors. [Tonelli theorem](#tonelli-theorem) makes their conditional errors tend to zero almost everywhere. Choose a positive base set on which the conditional mass of $A$ is bounded below, then use the [Egorov theorem](real-analysis.md#egorov-s-theorem) to make those errors uniform on a smaller positive set $C$. [Localization of relative almost periodicity to base sets](#localization-of-relative-almost-periodicity-to-base-sets) and conditional-norm closure prove $\mathbf1_B$ is relatively almost periodic and $\mu(B)>0$.

###### Relatively almost periodic observable

↑ **Parent:** [Factor map between measure-preserving systems](#factor-map-between-measure-preserving-systems)

For every positive $\varepsilon$, require finitely many global $L^2$ centers $g_j$ such that the displayed inequality holds for every integer $n$ on almost every fiber of the [factor map](#factor-map-between-measure-preserving-systems). A center can depend on the fiber and time; its finite list is fixed. This is weaker than [almost periodic observable](#almost-periodic-observable) in global norm. For noninvertible systems use nonnegative times.

###### Localization of relative almost periodicity to base sets

↑ **Parent:** [Relatively almost periodic observable](#relatively-almost-periodic-observable)

Multiplying a [relatively almost periodic observable](#relatively-almost-periodic-observable) by a base-set indicator preserves [relative almost periodicity](#relatively-almost-periodic-observable): on each fiber an orbit value is either unchanged or zero, so add zero to the finite list of centers. [Conditional norm covariance under a factor map](#conditional-norm-covariance-under-a-factor-map) also proves closure under convergence in the [uniform conditional L2 norm](#uniform-conditional-l2-norm).

#### Finite full-support measure-preserving map is bijective

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

Let $X$ be a [finite set](set.md#finite-set), let every singleton have positive probability, and let $T:X\to X$ preserve that probability measure. For every $x\in X$,

$$
\mu(T^{-1}\{x\})=\mu(\{x\})>0,
$$

so every $x$ has a preimage. Thus $T$ is a [surjection](algebra.md#surjective-function), and every surjection from a finite set to itself is a [bijection](function.md#bijection).

#### Invertible measure-preserving system

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

An invertible measure-preserving system has a measurable inverse modulo null sets and preserves its measure in both time directions. Its [Koopman operator](#koopman-operator) on $L^2$ is unitary.

#### Invariant sigma-algebra

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)

The invariant sigma-algebra of $T$ consists, modulo null sets, of measurable sets $A$ satisfying $T^{-1}A=A$.

##### Invariant set of a measure-preserving transformation

↑ **Parent:** [Invariant sigma-algebra](#invariant-sigma-algebra)

A measurable set $A$ satisfying $T^{-1}A=A$, or equality modulo null sets in the measure-theoretic convention. These sets form a $\sigma$-algebra, and an [ergodic measure-preserving transformation](#ergodicity) gives each invariant set probability zero or one.

#### Ergodicity

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ergodicity)

A [measure-preserving transformation](#measure-preserving-transformation) is ergodic when every set in its [invariant sigma-algebra](#invariant-sigma-algebra) has measure zero or full measure. Equivalently, every integrable invariant function is almost everywhere constant.

##### Strong mixing

↑ **Parent:** [Ergodicity](#ergodicity)

A probability [measure-preserving transformation](#measure-preserving-transformation) is strongly mixing when $\mu(T^{-n}A\cap B)\to\mu(A)\mu(B)$ for every pair of measurable sets $A,B$. Unlike weak mixing, this is an ordinary limit along all sufficiently large times.

###### Diagonal set-correlation criterion for mixing

↑ **Parent:** [Strong mixing](#strong-mixing)

A probability [measure-preserving transformation](#measure-preserving-transformation) is [strong mixing](#strong-mixing) exactly when $\mu(T^{-n}A\cap A)\to\mu(A)^2$ for every measurable $A$. The converse follows by applying [decay of autocorrelation implies weak convergence of an observable](#decay-of-autocorrelation-implies-weak-convergence-of-an-observable) to $f=\mathbf1_A$ and then testing against $\mathbf1_B$. Diagonal polarization alone controls a sum of the two directed cross-correlations and does not suffice as a proof.

##### Ergodic decomposition

↑ **Parent:** [Ergodicity](#ergodicity)

For a [measure-preserving system](#measure-preserving-system) on a standard probability space, an invariant probability measure is an integral of ergodic invariant probability measures. Its conditional measures given the [invariant sigma-algebra](#invariant-sigma-algebra) are the ergodic components.

###### Ergodic components of a rational circle rotation

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

For rotation by $p/q$ with coprime integers and Haar probability on the circle, components are the equal measures on the $q$-point orbits. The quotient map is $x\mapsto qx\pmod1$. Integration over the quotient recovers Haar measure, and the rotation permutes each orbit transitively, making its [probability measure](probability-theory.md#probability-measure) [ergodic](#ergodicity).

###### Ergodic component

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

A conditional probability of an invariant [probability measure](probability-theory.md#probability-measure) given its [invariant sigma-algebra](#invariant-sigma-algebra). In a standard Borel probability system, almost every such probability is invariant and [ergodic](#ergodicity). Their integral recovers the original measure. The [countable-test proof of ergodicity of conditional components](#countable-test-proof-of-ergodicity-of-conditional-components) explains why invariance alone is not the whole conclusion.

###### Countable-test proof of ergodicity of conditional components

↑ **Parent:** [Ergodic component](#ergodic-component)

Apply the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) to a countable generating algebra, and disintegrate the resulting common full-measure convergence set over the [invariant sigma-algebra](#invariant-sigma-algebra). The orbit limits on a fiber are its conditional masses. Applying the theorem to that invariant component shows its invariant projection is constant on all generating indicators, hence on all $L^2$ functions by density. This proves [ergodicity](#ergodicity) without an uncountable intersection of null sets.

###### Affinity of entropy under ergodic decomposition

↑ **Parent:** [Ergodic decomposition](#ergodic-decomposition)

If $\mu=\int\nu\,d\tau(\nu)$ is an [ergodic decomposition](#ergodic-decomposition), then the [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy) satisfies $h_\mu(T)=\int h_\nu(T)\,d\tau(\nu)$.

##### Ergodic invariant probability on a countable state space has finite cyclic support

↑ **Parent:** [Ergodicity](#ergodicity)

Let $T$ be an [ergodic transformation](#ergodicity) preserving a probability measure $\mu$ on a [countable set](set-theory.md#countable-set). Some state $x$ has $\mu(\{x\})>0$. Along its forward orbit,

$$
\mu(\{T^{n+1}x\})
=\mu(T^{-1}\{T^{n+1}x\})
\geq\mu(\{T^nx\}).
$$

An infinite sequence of distinct states with masses bounded below by $\mu(\{x\})$ is impossible, so the orbit eventually reaches a finite cycle $Y$. Since $Y\subseteq T^{-1}Y$ and invariance gives $\mu(T^{-1}Y)=\mu(Y)>0$, the difference is null. The cycle is invariant modulo null sets, and ergodicity therefore gives $\mu(Y)=1$.

##### Invariant-function characterization of ergodicity

↑ **Parent:** [Ergodicity](#ergodicity)

An invertible measure-preserving system is ergodic exactly when the fixed space of its [Koopman operator](#koopman-operator) on $L^2$ consists only of almost-everywhere constant functions. One direction applies invariance to level sets; the other applies it to indicator functions of invariant sets.

##### Bernoulli shift

↑ **Parent:** [Ergodicity](#ergodicity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_shift)

On a one-sided sequence space $E^{\mathbb N}$ with [product measure](probability-theory.md#product-measure), the Bernoulli shift is

$$
S(x_0,x_1,x_2,\ldots)=(x_1,x_2,x_3,\ldots).
$$

It preserves the product measure. Every invariant event lies in the [tail sigma-algebra](probability-theory.md#tail-sigma-algebra) of the coordinate process, so the [Kolmogorov zero-one law](probability-theory.md#kolmogorov-s-zero-one-law) makes the shift an [ergodic transformation](#ergodicity).

###### Bernoulli coordinate observable is not almost periodic

↑ **Parent:** [Bernoulli shift](#bernoulli-shift)

For independent fair signs on a two-sided [Bernoulli shift](#bernoulli-shift), the coordinate observable $f(y)=y_0$ has unit norm and pairwise orthogonal orbit values. Their pairwise squared distance is two, excluding a finite small net in global $L^2$. Its pullback along a [factor map](#factor-map-between-measure-preserving-systems) can nevertheless be a [relatively almost periodic observable](#relatively-almost-periodic-observable), since it is fiber-constant and takes only two values.

###### Cantor Bernoulli measure

↑ **Parent:** [Bernoulli shift](#bernoulli-shift)

The law of $\sum_{j\geq1}2\omega_j3^{-j}$, for independent fair binary digits $\omega_j$, is supported on the [Cantor set](geometry-and-topology.md#cantor-set). It is invariant and ergodic under $T_3$, as the image of a [Bernoulli shift](#bernoulli-shift). Each permitted ternary cylinder of length $n$ has measure $2^{-n}$, giving entropy rate $\log2$. The [Host equidistribution theorem](#host-equidistribution-theorem) makes almost every point a [normal number](number-theory.md#normal-number) in base $2$, while its ternary digits omit $1$.

##### Irrational rotation

↑ **Parent:** [Ergodicity](#ergodicity)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Irrational_rotation)

For irrational $\alpha$, the circle rotation $T(x)=x+\alpha\pmod1$ preserves [Lebesgue measure](#lebesgue-measure) and is an [ergodic transformation](#ergodicity).

###### Ergodicity criterion for a circle rotation

↑ **Parent:** [Irrational rotation](#irrational-rotation)

The rotation $x\mapsto x+a$ of a circle of circumference $2\pi$ is ergodic exactly when $a/\pi$ is irrational. In the [Fourier basis](fourier-series.md#fourier-basis), an invariant function can have a nonzero $k$th coefficient only when $e^{ika}=1$.

###### Everywhere interval frequency under an irrational rotation

↑ **Parent:** [Irrational rotation](#irrational-rotation)

Every orbit of an [irrational rotation of the circle](#irrational-rotation) visits a half-open interval $I$ with limiting frequency equal to its length. One proof sandwiches the orbit of an arbitrary point between inner and outer intervals along a nearby orbit for which the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) holds.

##### Weakly mixing measure-preserving transformation

↑ **Parent:** [Ergodicity](#ergodicity)

A probability [measure-preserving transformation](#measure-preserving-transformation) $T$ is weakly mixing when, for every pair of measurable sets $A,B$, the average absolute correlation discrepancy tends to zero:

$$
\frac1N\sum_{n=0}^{N-1}|\mu(T^{-n}A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Equivalently, the correlations converge to their products in [convergence in density of a sequence](#convergence-in-density-of-a-sequence), its [Cartesian product](set-theory.md#cartesian-product) with itself is an [ergodic transformation](#ergodicity), or its product with every [ergodic transformation](#ergodicity) is ergodic. The absolute values are essential: signed [Cesaro convergence of a sequence](#cesaro-convergence-of-a-sequence) of the correlations to their products characterizes [ergodic transformations](#ergodicity) and does not imply weak mixing. For example, the transformation interchanging two equally weighted points has discrepancy $(-1)^n/4$ for a singleton $A=B$: its signed average tends to zero while its average absolute discrepancy stays $1/4$.

###### Arithmetic-progression multiple averages under weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

For bounded observables of a probability [weak mixing](#weakly-mixing-measure-preserving-transformation) system, the displayed convergence holds in $L^2$. Induct on $k$: center the final observable, compute the lagged Hilbert-space correlations, apply the induction hypothesis to the $k-1$ remaining factors, and use [weak mixing](#weakly-mixing-measure-preserving-transformation) of $T^k$ with the [Van der Corput lemma](#van-der-corput-lemma-hilbert-space-sequences) to obtain zero. Adding back the final mean completes the induction.

###### Density convergence of multiple weak-mixing correlations

↑ **Parent:** [Arithmetic-progression multiple averages under weak mixing](#arithmetic-progression-multiple-averages-under-weak-mixing)

For real bounded observables, the [Cesaro limit](#cesaro-convergence-of-a-sequence) of the correlation comes from [arithmetic-progression multiple averages under weak mixing](#arithmetic-progression-multiple-averages-under-weak-mixing). Apply the same result on the weakly mixing product system to $f_j\otimes f_j$ to obtain its second moment. The averaged squared error tends to zero, so the [mean-square criterion for convergence in density](#mean-square-criterion-for-convergence-in-density) gives the displayed density limit.

###### Stability of weak mixing under powers and products

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

Every positive power of a [weak mixing](#weakly-mixing-measure-preserving-transformation) transformation is weakly mixing: its nonnegative discrepancies are a subsequence whose average is bounded by $r$ times the full average. Products are weakly mixing because correlations of simple tensors factor; the absolute product discrepancy is bounded by the sum of bounded multiples of the single-system discrepancies. Density of finite tensor sums gives the full $L^2$ assertion.

###### Product characterization of weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

If $T$ is weakly mixing, then $T\times S$ is ergodic exactly when $S$ is ergodic. In particular, ergodicity of $T\times T$ is equivalent to weak mixing of $T$.

###### Square-correlation proof of weak mixing from product ergodicity

↑ **Parent:** [Product characterization of weak mixing](#product-characterization-of-weak-mixing)

For mean-zero $f$, apply the [mean ergodic theorem](vector-space.md#von-neumann-mean-ergodic-theorem) on an ergodic product system to $f\otimes\overline f$, paired with $g\otimes\overline g$. Its correlation is $|\langle U^nf,g\rangle|^2$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) then gives averaged absolute correlation decay, the definition of [weak mixing](#weakly-mixing-measure-preserving-transformation).

###### Koopman eigenfunction obstruction to weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

A weakly mixing system has no nonconstant [Koopman operator](#koopman-operator) eigenfunction. If $U_Tf=\lambda f$, then $f(x)\overline{f(y)}$ is invariant under $T\times T$, contradicting the [product characterization of weak mixing](#product-characterization-of-weak-mixing) unless $f$ is constant.

###### Simultaneous hitting characterization of weak mixing

↑ **Parent:** [Weakly mixing measure-preserving transformation](#weakly-mixing-measure-preserving-transformation)

A system is weakly mixing exactly when, for every positive-measure $A,B,C$, some $n\geq1$ makes both $T^{-n}A\cap B$ and $T^{-n}A\cap C$ have positive measure. This is the finite simultaneous-hitting form of the density-one correlation characterization.

<h4 id="poincare-recurrence-theorem">Poincaré recurrence theorem</h4>

↑ **Parent:** [Measure-preserving transformation](#measure-preserving-transformation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Poincaré_recurrence_theorem)

In a finite [measure-preserving system](#measure-preserving-system), almost every point of every measurable set $A$ returns to $A$ infinitely often. The points of $A$ that never return form a wandering set: all its inverse images are pairwise disjoint and have equal measure, so that set must be null.

##### Furstenberg multiple recurrence theorem

↑ **Parent:** [Poincaré recurrence theorem](#poincare-recurrence-theorem)

For a probability [measure-preserving system](#measure-preserving-system), every measurable $B$ of positive measure and every integer $k\geq2$ admit an integer $n\geq1$ with $\mu(\bigcap_{j=0}^{k-1}T^{-jn}B)>0$. The sets are preimages; neither invertibility nor an [ergodic transformation](#ergodicity) is required. The [Furstenberg correspondence principle](#furstenberg-correspondence-principle) converts this simultaneous return into [arithmetic progressions](arithmetic.md#arithmetic-progression) and yields the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem). The case $k=2$ follows from the [Poincaré recurrence theorem](#poincare-recurrence-theorem).

###### SZ property

↑ **Parent:** [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem)

A probability [measure-preserving system](#measure-preserving-system) has the SZ property at level $k$ if the displayed lower limit is positive for every measurable set $A$ of positive measure. This convention counts $k$ nonzero shifts, hence progressions of length $k+1$. The [Furstenberg correspondence principle](#furstenberg-correspondence-principle) turns this property at all levels into the [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem). A [compact measure-preserving system](#compact-measure-preserving-system) has the property because [syndetic near returns of an almost periodic observable](#syndetic-near-returns-of-an-almost-periodic-observable) applied to an indicator give uniformly positive multiple intersections at bounded-gap times.

###### Multiple recurrence for circle rotations

↑ **Parent:** [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem)

Every circle rotation has the [Furstenberg multiple recurrence theorem](#furstenberg-multiple-recurrence-theorem) property for normalized [Lebesgue measure](#lebesgue-measure). For a rational angle, use a period. For an irrational angle, choose a positive return time with angle close to zero; [translation continuity in L1 on the circle](#translation-continuity-in-l1-on-the-circle) then makes finitely many translates of a given positive-measure set simultaneously close to that set, and the [union bound](probability-inequality.md#boole-s-inequality) leaves a positive-measure intersection.

### Birkhoff ergodic theorem

↑ **Parent:** [Ergodic theory](#ergodic-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Birkhoff_ergodic_theorem)

For a [measure-preserving transformation](#measure-preserving-transformation) $T$ and $f\in L^1(\mu)$, the ergodic averages

$$
A_nf=\frac1n\sum_{j=0}^{n-1}f\circ T^j
$$

converge almost everywhere to $\mathbb E[f\mid\mathcal I]$, the [conditional expectation](#conditional-expectation) on the [invariant sigma-algebra](#invariant-sigma-algebra). The limit has the same integral as $f$.

#### Nonnegative ergodic averages with infinite integral

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

In a probability [measure-preserving system](#measure-preserving-system) whose transformation is an [ergodic transformation](#ergodicity), a nonnegative measurable $f$ with $\int f\,d\mu=+\infty$ has $N^{-1}\sum_{j=0}^{N-1}f(T^jx)\to+\infty$ [almost everywhere](#almost-everywhere). Apply the [pointwise ergodic theorem](#birkhoff-ergodic-theorem) to $\min(f,K)$ on a common full-measure set for integer $K$, then bound the lower limit by each truncated integral. The [monotone convergence theorem](#monotone-convergence-theorem) sends those integrals to infinity. The finite-integral case is the ordinary [pointwise ergodic theorem](#birkhoff-ergodic-theorem).

#### Maximal ergodic lemma

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

For a [measure-preserving transformation](#measure-preserving-transformation) and real integrable $f$, let $S_kf=\sum_{j<k}f\circ T^j$. For $E_N=\{\max_{1\leq k\leq N}S_kf>0\}$ the lemma asserts $\int_{E_N}f\,d\mu\geq0$. Passing to the increasing [union](set.md#set-union) gives the corresponding infinite-supremum inequality.

#### Triangular ergodic averaging lemma

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

Suppose $f_k\to f$ [almost everywhere](#almost-everywhere) and $\sup_k|f_k|\in L^1$ in a probability [measure-preserving system](#measure-preserving-system). Then

$$
\frac1n\sum_{j=0}^{n-1}f_{n-1-j}(T^jx)
\longrightarrow\mathbb E[f\mid\mathcal I]
$$

[almost everywhere](#almost-everywhere) and in $L^1$, where $\mathcal I$ is the [invariant sigma-algebra](#invariant-sigma-algebra). For the almost-everywhere assertion, bound the terms with index at least $M$ by $\sup_{k\geq M}|f_k-f|$, apply the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem), and then let $M\to\infty$. The finitely many remaining end terms vanish by the [linear growth bound for integrable observables](#linear-growth-bound-for-integrable-observables).

#### Linear growth bound for integrable observables

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

In a probability [measure-preserving system](#measure-preserving-system), $f\in L^1$ implies $f(T^nx)/n\to0$ [almost everywhere](#almost-everywhere). For every $\varepsilon>0$, the [tail integral formula for moments](probability-theory.md#tail-integral-formula-for-moments) gives $\sum_{n\geq1}\mu(|f|>\varepsilon n)\leq\|f\|_1/\varepsilon$. Invariance and the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) finish the proof. Consequently division by $n^a$ also gives zero for every $a\geq1$.

##### Sharpness of the linear growth bound for integrable observables

↑ **Parent:** [Linear growth bound for integrable observables](#linear-growth-bound-for-integrable-observables)

For every $0<a<1$, choose $1<p<1/a$. On the [Bernoulli shift](#bernoulli-shift) over independent uniform coordinates in $(0,1)$, the observable $f(x)=x_0^{-1/p}$ is integrable, but $\mu(f(T^nx)>n^a)=n^{-ap}$. The events are independent and their probabilities have divergent sum, so the [Borel-Cantelli lemma](probability-theory.md#borel-cantelli-lemmas) implies that $f(T^nx)/n^a>1$ infinitely often [almost surely](convergence-of-random-variables.md#almost-sure-convergence). No exponent below one gives a universal bound for all integrable observables.

#### L1 convergence in the Birkhoff ergodic theorem on a finite measure space

↑ **Parent:** [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem)

On a [finite measure](#finite-measure) space, the convergence in the [Birkhoff ergodic theorem](#birkhoff-ergodic-theorem) also holds in $L^1$. Prove it first for bounded truncations by the [dominated convergence theorem](#dominated-convergence-theorem), then use the $L^1$ contraction $\|A_nh\|_1\leq\|h\|_1$ and [Fatou lemma](#fatou-s-lemma) to remove the truncation.

### Upper Banach density

↑ **Parent:** [Ergodic theory](#ergodic-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Upper_Banach_density)

For $S\subseteq\mathbb Z$, its upper Banach density is

$$
d^*(S)=\limsup_{N\to\infty}\sup_{m\in\mathbb Z}\frac{|S\cap[m,m+N-1]|}{N}.
$$

#### Furstenberg correspondence principle

↑ **Parent:** [Upper Banach density](#upper-banach-density)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Furstenberg_correspondence_principle)

The Furstenberg correspondence principle turns a subset $S\subseteq\mathbb Z$ of positive [upper Banach density](#upper-banach-density) into a shift-invariant probability system and a positive-measure cylinder $A$ such that recurrence times of $A$ produce differences of elements of $S$.

### Convergence in density of a sequence

↑ **Parent:** [Ergodic theory](#ergodic-theory)

A sequence $a_n$ converges in density to $a$ when, for every $\varepsilon>0$,

$$
\frac1N\left|\{1\leq n\leq N:|a_n-a|\geq\varepsilon\}\right|\longrightarrow0.
$$

#### Mean-square criterion for convergence in density

↑ **Parent:** [Convergence in density of a sequence](#convergence-in-density-of-a-sequence)

The displayed condition implies [convergence in density of a sequence](#convergence-in-density-of-a-sequence) to $\ell$, since the fraction of indices with $|a_n-\ell|\geq\varepsilon$ is at most $\varepsilon^{-2}$ times the averaged squared error. A signed [Cesaro limit](#cesaro-convergence-of-a-sequence) alone is insufficient: $a_n=(-1)^n$ has zero signed average but no density limit.

#### Cesaro convergence of a sequence

↑ **Parent:** [Convergence in density of a sequence](#convergence-in-density-of-a-sequence)

A sequence $a_n$ converges in the Cesaro sense to $a$ when $N^{-1}\sum_{n=1}^Na_n\to a$. For bounded sequences, convergence in density to $a$ is equivalent to Cesaro convergence of $|a_n-a|$ to zero.

### Entropy of a finite measurable partition

↑ **Parent:** [Ergodic theory](#ergodic-theory)

For a finite measurable partition $\xi$, its entropy is

$$
H_\mu(\xi)=-\sum_{A\in\xi}\mu(A)\log\mu(A),
$$

with $0\log0=0$.

#### Conditional entropy of finite measurable partitions

↑ **Parent:** [Entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition)

For finite partitions $\xi,\eta$,

$$
H_\mu(\xi\mid\eta)
=\sum_{B\in\eta}\mu(B)H_\mu(\xi\mid B)
=H_\mu(\xi\vee\eta)-H_\mu(\eta).
$$

[Conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy), so $H_\mu(\xi\mid\eta)\leq H_\mu(\xi)$.

#### Entropy rate of a measurable partition

↑ **Parent:** [Entropy of a finite measurable partition](#entropy-of-a-finite-measurable-partition)

The entropy rate of $\xi$ is

$$
h_\mu(T,\xi)=\lim_{N\to\infty}\frac1N
H_\mu\left(\bigvee_{n=0}^{N-1}T^{-n}\xi\right).
$$

The numerator is a [subadditive sequence](real-analysis.md#subadditive-sequence), so the limit exists and equals the infimum of the displayed ratios.

##### Infinite-future formula for partition entropy rate

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a finite [measurable partition](#measurable-partition) $\xi$, put $\mathcal F_1=\sigma(\bigvee_{j\ge1}T^{-j}\xi)$. Then $h_\mu(T,\xi)=H_\mu(\xi\mid\mathcal F_1)=\lim_{n\to\infty}H_\mu(\xi\mid\xi_1^n)$. The backward entropy chain rule writes $H_\mu(\xi_0^{N-1})$ as the sum of the first $N$ decreasing finite-future conditional entropies. Their averages have the same limit. Increasing conditioning fields converge by the [martingale convergence theorem](martingale.md#martingale-convergence-theorem).

###### Block conditional entropy given the infinite future

↑ **Parent:** [Infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate)

For $\mathcal F_L=\sigma(\bigvee_{j\ge L}T^{-j}\xi)$ and a finite [measurable partition](#measurable-partition) $\xi$, $H_\mu(\xi_0^{L-1}\mid\mathcal F_L)=Lh_\mu(T,\xi)$. The backward conditional entropy chain rule expresses the left side as $\sum_{j=0}^{L-1}H_\mu(T^{-j}\xi\mid\mathcal F_{j+1})$. Each term equals $h_\mu(T,\xi)$ by measure preservation and the [infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate). No invertibility is needed.

##### Shannon-McMillan-Breiman theorem

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a probability [measure-preserving system](#measure-preserving-system) and a countable [measurable partition](#measurable-partition) $\xi$ of finite entropy, $-n^{-1}\log\mu(\xi_0^{n-1}(x))$ converges [almost everywhere](#almost-everywhere) and in $L^1$ to an invariant function whose integral is $h_\mu(T,\xi)$. For an [ergodic transformation](#ergodicity), the limit is the constant $h_\mu(T,\xi)$. In general it is $\mathbb E[I_\mu(\xi\mid\bigvee_{j=1}^\infty T^{-j}\xi)\mid\mathcal I]$. The [martingale convergence theorem](martingale.md#martingale-convergence-theorem), [maximal inequality for conditional information functions](#maximal-inequality-for-conditional-information-functions), and [triangular ergodic averaging lemma](#triangular-ergodic-averaging-lemma) prove this directly, without invertibility.

##### Monotonicity of normalized block entropy

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a stationary process associated with a finite-entropy [measurable partition](#measurable-partition), $H_\mu(\xi_0^{n-1})/n$ is non-increasing. The increments $c_k=H_\mu(\xi\mid\bigvee_{j=1}^kT^{-j}\xi)$ are non-increasing by [conditioning reduces entropy](information-theory.md#conditioning-reduces-entropy), and the chain rule gives $H_\mu(\xi_0^{n-1})=\sum_{k=0}^{n-1}c_k$. Averages of a decreasing sequence are decreasing.

##### Kolmogorov-Sinai entropy

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kolmogorov-Sinai_entropy)

The Kolmogorov-Sinai entropy is $h_\mu(T)=\sup_\xi h_\mu(T,\xi)$ over finite measurable partitions.

###### Completely positive entropy

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

A probability [measure-preserving system](#measure-preserving-system) has completely positive entropy if $h_\mu(T,\xi)>0$ for every finite [measurable partition](#measurable-partition) with $H_\mu(\xi)>0$. Equivalently, its [Pinsker sigma-algebra](#pinsker-sigma-algebra) is trivial. Since [finite partitions measurable in a partition tail have zero entropy rate](#finite-partitions-measurable-in-a-partition-tail-have-zero-entropy-rate), this property forces every finite-partition [tail sigma-algebra of a measurable partition](#tail-sigma-algebra-of-a-measurable-partition) to be trivial.

###### Generating measurable partition

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

For an invertible [measure-preserving system](#measure-preserving-system), a generating measurable partition $\xi$ has $\sigma(\bigvee_{j\in\mathbb Z}T^{-j}\xi)=\mathcal B$ modulo null sets. Thus knowing the entire two-sided itinerary determines all measurable observations. A finite or countable finite-entropy generating partition computes the system entropy through the [Kolmogorov-Sinai generator theorem](#kolmogorov-sinai-generator-theorem).

###### One-sided generator

↑ **Parent:** [Generating measurable partition](#generating-measurable-partition)

A one-sided generator is a [measurable partition](#measurable-partition) $\xi$ with $\sigma(\bigvee_{j\ge0}T^{-j}\xi)=\mathcal B$ modulo null sets. Equivalently, every measurable set can be approximated in measure by unions of atoms of finite forward-name blocks. A one-sided coordinate partition generates a one-sided [Bernoulli shift](#bernoulli-shift); for a nontrivial base distribution, it does not generate the two-sided version, whose negative coordinates are independent of the nonnegative ones.

###### Finite one-sided generator of an invertible system forces zero entropy

↑ **Parent:** [One-sided generator](#one-sided-generator)

If an invertible probability [measure-preserving system](#measure-preserving-system) has a finite [one-sided generator](#one-sided-generator) $\xi$, then its future sigma-algebra $\mathcal F_1=T^{-1}\mathcal B$ equals $\mathcal B$ modulo null sets. Hence $H_\mu(\xi\mid\mathcal F_1)=0$, and the [infinite-future formula for partition entropy rate](#infinite-future-formula-for-partition-entropy-rate) and [Kolmogorov-Sinai generator theorem](#kolmogorov-sinai-generator-theorem) give $h_\mu(T)=0$. Invertibility matters: a fair binary one-sided [Bernoulli shift](#bernoulli-shift) has entropy $\log2$ and a finite one-sided generator.

###### Kolmogorov-Sinai generator theorem

↑ **Parent:** [Generating measurable partition](#generating-measurable-partition)

For an invertible probability [measure-preserving system](#measure-preserving-system) with a finite or countable finite-entropy [generating measurable partition](#generating-measurable-partition) $\xi$, $h_\mu(T)=h_\mu(T,\xi)$. For a noninvertible system the same conclusion holds for a finite-entropy [one-sided generator](#one-sided-generator). The finite-entropy hypothesis is part of this form of the theorem.

###### Host equidistribution theorem

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

Let $p,q\geq2$ be relatively prime integers. If $\nu$ is invariant and ergodic for the [integer multiplication map on the circle](#integer-multiplication-map-on-the-circle) $T_p$ and $h_\nu(T_p)>0$, then for $\nu$-almost every $x$ the sequence $(T_q^nx)$ is an [equidistributed sequence](#equidistributed-sequence) for [Lebesgue measure](#lebesgue-measure). For a non-ergodic $T_p$ invariant measure, the same conclusion holds if almost every measure in its [ergodic decomposition](#ergodic-decomposition) has positive entropy. Positive entropy of the whole measure alone does not suffice.

###### Rudolph measure rigidity theorem

↑ **Parent:** [Host equidistribution theorem](#host-equidistribution-theorem)

A probability measure on the circle invariant under $T_2$ and $T_3$ and ergodic for their jointly generated semigroup is [Lebesgue measure](#lebesgue-measure) if either transformation has positive [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy). Without joint ergodicity, a mixture of [Lebesgue measure](#lebesgue-measure) and an atomic invariant measure shows why positive entropy alone is insufficient.

###### Entropy preservation under a finite-to-one factor

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

For standard probability systems, a [factor of a measure-preserving system](#factor-of-a-measure-preserving-system) with at most $q$ points in every fibre preserves [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy). Conditional on the complete factor point, every finite orbit name has at most $q$ possibilities, so its conditional entropy is at most $\log q$. Dividing by the orbit length gives zero relative entropy.

###### Pinsker sigma-algebra

↑ **Parent:** [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy)

The Pinsker sigma-algebra consists of the measurable sets $A$ whose binary partition $\{A,X\setminus A\}$ has entropy rate zero. It is a sigma-algebra and is the largest invariant factor with zero [Kolmogorov-Sinai entropy](#kolmogorov-sinai-entropy).

###### Tail characterization of the Pinsker sigma-algebra

↑ **Parent:** [Pinsker sigma-algebra](#pinsker-sigma-algebra)

A set belongs to the [Pinsker sigma-algebra](#pinsker-sigma-algebra) exactly when, modulo a null set, it belongs to $\mathcal T(\xi)$ for some finite measurable partition $\xi$. For a zero-entropy binary partition one may take that partition itself: zero conditional entropy makes its present atom measurable from every remote future.

##### Infimum rule for partition entropy rate

↑ **Parent:** [Entropy rate of a measurable partition](#entropy-rate-of-a-measurable-partition)

For a measure-preserving action of $\mathbb Z$ and a finite partition $\xi$,

$$
h_\mu(T,\xi)=\inf_{\varnothing\ne F\subseteq\mathbb Z_{\geq0}\text{ finite}}
\frac1{|F|}H_\mu\left(\bigvee_{n\in F}T^{-n}\xi\right).
$$

The reverse inequality to the interval formula follows from [Shearer's inequality](information-theory.md#shearer-s-inequality) applied to translates of $F$ along long intervals; the uncovered boundary has sublinear size.

### K-mixing

↑ **Parent:** [Ergodic theory](#ergodic-theory)

A system is K-mixing when every finite partition becomes asymptotically independent of every event in its remote future: if $\mathcal F_n(\xi)=\bigvee_{k=n}^\infty T^{-k}\xi$, then

$$
\sup_{B\in\mathcal F_n(\xi)}|\mu(A\cap B)-\mu(A)\mu(B)|\longrightarrow0
$$

for every measurable $A$ and every finite $\xi$.

#### Tail sigma-algebra of a measurable partition

↑ **Parent:** [K-mixing](#k-mixing)

The tail sigma-algebra of a finite partition $\xi$ is

$$
\mathcal T(\xi)=\bigcap_{n\geq0}\bigvee_{k=n}^\infty T^{-k}\xi.
$$

By the [reverse martingale convergence theorem](martingale.md#reverse-martingale-convergence-theorem), K-mixing is equivalent to triviality of $\mathcal T(\xi)$ for every finite partition $\xi$.

##### Finite partitions measurable in a partition tail have zero entropy rate

↑ **Parent:** [Tail sigma-algebra of a measurable partition](#tail-sigma-algebra-of-a-measurable-partition)

Let $\alpha$ be finite and measurable in $\mathcal T(\xi)$ for a finite [measurable partition](#measurable-partition) $\xi$, and put $h=h_\mu(T,\xi)$. Choose $r$ with $H(\alpha\mid\xi_0^r)<\varepsilon$. For $\gamma=\alpha_0^{n-1}$ and $\beta=\xi_0^{n+r-1}$, conditional subadditivity gives $H(\gamma\mid\beta)<n\varepsilon$. Tail measurability and [block conditional entropy given the infinite future](#block-conditional-entropy-given-the-infinite-future) give $H(\beta\mid\gamma)\ge(n+r)h$. Thus $H(\gamma)\le H(\beta)-(n+r)h+n\varepsilon$. Divide by $n$, then let $n\to\infty$ and $\varepsilon\downarrow0$, proving $h_\mu(T,\alpha)=0$. The proof also works for noninvertible transformations.

## Outer measure

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Outer_measure)

An outer measure $\mu^*$ is defined on every subset, vanishes on the empty set, is monotone, and is countably subadditive.

<h3 id="caratheodory-s-criterion">Carathéodory's criterion</h3>

↑ **Parent:** [Outer measure](#outer-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carathéodory's_criterion)

A set $E$ is measurable for an [outer measure](#outer-measure) $\mu^*$ when every set $A$ is split additively by $E$:

$$
\mu^*(A)=\mu^*(A\cap E)+\mu^*(A\setminus E).
$$

The measurable sets form a [sigma-algebra](#sigma-algebra), and the restriction of $\mu^*$ to it is a complete measure.

### Lebesgue outer measure

↑ **Parent:** [Outer measure](#outer-measure)

The resulting [Lebesgue measure](#lebesgue-measure) is the restriction of this outer measure to the sets satisfying the measurability criterion.

Lebesgue outer measure on $\mathbb R$ is

$$
m^*(E)=\inf\left\{\sum_{n=1}^{\infty}|I_n|:E\subseteq\bigcup_{n=1}^{\infty}I_n\right\},
$$

where the infimum is over countable interval covers. The [Caratheodory measurability criterion](#caratheodory-s-criterion) selects the Lebesgue-measurable sets.

## Measure

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measure)

On a [measurable space](#measurable-space) $(X,\mathcal F)$, a measure is a [function](function.md) $\mu:\mathcal F\to[0,\infty]$ with $\mu(\varnothing)=0$ and [countable additivity](#countable-additivity): for pairwise disjoint [measurable sets](#measurable-set) $A_n$,

$$
\mu\left(\bigcup_{n=1}^{\infty}A_n\right)=\sum_{n=1}^{\infty}\mu(A_n).
$$

Infinite size is permitted. Nonnegativity implies that if [measurable sets](#measurable-set) satisfy $A\subseteq B$, then $\mu(A)\leq\mu(B)$: decompose $B$ into $A$ and $B\setminus A$. For overlapping [measurable sets](#measurable-set), use [countable subadditivity](#countable-subadditivity-of-a-measure) rather than adding their full sizes twice.

For example, [counting measure](#counting-measure) gives $\mu(\{a,b,c\})=3$, while a [Dirac measure](#dirac-measure) $\delta_a$ gives that same [set](set.md) size $1$ if it contains $a$. Under [Lebesgue measure](#lebesgue-measure), $[0,1/4]\cup[3/4,1]$ has size $1/4+1/4=1/2$. These are all [measures](#measure), but they answer different questions: how many objects, whether a distinguished object is present, or how much length is occupied.

### Inner regular measure

↑ **Parent:** [Measure](#measure)

A [measure](#measure) is inner regular on its measurable sets if their measures are suprema of the measures of contained [compact sets](topology.md#compact-space). Every [Borel probability measure](#borel-probability-measure) on a [compact metric space](topological-analysis.md#compact-metric-space) is inner regular and has [outer regularity](#outer-regular-measure). Combining the two properties allows approximation of an [indicator function](#indicator-function) by a [continuous function](calculus.md#continuous-function) in the $L^1$ norm.

### p-adic measure

↑ **Parent:** [Measure](#measure)

For a [profinite group](topological-group.md#profinite-group) $G$ and a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) $I$ with a continuous $\mathbb Z_p$-algebra structure, an $I$-valued measure is a bounded $I$-linear functional on continuous $I$-valued functions, with the [uniform norm](functional-analysis.md#supremum-norm). Equivalently it assigns finitely additive values in $I$ to [clopen sets](topology.md#clopen-set). [Locally constant functions](calculus.md#locally-constant-function) are uniformly dense, so [integration](calculus.md#integral) extends uniquely from finite sums. [Countable additivity](#countable-additivity) in the usual real-measure sense is not imposed. The coefficient ring may have infinite [residue field](commutative-algebra.md#residue-field) and need not be compact.

#### Mahler expansion of continuous p-adic functions

↑ **Parent:** [p-adic measure](#p-adic-measure)

Let $I$ be a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) with a continuous $\mathbb Z_p$-algebra structure. Every [continuous function](calculus.md#continuous-function) on $\mathbb Z_p$ with values in $I$ has a unique uniformly convergent expansion in the [binomial polynomials](commutative-algebra.md#binomial-polynomial), with $a_n=\Delta^nf(0)$. This is the coefficient-ring version of the [Mahler theorem](arithmetic.md#mahler-s-theorem). To see that $a_n\to0$, approximate the function modulo any power of the [maximal ideal](commutative-algebra.md#maximal-ideal) by a function of period $p^k$. In the expansion of $(E-1)^{p^k}$, all intermediate [binomial coefficients](combinatorics.md#binomial-coefficient) are divisible by $p$, while $(E^{p^k}-1)$ kills the periodic function. Iterating makes its differences vanish modulo the prescribed ideal power. [Finite differences](finite-difference.md) do not increase the [uniform norm](functional-analysis.md#supremum-norm), so the same conclusion holds for the original function. [Binomial inversion](combinatorics.md#binomial-inversion) gives agreement at the nonnegative [integers](number-theory.md#integer), and their density in the [p-adic integers](number-theory.md#p-adic-integer) gives the expansion everywhere. This gives the dual description of [p-adic measures](#p-adic-measure) by arbitrary bounded sequences of binomial moments, and hence the [Amice transform](#amice-transform).

#### Amice transform

↑ **Parent:** [p-adic measure](#p-adic-measure)

The coefficient of $T^n$ is $\int\binom{x}{n}\,d\mu(x)$. The [Mahler expansion of continuous p-adic functions](#mahler-expansion-of-continuous-p-adic-functions) identifies $I$-valued [p-adic measures](#p-adic-measure) on $\mathbb Z_p$ with $I[[T]]$. If $D=(1+T)d/dT$, then $D^k\mathcal A_\mu(0)=\int x^k\,d\mu(x)$. A measure supported on $\mathbb Z_p^\times$ has $\sum_{\zeta^p=1}\mathcal A_\mu(\zeta(1+T)-1)=0$, because the sum of $\zeta^x$ is zero for $p\nmid x$.

#### Convolution of p-adic measures

↑ **Parent:** [p-adic measure](#p-adic-measure)

On a [profinite group](topological-group.md#profinite-group), convolution is first defined for functions on a finite quotient by summing products of the two measures' coset coefficients, then extended by uniform approximation. Finite-quotient associativity proves associativity. For an abelian [group](group.md) it is commutative; the Dirac measure at the identity is the identity element. Under the [measure realization of an Iwasawa algebra](associative-algebra.md#measure-realization-of-an-iwasawa-algebra), it becomes group-algebra multiplication.

### Stieltjes transform of a measure

↑ **Parent:** [Measure](#measure)

For a finite positive [measure](#measure) on the real line, this convention for its Stieltjes transform is analytic off the real line and has positive imaginary part in the upper half-plane if the measure is nonzero. Some sources use $(z-x)^{-1}$ instead, changing the sign. The transform of an [empirical spectral measure](probability-theory.md#empirical-spectral-measure) equals the normalized trace of the [Stieltjes matrix resolvent](functional-analysis.md#stieltjes-matrix-resolvent).

### Outer regular measure

↑ **Parent:** [Measure](#measure)

A [measure](#measure) on a topological space is outer regular on its measurable sets when the displayed open-cover identity holds. [Lebesgue measure](#lebesgue-measure) has this property. It allows a null set to be placed in arbitrarily small open neighborhoods, and a compact small set to receive a smooth cutoff of similarly small integral.

### Complex measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complex_measure)

A complex measure is a countably additive complex-valued set function on a [sigma-algebra](#sigma-algebra). Its [total variation norm of a measure](#total-variation-norm-of-a-measure) is obtained by taking the supremum of sums $\sum_j|\nu(E_j)|$ over finite measurable partitions. For finite variation and [absolute continuity of measures](#absolute-continuity-of-measures) with respect to a sigma-finite positive measure, the [Radon-Nikodym theorem](#radon-nikodym-theorem) supplies an integrable complex density.

### Countable subadditivity of a measure

↑ **Parent:** [Measure](#measure)

For measurable [sets](set.md) $E_n$, a [measure](#measure) satisfies

$$
\mu\left(\bigcup_{n\ge1}E_n\right)\le\sum_{n\ge1}\mu(E_n).
$$

Replace $E_n$ by the disjoint [sets](set.md) $E_n\setminus\bigcup_{j<n}E_j$, use [countable additivity](#countable-additivity), and then monotonicity. The same property is an axiom for an [outer measure](#outer-measure) on arbitrary [sets](set.md).

### Complete measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Complete_measure)

A [measure](#measure) is complete when every [subset](set.md#subset) of each [null set](#null-set) is a [measurable set](#measurable-set). Such a subset also has measure zero by monotonicity. The [completion of a measure](#completion-of-a-measure) extends it to a complete measure by adjoining all subsets of measurable null sets to its [sigma-algebra](#sigma-algebra).

#### Completion of a measure

↑ **Parent:** [Complete measure](#complete-measure)

The completion of a measure space adjoins every [subset](set.md#subset) of every measurable [null set](#null-set) to its [sigma-algebra](#sigma-algebra). A statement that two events or σ-algebras agree modulo null sets becomes literal after passing to the corresponding measure-algebra completion.

### Variation measure

↑ **Parent:** [Measure](#measure)

For a finite signed or complex [measure](#measure) $\mu$, its variation is the positive [measure](#measure)

$$
|\mu|(E)=\sup\left\{\sum_j|\mu(E_j)|:(E_j)\text{ is a finite measurable partition of }E\right\}.
$$

It controls integration by $|\int f\,d\mu|\leq\int|f|\,d|\mu|$.

#### Total variation norm of a measure

↑ **Parent:** [Variation measure](#variation-measure)

The total variation norm of a finite signed or complex [measure](#measure) is the total mass of its [variation measure](#variation-measure). Under the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem), it equals the norm of the corresponding member of $C(K)^*$.

### Signed measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Signed_measure)

A signed measure is a countably additive real-valued set function, allowing negative values. A finite signed measure has a [variation measure](#variation-measure), whose total mass is its [total variation norm of a measure](#total-variation-norm-of-a-measure).

### Dirac measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirac_measure)

On a [measurable space](#measurable-space) $(X,\mathcal F)$, the [Dirac measure](#dirac-measure) at $x\in X$ assigns unit mass according to whether a [measurable set](#measurable-set) contains that point:

$$
\delta_x(A)=\mathbf1_A(x)=\begin{cases}1,&x\in A,\\0,&x\notin A,\end{cases}\qquad A\in\mathcal F.
$$

Here $\mathbf1_A$ is the [indicator function](#indicator-function). This is a [probability measure](probability-theory.md#probability-measure), since $\delta_x(X)=1$. For pairwise disjoint [measurable sets](#measurable-set) $A_n$, at most one contains $x$, so $\delta_x(\bigcup_nA_n)=\sum_n\delta_x(A_n)$: [countable additivity](#countable-additivity) reduces to a membership test. The definition works even when the [singleton](set.md#singleton-mathematics) $\{x\}$ is not a [measurable set](#measurable-set). [Terence Tao, 245B notes 0, Example 7: Dirac measures](https://terrytao.wordpress.com/2009/01/01/245b-notes-0-a-quick-review-of-measure-and-integration-theory/)

To assert that its [support of a measure](#support-of-a-measure) is exactly $\{x\}$, assume that $X$ is a [metric space](topological-analysis.md#metric-space) and $\mathcal F$ is its [Borel sigma-algebra](#borel-sigma-algebra). The [singleton](set.md#singleton-mathematics) $\{x\}$ is then a [closed set](topology.md#closed-set) and a [Borel set](#borel-set), with $\delta_x(\{x\})=1$. Every open [neighbourhood](topology.md#neighbourhood-mathematics) of $x$ has mass one; every other point $y$ has an open [ball](topological-analysis.md#ball-mathematics) of radius less than its distance from $x$, with mass zero. Thus $\operatorname{supp}\delta_x=\{x\}$. An abstract [measurable space](#measurable-space) has no specified [topology](topology.md), so this topological conclusion is not part of the bare definition. Indeed, on the [sigma-algebra](#sigma-algebra) $\{\varnothing,X\}$, all [Dirac measures](#dirac-measure) coincide: the available [measurable sets](#measurable-set) cannot distinguish points.

The [Lebesgue integral](#lebesgue-integral) against a [Dirac measure](#dirac-measure) is evaluation:

$$
\int_X f\,d\delta_x=f(x).
$$

This holds for every nonnegative [measurable function](#measurable-function), allowing an infinite value, and for real or complex [measurable functions](#measurable-function) satisfying $|f(x)|<\infty$, which are precisely the [integrable functions](#lebesgue-integrable-function) for $\delta_x$. For a nonnegative [simple function](#simple-function), only the cell containing $x$ contributes to its [integral](calculus.md#integral); increasing [simple functions](#simple-function) and the [monotone convergence theorem](#monotone-convergence-theorem) extend the identity. Splitting into positive and negative parts, and then real and imaginary parts, gives the remaining cases. This is why a [Dirac measure](#dirac-measure) turns [integration](calculus.md#integral) into a point query.

For a [measurable function](#measurable-function) $T:(X,\mathcal F)\to(Y,\mathcal G)$, its [pushforward measure](#pushforward-measure) satisfies

$$
(T_*\delta_x)(B)=\delta_x(T^{-1}(B))=\mathbf1_B(T(x)),\qquad T_*\delta_x=\delta_{T(x)}.
$$

Consequently $\int_Y g\,d(T_*\delta_x)=g(T(x))$ for nonnegative or integrable [measurable functions](#measurable-function) $g$. For example, on the [real numbers](arithmetic.md#real-number) with their [Borel sigma-algebra](#borel-sigma-algebra), $T(t)=2t+1$ sends $\delta_1$ to $\delta_3$, so integrating $g(y)=y^2$ against that [pushforward measure](#pushforward-measure) gives $9$. [Terence Tao, 245B notes 0, Example 10 and Theorem 2(8): pushforward and change of variables](https://terrytao.wordpress.com/2009/01/01/245b-notes-0-a-quick-review-of-measure-and-integration-theory/)

Finite weighted sums of [Dirac measures](#dirac-measure) give useful [measures](#measure) with finitely many point masses. For finite nonnegative weights $w_j$,

$$
\mu=\sum_{j=1}^m w_j\delta_{x_j},\qquad\mu(A)=\sum_{j=1}^m w_j\mathbf1_A(x_j),\qquad\int f\,d\mu=\sum_{j=1}^m w_jf(x_j)
$$

for nonnegative [measurable functions](#measurable-function) $f$, or whenever $\sum_jw_j|f(x_j)|<\infty$, with zero-weight terms omitted. Repeated locations have their weights added. On the [real numbers](arithmetic.md#real-number), this is the finite version of the [measure](#measure) underlying the [left-continuous cumulative function of an atomic measure](calculus.md#left-continuous-cumulative-function-of-an-atomic-measure); a positive-weight [singleton](set.md#singleton-mathematics) is an [atom of a measure](#atom-measure-theory). Unit weights at the distinct points of a [finite set](set.md#finite-set) recover [counting measure](#counting-measure) on that [set](set.md). [Terence Tao, 245A notes 3, Exercises 21 and 25: representation by weighted Dirac measures](https://terrytao.wordpress.com/2010/09/25/245a-notes-3-integration-on-abstract-measure-spaces-and-the-convergence-theorems/)

The same [function](function.md) can have sharply different [integrals](calculus.md#integral) for different [measures](#measure). On $[0,2]$ with its [Borel sigma-algebra](#borel-sigma-algebra), define

$$
f(t)=\begin{cases}5,&t=1,\\t+1,&t\ne1.\end{cases}\qquad\int_{[0,2]}f\,d\delta_1=5,\qquad\int_{[0,2]}f\,d\lambda=4,\qquad\int_{[0,2]}f\,d\#=\infty.
$$

Here $\lambda$ is [Lebesgue measure](#lebesgue-measure) and $\#$ is [counting measure](#counting-measure). The [singleton](set.md#singleton-mathematics) $\{1\}$ is a [Lebesgue null set](#lebesgue-null-set), so its changed value leaves the [Lebesgue integral](#lebesgue-integral) equal to $\int_0^2(t+1)\,dt=4$. For [counting measure](#counting-measure) on the whole [interval](real-analysis.md#interval-mathematics), $f\geq1$ on an [infinite set](set.md#infinite-set), forcing an infinite [integral](calculus.md#integral). On the smaller [measure space](#measure-space) $D=\{0,1,2\}$ with its [power set](set.md#power-set) and [counting measure](#counting-measure), the restricted [function](function.md) instead has [integral](calculus.md#integral) $1+5+3=9$.

<a id="image-an-isolated-value-contributes-differently-to-dirac-measure-counting-measure-and-lebesgue-measure"></a>
![](counting-dirac-measures-evaluation-and-integration.png)

**[Figure 5](#image-an-isolated-value-contributes-differently-to-dirac-measure-counting-measure-and-lebesgue-measure). An isolated value contributes differently to Dirac measure, counting measure, and Lebesgue measure**. Original analytical illustration of the specified [function](function.md), with an open circle at the excluded value $2$ and a filled point at the actual value $f(1)=5$. The finite sum uses $D=\{0,1,2\}$; the other three [integrals](calculus.md#integral) use the same ambient [interval](real-analysis.md#interval-mathematics) $[0,2]$. The drawn area is the [Lebesgue integral](#lebesgue-integral), and no density curve is assigned to the [Dirac measure](#dirac-measure).

This also explains the [almost everywhere](#almost-everywhere) convention in [Lp spaces](#lp-space): equality [almost everywhere](#almost-everywhere) for $\delta_x$ requires equality at $x$, whereas equality [almost everywhere](#almost-everywhere) for [Lebesgue measure](#lebesgue-measure) allows different values at that [singleton](set.md#singleton-mathematics). A point value therefore cannot be read unambiguously from an equivalence class in an [Lp space](#lp-space) formed using [Lebesgue measure](#lebesgue-measure).

On the [real numbers](arithmetic.md#real-number), a [Dirac measure](#dirac-measure) gives the [Dirac delta distribution](distribution-theory.md#dirac-delta-function) by $\langle\delta_x,\varphi\rangle=\int\varphi\,d\delta_x=\varphi(x)$ for every [test function](distribution-theory.md#test-function). The name [Dirac delta function](distribution-theory.md#dirac-delta-function) does not mean an ordinary [function](function.md) that is zero away from $x$ and infinitely high at $x$. Such a nonnegative [measurable function](#measurable-function) still has [Lebesgue integral](#lebesgue-integral) zero, because its nonzero values occur on a [Lebesgue null set](#lebesgue-null-set). More generally, no nonnegative density $h$ with respect to [Lebesgue measure](#lebesgue-measure) can represent $\delta_x$: it would give $\delta_x(\{x\})=\int_{\{x\}}h\,d\lambda=0$, contradicting unit mass. The [measure](#measure) and its associated [distribution](distribution-theory.md#distribution-mathematical-analysis) act on different kinds of inputs, namely [measurable sets](#measurable-set) and [test functions](distribution-theory.md#test-function), but express the same point evaluation. [Terence Tao, 245C notes 3: Radon measures, test functions, and the Dirac delta distribution](https://terrytao.wordpress.com/2009/04/19/245c-notes-3-distributions/)

### Atom (measure theory)

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Atom_(measure_theory))

An atom of a [measure](#measure) $\mu$ is a measurable set $A$ of positive measure for which every measurable $B\subseteq A$ has either $\mu(B)=0$ or $\mu(B)=\mu(A)$. A singleton of positive mass is an example. A [transport map](mathematical-optimization.md#transport-map) cannot split the mass of a singleton among several destinations.

#### Non-atomic measure

↑ **Parent:** [Atom (measure theory)](#atom-measure-theory)

A non-atomic [measure](#measure) contains no [atom of a measure](#atom-measure-theory). For a finite [Borel measure](#borel-measure) on a [Polish space](topological-analysis.md#polish-space), this is equivalent to giving every singleton mass zero. For a [probability measure](probability-theory.md#probability-measure) on $\mathbb R$, it is also equivalent to continuity of its [cumulative distribution function](probability-theory.md#cumulative-distribution-function).

##### Lyapunov convexity theorem

↑ **Parent:** [Non-atomic measure](#non-atomic-measure)

The range of a finite-dimensional, finite, countably additive, atomless vector measure is [compact](topology.md#compact-space) and [convex](real-analysis.md#convex-function). In particular, an [atomless measure](#non-atomic-measure) restricted to a measurable set $E$ can realize every mass between zero and $\mu(E)$. This allows exact balancing by small disjoint consumer cohorts in an [exchange economy](mathematics.md#exchange-economy).

### Counting measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Counting_measure)

[Counting measure](#counting-measure) makes [integration](calculus.md#integral) into [summation](arithmetic.md#summation) by giving every measurable [singleton](set.md#singleton-mathematics) unit weight. On any [measurable space](#measurable-space) $(X,\mathcal F)$, it is the [measure](#measure) $\#$ defined by

$$
\#(A)=\begin{cases}|A|,&A\text{ is finite},\\\infty,&A\text{ is infinite},\end{cases}\qquad A\in\mathcal F.
$$

Thus $\#(\varnothing)=0$, a [finite set](set.md#finite-set) has its usual [cardinality](set-theory.md#cardinality), and every [infinite set](set.md#infinite-set) has the same value $\infty$ in the [extended real number line](arithmetic.md#extended-real-number-line). In particular, [countably infinite sets](set-theory.md#countably-infinite-set) and [uncountable sets](set-theory.md#uncountable-set) are not distinguished by their [counting measure](#counting-measure). Taking $\mathcal F$ to be the [power set](set.md#power-set) makes every [subset](set.md#subset) measurable; restricting the same rule to a smaller [sigma-algebra](#sigma-algebra) is also allowed. [John K. Hunter, Measure Theory, Example 1.11: counting measure](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch1.pdf)

Why is this a [countably additive](#countable-additivity) [measure](#measure)? For pairwise disjoint [measurable sets](#measurable-set) $A_n$,

$$
\#\left(\bigcup_{n=1}^{\infty}A_n\right)=\sum_{n=1}^{\infty}\#(A_n).
$$

If the [union](set.md#set-union) is finite, only finitely many $A_n$ are nonempty, and finite [cardinality](set-theory.md#cardinality) adds. If the [union](set.md#set-union) is infinite, either one $A_n$ is infinite or infinitely many $A_n$ are nonempty; in both cases the nonnegative [series](real-analysis.md#series-mathematics) on the right is infinite. For example, $\{0,2\}$ and $\{1\}$ have [counting measures](#counting-measure) $2$ and $1$, and their [union](set.md#set-union) has [counting measure](#counting-measure) $3$. The [singletons](set.md#singleton-mathematics) $\{n\}$ for positive [natural numbers](arithmetic.md#natural-number) give the infinite case: $\#(\mathbb N)=\sum_{n=1}^{\infty}1=\infty$.

With the [power set](set.md#power-set) as [sigma-algebra](#sigma-algebra), [counting measure](#counting-measure) is a [finite measure](#finite-measure) exactly when $X$ is finite, and a [sigma-finite measure](#sigma-finite-measure) exactly when $X$ is at most [countable](set-theory.md#countable-set). For the latter assertion, enumerate $X$ by measurable [singletons](set.md#singleton-mathematics); conversely, every finite-measure [set](set.md) is finite, and a [countable union](set.md#countable-union) of [finite sets](set.md#finite-set) is [countable](set-theory.md#countable-set). Specifying the [sigma-algebra](#sigma-algebra) matters: if $X=\mathbb N$ and $\mathcal F=\{\varnothing,\mathbb N\}$, [counting measure](#counting-measure) is not a [sigma-finite measure](#sigma-finite-measure), since the only measurable finite-measure [set](set.md) is the [empty set](set.md#empty-set).

For a finite or [countably infinite set](set-theory.md#countably-infinite-set) $X$ equipped with its [power set](set.md#power-set), every nonnegative [function](function.md) is a [measurable function](#measurable-function), and

$$
\int_X f\,d\#=\sum_{x\in X}f(x):=\sup_{F\subseteq X\text{ finite}}\sum_{x\in F}f(x).
$$

The [supremum](real-analysis.md#supremum) allows an infinite result and avoids choosing an order for the terms. On a [finite set](set.md#finite-set), expand $f$ as a [simple function](#simple-function) using [singleton](set.md#singleton-mathematics) [indicator functions](#indicator-function). On a [countably infinite set](set-theory.md#countably-infinite-set), enumerate the points and apply the [monotone convergence theorem](#monotone-convergence-theorem) to finite truncations. Real or complex [functions](function.md) are [integrable functions](#lebesgue-integrable-function) for [counting measure](#counting-measure) exactly when $\sum_{x\in X}|f(x)|<\infty$; then their [integral](calculus.md#integral) equals the absolutely convergent sum. This is the discrete counterpart of [Lebesgue integration](calculus.md#lebesgue-integration), developed further in [series as a Lebesgue integral against counting measure](#series-as-a-lebesgue-integral-against-counting-measure). [John K. Hunter, Measure Theory, Example 4.10: absolutely convergent series as integrals](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch4.pdf)

For example, $f(n)=2^{-n}$ on the positive [natural numbers](arithmetic.md#natural-number) has [counting measure](#counting-measure) [integral](calculus.md#integral) one, by the [geometric series](real-analysis.md#geometric-series). The [alternating harmonic series](real-analysis.md#alternating-harmonic-series) has a finite ordered sum but is not the [integral](calculus.md#integral) of an [integrable function](#lebesgue-integrable-function) for [counting measure](#counting-measure): its positive and negative parts both have infinite sums. [Absolute convergence](real-analysis.md#absolute-convergence) is what makes the finite [integral](calculus.md#integral) independent of enumeration. In particular, the [Lp spaces](#lp-space) for [counting measure](#counting-measure) on $\mathbb N$ are the [l-p sequence spaces](banach-space.md#l-p-sequence-space), with their sums replacing continuous [integrals](calculus.md#integral).

Compare three [measures](#measure) on the same [Borel sigma-algebra](#borel-sigma-algebra) of the [real numbers](arithmetic.md#real-number): [counting measure](#counting-measure) $\#$, [Dirac measure](#dirac-measure) $\delta_1$, and [Lebesgue measure](#lebesgue-measure) $\lambda$.

$$
\begin{array}{c|ccc}
A&\#(A)&\delta_1(A)&\lambda(A)\\\hline
\varnothing&0&0&0\\
\{0\}&1&0&0\\
\{0,1,2\}&3&1&0\\
[0,2]&\infty&1&2\\
\mathbb Q\cap[0,2]&\infty&1&0
\end{array}
$$

The [rational numbers](number-theory.md#rational-number) in the last row form a [countably infinite set](set-theory.md#countably-infinite-set); their [Lebesgue measure](#lebesgue-measure) is zero by [countable additivity](#countable-additivity) applied to [singletons](set.md#singleton-mathematics), even though they are [dense](topology.md#dense-set) in the [interval](real-analysis.md#interval-mathematics).

<a id="image-the-same-borel-sets-have-different-sizes-under-counting-measure-dirac-measure-and-lebesgue-measure"></a>
![](counting-dirac-measures-same-sets.png)

**[Figure 6](#image-the-same-borel-sets-have-different-sizes-under-counting-measure-dirac-measure-and-lebesgue-measure). The same Borel sets have different sizes under counting measure, Dirac measure, and Lebesgue measure**. Original analytical comparison on the [real numbers](arithmetic.md#real-number), with the selected point $1$ marked in orange. Drawings show the finite [sets](set.md) and the [interval](real-analysis.md#interval-mathematics); the [rational numbers](number-theory.md#rational-number) are named symbolically because finitely many plotted points cannot depict that infinite dense [set](set.md). Green zero entries mark the [null sets](#null-set) for each column's [measure](#measure).

These are different answers to different questions: [counting measure](#counting-measure) asks how many points occur, [Dirac measure](#dirac-measure) asks whether the selected point occurs, and [Lebesgue measure](#lebesgue-measure) asks how much [length](physics.md#length) occurs. A [null set](#null-set) therefore depends on its [measure](#measure). For [counting measure](#counting-measure), the only [null set](#null-set) is the [empty set](set.md#empty-set), so equality [almost everywhere](#almost-everywhere) is equality everywhere. For $\delta_1$, a [measurable set](#measurable-set) is a [null set](#null-set) exactly when it misses $1$; for [Lebesgue measure](#lebesgue-measure), even the [infinite set](set.md#infinite-set) $\mathbb Q\cap[0,2]$ is a [null set](#null-set). Integrating an [indicator function](#indicator-function) recovers each table entry through $\int\mathbf1_A\,d\mu=\mu(A)$. This lets the same [Lebesgue integral](#lebesgue-integral) framework handle point counts, point evaluation, and geometric [length](physics.md#length).

#### Series as a Lebesgue integral against counting measure

↑ **Parent:** [Counting measure](#counting-measure)

For $f:\mathbb N\to[0,\infty]$,

$$
\int_{\mathbb N}f\,d\#
=\sum_{n=1}^{\infty}f(n)
:=\sup_{F\subseteq\mathbb N\text{ finite}}\sum_{n\in F}f(n).
$$

A complex-valued function is integrable for counting measure exactly when its series is absolutely convergent.

### Premeasure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Premeasure)

A premeasure is a countably additive nonnegative set function on an algebra of sets, with countable additivity required whenever the union remains in that algebra.

#### Cylinder premeasure from a positive functional

↑ **Parent:** [Premeasure](#premeasure)

A normalized [positive linear functional](continuous-dual-space.md#positive-linear-functional) on $C(\Omega)$ for [Cantor space](geometry-and-topology.md#cantor-space) gives a finitely additive set function on the algebra of [clopen sets](topology.md#clopen-set). If a countable disjoint union of such sets is itself clopen, [compactness](topology.md#compact-space) gives a finite subcover; all other terms are empty. Finite additivity therefore gives the required [countable additivity](#countable-additivity), making $\ell$ a [premeasure](#premeasure). The [Caratheodory extension theorem](#caratheodory-s-extension-theorem) produces a unique [Borel probability measure](#borel-probability-measure).

<h4 id="caratheodory-s-extension-theorem">Carathéodory's extension theorem</h4>

↑ **Parent:** [Premeasure](#premeasure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carathéodory's_extension_theorem)

A premeasure on an algebra of sets extends to a measure on the generated [sigma-algebra](#sigma-algebra). The extension is unique when the premeasure is [sigma-finite](#sigma-finite-measure).

### Positive measure

↑ **Parent:** [Measure](#measure)

A positive measure takes values in $[0,\infty]$, in contrast with signed and complex measures.

### Borel measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borel_measure)

A Borel measure on a [topological space](topology.md#topological-space) is a [measure](#measure) defined on the [sigma-algebra](#sigma-algebra) generated by the [open sets](topology.md#open-set), equivalently on the [Borel sets](#borel-set).

#### Support of a measure

↑ **Parent:** [Borel measure](#borel-measure)

For a positive Borel measure on a topological space, the support consists of the points whose every open neighborhood has positive measure. For a finite regular [complex measure](#complex-measure) use its [variation measure](#variation-measure). Regularity makes the complement of the support null: compact subsets of that open complement have finite covers by null neighborhoods. A regular probability measure on a compact Hausdorff space whose support is a single point is therefore a [Dirac measure](#dirac-measure).

##### Support under a continuous map

↑ **Parent:** [Support of a measure](#support-of-a-measure)

For a [Borel probability measure](#borel-probability-measure) on a [Polish space](topological-analysis.md#polish-space) and a continuous map to another Polish space, the image measure has the displayed support. Every neighborhood of an image of a support point has an open inverse image of positive measure. Conversely, the closed image closure has full image measure because the original support has full measure. This transfers a support description for a driving [rough path](analysis.md#rough-path) to the solution of a [rough differential equation](analysis.md#rough-differential-equation).

#### Borel probability measure

↑ **Parent:** [Borel measure](#borel-measure)

A Borel probability measure is a [Borel measure](#borel-measure) with total mass one. On a compact [metric space](topological-analysis.md#metric-space) it is determined by its integrals against continuous functions. On that compact [metric space](topological-analysis.md#metric-space), the family of [Borel probability measures](#borel-probability-measure) is compact for [weak convergence of probability measures](convergence-of-random-variables.md#weak-convergence-of-probability-measures).

##### Continuous approximation of Borel indicators on a compact metric space

↑ **Parent:** [Borel probability measure](#borel-probability-measure)

For a [Borel probability measure](#borel-probability-measure) on a [compact metric space](topological-analysis.md#compact-metric-space), [inner regularity](#inner-regular-measure) and [outer regularity](#outer-regular-measure) give $K\subseteq B\subseteq U$ with $K$ compact, $U$ open and $\mu(U\setminus K)<\epsilon$. The [Urysohn lemma](topology.md#urysohn-s-lemma) supplies a [continuous function](calculus.md#continuous-function) $\varphi$ equal to one on $K$ and zero outside $U$, with values in $[0,1]$. Its difference from the [indicator function](#indicator-function) of $B$ is supported in $U\setminus K$ and bounded by one, proving the displayed estimate. This transfers identities established for continuous test functions to measurable sets.

#### Regular Borel measure

↑ **Parent:** [Borel measure](#borel-measure)

A finite positive [Borel measure](#borel-measure) on a [compact Hausdorff space](topology.md#compact-hausdorff-space) is regular when its values on Borel sets can be approximated from inside by compact sets and from outside by open sets. For signed or complex measures require this property of the [variation measure](#variation-measure). These are the measures representing the [continuous dual space](continuous-dual-space.md) of $C(K)$ in the [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem).

#### Radon measure

↑ **Parent:** [Borel measure](#borel-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radon_measure)

A Radon measure is a Borel measure that is finite on compact sets and is inner regular, so the measure of a Borel set can be approximated from below by compact subsets. On a locally compact Hausdorff space one also usually includes outer regularity.

##### Regularity of finite Borel measures on Euclidean space

↑ **Parent:** [Radon measure](#radon-measure)

Every finite positive [Borel measure](#borel-measure) on Euclidean space is inner regular by [compact sets](topology.md#compact-space) and outer regular by open sets. For an [open set](topology.md#open-set) $U$, the [compact sets](topology.md#compact-space) $\{x:|x|\le n,\ \operatorname{dist}(x,U^c)\ge1/n\}$ increase to $U$, so [continuity from below of a measure](#continuity-from-below-of-a-measure) gives inner approximation. The empty complement is handled by compact balls. The class of Borel sets admitting both approximations is closed under complements: interchange inner and outer approximations, then truncate the inner closed set by a large compact ball, using finiteness of the [measure](#measure). For a countable union, approximate its components from outside with summable errors, and approximate finitely many components from inside after making the remaining union's [measure](#measure) small. Thus this class is a [sigma-algebra](#sigma-algebra) containing the open sets. In particular, a finite [measure](#measure) carried by a Borel [null set](#null-set) has [compact subsets](topology.md#compact-space) of that carrier capturing arbitrarily nearly all its mass.

### Measure space

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Measure_space)

A measure space is a [set](set.md) $X$, a [sigma-algebra](#sigma-algebra) $\mathcal M$ of its [subsets](set.md#subset), and a [measure](#measure) $\mu$ defined on $\mathcal M$. Specifying only $X$ leaves both the measurable questions and their weights undetermined.

For a concrete [probability space](probability-theory.md#probability-space), take $X=\{a,b,c\}$, $\mathcal M$ its [power set](set.md#power-set), and weights $1/2,1/3,1/6$. Define $\mu(A)$ by adding the weights of the elements in $A$. Then

$$
\mu(X)=\frac12+\frac13+\frac16=1,\qquad
\mu(\{b,c\})=\frac12.
$$

A [probability measure](probability-theory.md#probability-measure) is exactly a [measure](#measure) normalized by $\mu(X)=1$, usually written $\mathbb P(\Omega)=1$. An [indicator function](#indicator-function) has [expected value](probability-theory.md#expected-value) equal to its [event](probability-theory.md#event)'s [probability](probability-theory.md#probability). For a different continuous example, $[0,1]$ with the restricted [Lebesgue measure](#lebesgue-measure) is a [probability space](probability-theory.md#probability-space); the [event](probability-theory.md#event) $[0,1/4]$ has [probability](probability-theory.md#probability) $1/4$.

### Pushforward measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pushforward_measure)

For a measurable map $f:X\to Y$, the pushforward of $\mu$ is the measure

$$
(f_*\mu)(B)=\mu(f^{-1}(B)).
$$

It is the distribution induced on $Y$ by mapping points distributed according to $\mu$ through $f$.

#### Probability pushforward embedding theorem

↑ **Parent:** [Pushforward measure](#pushforward-measure)

A homeomorphic embedding of a [metric](topological-analysis.md#metric) space induces a homeomorphic embedding of its [probability measures](probability-theory.md#probability-measure) for their weak topologies. The inverse continuity follows from the open-set [Portmanteau theorem](convergence-of-random-variables.md#portmanteau-theorem), since every relatively [open set](topology.md#open-set) is the trace of an ambient [open set](topology.md#open-set). This does not give surjectivity onto $P(Z)$ when points of $Z$ are outside the embedded image.

### Change of measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Change_of_measure)

If a measure $\nu$ has density $w=d\nu/d\mu$ with respect to $\mu$, then

$$
\int g\,d\nu=\int gw\,d\mu.
$$

This identity is the basis of likelihood ratios and [importance sampling](probability-and-statistics.md#importance-sampling).

#### Density process

↑ **Parent:** [Change of measure](#change-of-measure)

For a [Radon-Nikodym derivative](#radon-nikodym-derivative) $L_T\geq0$ with $\mathbb EL_T=1$, its conditional-expectation process is a nonnegative [martingale](martingale.md). If $L_T>0$ [almost surely](convergence-of-random-variables.md#almost-sure-convergence), it defines an [equivalent probability measure](#equivalent-probability-measure). A [stochastic exponential](stochastic-calculus.md#doleans-dade-exponential) satisfying the [Novikov condition](stochastic-calculus.md#novikov-s-condition) is a common positive density process.

### Haar measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Haar_measure)

A left [Haar measure](#haar-measure) on a [locally compact group](topological-group.md#locally-compact-group) that is a [Hausdorff space](topology.md#hausdorff-space) is a nonzero regular [Borel measure](#borel-measure), finite on [compact sets](topology.md#compact-space), satisfying $\mu(gA)=\mu(A)$ for every [Borel set](#borel-set) $A$. Such a [measure](#measure) exists and is unique up to a positive scalar. Right [Haar measure](#haar-measure) instead satisfies $\mu(Ag)=\mu(A)$; the two need not coincide. On a [compact group](topological-group.md#compact-group), normalization gives total mass one and invariance on both sides. See [Tornier, Haar Measures, Definition 2.1 and Theorem 2.2](https://arxiv.org/html/2006.10956v1#S2).

For a [finite group](group.md#finite-group), normalized [Haar measure](#haar-measure) is uniform counting; for the [circle group](lie-theory.md#circle-group), it is [normalized angle integration on the circle](topological-group.md#normalized-angle-integration-on-the-circle). These examples turn symmetry into a rule for averaging.

#### Haar measure from a left-invariant coframe

↑ **Parent:** [Haar measure](#haar-measure)

On a $d$-dimensional [Lie group](lie-theory.md#lie-group), take the [coframe](fiber-bundle.md#coframe) dual to a basis of [left-invariant vector fields](lie-theory.md#left-invariant-vector-field). Its top wedge is nonvanishing and invariant under left translations, so its absolute density defines a left [Haar measure](#haar-measure). If the frame has coordinate matrix $A(x)$, the density is $|\det A(x)|^{-1}dx^1\cdots dx^d$. This makes explicit computation of Haar measure a determinant calculation.

#### Haar measure from normalized covering functionals

↑ **Parent:** [Haar measure](#haar-measure)

For nonzero nonnegative $u,h\in C_c(G)$, let $(f:u)$ be the infimum of $\sum_j a_j$ over finite dominations $f\leq\sum_j a_j u(x_j^{-1}\,\cdot)$ with $a_j>0$. Composition of covers gives $(f:u)\leq(f:h)(h:u)$, so $I_u(f)$ is uniformly bounded while $I_u(h)=1$. It is invariant under left translation, homogeneous, monotone and subadditive. As the support of $u$ shrinks to the identity, its additivity defect tends to zero: use the continuous proportions $f_i/(f_1+f_2+\delta p)$, with a cutoff $p$ positive on both supports, whose oscillations are small on every translate of that small support. In a locally compact sigma-compact metrizable group, diagonal convergence on a countable dense family, followed by uniform approximation on fixed compact supports, gives a positive invariant linear functional on all $C_c(G)$. The [Riesz representation on compactly supported continuous functions](functional-analysis.md#riesz-representation-on-compactly-supported-continuous-functions) turns it into [Haar measure](#haar-measure). Local compactness is essential for the compactly supported cutoffs and small-support test functions.

#### Compact-group invariant probability by finite averaging

↑ **Parent:** [Haar measure](#haar-measure)

For a [compact group](topological-group.md#compact-group) $G$, positive normalized [linear functionals](linear-algebra.md#linear-functional) on $C(G)$ form a nonempty [weak-star topology](weak-topology.md#weak-star-topology) compact convex set. For finitely many translations, apply the [Schauder-Tychonoff fixed-point theorem](analysis.md#schauder-tychonoff-fixed-point-theorem) to the average of their induced affine dual maps. A fixed functional is stationary under this average. For each real continuous $f$, its orbit function $h(g)=\phi(l_gf)$ is continuous on the compact subgroup generated by those translations and satisfies a finite averaging identity. At a maximum, every summand must attain that same maximum; iteration and density of the positive-word semigroup force $h$ to be constant. Thus the functional is fixed by each of the finitely many translations. Compactness and the [finite intersection property](topology.md#finite-intersection-property) now give a functional invariant under every translation. The [Riesz-Markov-Kakutani representation theorem](functional-analysis.md#riesz-markov-kakutani-representation-theorem) turns it into a normalized [Haar measure](#haar-measure), without assuming commutativity of the group.

#### Haar integral

↑ **Parent:** [Haar measure](#haar-measure)

A Haar integral integrates a function against [Haar measure](#haar-measure). On a compact [group](group.md), normalizing the measure to total mass one makes it an averaging operation. Translation invariance then implies that the average of a nontrivial continuous unitary character is zero: translating the integral multiplies it by a character value different from one.

<h4 id="weyl-integration-formula-for-su-2">Weyl integration formula for SU(2)</h4>

↑ **Parent:** [Haar measure](#haar-measure)

For a [class function](representation-theory.md#class-function) on [SU(2)](topological-group.md#su-2-group) and normalized [Haar measure](#haar-measure), the displayed formula reduces a group integral to its conjugacy-class angle. The weight follows by identifying [SU(2)](topological-group.md#su-2-group) with the unit sphere in four real dimensions: writing a unit quaternion as $\cos\theta+\mathbf n\sin\theta$ gives spherical volume proportional to $\sin^2\theta\,d\theta\,d\mathbf n$. Since $\int_0^\pi\sin^2\theta\,d\theta=\pi/2$, normalization gives $2/\pi$.

<h4 id="pauli-coordinate-haar-measure-on-su-2">Pauli-coordinate Haar measure on SU(2)</h4>

↑ **Parent:** [Haar measure](#haar-measure)

The hemisphere graph $u_0=\pm\sqrt{1-|\mathbf u|^2}$ of [SU(2) as the three-sphere](topological-group.md#su-2-as-the-three-sphere) has induced metric $g_{ij}=\delta_{ij}+u_iu_j/u_0^2$, whose [determinant](linear-algebra.md#determinant) is $1/u_0^2$. Its volume density is therefore $d^3u/|u_0|$. Fixed left or right multiplication preserves the Euclidean norm on the four Pauli coefficients, so the round volume is [Haar measure](#haar-measure). Both hemispheres have volume $\pi^2$, giving total volume $2\pi^2$ and normalized density $d^3u/(2\pi^2|u_0|)$ on each hemisphere. The apparent equatorial divergence is an integrable coordinate singularity.

#### Minimal left covering net of a compact group

↑ **Parent:** [Haar measure](#haar-measure)

For an open identity neighbourhood $V$ in a compact [topological group](topological-group.md), a finite left covering net is a finite set $F$ such that the left translates $fV$, $f\in F$, cover the group. Compactness gives such finite sets; minimum cardinality gives a minimal one. Left translation preserves minimality because $G=FV$ implies $G=gFV$.

##### Matching minimal covering nets of a compact group

↑ **Parent:** [Minimal left covering net of a compact group](#minimal-left-covering-net-of-a-compact-group)

Two minimal left covering nets for the same identity neighbourhood $V$ can be matched bijectively so that paired translates intersect. Join $f\in F$ to $f'\in F'$ when $fV\cap f'V\ne\varnothing$. For $S\subseteq F$, its neighbours $N(S)$ cover every point covered by $S$, so $(F\setminus S)\cup N(S)$ still covers the group. Minimality forces $|N(S)|\geq|S|$. [Hall's marriage theorem](graph-theory.md#hall-s-marriage-theorem) supplies the matching, and an intersection $fv=f'v'$ gives $f^{-1}f'=vv'^{-1}\in VV^{-1}$. Averaging a continuous function over matched nets therefore gives values differing by at most its uniform oscillation on right displacements in $VV^{-1}$. This is the finite combinatorial step in constructing [Haar measure](#haar-measure) on a compact group.

### Countable additivity

↑ **Parent:** [Measure](#measure)

For pairwise disjoint [measurable sets](#measurable-set) $E_n$, countable additivity means

$$
\mu\!\left(\bigcup_{n=1}^{\infty}E_n\right)
=\sum_{n=1}^{\infty}\mu(E_n).
$$

The infinite [series](real-analysis.md#series-mathematics) is the [limit](calculus.md#limit-of-a-function) of its nonnegative partial sums. This controls an entire [countable union](set.md#countable-union), not merely each finite stage. If $q_1,q_2,\ldots$ enumerate the [rational numbers](number-theory.md#rational-number) in $[0,1]$, their finite collections have [Lebesgue measure](#lebesgue-measure) zero, and [countable additivity](#countable-additivity) gives their whole [union](set.md#set-union) [Lebesgue measure](#lebesgue-measure) zero. Their being a [dense set](topology.md#dense-set) does not change this calculation.

The axiom makes no assertion about an arbitrary [uncountable set](set-theory.md#uncountable-set) of disjoint pieces. In particular, $[0,1]$ is the [union](set.md#set-union) of its [singletons](set.md#singleton-mathematics), each of [Lebesgue measure](#lebesgue-measure) zero, yet its [Lebesgue measure](#lebesgue-measure) is one. Extending additivity to all such [unions](set.md#set-union) would contradict interval length.

#### Continuity from below of a measure

↑ **Parent:** [Countable additivity](#countable-additivity)

If $E_n\uparrow E$, then [countable additivity](#countable-additivity) gives $\mu(E_n)\uparrow\mu(E)$, even when the limiting measure is infinite.

#### Continuity from above of a measure

↑ **Parent:** [Countable additivity](#countable-additivity)

If $E_n\downarrow E$ and $\mu(E_1)<\infty$, then $\mu(E_n)\downarrow\mu(E)$. Apply [continuity from below of a measure](#continuity-from-below-of-a-measure) to the increasing differences $E_1\setminus E_n$.

### Finite measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Finite_measure)

A measure $\mu$ on $X$ is finite when $\mu(X)<\infty$.

#### Finite-measure set

↑ **Parent:** [Finite measure](#finite-measure)

A finite-measure set is a [measurable set](#measurable-set) on which the ambient [measure](#measure) is finite. Restricting to such a set makes its [indicator function](#indicator-function) belong to every [Lp space](#lp-space) with finite exponent, enabling local [Radon-Nikodym theorem](#radon-nikodym-theorem) arguments even when the whole [measure space](#measure-space) is not sigma-finite.

### Sigma-finite measure

↑ **Parent:** [Measure](#measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sigma-finite_measure)

A [measure](#measure) is sigma-finite when its space is a countable [union](set.md#set-union) of measurable sets of finite measure.

## Step function

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Step_function)

A step function is constant on each member of a finite or countable measurable partition of its domain. Indicator functions of measurable sets are basic examples.

## Lebesgue integral

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_integral)

For a nonnegative [measurable function](#measurable-function) $f:X\to[0,\infty]$ on a [measure space](#measure-space), define

$$
\int_X f\,d\mu=\sup\left\{\int_X s\,d\mu: s\text{ is a nonnegative simple function},\ 0\leq s\leq f\right\}.
$$

The [supremum](real-analysis.md#supremum) may be infinite. A [simple function](#simple-function) assigns finitely many heights to [measurable sets](#measurable-set), so its [integral](calculus.md#integral) is height times [measure](#measure), summed over those pieces. This definition groups points by their values rather than requiring a partition into short intervals. See [MIT lecture 11, Definition 108](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/615c26170233747c081d6dab928f7d91_MIT18_102s21_lec11.pdf).

A [real-valued function](function.md#real-valued-function) is [Lebesgue integrable](#lebesgue-integrable-function) when $\int_X|f|\,d\mu<\infty$. Its [integral](calculus.md#integral) is $\int_X f_+\,d\mu-\int_X f_-\,d\mu$, where $f_+=\max(f,0)$ is its [positive part](function.md#positive-part-of-a-real-valued-function) and $f_-=\max(-f,0)$. This finiteness requirement avoids subtracting two infinities. For [functions](function.md) taking values in the [complex numbers](complex-analysis.md#complex-number), integrate the [real part](complex-analysis.md#real-part) and [imaginary part](complex-analysis.md#imaginary-part) separately.

Consider the [Dirichlet function](real-analysis.md#dirichlet-function) $f=\mathbf1_{\mathbb Q\cap[0,1]}$ on $[0,1]$. It is a [simple function](#simple-function), and

$$
\int_{[0,1]}f\,d\lambda=\lambda(\mathbb Q\cap[0,1])=0.
$$

Its [Riemann integral](real-analysis.md#riemann-integral) does not exist. For every [partition of an interval](real-analysis.md#partition-of-an-interval) $0=x_0<\cdots<x_n=1$, each nondegenerate $[x_{i-1},x_i]$ contains both [rational numbers](number-theory.md#rational-number) and [irrational numbers](algebra.md#irrational-number), by their respective [density of the rational numbers](number-theory.md#density-of-the-rational-numbers) and [density of the irrational numbers](algebra.md#density-of-the-irrational-numbers). Thus its [infimum](real-analysis.md#infimum) there is $0$ and its [supremum](real-analysis.md#supremum) is $1$. The [lower Darboux sum](real-analysis.md#lower-darboux-sum) is $\sum_i0(x_i-x_{i-1})=0$, whereas the [upper Darboux sum](real-analysis.md#upper-darboux-sum) is $\sum_i1(x_i-x_{i-1})=1$. Refinement never closes this gap. A finite scatterplot cannot represent this behavior: the assertion concerns every subinterval and every [partition of an interval](real-analysis.md#partition-of-an-interval).

Another view builds the [Lebesgue integral](#lebesgue-integral) from horizontal layers. For any nonnegative [measurable function](#measurable-function), the [layer cake representation](functional-analysis.md#layer-cake-representation) states

$$
\int_X f\,d\mu=\int_0^\infty\mu\bigl(\{x\in X:f(x)>t\}\bigr)\,dt.
$$

Both sides may be infinite. The right side integrates the [measure](#measure) of a [superlevel set](topology.md#superlevel-set) against [Lebesgue measure](#lebesgue-measure) in the height variable $t$. See [Gautam Iyer's measure theory notes, Theorem 9.5](https://www.math.cmu.edu/~gautam/sj/teaching/2022-23/720-measure/pdfs/measure-twocolumn.pdf).

For $f(x)=x^2$ on $[0,1]$ with [Lebesgue measure](#lebesgue-measure), the [superlevel set](topology.md#superlevel-set) at $0\leq t<1$ is $(\sqrt t,1]$, of [Lebesgue measure](#lebesgue-measure) $1-\sqrt t$; for $t\geq1$ it is empty. Consequently

$$
\int_0^1 x^2\,d\lambda(x)=\int_0^1(1-\sqrt t)\,dt
=\left[t-\frac23t^{3/2}\right]_0^1=\frac13.
$$

At height $t=1/4$, the layer extends from $x=1/2$ to $x=1$, a width of $1/2$. The picture shows why the same area can be accumulated vertically or horizontally. In a [probability space](probability-theory.md#probability-space), the identical formula expresses the [expected value](probability-theory.md#expected-value) of a nonnegative [random variable](random-variable.md) through its exceedance [probabilities](probability-theory.md#probability).

<a id="image-integrating-x-2-by-horizontal-layers-and-their-widths"></a>
![](lebesgue-level-sets.png)

**[Figure 7](#image-integrating-x-2-by-horizontal-layers-and-their-widths). Integrating $x^2$ by horizontal layers and their widths**.

A proof outline avoids extra assumptions on the [measure space](#measure-space). For a nonnegative [simple function](#simple-function) $s=\sum_ja_j\mathbf1_{A_j}$ with disjoint [measurable sets](#measurable-set) $A_j$, the [superlevel set](topology.md#superlevel-set) has [measure](#measure) $\sum_{a_j>t}\mu(A_j)$. Integrating this finite sum gives $\sum_ja_j\mu(A_j)=\int s\,d\mu$. Next use [approximation by nonnegative simple functions](#approximation-by-nonnegative-simple-functions) $s_n\uparrow f$. For every $t$, the [superlevel sets](topology.md#superlevel-set) $\{s_n>t\}$ increase to $\{f>t\}$. [Continuity from below of a measure](#continuity-from-below-of-a-measure) and the [monotone convergence theorem](#monotone-convergence-theorem) on the height variable give the formula for $f$.

### Integral average

↑ **Parent:** [Lebesgue integral](#lebesgue-integral)

The [integral average](#integral-average) of an integrable function over a measurable set $E$ of finite positive measure is $\langle v\rangle_E=|E|^{-1}\int_Ev$. Normalization removes the volume factor when comparing estimates on balls of different radii.

#### Volume average

↑ **Parent:** [Integral average](#integral-average)

A [volume average](#volume-average) is the normalized [integral average](#integral-average) of a field over a three-dimensional region of finite positive [volume](geometry-and-topology.md#volume). For a fixed region, differentiating in time commutes with this average under the usual regularity conditions. The [divergence theorem](calculus.md#divergence-theorem) converts the average of a divergence into its net boundary flux divided by volume.

### Simple function

↑ **Parent:** [Lebesgue integral](#lebesgue-integral)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simple_function)

A simple function is a [measurable function](#measurable-function) whose [image](set-theory.md#image-of-a-function) is a [finite set](set.md#finite-set). Its value sets $A_j=\{x:s(x)=a_j\}$ form a finite [measurable partition](#measurable-partition). For nonnegative $a_j$, its [Lebesgue integral](#lebesgue-integral) is $\sum_ja_j\mu(A_j)$, with the convention $0\cdot\infty=0$. The pieces need not be intervals, or even [connected](geometry-and-topology.md#connected-space) [sets](set.md). See [MIT lecture 10, Definitions 100 and 106](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/ebbbc59aa40252dff3d4ec766c057451_MIT18_102s21_lec10.pdf).

For example, on $[0,1]$ let $s$ be $2$ on $[0,1/4)$, $1$ on $[1/4,3/4)$, and $0$ on $[3/4,1]$. Its [Lebesgue integral](#lebesgue-integral) is $2(1/4)+1(1/2)=1$. Its [superlevel sets](topology.md#superlevel-set) have [Lebesgue measure](#lebesgue-measure) $3/4$ for $0\leq t<1$, $1/4$ for $1\leq t<2$, and $0$ thereafter. The [layer cake representation](functional-analysis.md#layer-cake-representation) gives the same answer: $(3/4)(1)+(1/4)(1)=1$. These two calculations are the building blocks of the general [Lebesgue integral](#lebesgue-integral).

## Indicator function

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indicator_function)

The indicator function of a set $E$ is $\mathbf1_E(x)=1$ for $x\in E$ and $0$ otherwise.

### Indicator vector

↑ **Parent:** [Indicator function](#indicator-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Indicator_vector)

The indicator vector of a subset $E\subseteq\{1,\ldots,n\}$ has coordinate $1$ on $E$ and coordinate $0$ outside $E$.

## Sigma-algebra

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sigma-algebra)

A sigma-algebra on a [set](set.md) $\Omega$ is a collection $\mathcal F$ of [subsets](set.md#subset) such that $\Omega\in\mathcal F$, $A\in\mathcal F$ implies $\Omega\setminus A\in\mathcal F$, and $A_n\in\mathcal F$ for all $n$ implies $\bigcup_nA_n\in\mathcal F$. Thus it contains the [empty set](set.md#empty-set) and is closed under countable [intersections](set.md#set-intersection) as well. This is precisely the closure needed to apply [countable additivity](#countable-additivity) without leaving the domain of a [measure](#measure).

For $\Omega=\{a,b,c\}$,

$$
\mathcal F=\{\varnothing,\{a\},\{b,c\},\Omega\}
$$

is a [sigma-algebra](#sigma-algebra). It describes observations that distinguish $a$ from the pair $\{b,c\}$, but cannot distinguish $b$ from $c$. The [power set](set.md#power-set) provides a finer [sigma-algebra](#sigma-algebra) with all eight [subsets](set.md#subset). Both are valid; choosing a [sigma-algebra](#sigma-algebra) records which questions the model can answer.

On the [real numbers](arithmetic.md#real-number), the [Borel sigma-algebra](#borel-sigma-algebra) contains all [open sets](topology.md#open-set) and everything generated from them by these operations. The [Lebesgue measurable sets](#lebesgue-measurable-set) form a larger [sigma-algebra](#sigma-algebra), including all [subsets](set.md#subset) of [Borel null sets](#borel-null-set). Closure under [countable unions](set.md#countable-union) accommodates constructions involving an entire [sequence](real-analysis.md#sequence) of observations or approximations.

### Algebra of sets

↑ **Parent:** [Sigma-algebra](#sigma-algebra)

A nonempty collection of subsets of a fixed universe closed under complements and finite unions, hence also finite intersections. It generates a [sigma-algebra](#sigma-algebra) by allowing countable set operations. A [countable generating algebra](#countable-generating-algebra) provides one simultaneous family of test indicators for measure-theoretic arguments.

#### Countable generating algebra

↑ **Parent:** [Algebra of sets](#algebra-of-sets)

A countable [algebra of sets](#algebra-of-sets) generating the intended sigma-algebra. Standard Borel spaces admit such algebras by taking finite Boolean combinations from a countable topological base. Finite linear combinations of its indicators are dense in $L^2$ for every Borel [probability measure](probability-theory.md#probability-measure), by the [Monotone class theorem](#monotone-class-theorem). Countability permits a common full-measure convergence set for all test indicators.

### Measurable set

↑ **Parent:** [Sigma-algebra](#sigma-algebra)

A [subset](set.md#subset) of $X$ is measurable relative to a [sigma-algebra](#sigma-algebra) $\mathcal F$ when it belongs to $\mathcal F$. A [measure](#measure) defined on $\mathcal F$ assigns sizes to these sets. Measurability depends on the chosen [sigma-algebra](#sigma-algebra); for example, a [Lebesgue measurable set](#lebesgue-measurable-set) need not be a [Borel set](#borel-set).

### Atom of a sigma-algebra

↑ **Parent:** [Sigma-algebra](#sigma-algebra)

A sigma-algebra atom is set-theoretically minimal. An [atom](#atom-measure-theory) is instead indivisible only modulo sets of measure zero.

An atom of a sigma-algebra is a nonempty measurable set containing no proper nonempty measurable subset. A finite sigma-algebra partitions its underlying set into atoms, and each measurable set is a union of them.

### Borel set

↑ **Parent:** [Sigma-algebra](#sigma-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borel_set)

A Borel set in a [topological space](topology.md#topological-space) belongs to the smallest [sigma-algebra](#sigma-algebra) containing every [open set](topology.md#open-set).

#### Borel hierarchy

↑ **Parent:** [Borel set](#borel-set)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Borel_hierarchy)

For a topological space, $\Sigma^0_1$ is the class of open sets and $\Pi^0_\alpha$ consists of complements of $\Sigma^0_\alpha$ sets. For countable $\alpha>1$, $\Sigma^0_\alpha$ consists of countable unions of sets in $\bigcup_{\beta<\alpha}\Pi^0_\beta$. These countable levels contain every [Borel set](#borel-set). Continuous inverse images preserve each level, by induction using openness, complementation and countable unions.

#### Borel sigma-algebra

↑ **Parent:** [Borel set](#borel-set)

The Borel sigma-algebra of a [topological space](topology.md#topological-space) $X$ is the [sigma-algebra](#sigma-algebra) generated by its [open sets](topology.md#open-set). Its members are exactly the [Borel sets](#borel-set).

##### Borel sigma-algebra of a discrete space

↑ **Parent:** [Borel sigma-algebra](#borel-sigma-algebra)

Every subset of a [discrete space](topology.md#discrete-space) is open, so its Borel sigma-algebra is the full [power set](set.md#power-set).

### Pi-system

↑ **Parent:** [Sigma-algebra](#sigma-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pi-system)

A pi-system is a nonempty family of subsets closed under finite intersections.

### Dynkin system

↑ **Parent:** [Sigma-algebra](#sigma-algebra)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dynkin_system)

A Dynkin system contains $\Omega$, is closed under complements, and is closed under countable disjoint unions. Equivalently, it contains differences $B\setminus A$ whenever $A\subseteq B$ are members.

#### Dynkin lemma

↑ **Parent:** [Dynkin system](#dynkin-system)

Every Dynkin system containing a pi-system $\mathcal P$ also contains the sigma-algebra $\sigma(\mathcal P)$. Equivalently, the Dynkin system generated by a pi-system equals the sigma-algebra it generates.

<h2 id="fubini-s-theorem">Fubini's theorem</h2>

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fubini's_theorem)

Fubini's theorem permits the order of integration of an absolutely integrable function on a product measure space to be exchanged.

### Frullani integral

↑ **Parent:** [Fubini's theorem](#fubini-s-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Frullani_integral)

For $0<a<b$, the nonnegative function $e^{-xy}\mathbf1_{\{x>0,\ a\le y\le b\}}$ is measurable and has integral $\int_a^bdy/y=\log(b/a)$. [Tonelli theorem](#tonelli-theorem) first proves integrability without assuming it; [Fubini theorem](#fubini-s-theorem) then permits the order of integration to be exchanged. Integrating in $y$ gives the stated [Frullani integral](#frullani-integral). The cancellation between the exponentials is essential at $x=0$.

## Sigma-finite uniqueness theorem for measures

↑ **Parent:** [Measure theory](measure-theory.md)

If two measures agree on a generating $\pi$-system and the space is a countable union of members having finite common measure, then they agree on the generated $\sigma$-algebra.

### Lebesgue measure

↑ **Parent:** [Sigma-finite uniqueness theorem for measures](#sigma-finite-uniqueness-theorem-for-measures)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_measure)

Lebesgue measure on the [real numbers](arithmetic.md#real-number) extends interval length: $\lambda([a,b])=b-a$ for $a\leq b$. Its restriction to the [Borel sigma-algebra](#borel-sigma-algebra) is the unique translation-invariant [sigma-finite measure](#sigma-finite-measure) on that [sigma-algebra](#sigma-algebra) normalized by $\lambda((0,1])=1$. The full [Lebesgue measure](#lebesgue-measure) is the [completion of a measure](#completion-of-a-measure) of this restriction; its domain is the [Lebesgue measurable sets](#lebesgue-measurable-set). Translation invariance follows by comparing a translated [Borel measure](#borel-measure) on half-open intervals and applying the [uniqueness theorem for measures](#sigma-finite-uniqueness-theorem-for-measures). For the construction and interval properties, see [MIT lecture 8](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/1bf275c0667d3e903e4de22b9fb4481b_MIT18_102s21_lec8.pdf).

Every [singleton](set.md#singleton-mathematics) has [Lebesgue measure](#lebesgue-measure) zero: $\{x\}\subseteq[x-\varepsilon,x+\varepsilon]$ gives $0\leq\lambda(\{x\})\leq2\varepsilon$ for every $\varepsilon>0$. Enumerating the [countable set](set-theory.md#countable-set) $\mathbb Q\cap[0,1]$ and applying [countable additivity](#countable-additivity) yields

$$
\lambda(\mathbb Q\cap[0,1])=\sum_{n=1}^{\infty}\lambda(\{q_n\})=0,
\qquad\lambda([0,1])=1.
$$

Thus a [dense set](topology.md#dense-set) can be a [null set](#null-set), and a [union](set.md#set-union) of [null sets](#null-set) indexed by an [uncountable set](set-theory.md#uncountable-set) can have positive [Lebesgue measure](#lebesgue-measure). The distinction explains both the [Dirichlet function](real-analysis.md#dirichlet-function) example and why [almost everywhere](#almost-everywhere) is weaker than everywhere.

#### Null-set limsup cover by finite arc families

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)

For any circle null set and any positive sequence $\epsilon_j$, take infinitely many countable covers with summable total lengths. Regard their arcs as a two-index array. Choose increasing finite-square cutoffs so the length sum outside each square is smaller than the next desired bound. The finite square annuli then give finite arc families with the stated small lengths. Every point belongs to some arc in every row, hence to infinitely many annular families. This handles dense and nonclosed null sets without claiming that they have finite small covers.

#### Compact batching of a small open set

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)

An open subset of the circle can be covered by countably many closed subarcs with disjoint interiors. Grouping a fixed enumeration into finite batches gives compact sets covering every point of the open set. By taking each finite batch long enough, the remaining total measure can be forced below any prescribed positive sequence tending to zero. This controls the measure of subsequent batches without assuming that a prescribed null subset is itself a countable union of compact null sets.

#### Inner regularity of Lebesgue measure

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)

The [Lebesgue measure](#lebesgue-measure) of a measurable set is the supremum of the measures of its compact subsets. In particular, an open set of finite positive measure contains a compact subset with at least half its measure. Together with a finite subcover, this turns a finite [Wiener covering lemma](#wiener-covering-lemma) estimate into an estimate for arbitrary open superlevel sets.

<h4 id="sierpinski-set">Sierpiński set</h4>

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sierpiński_set)

An uncountable [subset](set.md#subset) $S$ of the [real numbers](arithmetic.md#real-number) whose intersection with every [null set](#null-set) for [Lebesgue measure](#lebesgue-measure) is countable. Testing only [Borel sets](#borel-set) suffices because every Lebesgue-null [set](set.md) has a Borel null superset. No measurability of $S$ is assumed.

#### Divisibility of Lebesgue measure

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)

If $E\subseteq[0,1]$ is a [Lebesgue measurable set](#lebesgue-measurable-set) and $0\leq b\leq\lambda(E)$, some measurable [subset](set.md#subset) $B\subseteq E$ has [Lebesgue measure](#lebesgue-measure) $b$. The function $F(t)=\lambda(E\cap[0,t])$ has [Lipschitz continuity](real-analysis.md#lipschitz-continuity) with constant $1$, starts at $0$ and ends at $\lambda(E)$; the [intermediate value theorem](calculus.md#intermediate-value-theorem) proves the assertion. Applying the assertion successively to remaining portions of $E$ gives pairwise disjoint measurable pieces with any finite list of nonnegative measures whose sum is at most $\lambda(E)$. This is a concrete consequence of [non-atomic measure](#non-atomic-measure) structure, which fails for general [measures](#measure) containing an [atom of a measure](#atom-measure-theory).

#### Completeness of Lebesgue measure

↑ **Parent:** [Lebesgue measure](#lebesgue-measure)

Every subset of a [Lebesgue-null](#lebesgue-measure) set is [Lebesgue measurable](#lebesgue-measurable-set) and has measure zero.

## Bochner integral

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bochner_integral)

The Bochner integral integrates a strongly measurable function taking values in a [Banach space](banach-space.md). It is obtained as a norm limit of integrals of simple vector-valued functions and satisfies the usual linearity and norm bound.

### Mean-square integral

↑ **Parent:** [Bochner integral](#bochner-integral)

An ordinary time integral of [random variables](random-variable.md) taken in the [L2 space](#l2-space-is-a-hilbert-space) of the underlying [probability space](probability-theory.md#probability-space). Under strong measurability and $\int_a^b(\mathbb E|X_t|^2)^{1/2}dt<\infty$, it exists as a [Bochner integral](#bochner-integral); for a mean-square continuous process it is also the limit of [Riemann sums](real-analysis.md#riemann-sum) in that space. If the process is centered and the covariance is integrable, [Fubini's theorem](#fubini-s-theorem) gives

$$
\operatorname{Var}\left(\int_a^bX_tdt\right)=\int_a^b\int_a^b\operatorname{Cov}(X_u,X_v)\,du\,dv.
$$

For a [Gaussian process](stochastic-process.md#gaussian-process), the integral is a [Gaussian random variable](probability-theory.md#gaussian-random-variable), by approximating it in mean square by finite linear combinations of jointly [Gaussian random variables](probability-theory.md#gaussian-random-variable).

### Barycenter of a measure on a Banach space

↑ **Parent:** [Bochner integral](#bochner-integral)

For a [probability measure](probability-theory.md#probability-measure) whose identity map is strongly measurable with integrable norm, its barycenter is the [Bochner integral](#bochner-integral) of that map. It is characterized by $\varphi(b(\mu))=\int\varphi(x)\,d\mu(x)$ for every [continuous linear functional](topological-vector-space.md#continuous-linear-functional). For a measure on a [weakly compact set](weak-topology.md#weakly-compact-set) in a [separable Banach space](banach-space.md#separable-banach-space), its barycenter belongs to the norm-closed [convex hull](mathematical-optimization.md#convex-hull) of that set.

### Strongly measurable function

↑ **Parent:** [Bochner integral](#bochner-integral)

A function into a [Banach space](banach-space.md) is strongly measurable if, outside a null set, it is a pointwise norm limit of measurable simple functions. A [measurable function](#measurable-function) with values in a separable [Banach space](banach-space.md) is strongly measurable: approximate values by a countable collection of balls of shrinking radii and then truncate the resulting countably valued approximants to simple functions. A strongly measurable function is [Bochner integral](#bochner-integral) integrable exactly when its norm is integrable. Finite second [moments](probability-theory.md#moment) under a [probability measure](probability-theory.md#probability-measure) therefore imply existence of its [Bochner integral](#bochner-integral) [expected value](probability-theory.md#expected-value) by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality).

## Essential supremum

↑ **Parent:** [Measure theory](measure-theory.md)

The [essential supremum](#essential-supremum) is the upper bound for a [measurable function](#measurable-function) after disregarding [null sets](#null-set) for a specified [measure](#measure) $\mu$. Its definition is

$$
\operatorname{ess\,sup}_\mu f=\inf\{M\in\mathbb R:\mu(\{x:f(x)>M\})=0\},
$$

with values allowed in the [extended real number line](arithmetic.md#extended-real-number-line). A [supremum](real-analysis.md#supremum) controls every value; an [essential supremum](#essential-supremum) controls values [almost everywhere](#almost-everywhere). It therefore depends on the chosen [measure](#measure), as well as on the [function](function.md). [Hunter, Measure Theory, Definition 7.3: essential supremum](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch7.pdf).

For a worked example, use [Lebesgue measure](#lebesgue-measure) on $[0,1]$ and put

$$
f(x)=\begin{cases}10,&x=1/2,\\x,&x\ne1/2.\end{cases}
$$

Its [supremum](real-analysis.md#supremum) is ten, attained at $1/2$. But **its [essential supremum](#essential-supremum) is one**: $f\leq1$ outside the [singleton](set.md#singleton-mathematics) $\{1/2\}$, which is a [null set](#null-set). Every candidate $M<1$ fails, because the [interval](real-analysis.md#interval-mathematics) $(\max(0,M),1)$ has positive [Lebesgue measure](#lebesgue-measure) and includes values larger than $M$; changing one point cannot remove that interval. In particular, $\mu(\{f>0.8\})=0.2$, while $\mu(\{f>1\})=0$.

<a id="image-a-supremum-sees-an-isolated-exceptional-value-an-essential-supremum-depends-on-positive-measure"></a>
![](essential-bounds-ignore-null-sets.png)

**[Figure 8](#image-a-supremum-sees-an-isolated-exceptional-value-an-essential-supremum-depends-on-positive-measure). A supremum sees an isolated exceptional value; an essential supremum depends on positive measure**. Left: $f(1/2)=10$, with the ordinary value $1/2$ excluded at that input. Right: a zoom shows that values above $0.8$ still occur on an [interval](real-analysis.md#interval-mathematics) of [Lebesgue measure](#lebesgue-measure) $0.2$. The isolated value at ten lies outside the zoom. Thus the [essential supremum](#essential-supremum) is one, despite the pointwise [supremum](real-analysis.md#supremum) being ten.

Why is this useful? [Lebesgue integrals](#lebesgue-integral) ignore changes on [null sets](#null-set), and [Lp spaces](#lp-space) identify [functions](function.md) that agree [almost everywhere](#almost-everywhere). The [L-infinity norm](real-analysis.md#l-infinity-norm) uses $\operatorname{ess\,sup}|f|$ so it respects that identification. For this nonnegative example the [supremum norm](functional-analysis.md#supremum-norm) is ten and the [L-infinity norm](real-analysis.md#l-infinity-norm) is one; replacing $f(1/2)$ by $1/2$ changes the former while leaving the latter unchanged. [Hunter, Measure Theory, Definition 7.4: the L-infinity norm](https://www.math.ucdavis.edu/~hunter/measure_theory/measure_notes_ch7.pdf).

The [measure](#measure) qualification is essential. For $\mu=\delta_{1/2}$, the [Dirac measure](#dirac-measure) concentrated at the exceptional input, that [singleton](set.md#singleton-mathematics) has [measure](#measure) one and this [function](function.md) has [essential supremum](#essential-supremum) ten. A set ignored by one [measure](#measure) need not be ignored by another. The lower counterpart is the [essential infimum](real-analysis.md#essential-infimum), with $\operatorname{ess\,inf}f=-\operatorname{ess\,sup}(-f)$.

## Lp space

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lp_space)

The space $L^p$ consists of measurable functions with finite $p$-norm, identified when they agree almost everywhere. This quotient is necessary because the integral seminorm vanishes on functions supported on null sets.

### L1 space

↑ **Parent:** [Lp space](#lp-space)

The [Lp space](#lp-space) for $p=1$ consists of equivalence classes of [integrable functions](#lebesgue-integrable-function), with [L1 norm](functional-analysis.md#l1-norm) $\|f\|_1=\int|f|d\mu$. [Conditional expectation](#conditional-expectation) is a contraction in this norm. Convergence in this space is [L1 convergence](convergence-of-random-variables.md#convergence-in-l1), which controls the change in every integral over a [measurable](#measurability) subset.

### Sum of Lp spaces

↑ **Parent:** [Lp space](#lp-space)

The sum consists of [measurable functions](#measurable-function) $f=g+h$ with $g\in L^{p_0}$ and $h\in L^{p_1}$, with [norm](functional-analysis.md#norm) $\inf_{f=g+h}(\|g\|_{p_0}+\|h\|_{p_1})$. It is a [Banach space](banach-space.md). One construction identifies it with the quotient of $L^{p_0}\oplus_1L^{p_1}$ by the closed kernel of the addition map. Bounded endpoint operators are therefore bounded on the corresponding sum spaces.

#### Threshold decomposition between Lp spaces

↑ **Parent:** [Sum of Lp spaces](#sum-of-lp-spaces)

If $p_0<p<p_1$, the displayed split of an $L^p$ function gives $\|g\|_{p_0}\leq a^{1-p/p_0}\|f\|_p^{p/p_0}$ and $\|h\|_{p_1}\leq a^{1-p/p_1}\|f\|_p^{p/p_1}$. Weighted multiplication with $1/p=(1-\theta)/p_0+\theta/p_1$ cancels the threshold, yielding $\|g\|_{p_0}^{1-\theta}\|h\|_{p_1}^{\theta}\leq\|f\|_p$. Choosing $a=\|f\|_p$ also gives the continuous inclusion $\|f\|_{L^{p_0}+L^{p_1}}\leq2\|f\|_p$. The analogous split works if the larger endpoint is infinity.

### Sine sequence is not Cauchy in the integral norm

↑ **Parent:** [Lp space](#lp-space)

On $[0,1]$, the [continuous functions](calculus.md#continuous-function) $f_n(x)=\sin(nx)$ do not form a [Cauchy sequence](real-analysis.md#cauchy-sequence) in the [Lp space](#lp-space) with $p=1$. Put $d_n=f_n-f_{2n}$. The identity $\int_0^1d_n^2\,dx=1-\sin(2n)/(4n)-\sin(4n)/(8n)-\sin n/n+\sin(3n)/(3n)$ tends to $1$. Since $|d_n|\leq2$, one has $\int_0^1|d_n|\,dx\geq\frac12\int_0^1d_n^2\,dx$, which stays bounded away from zero. Thus arbitrarily late pairs are separated in the integral [norm](functional-analysis.md#norm); in particular the sequence cannot converge in that [norm](functional-analysis.md#norm).

### Translation continuity in Lp on a locally compact group

↑ **Parent:** [Lp space](#lp-space)

For left [Haar measure](#haar-measure), $T_xf(t)=f(x^{-1}t)$ is an isometry on $L^p(G)$, $1\leq p<\infty$. For compactly supported continuous functions, uniform continuity on a slightly enlarged compact support proves norm continuity. Approximation by those functions and the triangle inequality extend it to all $L^p$. The continuous image of a compact set of translation parameters is consequently compact in $L^p$.

### Derivative of a power of the Lp norm

↑ **Parent:** [Lp space](#lp-space)

For $1<p<\infty$ and $u,v$ in an [Lp space](#lp-space), the derivative with respect to the real scalar $t$ has the displayed form; the integrand is zero where $u=0$. The pointwise [chain rule](calculus.md#chain-rule) gives the derivative, while the [Holder inequality](functional-analysis.md#holder-inequality) makes $(|u|+|v|)^{p-1}|v|$ integrable and permits the [dominated convergence theorem](#dominated-convergence-theorem). This variational derivative characterizes nearest points to [closed](topology.md#closed-set) [convex sets](mathematical-optimization.md#convex-set) and constructs the [Lp duality](continuous-dual-space.md#lp-duality-on-an-arbitrary-measure-space) density of a [bounded linear functional](topological-vector-space.md#continuous-linear-functional).

### Closest point theorem for a closed convex subset of Lp

↑ **Parent:** [Lp space](#lp-space)

For $2\le p<\infty$, a nonempty [closed](topology.md#closed-set) [convex set](mathematical-optimization.md#convex-set) $K$ in an [Lp space](#lp-space) has exactly one nearest point to every $f$. A [minimizing sequence](calculus-of-variations.md#minimizing-sequence) $g_j$ is a [Cauchy sequence](real-analysis.md#cauchy-sequence): the [Clarkson inequality](banach-space.md#clarkson-s-inequalities) bounds $\|g_j-g_k\|_p^p$ by $2^{p-1}(\|g_j-f\|_p^p+\|g_k-f\|_p^p)-2^pd^p$, where $d$ is the infimum of the distances. [Completeness of Lp spaces](#completeness-of-lp-spaces) and the [closed set](topology.md#closed-set) property give a limit in $K$. Applying the same inequality to two minimizers proves uniqueness. Nonemptiness is essential.

### Completeness of Lp spaces

↑ **Parent:** [Lp space](#lp-space)

From an [Lp norm](real-analysis.md#lp-norm) Cauchy sequence choose a subsequence with successive difference norms at most $2^{-j}$. [Minkowski inequality](real-analysis.md#minkowski-inequality) and [monotone convergence theorem](#monotone-convergence-theorem) make the sum of the absolute differences an $L^p$ function, hence finite almost everywhere. The telescoping series defines an $L^p$ limit; the geometric bound on its tail proves norm convergence of the subsequence, and the original Cauchy property proves convergence of the whole sequence. No sigma-finiteness assumption is needed.

### Weak Lq space

↑ **Parent:** [Lp space](#lp-space)

For $1<q<\infty$, the weak Lq space consists of measurable functions for which $A_q(f)=\sup_{t>0}t|\{|f|>t\}|^{1/q}$ is finite. This distribution-function expression is a [quasi-norm](functional-analysis.md#quasi-norm). The equivalent norm $N_q(f)=\sup_{0<|E|<\infty}|E|^{-1/q'}\int_E|f|$ satisfies $A_q\leq N_q\leq q'A_q$, with $q'=q/(q-1)$. The [layer cake representation](functional-analysis.md#layer-cake-representation) bounds the integral by $\int_0^\infty\min(|E|,(A_q/t)^q)dt=q'A_q|E|^{1/q'}$. The lower bound uses finite-measure subsets of a superlevel set.

#### Integral norm for weak Lq

↑ **Parent:** [Weak Lq space](#weak-lq-space)

The integral expression for the [weak Lq space](#weak-lq-space) is homogeneous, positive definite up to equality almost everywhere, and obeys the [triangle inequality](topological-analysis.md#triangle-inequality) by integrating $|f+g|\leq|f|+|g|$ over each set. Its exponent is $-1/q'$, not $-1/q$. The sharp comparison constant with the distribution-function quasi-norm is $q'$; the power function $x^{-1/q}$ on $(0,\infty)$ attains that ratio on initial intervals.

### Mixed Lebesgue norm

↑ **Parent:** [Lp space](#lp-space)

A [mixed Lebesgue norm](#mixed-lebesgue-norm) first takes the [Lp norm](real-analysis.md#lp-norm) in one variable and then the norm in another. For finite $p,q$, $\|f\|_{L_x^pL_v^q}=(\int(\int|f(x,v)|^q\,dv)^{p/q}dx)^{1/p}$; an infinite exponent replaces that integral norm by an [essential supremum](#essential-supremum). The order matters: generally $L_x^pL_v^q$ and $L_v^qL_x^p$ are different spaces. This distinction is crucial in [free transport dispersion](partial-differential-equation.md#free-transport-dispersion).

### Locally square-integrable function

↑ **Parent:** [Lp space](#lp-space)

A measurable [function](function.md) belongs to $L^2_{\mathrm{loc}}(U)$ when its squared absolute value has finite integral on every compact subset of $U$. Functions are identified if they agree almost everywhere. This is a local integrability condition, not a specified global [Hilbert space](hilbert-space.md) [norm](functional-analysis.md#norm). For example, $x$ belongs to $L^2_{\mathrm{loc}}(\mathbb R)$ but its mean-square averages on expanding intervals diverge.

### Translation continuity in Lp

↑ **Parent:** [Lp space](#lp-space)

For $1\leq p<\infty$ and $f\in L^p(\mathbb R^d)$, translations converge to $f$ in the [Lp space](#lp-space) [norm](functional-analysis.md#norm). First prove this for continuous compactly supported [functions](function.md), using uniform continuity and a common bounded support. Their density in [Lp space](#lp-space), together with the norm-preserving translation map and the [triangle inequality](topological-analysis.md#triangle-inequality), proves the assertion for arbitrary $f$. It implies convergence of averages over shrinking intervals, a basic [approximate identity](fourier-analysis.md#approximate-identity) argument. The corresponding assertion fails for general $L^\infty$ functions, such as an [indicator function](#indicator-function) with a jump.

### Translation continuity in L1 on the circle

↑ **Parent:** [Lp space](#lp-space)

For $f\in L^1(\mathbb T,m)$ with $m$ normalized [Lebesgue measure](#lebesgue-measure), translation on the [circle group](lie-theory.md#circle-group) is continuous in the [L1 norm](functional-analysis.md#l1-norm): $\|f(\cdot+t)-f\|_1\to0$ as $t\to0$ modulo one. Approximate $f$ in the [L1 norm](functional-analysis.md#l1-norm) by a continuous function, use its [uniform continuity](topological-analysis.md#uniform-continuity), and use translation invariance to preserve the approximation error. In particular, $m(B\mathbin\triangle(B-t))\to0$ for every measurable $B$.

### Lp norms converge to the supremum norm

↑ **Parent:** [Lp space](#lp-space)

On a measure space of finite measure, a bounded measurable function satisfies the displayed limit, where the right side is the [essential supremum](#essential-supremum) of its absolute value. The upper estimate is $\|f\|_p\leq\mu(X)^{1/p}\|f\|_\infty$. For every $a<\|f\|_\infty$, the set where $|f|>a$ has positive measure, giving the reverse limiting estimate. For a continuous function on an open Euclidean domain, the [essential supremum](#essential-supremum) equals the ordinary supremum. Finiteness of the measure is part of this statement.

#### Moment ratios converge to the essential supremum

↑ **Parent:** [Lp norms converge to the supremum norm](#lp-norms-converge-to-the-supremum-norm)

For a bounded measurable function with positive essential supremum on a finite measure space, put $M_n=\int|f|^n$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) makes these moments log-convex, so successive ratios are nondecreasing. Their product satisfies $M_n/M_0\leq(M_{n+1}/M_n)^n$, while each ratio is at most the [essential supremum](#essential-supremum). Positive-measure level sets arbitrarily close to that supremum make $\mu(E)^{-1/n}\|f\|_n$ converge to it. Squeezing then proves the ratio limit.

### Lp interpolation inequality

↑ **Parent:** [Lp space](#lp-space)

If $1\leq p,r\leq\infty$, $0\leq\theta\leq1$ and $1/q=\theta/p+(1-\theta)/r$, then the displayed bound follows by applying the [Holder inequality](functional-analysis.md#holder-inequality) to $|u|^{\theta q}|u|^{(1-\theta)q}$. Interpret the endpoint cases using the essential supremum. In particular convergence in [Lp space](#lp-space) and boundedness in a larger-exponent [Lp space](#lp-space) imply convergence at intermediate exponents.

#### Nonvanishing level-set bound between three Lp norms

↑ **Parent:** [Lp interpolation inequality](#lp-interpolation-inequality)

Suppose $1\le p<q<r<\infty$, $\|f\|_p\le C_p$, $\|f\|_q\ge C_q>0$ and $\|f\|_r\le C_r$. Set $\varepsilon=(C_q^q/(2C_p^p))^{1/(q-p)}$. The part of $\int|f|^q$ where $|f|\le\varepsilon$ is at most $\varepsilon^{q-p}C_p^p=C_q^q/2$. On the complementary [level set](topology.md#level-set), the [Holder inequality](functional-analysis.md#holder-inequality) bounds the integral by $C_r^q\mu\{|f|>\varepsilon\}^{1-q/r}$, proving the bound. For $r=\infty$ the bound becomes $C_q^q/(2C_r^q)$. The lower-exponent bound prevents spreading into low amplitudes, while the higher-exponent bound prevents concentration into arbitrarily narrow spikes.

### Square-integrable function

↑ **Parent:** [Lp space](#lp-space)

A [measurable function](#measurable-function) is square-integrable when the [integral](calculus.md#integral) of its squared absolute value is finite. Its equivalence class belongs to the [L2 space](#l2-space-is-a-hilbert-space); on a [probability space](probability-theory.md#probability-space), this means a finite second [moment](probability-theory.md#moment).

### L2 space is a Hilbert space

↑ **Parent:** [Lp space](#lp-space)

The space $L^2(X,\mathcal F,\nu)$ consists of almost-everywhere equivalence classes of measurable functions with $\int|f|^2\,d\nu<\infty$. The inner product

$$
\langle f,g\rangle=\int f\overline g\,d\nu
$$

induces its norm, and the [Riesz-Fischer theorem](#riesz-fischer-theorem) makes it complete; hence it is a [Hilbert space](hilbert-space.md).

#### Exponentially weighted L2 space

↑ **Parent:** [L2 space is a Hilbert space](#l2-space-is-a-hilbert-space)

The exponentially weighted [Hilbert space](hilbert-space.md) consists of measurable functions with $\int_{\mathbb R}|u(x)|^2e^{2\gamma x}\,dx<\infty$. Multiplication by $e^{\gamma x}$ is a unitary map onto [L2 space](#l2-space-is-a-hilbert-space). Requiring unweighted square integrability as well produces an intersection that is incomplete under the weighted norm alone. For example, $\mathbf1_{[-N,0]}$ is a weighted [Cauchy sequence](real-analysis.md#cauchy-sequence) for $\gamma>0$, but its weighted limit $\mathbf1_{(-\infty,0]}$ is not in unweighted [L2 space](#l2-space-is-a-hilbert-space).

##### Weighted essential spectrum of a Fisher travelling front

↑ **Parent:** [Exponentially weighted L2 space](#exponentially-weighted-l2-space)

The [linearization](algebra.md#linearization) at a [travelling wave](analysis.md#travelling-wave) $w_c$ is $A=\partial_z^2+c\partial_z+k-2w_c$. Conjugation by $e^{\gamma z}$ changes this to $\partial_z^2+(c-2\gamma)\partial_z+\gamma^2-c\gamma+k-2w_c$. The choice $\gamma=c/2$ removes the first derivative and makes the operator [self-adjoint](linear-operator-theory.md#self-adjoint-operator). Its two limiting potentials are $-k-c^2/4$ and $k-c^2/4$, so [essential-spectrum invariance under relatively compact perturbations](functional-analysis.md#essential-spectrum-invariance-under-relatively-compact-perturbations) gives $\sigma_{\mathrm{ess}}=(-\infty,k-c^2/4]$. This lies strictly below zero for $c>2\sqrt{k}$ but touches zero at the critical speed. Stability of this [essential spectrum](functional-analysis.md#essential-spectrum-of-a-closed-operator) alone is not a general nonlinear stability theorem.

#### Mean-zero L2 space

↑ **Parent:** [L2 space is a Hilbert space](#l2-space-is-a-hilbert-space)

The mean-zero L2 space is the kernel of the [bounded linear functional](topological-vector-space.md#continuous-linear-functional) $h\mapsto Ph$ on [L2 space](#l2-space-is-a-hilbert-space) for a [probability measure](probability-theory.md#probability-measure) $P$. It is a [closed subspace of a Hilbert space](hilbert-space.md#closed-subspace-of-a-hilbert-space), with [inner product](linear-algebra.md#inner-product) $P(hk)$, and is the natural ambient space for [score functions](statistical-modelling.md#informant-function) and [canonical gradients](statistical-inference.md#canonical-gradient).

#### L2 inner product

↑ **Parent:** [L2 space is a Hilbert space](#l2-space-is-a-hilbert-space)

The L2 inner product is the [inner product](linear-algebra.md#inner-product) $\langle f,g\rangle=\int f\overline g\,d\mu$ on [L2 space](#l2-space-is-a-hilbert-space). Its induced [norm](functional-analysis.md#norm) is the [L2 norm](real-analysis.md#l2-norm), and the [mass matrix](numerical-analysis.md#mass-matrix) represents it in a [finite element](numerical-analysis.md#finite-element) basis.

### Riesz-Fischer theorem

↑ **Parent:** [Lp space](#lp-space)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riesz-Fischer_theorem)

For $1\leq p\leq\infty$, the Lebesgue space $L^p$ is complete in its usual norm.

### Banach intersection of L1 and L2

↑ **Parent:** [Lp space](#lp-space)

The intersection $L^1\cap L^2$ is Banach for $\lVert f\rVert_1+\lVert f\rVert_2$, but it is generally incomplete when equipped with the $L^1$ norm alone. Truncations of an $L^1$ function outside $L^2$ provide an $L^1$-Cauchy sequence with no limit in the intersection.

## Approximation by nonnegative simple functions

↑ **Parent:** [Measure theory](measure-theory.md)

Every nonnegative measurable function is the pointwise increasing limit of nonnegative simple functions, and its integral is the supremum of their integrals.

## Monotone convergence theorem

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Monotone_convergence_theorem)

If nonnegative measurable functions satisfy $f_n\uparrow f$ almost everywhere, then $\int f_n\uparrow\int f$, allowing the value infinity.

### Moving-spike obstruction to interchanging a limit and an infinite sum

↑ **Parent:** [Monotone convergence theorem](#monotone-convergence-theorem)

Let $f(t,n)=\mathbf1_{[n,n+1)}(t)$ for $t\geq1$. For every fixed $n$, $f(t,n)\to0$ as $t\to\infty$, but $\sum_nf(t,n)=1$ for every $t\geq1$. Pointwise convergence without monotonicity or domination therefore does not justify interchanging a limit and an infinite sum.

## Dominated convergence theorem

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dominated_convergence_theorem)

If $f_n\to f$ almost everywhere and $|f_n|\leq g$ for one integrable function $g$, then $f$ is integrable and $\int|f_n-f|\to0$.

## Bounded convergence theorem

↑ **Parent:** [Measure theory](measure-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bounded_convergence_theorem)

On a [finite measure](#finite-measure) space, if measurable functions are uniformly bounded and converge pointwise, then their integrals converge. This is the [dominated convergence theorem](#dominated-convergence-theorem) with a constant dominating function.

## Tonelli theorem

↑ **Parent:** [Measure theory](measure-theory.md)

Tonelli’s theorem permits interchange of integrals for a nonnegative measurable function, even before finiteness is known.

## Mutually singular measures

↑ **Parent:** [Measure theory](measure-theory.md)

Two measures are mutually singular when the underlying space splits into disjoint measurable sets on which the respective measures are concentrated.

### Density level sets separate a singular measure

↑ **Parent:** [Mutually singular measures](#mutually-singular-measures)

Suppose a finite nonnegative [measure](#measure) has finite-level densities $Y_n$ with respect to a [probability](probability-theory.md#probability) [measure](#measure) $\lambda$. The event $\{Y_n\leq\varepsilon\}$ belongs to that level's [sigma-algebra](#sigma-algebra), so its [measure](#measure) is $\int\mathbf1_{\{Y_n\leq\varepsilon\}}Y_n\,d\lambda\leq\varepsilon$. The set where nonnegative $Y_n$ tends to zero is contained in the eventual occurrence of every such level event; it therefore has [measure](#measure) at most $\varepsilon$ for every $\varepsilon>0$, hence zero. If the same limit set has full $\lambda$-measure, the two [measures](#measure) are singular.

## Absolute continuity of measures

↑ **Parent:** [Measure theory](measure-theory.md)

A measure $\nu$ is absolutely continuous with respect to $\mu$, written $\nu\ll\mu$, when every $\mu$-null measurable set is also $\nu$-null. This is distinct from the regularity property of functions called [absolute continuity](sobolev-space.md#absolutely-continuous-function).

A measure $\nu$ is absolutely continuous with respect to $\mu$ when every $\mu$-null set is also $\nu$-null.

### Dominating measure

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

A measure $\rho$ dominates a family of measures when every member is [absolutely continuous](#absolute-continuity-of-measures) with respect to $\rho$. Any two finite positive measures $\mu$ and $\nu$ have the common dominating measure $\mu+\nu$.

### Lusin condition N

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

A function $f$ has Lusin's condition $(N)$ when it maps every [Lebesgue-null](#lebesgue-measure) set to a Lebesgue-null set.

### Image-length measure of a strictly increasing continuous function

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

Let $h:\mathbb R\to\mathbb R$ be [continuous](calculus.md#continuous-function), [strictly increasing](calculus.md#strictly-increasing-function), and satisfy [Lusin condition N](#lusin-condition-n). Then

$$
\nu(A)=\lambda(h(A))
$$

defines a [measure](#measure) on the [Lebesgue measurable sets](#lebesgue-measurable-set), and $\nu\ll\lambda$. Moreover,

$$
\nu([a,b])=h(b)-h(a)
$$

for $a\leq b$.

### Uniform absolute continuity for a finite measure

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

If $\mu(\Omega)<\infty$, then $\mu\ll\nu$ exactly when for every $\varepsilon>0$ there is $\delta>0$ such that $\nu(A)<\delta$ implies $\mu(A)<\varepsilon$. For necessity, a contrary sequence with $\nu(A_n)<2^{-n}$ and $\mu(A_n)\geq\varepsilon$ has tail unions decreasing to a $\nu$-null limsup; continuity from above for finite $\mu$ contradicts absolute continuity.

### Mutually absolutely continuous measures

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

Two measures are mutually absolutely continuous when they have exactly the same null sets.

#### Equivalent probability measure

↑ **Parent:** [Mutually absolutely continuous measures](#mutually-absolutely-continuous-measures)

Two [probability measures](probability-theory.md#probability-measure) are equivalent when each is [absolutely continuous](#absolute-continuity-of-measures) with respect to the other, or equivalently when they have the same null events.

### Radon-Nikodym theorem

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radon-Nikodym_theorem)

For sigma-finite measures, $\nu\ll\mu$ implies $\nu(A)=\int_A(d\nu/d\mu)d\mu$ for a nonnegative measurable density unique almost everywhere.

#### Hilbert-space construction of dominated measure densities

↑ **Parent:** [Radon-Nikodym theorem](#radon-nikodym-theorem)

For finite [positive measures](#positive-measure) $\mu,\nu$, put $\rho=\mu+\nu$. The [linear functional](linear-algebra.md#linear-functional) $g\mapsto\int g\,d\nu$ is bounded on real $L^2(\rho)$ by the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). The [Riesz representation theorem](hilbert-space.md#riesz-representation-theorem) gives a measurable $h$ with $\nu(A)=\int_Ah\,d\rho$. Testing indicators of its negative and greater-than-one level sets shows $0\le h\le1$ almost everywhere. Subtraction gives $\mu(A)=\int_A(1-h)\,d\rho$. This constructs the densities without assuming the [Radon-Nikodym theorem](#radon-nikodym-theorem) as a prior result.

#### Radon-Nikodym derivative

↑ **Parent:** [Radon-Nikodym theorem](#radon-nikodym-theorem)

When $\nu\ll\mu$, the Radon-Nikodym derivative is the almost-everywhere unique measurable function satisfying $\nu(A)=\int_A(d\nu/d\mu)d\mu$.

##### Radon-Nikodym density martingale

↑ **Parent:** [Radon-Nikodym derivative](#radon-nikodym-derivative)

For an absolutely continuous change of probability measure, restricting its [Radon-Nikodym derivative](#radon-nikodym-derivative) to the current sigma-algebra gives this nonnegative uniformly integrable [martingale](martingale.md). If $Z_T>0$ almost surely, the measures are equivalent on $\mathcal F_T$. This finite-horizon equivalence need not imply equivalence on a larger sigma-algebra.

#### Positive Radon-Nikodym derivative

↑ **Parent:** [Radon-Nikodym theorem](#radon-nikodym-theorem)

Mutual absolute continuity is equivalent to the Radon--Nikodym derivative being finite and strictly positive almost everywhere.

### Lebesgue decomposition theorem

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue_decomposition_theorem)

For sigma-finite measures $\nu$ and $\mu$, there is a unique decomposition $\nu=\nu_{\mathrm{ac}}+\nu_{\mathrm{s}}$ in which $\nu_{\mathrm{ac}}\ll\mu$ and $\nu_{\mathrm{s}}\perp\mu$.

#### Dyadic density martingale

↑ **Parent:** [Lebesgue decomposition theorem](#lebesgue-decomposition-theorem)

For a finite positive [measure](#measure) on $[0,1)$, average its mass over each half-open [dyadic interval](real-analysis.md#dyadic-interval). The resulting nonnegative [martingale](martingale.md) has constant [expectation](probability-theory.md#expected-value) $\mu([0,1))$: a parent interval's mass is the sum of its children's masses. Its almost-sure limit is integrable but the [martingale](martingale.md) need not be [uniformly integrable](convergence-of-random-variables.md#uniform-integrability). The limit recovers the density of the absolutely continuous component in the [Lebesgue decomposition theorem](#lebesgue-decomposition-theorem).

##### Martingale construction of Lebesgue decomposition

↑ **Parent:** [Dyadic density martingale](#dyadic-density-martingale)

The [Conditional Fatou lemma](#conditional-fatou-lemma) gives $X_n\geq\mathbb E[X_\infty\mid\mathcal F_n]$ for the [dyadic density martingale](#dyadic-density-martingale). Integration first on dyadic sets, then extension by the [Monotone class theorem](#monotone-class-theorem), makes $\nu=\mu-X_\infty\lambda$ a nonnegative [measure](#measure). Its finite-level density is $Y_n=X_n-\mathbb E[X_\infty\mid\mathcal F_n]$, which tends to zero almost everywhere for [Lebesgue measure](#lebesgue-measure). The [density level sets separate a singular measure](#density-level-sets-separate-a-singular-measure) argument shows that this zero-limit set has $\nu$-measure zero. Thus $\nu$ and $\lambda$ are [mutually singular measures](#mutually-singular-measures), obtaining the decomposition without assuming it to identify the [martingale](martingale.md) limit.

#### Lebesgue decomposition from a sum-measure density

↑ **Parent:** [Lebesgue decomposition theorem](#lebesgue-decomposition-theorem)

Use the [Hilbert-space construction of dominated measure densities](#hilbert-space-construction-of-dominated-measure-densities) with $\rho=\mu+\nu$. The set $B=\{h=1\}$ is a [null set](#null-set) for $\mu$. Put $f=0$ on $B$ and $f=h/(1-h)$ elsewhere. Then $\int f\,d\mu=\nu(B^c)<\infty$ and $\nu(A)=\int_Af\,d\mu+\nu(A\cap B)$. This is the [Lebesgue decomposition](#lebesgue-decomposition-theorem) into a density part and a part concentrated on a $\mu$-[null set](#null-set).

### Dominating mixture measure

↑ **Parent:** [Absolute continuity of measures](#absolute-continuity-of-measures)

A countable family of probability measures is dominated by any mixture $\sum_nw_n\nu_n$ with every $w_n>0$ and $\sum_nw_n=1$.

## Lebesgue-Stieltjes measure

↑ **Parent:** [Measure theory](measure-theory.md)

An increasing right-continuous function $F:\mathbb R\to\mathbb R$ determines a measure by

$$
\mu_F((a,b])=F(b)-F(a).
$$

The [Radon-Nikodym theorem](#radon-nikodym-theorem) and [Lebesgue differentiation theorem](#lebesgue-differentiation-theorem) identify the density of the absolutely continuous part of this measure with $F'$ almost everywhere.

<h3 id="lebesgue-stieltjes-integration">Lebesgue–Stieltjes integration</h3>

↑ **Parent:** [Lebesgue-Stieltjes measure](#lebesgue-stieltjes-measure)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lebesgue–Stieltjes_integration)

The Lebesgue–Stieltjes integral $\int f\,dF$ integrates $f$ against the [Lebesgue-Stieltjes measure](#lebesgue-stieltjes-measure) generated by an increasing right-continuous function $F$. An atom at $x$ contributes $f(x)\Delta F(x)$.

## Lp inclusion on a finite measure space

↑ **Parent:** [Measure theory](measure-theory.md)

On a finite measure space, $L^q\subseteq L^p$ for $0<p<q\leq\infty$. For $1\leq p<q<\infty$, [Hölder's inequality](functional-analysis.md#holder-inequality) gives

$$
\lVert f\rVert_p
\leq\mu(X)^{1/p-1/q}\lVert f\rVert_q,
$$

with the same formula interpreted as $\lVert f\rVert_p\leq\mu(X)^{1/p}\lVert f\rVert_\infty$ when $q=\infty$.

### Almost-everywhere convergent subsequence from Lp convergence

↑ **Parent:** [Lp inclusion on a finite measure space](#lp-inclusion-on-a-finite-measure-space)

If $f_n\to f$ in $L^p$ for $1\leq p<\infty$, choose a subsequence with $\lVert f_{n_k}-f\rVert_p^p\leq2^{-k}$. Tonelli's theorem makes $\sum_k|f_{n_k}-f|^p$ finite almost everywhere, so $f_{n_k}\to f$ almost everywhere. For $p=\infty$, norm convergence itself gives almost-everywhere convergence after removing one common null set.

### Lq inclusion implies finite measure on a Euclidean Borel subset

↑ **Parent:** [Lp inclusion on a finite measure space](#lp-inclusion-on-a-finite-measure-space)

Let $X\subseteq\mathbb R^n$ be Borel. If $L^q(X)\subseteq L^p(X)$ for $1\leq p<q\leq\infty$, the [closed graph theorem](functional-analysis.md#closed-graph-theorem) makes the inclusion continuous. Applying its norm bound to indicators of $X\cap B(0,R)$ shows that their measures are uniformly bounded, hence $\mu(X)<\infty$.

### Power singularity integrability

↑ **Parent:** [Lp inclusion on a finite measure space](#lp-inclusion-on-a-finite-measure-space)

On $(0,1)$, $x^{-a}$ is integrable exactly when $a<1$, providing sharp counterexamples between finite-measure $L^p$ spaces.

## ↑ Ancestors (5)

1. [Real analysis](real-analysis.md)
2. [Analysis](analysis.md)
3. [Area of mathematics](mathematics.md#area-of-mathematics)
4. [Mathematics](mathematics.md)
5. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Cantor set](geometry-and-topology.md#cantor-set)
- [Convex conjugate of a constrained quadratic](convex-optimization.md#convex-conjugate-of-a-constrained-quadratic)
- [Kolmogorov axioms](probability-theory.md#kolmogorov-axioms)
- [Lebesgue integration](calculus.md#lebesgue-integration)
