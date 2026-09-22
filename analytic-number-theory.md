# Analytic number theory

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Analytic_number_theory)

Analytic number theory studies [integers](number-theory.md#integer), [prime numbers](number-theory.md#prime-number), and [arithmetic functions](number-theory.md#arithmetic-function) using tools from [real analysis](real-analysis.md) and [complex analysis](complex-analysis.md), especially [Dirichlet series](#dirichlet-series) and their singularities.

**Table of contents**

- [Hardy-Littlewood circle method](#hardy-littlewood-circle-method)
  - [Vinogradov's three-primes theorem](#vinogradov-s-three-primes-theorem)
  - [Singular series](#singular-series)
  - [Minor arc](#minor-arc)
  - [Major arc](#major-arc)
- [L-function](#l-function)
  - [Hasse–Weil zeta function](#hasse-weil-zeta-function)
  - [Hasse-Weil L-function](#hasse-weil-l-function)
  - [Hecke L-function](#hecke-l-function)
  - [p-adic L-function](#p-adic-l-function)
    - [Kubota-Leopoldt p-adic L-function](#kubota-leopoldt-p-adic-l-function)
      - [p-adic zeta pseudomeasure](#p-adic-zeta-pseudomeasure)
- [Linnik's theorem](#linnik-s-theorem)
- [Character sum](#character-sum)
  - [Pólya–Vinogradov inequality](#polya-vinogradov-inequality)
- [Prime sum](#prime-sum)
- [Bombieri–Vinogradov theorem](#bombieri-vinogradov-theorem)
  - [Weighted arithmetic-progression error bound](#weighted-arithmetic-progression-error-bound)
- [Exponential sum](#exponential-sum)
  - [Weyl differencing](#weyl-differencing)
    - [Weyl inequality](#weyl-inequality)
    - [Cubic Weyl inequality](#cubic-weyl-inequality)
    - [Hua's lemma](#hua-s-lemma)
      - [Cubic eighth-moment proof by differencing](#cubic-eighth-moment-proof-by-differencing)
  - [Power Gauss sum over a prime field](#power-gauss-sum-over-a-prime-field)
    - [Three power summands over a large prime field](#three-power-summands-over-a-large-prime-field)
  - [Quadratic exponential sum](#quadratic-exponential-sum)
    - [Quadratic Weyl inequality](#quadratic-weyl-inequality)
  - [Vinogradov mean value](#vinogradov-mean-value)
    - [Vinogradov mean-value method for a bilinear exponential sum](#vinogradov-mean-value-method-for-a-bilinear-exponential-sum)
  - [Bilinear shift averaging for a logarithmic phase](#bilinear-shift-averaging-for-a-logarithmic-phase)
  - [Van der Corput sum-integral lemma](#van-der-corput-sum-integral-lemma)
  - [Cancellation in an exponential sum](#cancellation-in-an-exponential-sum)
- [Probabilistic number theory](#probabilistic-number-theory)
  - [Erdős-Kac theorem](#erdos-kac-theorem)
    - [Centered moment comparison for additive arithmetic functions](#centered-moment-comparison-for-additive-arithmetic-functions)
  - [Cramér model](#cramer-model)
    - [Cramér model prime-gap upper bound](#cramer-model-prime-gap-upper-bound)
  - [Multiplication table problem](#multiplication-table-problem)
    - [Multiplication table bound from distinct prime factors](#multiplication-table-bound-from-distinct-prime-factors)
  - [Turán-Kubilius inequality](#turan-kubilius-inequality)
- [Landau theorem for a Dirichlet series with nonnegative coefficients](#landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients)
- [Nonvanishing of a nonprincipal Dirichlet L-function at one](#nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one)
- [Chebyshev function in an arithmetic progression](#chebyshev-function-in-an-arithmetic-progression)
- [Classical zero-free region for Dirichlet L-functions](#classical-zero-free-region-for-dirichlet-l-functions)
  - [Uniqueness of a possible exceptional real Dirichlet zero](#uniqueness-of-a-possible-exceptional-real-dirichlet-zero)
  - [Siegel zero](#siegel-zero)
    - [Landau theorem for two real Dirichlet characters](#landau-theorem-for-two-real-dirichlet-characters)
      - [Sparse conductors of exceptional real Dirichlet zeros](#sparse-conductors-of-exceptional-real-dirichlet-zeros)
    - [Prime number theorem in an arithmetic progression with an exceptional zero](#prime-number-theorem-in-an-arithmetic-progression-with-an-exceptional-zero)
      - [Exceptional-zero bound from a uniform upper bound in arithmetic progressions](#exceptional-zero-bound-from-a-uniform-upper-bound-in-arithmetic-progressions)
- [Pretentious number theory](#pretentious-number-theory)
- [Normal order of an arithmetic function](#normal-order-of-an-arithmetic-function)
  - [Turán normal-order theorem for distinct prime divisors](#turan-normal-order-theorem-for-distinct-prime-divisors)
- [Dirichlet's theorem on arithmetic progressions](#dirichlet-s-theorem-on-arithmetic-progressions)
  - [Reciprocal primes in a fixed arithmetic progression](#reciprocal-primes-in-a-fixed-arithmetic-progression)
  - [Siegel–Walfisz theorem](#siegel-walfisz-theorem)
    - [Major-arc value of the prime exponential sum](#major-arc-value-of-the-prime-exponential-sum)
  - [Prime-character sum near one](#prime-character-sum-near-one)
- [Harmonic number](#harmonic-number)
- [Abel's summation formula](#abel-s-summation-formula)
  - [Reciprocal-sum convergence from a counting bound](#reciprocal-sum-convergence-from-a-counting-bound)
  - [Bounded-variation multipliers of a convergent series](#bounded-variation-multipliers-of-a-convergent-series)
  - [Exponentially damped reciprocal-prime sum](#exponentially-damped-reciprocal-prime-sum)
- [Reciprocal fractional-part sum near a rational](#reciprocal-fractional-part-sum-near-a-rational)
- [Bilinear quadratic exponential sum fourth-moment bound](#bilinear-quadratic-exponential-sum-fourth-moment-bound)
  - [Factorized fourth moment for a bilinear quadratic exponential sum](#factorized-fourth-moment-for-a-bilinear-quadratic-exponential-sum)
    - [Truncation of a divisor weight by its second moment](#truncation-of-a-divisor-weight-by-its-second-moment)
- [Bilinear sum](#bilinear-sum)
  - [Vinogradov Type I–II method](#vinogradov-type-i-ii-method)
    - [Small Type I and Type II sums](#small-type-i-and-type-ii-sums)
  - [Fourier separation of interval cutoffs](#fourier-separation-of-interval-cutoffs)
  - [Bilinear cancellation for badly approximable phases](#bilinear-cancellation-for-badly-approximable-phases)
  - [Type II sum](#type-ii-sum)
    - [Rational-phase Type II estimate](#rational-phase-type-ii-estimate)
  - [Type I sum](#type-i-sum)
  - [Dyadic decomposition](#dyadic-decomposition)
- [Sieve theory](#sieve-theory)
  - [Parity problem](#parity-problem)
  - [Integers with all prime factors congruent to one modulo four](#integers-with-all-prime-factors-congruent-to-one-modulo-four)
  - [Large sieve](#large-sieve)
    - [Large sieve upper bound for sifted intervals](#large-sieve-upper-bound-for-sifted-intervals)
    - [Character large sieve](#character-large-sieve)
    - [Variance form of the large sieve](#variance-form-of-the-large-sieve)
    - [Exponential-sum large sieve](#exponential-sum-large-sieve)
      - [Fejér-kernel proof of the analytic large sieve](#fejer-kernel-proof-of-the-analytic-large-sieve)
      - [Local-multiplicity large sieve](#local-multiplicity-large-sieve)
        - [Prime-denominator large sieve](#prime-denominator-large-sieve)
    - [Circular spacing](#circular-spacing)
  - [Buchstab function](#buchstab-function)
    - [Oscillation of the Buchstab function](#oscillation-of-the-buchstab-function)
    - [Buchstab theorem](#buchstab-theorem)
  - [Rough number](#rough-number)
  - [Sifting function](#sifting-function)
    - [Sieve distribution](#sieve-distribution)
    - [Buchstab identity](#buchstab-identity)
  - [Upper-bound sieve](#upper-bound-sieve)
    - [Brun–Titchmarsh theorem](#brun-titchmarsh-theorem)
    - [Selberg sieve](#selberg-sieve)
      - [Selberg upper-bound sieve](#selberg-upper-bound-sieve)
        - [Uniform interval bound from optimal Selberg weights](#uniform-interval-bound-from-optimal-selberg-weights)
        - [Half-dimensional interval sieve](#half-dimensional-interval-sieve)
        - [Selberg sieve weights](#selberg-sieve-weights)
          - [Selberg sieve denominator asymptotic](#selberg-sieve-denominator-asymptotic)
          - [Selberg sieve diagonalization](#selberg-sieve-diagonalization)
            - [Selberg least-common-multiple weights](#selberg-least-common-multiple-weights)
            - [Optimal Selberg weights have modulus at most one](#optimal-selberg-weights-have-modulus-at-most-one)
        - [Polynomial root density in a sieve](#polynomial-root-density-in-a-sieve)
          - [Elementary lower bound for the twin-prime sieve denominator](#elementary-lower-bound-for-the-twin-prime-sieve-denominator)
          - [Twin-prime upper bound from a quadratic sieve](#twin-prime-upper-bound-from-a-quadratic-sieve)
          - [Prime-tuple upper bound from the Selberg sieve](#prime-tuple-upper-bound-from-the-selberg-sieve)
        - [Almost-primes from an upper-bound sieve and Buchstab identity](#almost-primes-from-an-upper-bound-sieve-and-buchstab-identity)
        - [Fourier representation of a smooth Selberg weight](#fourier-representation-of-a-smooth-selberg-weight)
          - [Smooth divisor-square sieve asymptotic](#smooth-divisor-square-sieve-asymptotic)
            - [Euler product for a smoothed divisor-square correlation](#euler-product-for-a-smoothed-divisor-square-correlation)
            - [Derivative energy constant for a smooth sieve cutoff](#derivative-energy-constant-for-a-smooth-sieve-cutoff)
          - [Short-interval prime upper bound from a smooth divisor weight](#short-interval-prime-upper-bound-from-a-smooth-divisor-weight)
    - [Dimension-three upper-bound sieve](#dimension-three-upper-bound-sieve)
- [Mertens' theorems](#mertens-theorems)
  - [Mertens first theorem](#mertens-first-theorem)
    - [Square-root logarithmic sum over primes](#square-root-logarithmic-sum-over-primes)
    - [Positive logarithmic moments of reciprocal primes](#positive-logarithmic-moments-of-reciprocal-primes)
    - [Factorial proof of Mertens first theorem](#factorial-proof-of-mertens-first-theorem)
    - [Logarithmically weighted reciprocal-prime tail](#logarithmically-weighted-reciprocal-prime-tail)
  - [Mertens second theorem](#mertens-second-theorem)
    - [Reciprocal-prime sum in residue class one modulo four](#reciprocal-prime-sum-in-residue-class-one-modulo-four)
  - [Mertens third theorem](#mertens-third-theorem)
    - [Totient lower bound from the Mertens product](#totient-lower-bound-from-the-mertens-product)
- [Dirichlet series](#dirichlet-series)
  - [Holomorphy of a Dirichlet series from bounded partial sums](#holomorphy-of-a-dirichlet-series-from-bounded-partial-sums)
  - [Epstein zeta function](#epstein-zeta-function)
    - [Completed Epstein zeta function](#completed-epstein-zeta-function)
      - [Pole-subtracted theta integral for an Epstein zeta function](#pole-subtracted-theta-integral-for-an-epstein-zeta-function)
  - [Dirichlet polynomial](#dirichlet-polynomial)
    - [Mean value of Dirichlet polynomials](#mean-value-of-dirichlet-polynomials)
      - [Odd moment of a prime cosine sum](#odd-moment-of-a-prime-cosine-sum)
  - [Euler product](#euler-product)
    - [Euler product positivity for L-function nonvanishing](#euler-product-positivity-for-l-function-nonvanishing)
    - [Truncated Euler-product lower bound](#truncated-euler-product-lower-bound)
    - [Euler proof that the sum of reciprocals of primes diverges](#euler-proof-that-the-sum-of-reciprocals-of-primes-diverges)
      - [Prime reciprocal lower bound](#prime-reciprocal-lower-bound)
    - [Three-four-one inequality for Euler products](#three-four-one-inequality-for-euler-products)
  - [Perron's formula](#perron-s-formula)
    - [Logarithmically smoothed Perron formula](#logarithmically-smoothed-perron-formula)
      - [Unsmoothing a logarithmically weighted sum](#unsmoothing-a-logarithmically-weighted-sum)
    - [Truncated Perron formula](#truncated-perron-formula)
      - [Short-interval Perron bound for the second Chebyshev function](#short-interval-perron-bound-for-the-second-chebyshev-function)
      - [Truncated Perron kernel estimate](#truncated-perron-kernel-estimate)
- [Riemann zeta function](#riemann-zeta-function)
  - [Reciprocal Dirichlet-series bound on boundary-zero multiplicity](#reciprocal-dirichlet-series-bound-on-boundary-zero-multiplicity)
  - [Reciprocal zeta bounds near the line one](#reciprocal-zeta-bounds-near-the-line-one)
  - [Three-four-one product proof of zeta boundary nonvanishing](#three-four-one-product-proof-of-zeta-boundary-nonvanishing)
  - [Lindelöf hypothesis](#lindelof-hypothesis)
  - [Truncated Möbius inverse identity for the Riemann zeta function](#truncated-mobius-inverse-identity-for-the-riemann-zeta-function)
  - [Richert bound for the Riemann zeta function](#richert-bound-for-the-riemann-zeta-function)
  - [Hardy-Littlewood approximation to the Riemann zeta function](#hardy-littlewood-approximation-to-the-riemann-zeta-function)
  - [Fractional-part continuation formula for the Riemann zeta function](#fractional-part-continuation-formula-for-the-riemann-zeta-function)
  - [Completed Riemann zeta function](#completed-riemann-zeta-function)
    - [Riemann xi function](#riemann-xi-function)
      - [Order-one growth of the Riemann xi function](#order-one-growth-of-the-riemann-xi-function)
      - [Real logarithmic derivative of Riemann xi](#real-logarithmic-derivative-of-riemann-xi)
        - [Absolute convergence of the real xi logarithmic derivative](#absolute-convergence-of-the-real-xi-logarithmic-derivative)
  - [Trivial zero of the Riemann zeta function](#trivial-zero-of-the-riemann-zeta-function)
  - [Fourth moment of the Riemann zeta function](#fourth-moment-of-the-riemann-zeta-function)
  - [Bernoulli formula for zeta values at nonpositive integers](#bernoulli-formula-for-zeta-values-at-nonpositive-integers)
  - [Meromorphic continuation of the Riemann zeta function to the right half-plane](#meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane)
  - [Basel problem](#basel-problem)
  - [Functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function)
    - [Mellin representation of the completed Riemann zeta function](#mellin-representation-of-the-completed-riemann-zeta-function)
      - [Pole-subtracted theta integral for the completed zeta function](#pole-subtracted-theta-integral-for-the-completed-zeta-function)
    - [Vertical-strip factor in the Riemann zeta functional equation](#vertical-strip-factor-in-the-riemann-zeta-functional-equation)
  - [Euler-product nonvanishing of the Riemann zeta function](#euler-product-nonvanishing-of-the-riemann-zeta-function)
  - [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function)
    - [Critical strip](#critical-strip)
      - [Critical line](#critical-line)
    - [Riemann hypothesis](#riemann-hypothesis)
      - [Riemann hypothesis implies the Lindelöf hypothesis](#riemann-hypothesis-implies-the-lindelof-hypothesis)
      - [Subpower zeta bound to the right of the critical line](#subpower-zeta-bound-to-the-right-of-the-critical-line)
      - [Xi modulus criterion for the Riemann hypothesis](#xi-modulus-criterion-for-the-riemann-hypothesis)
      - [Riemann hypothesis equivalence for the second Chebyshev function](#riemann-hypothesis-equivalence-for-the-second-chebyshev-function)
    - [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)
      - [Vinogradov-Korobov zero-free region](#vinogradov-korobov-zero-free-region)
      - [Landau zero-free-region theorem](#landau-zero-free-region-theorem)
      - [Weak logarithmic zero-free region for the Riemann zeta function](#weak-logarithmic-zero-free-region-for-the-riemann-zeta-function)
      - [Three-four-one zero-free-region argument](#three-four-one-zero-free-region-argument)
      - [Logarithmic derivative inside the zeta zero-free region](#logarithmic-derivative-inside-the-zeta-zero-free-region)
    - [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula)
      - [Infinitely many reciprocal-logarithmic gaps between zeta zeros](#infinitely-many-reciprocal-logarithmic-gaps-between-zeta-zeros)
      - [Asymptotic inversion of the zeta zero count](#asymptotic-inversion-of-the-zeta-zero-count)
      - [Local zero count for the Riemann zeta function](#local-zero-count-for-the-riemann-zeta-function)
        - [Jensen disk proof of the zeta zero-count bound](#jensen-disk-proof-of-the-zeta-zero-count-bound)
        - [Smoothed zeta zero-count bound](#smoothed-zeta-zero-count-bound)
  - [Logarithmic derivative](#logarithmic-derivative)
    - [Global partial-fraction expansion of the zeta logarithmic derivative](#global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative)
    - [Local logarithmic-derivative lemma](#local-logarithmic-derivative-lemma)
    - [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](#local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative)
    - [Prime number theorem](#prime-number-theorem)
      - [Prime number theorem error from a fixed zero-free strip](#prime-number-theorem-error-from-a-fixed-zero-free-strip)
      - [Prime number theorem error from a logarithmic zero-free region](#prime-number-theorem-error-from-a-logarithmic-zero-free-region)
      - [Prime number theorem with classical zero-free-region error](#prime-number-theorem-with-classical-zero-free-region-error)
      - [Smoothed prime number theorem from a zero-free region](#smoothed-prime-number-theorem-from-a-zero-free-region)
    - [Twisted Von Mangoldt estimate implying the Riemann hypothesis](#twisted-von-mangoldt-estimate-implying-the-riemann-hypothesis)
  - [Dirichlet eta function](#dirichlet-eta-function)
    - [Analytic continuation of the Riemann zeta function to the right half-plane](#analytic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane)

## Hardy-Littlewood circle method

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

The circle method represents a weighted additive count as an integral of products of [exponential sums](#exponential-sum) against a character. Near rationals with small denominator, [major arcs](#major-arc) produce a structured main term involving a [singular series](#singular-series) and an archimedean singular integral. Away from those rationals, [minor arcs](#minor-arc) require cancellation bounds. The partition and approximation estimates depend on the problem; a formal integral alone is not a positivity proof.

<h3 id="vinogradov-s-three-primes-theorem">Vinogradov's three-primes theorem</h3>

↑ **Parent:** [Hardy-Littlewood circle method](#hardy-littlewood-circle-method)

Every sufficiently large odd integer is a sum of three primes, with repetitions allowed. The weighted count is asymptotic to $\mathfrak S(n)n^2/2$. [Siegel–Walfisz theorem](#siegel-walfisz-theorem) controls the [major arcs](#major-arc), and Type I/II estimates for the prime [exponential sum](#exponential-sum) make the [minor arcs](#minor-arc) negligible. Removing prime-power contributions gives genuine prime representations. This is the sufficiently-large theorem, not by itself a proof for every small odd integer.

### Singular series

↑ **Parent:** [Hardy-Littlewood circle method](#hardy-littlewood-circle-method)

A singular series assembles the local congruence densities in an additive counting asymptotic. For three prime summands it is $\sum_{q\ge1}\mu(q)c_q(n)/\varphi(q)^3$, with [Ramanujan sum](algebra.md#ramanujan-sum) $c_q(n)$. Its Euler product vanishes for even $n$ and has a uniform positive lower bound for odd $n$. Different additive problems have different local factors, so this is a specific instance rather than a universal formula.

### Minor arc

↑ **Parent:** [Hardy-Littlewood circle method](#hardy-littlewood-circle-method)

Minor arcs are the complement of the specified [major arcs](#major-arc). They contribute an error only when a suitable pointwise or mean-value cancellation estimate is proved; their name does not imply that their measure is small.

### Major arc

↑ **Parent:** [Hardy-Littlewood circle method](#hardy-littlewood-circle-method)

In a circle-method problem of scale $n$, major arcs are neighborhoods of reduced rational points $a/q$ with small denominator, where the relevant [exponential sum](#exponential-sum) is approximated using distribution in residue classes. For the three-prime problem one may take $q\le(\log n)^B$ and $|\theta-a/q|\le(\log n)^B/n$, with suitably fixed $B$.

## L-function

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

An L-function is an arithmetic function given initially by a [Dirichlet series](#dirichlet-series) and often an [Euler product](#euler-product), with analytic continuation and a functional equation in important cases. [Dirichlet L-functions](algebraic-number-theory.md#dirichlet-l-function) and [L-functions of cusp forms](modular-function.md#l-function-of-a-cusp-form) are basic examples; [p-adic L-functions](#p-adic-l-function) interpolate suitably modified special values.

<h3 id="hasse-weil-zeta-function">Hasse–Weil zeta function</h3>

↑ **Parent:** [L-function](#l-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hasse–Weil_zeta_function)

The Hasse–Weil zeta function of an [algebraic variety](algebraic-geometry.md#algebraic-variety) over a [number field](algebraic-number-theory.md#number-field) is assembled from local point-counting factors at finite places. At a good place with residue field of size $q$, the factor is $Z(V_q,q^{-s})$, where $Z(V_q,T)=\exp(\sum_{n\geq1}\#V_q(\mathbb F_{q^n})T^n/n)$. Defining all bad-place factors requires a specified integral model or convention. The [zeta function of an elliptic curve over a finite field](normalization-of-an-algebraic-curve.md#zeta-function-of-an-elliptic-curve-over-a-finite-field) is a local factor, rather than this global product.

### Hasse-Weil L-function

↑ **Parent:** [L-function](#l-function)

For an [elliptic curve](normalization-of-an-algebraic-curve.md#elliptic-curve) over a [number field](algebraic-number-theory.md#number-field), its Hasse-Weil L-function is the product of the local factors determined by its [Tate module](representation-theory.md#tate-module). At a good finite place, the factor is $(1-a_vNv^{-s}+Nv^{1-2s})^{-1}$, with $a_v=Nv+1-\#E(\kappa(v))$. At a bad place use the inertia-invariant subspace and an auxiliary prime different from the residue characteristic. For a [CM elliptic curve](algebraic-geometry.md#cm-elliptic-curve) with all endomorphisms defined over the base, this factors as the product of the two conjugate [Hecke L-functions](#hecke-l-function).

### Hecke L-function

↑ **Parent:** [L-function](#l-function)

The [L-function](#l-function) of a [Hecke character](algebraic-number-theory.md#hecke-character) is initially the displayed [Euler product](#euler-product) over prime ideals away from its conductor. The equivalent [Dirichlet series](#dirichlet-series) sums $\psi(\mathfrak a)N\mathfrak a^{-s}$ over integral ideals prime to the conductor. For a [CM elliptic curve](algebraic-geometry.md#cm-elliptic-curve) with its endomorphisms defined over the base, its [Hasse-Weil L-function](#hasse-weil-l-function) factors into the two conjugate Hecke L-functions.

### p-adic L-function

↑ **Parent:** [L-function](#l-function)

A p-adic L-function is a $p$-adic analytic function or measure interpolating suitably adjusted special values of an [L-function](#l-function). The [Kubota-Leopoldt p-adic L-function](#kubota-leopoldt-p-adic-l-function) is the basic example attached to a [Dirichlet character](algebraic-number-theory.md#dirichlet-character).

#### Kubota-Leopoldt p-adic L-function

↑ **Parent:** [p-adic L-function](#p-adic-l-function)

For an even [Dirichlet character](algebraic-number-theory.md#dirichlet-character) $\chi$, the Kubota-Leopoldt function interpolates generalized Bernoulli values with the relevant Euler factor and [Teichmüller character](arithmetic.md#teichmuller-character) adjustment. If $\chi\ne1$, it can be encoded by an integral power series. For $u=1+p$, the $p$-ramified convention is $g_\chi(u^{1-s}-1)=L_p(\chi,s)$. The trivial character requires separate treatment of the pole.

##### p-adic zeta pseudomeasure

↑ **Parent:** [Kubota-Leopoldt p-adic L-function](#kubota-leopoldt-p-adic-l-function)

On $G=\mathbb Z_p^\times/\{\pm1\}$, this element of the total quotient ring of the [Iwasawa algebra](associative-algebra.md#iwasawa-algebra) becomes an integral measure after multiplication by every difference $[a]-[1]$. Its even moments interpolate the displayed Euler-corrected zeta values. Its trivial-character component has a pole, so the pseudomeasure itself must not be treated as an element of the integral group algebra. Multiplication by the [augmentation ideal](commutative-algebra.md#augmentation-ideal) removes the pole.

<h2 id="linnik-s-theorem">Linnik's theorem</h2>

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linnik's_theorem)

There is an absolute finite exponent $L$ bounding the least [prime](number-theory.md#prime-number) in any reduced arithmetic progression by a constant times $q^L$. The [multiplicative large sieve inequality](#character-large-sieve) is one of the tools in proofs of this theorem.

## Character sum

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Character_sum)

A sum of character values over a set. Arithmetic cancellation, rather than the termwise absolute-value bound, is the useful feature. A [Gauss sum of a Dirichlet character](algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) is a weighted example, and the [Pólya–Vinogradov inequality](#polya-vinogradov-inequality) bounds interval sums.

<h3 id="polya-vinogradov-inequality">Pólya–Vinogradov inequality</h3>

↑ **Parent:** [Character sum](#character-sum)

For a primitive nonprincipal [Dirichlet character](algebraic-number-theory.md#dirichlet-character) modulo $q$, finite [Fourier inversion theorem](fourier-analysis.md#fourier-inversion-theorem) and the primitive Gauss magnitude give this bound uniformly in the interval. Bound the exponential sums by $C\|a/q\|^{-1}$ and sum the resulting [harmonic series](real-analysis.md#harmonic-series). The general Gauss identity follows from the prime-power identity by the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem).

## Prime sum

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

A prime sum is a [summation](arithmetic.md#summation) indexed by [prime numbers](number-theory.md#prime-number), for example $\sum_{p\leq x}1/p$. The indexing restriction distinguishes it from a sum over all [positive integers](number-theory.md#positive-integer).

<h2 id="bombieri-vinogradov-theorem">Bombieri–Vinogradov theorem</h2>

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bombieri–Vinogradov_theorem)

For every $A>0$ there is $B>0$ such that, for $Q\leq x^{1/2}/\log^Bx$,

$$
\sum_{q\leq Q}\max_{(a,q)=1}\max_{2\leq y\leq x}\left|\psi(y;q,a)-\frac y{\phi(q)}\right|\ll_A\frac{x}{\log^Ax}.
$$

Here $\psi(y;q,a)$ is the [Chebyshev function in an arithmetic progression](#chebyshev-function-in-an-arithmetic-progression) and $\phi$ is the [Euler totient function](number-theory.md#euler-totient-function). [Partial summation](#abel-s-summation-formula) gives the corresponding result for the [prime-counting function](number-theory.md#prime-counting-function) and the offset [logarithmic integral function](calculus.md#logarithmic-integral-function). The theorem controls the total error over many moduli; it need not give the same bound for each individual modulus.

### Weighted arithmetic-progression error bound

↑ **Parent:** [Bombieri–Vinogradov theorem](#bombieri-vinogradov-theorem)

Let $E_q=\max_{(a,q)=1}|\pi(x;q,a)-\operatorname{Li}(x)/\phi(q)|$. For $Q\leq x^{1-\eta}$, the [Brun–Titchmarsh theorem](#brun-titchmarsh-theorem) and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\sum_{q\leq Q}3^{\omega(q)}E_q\ll_\eta\left(\sum_{q\leq Q}E_q\right)^{1/2}\left(\frac{x}{\log x}\sum_{q\leq Q}\frac{9^{\omega(q)}}{\phi(q)}\right)^{1/2}.
$$

Write each summand as $\sqrt{E_q}\,3^{\omega(q)}\sqrt{E_q}$, then use $E_q\ll_\eta x/(\phi(q)\log x)$.

## Exponential sum

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

A finite [sum](arithmetic.md#sum) of [complex exponentials](calculus.md#complex-exponential-function), such as $S(\theta)=\sum_n a_ne(n\theta)$ with $e(t)=\exp(2\pi it)$, is an exponential sum. [Cancellation in an exponential sum](#cancellation-in-an-exponential-sum) between its terms can make it much smaller than the [sum](arithmetic.md#sum) of their [absolute values](real-analysis.md#absolute-value).

### Weyl differencing

↑ **Parent:** [Exponential sum](#exponential-sum)

Taking a [finite difference](finite-difference.md) lowers the degree of a polynomial phase. For $S(\theta)=\sum_{x=1}^n e(\theta P(x))$, expand $|S|^2$ by shifts $h$ and apply the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) to those shift sums. This gives $|S|^4\le2n\sum_{h,l}\sum_{x\in I_{h,l}}e(\theta\Delta_h\Delta_lP(x))$, where $I_{h,l}$ enforces that $x,x+h,x+l,x+h+l$ lie in $[1,n]$. Although individual terms can be complex, the entire sum is real and nonnegative because it equals a sum of squares. For $P(x)=x^3$, the phase is $3hl(2x+h+l)$.

#### Weyl inequality

↑ **Parent:** [Weyl differencing](#weyl-differencing)

For a real degree-$k$ polynomial with leading coefficient $\theta$, $k\ge2$, and coprime integers $a,q$ satisfying $|\theta-a/q|\le q^{-2}$, the displayed bound applies to its [exponential sum](#exponential-sum) over $1\le n\le N$. Repeated [Weyl differencing](#weyl-differencing) reduces the phase to slope $k!\theta h_1\cdots h_{k-1}$. A geometric-sum estimate, the [subpower bound for the divisor function](number-theory.md#subpower-bound-for-the-divisor-function) and the [reciprocal fractional-part sum near a rational](#reciprocal-fractional-part-sum-near-a-rational) complete the estimate. The arbitrary positive exponent $\eta$ absorbs divisor bounds and logarithms.

#### Cubic Weyl inequality

↑ **Parent:** [Weyl differencing](#weyl-differencing)

If $S(\theta)=\sum_{x\le n}e(\theta x^3)$ and $|\theta-a/q|\le q^{-2}$ with $(a,q)=1$, the displayed estimate holds. Twice applying [Weyl differencing](#weyl-differencing) bounds $|S|^4$ by $O(n^3+n\sum_{0<|h|,|l|<n}\min(n,\|6\theta hl\|^{-1}))$. Group by $6hl$ and use the [subpower bound for the divisor function](number-theory.md#subpower-bound-for-the-divisor-function). The [reciprocal fractional-part sum near a rational](#reciprocal-fractional-part-sum-near-a-rational) bounds the resulting sum by $O(\log(2q)(n^3/q+n^2+n+q))$. Take fourth roots, absorbing logarithms into $n^\eta$ when $q\le n^3$; for larger $q$ the trivial bound suffices. [Leiden lecture notes, Section 7.2](https://pub.math.leidenuniv.nl/~evertsejh/ant20-7.pdf) develop this cubic differencing estimate.

<h4 id="hua-s-lemma">Hua's lemma</h4>

↑ **Parent:** [Weyl differencing](#weyl-differencing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hua's_lemma)

For $1\le j\le k$ and every $\eta>0$, the displayed estimate bounds a mean value of a polynomial [exponential sum](#exponential-sum). For cubes its eighth-moment bound is $O_\eta(n^{5+\eta})$. It complements pointwise [Weyl differencing](#weyl-differencing) estimates: a ninth moment over a region is bounded by its supremum there times this eighth moment. [Leiden lecture notes, Section 8.1](https://pub.math.leidenuniv.nl/~evertsejh/ant20-8.pdf) give the cubic formulation.

##### Cubic eighth-moment proof by differencing

↑ **Parent:** [Hua's lemma](#hua-s-lemma)

Write $S(\theta)=\sum_{x\le n}e(\theta x^3)$ and $I_j=\int_0^1|S|^j$. [Character orthogonality](representation-theory.md#character-orthogonality) gives $I_2=n$. For $I_4$, fix the difference $D=x^3-y^3$. If $D=0$, there are $n^2$ choices for the two equal pairs. If $D\ne0$, any solution $z^3-w^3=D$ has $z-w\mid D$; fixing this divisor gives a quadratic equation for $w$, hence at most two choices. The [subpower bound for the divisor function](number-theory.md#subpower-bound-for-the-divisor-function) yields $I_4\ll_\eta n^{2+\eta}$.

The twice-differenced inequality in [Weyl differencing](#weyl-differencing) reads $|S|^4\le2n\sum_v c_ve(\theta v)$, with $c_v$ counting triples $(h,l,x)$ for which $v=3hl(2x+h+l)$ and all four shifted arguments are in $[1,n]$. Thus $c_0\ll n^2$, and $c_v\ll_\eta n^\eta$ for $v\ne0$: the product $hl$ divides $v$, and the remaining equation determines $x$. The [Fourier coefficients](fourier-series.md#fourier-coefficient) $r(v)$ of $|S|^4$ are nonnegative counts, with $r(0)=I_4$ and $\sum_vr(v)=n^4$. Multiply the inequality by $|S|^4$ and integrate. It follows that $I_8\ll n(n^2I_4+n^\eta n^4)\ll_\eta n^{5+\eta}$, after choosing the divisor-bound exponents small enough.

### Power Gauss sum over a prime field

↑ **Parent:** [Exponential sum](#exponential-sum)

For $a\ne0$ in the [finite field](algebra.md#finite-field) $\mathbb F_p$, put $d=\gcd(k,p-1)$. The [multiplicative group of a finite field is cyclic](algebra.md#multiplicative-group-of-a-finite-field-is-cyclic), and [character orthogonality](representation-theory.md#character-orthogonality) expresses the number of $k$th roots of $y\ne0$ as $\sum_{\chi^d=1}\chi(y)$. The trivial [character](representation-theory.md#character-of-a-representation) contributes $-1$, cancelling the $x=0$ term. Each of the remaining $d-1$ [Gauss sums of Dirichlet characters](algebraic-number-theory.md#gauss-sum-of-a-dirichlet-character) has modulus $\sqrt p$, by the [prime-field character Gauss sum identity](algebraic-number-theory.md#prime-field-character-gauss-sum-identity). Consequently $|G_{a,p}|\le(d-1)/\sqrt p\le k/\sqrt p$.

#### Three power summands over a large prime field

↑ **Parent:** [Power Gauss sum over a prime field](#power-gauss-sum-over-a-prime-field)

For $S(a)=\sum_u e(au^k/p)$, [character orthogonality](representation-theory.md#character-orthogonality) counts representations of $x$ by $p^{-1}\sum_a S(a)^3e(-ax/p)$. Its zero-frequency term is $p^2$. The [power Gauss sum over a prime field](#power-gauss-sum-over-a-prime-field) bounds the other terms in total by $k^3p^{3/2}$, strictly less than $p^2$ when $p>k^6$. Every [residue class](number-theory.md#residue-class) therefore has a representation.

### Quadratic exponential sum

↑ **Parent:** [Exponential sum](#exponential-sum)

A quadratic exponential sum has a polynomial phase of degree two. Its multiplicative derivative at lag $h$ has the [linear phase](additive-combinatorics.md#linear-phase) $2\alpha hn$ up to a constant factor. This degree reduction lets the [Van der Corput inequality for finite scalar sequences](measure-theory.md#van-der-corput-inequality-for-finite-scalar-sequences) reduce its size to estimates for [finite geometric series](real-analysis.md#finite-geometric-series).

#### Quadratic Weyl inequality

↑ **Parent:** [Quadratic exponential sum](#quadratic-exponential-sum)

For [coprime integers](number-theory.md#coprime-integers) $a,q$ with $1\le q\le Q$ and $|\alpha-a/q|\le1/(qQ)$, expand the squared [quadratic exponential sum](#quadratic-exponential-sum) by its difference $h$. The [exponential geometric sum bound](real-analysis.md#exponential-geometric-sum-bound) gives $|S|^2\ll N+\sum_{h\le N}\min(N+1,\|2\alpha h\|^{-1})$. In each block of length at most $q/4$, the rotations $2\alpha h$ are separated by at least $1/(2q)$: the reduced denominator of $2a/q$ is at least $q/2$, and the approximation error between two block points is at most $1/(2q)$. The [separated reciprocal-distance sum](number-theory.md#separated-reciprocal-distance-sum) bounds each block by $O(N+q\log(2N))$. There are $O(N/q+1)$ blocks, giving the displayed inequality. For bounded $q$ the trivial estimate supplies the same conclusion.

### Vinogradov mean value

↑ **Parent:** [Exponential sum](#exponential-sum)

By [orthogonality of integer Fourier modes](fourier-series.md#orthogonality-of-integer-fourier-modes), this integral counts pairs of $k$-tuples with the same first $r$ power sums. Diagonal pairs give $J_{k,r}(Z)\gg Z^k$. There are $O_{k,r}(Z^{r(r+1)/2})$ possible moment vectors; the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives $J_{k,r}(Z)\gg Z^{2k-r(r+1)/2}$. Upper bounds measure how much arithmetic coincidence remains beyond these necessary contributions, and enter the [Vinogradov mean-value method for a bilinear exponential sum](#vinogradov-mean-value-method-for-a-bilinear-exponential-sum).

#### Vinogradov mean-value method for a bilinear exponential sum

↑ **Parent:** [Vinogradov mean value](#vinogradov-mean-value)

Expand moments of the inner sum and group equal power-sum differences. Their multiplicities are bounded by $J_{k,r}(Z)$ through the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality). Two applications of the [Holder inequality](functional-analysis.md#holder-inequality) yield a bound for $|U|^{4k^2}$ containing $Z^{8k^2-4k}J_{k,r}(Z)^2$ and a product of short geometric-sum bounds over the moment differences. Thus a sharp mean-value estimate combines with rational approximation or spacing of the coefficients to prove cancellation. When all coefficients are integers, $U=\lfloor Z\rfloor^2$, so mean-value estimates alone cannot force cancellation.

### Bilinear shift averaging for a logarithmic phase

↑ **Parent:** [Exponential sum](#exponential-sum)

Translating an integer interval by $xy$ changes a sum of unit-modulus terms by at most $2xy$. Averaging gives the displayed formula. For $n\asymp N$, $Z=N^{2/5}$, expand $-t\log(1+xy/n)$ to degree $r=\lfloor5.01\log t/\log N\rfloor$. Its remainder is at most $tN^{-(r+1)/5}<t^{-1/500}$. This reduces the logarithmic [exponential sum](#exponential-sum) to bilinear polynomial sums while keeping explicit boundary and approximation errors.

### Van der Corput sum-integral lemma

↑ **Parent:** [Exponential sum](#exponential-sum)

For a real $C^1$ phase with continuous [monotone](calculus.md#monotonic-function) derivative and $|f'|\le\delta<1$, the sum-integral discrepancy has the displayed uniform bound. Periodization and the [Dirichlet-Jordan convergence theorem](fourier-series.md#dirichlet-jordan-convergence-theorem) express it as symmetric nonzero [Fourier modes](fourier-analysis.md#fourier-mode). [Integration by parts](calculus.md#integration-by-parts) gives endpoint terms and reciprocal-derivative variations. Monotonicity bounds their total variation by $\sum_{h\ne0}2\delta/(h^2-\delta^2)=O((1-\delta)^{-1})$. Pairing the leading $1/h$ endpoint terms reduces them to the uniformly bounded sine series. The exclusion of integer nonzero frequencies is essential.

### Cancellation in an exponential sum

↑ **Parent:** [Exponential sum](#exponential-sum)

Cancellation occurs when different [complex numbers](complex-analysis.md#complex-number) in an [exponential sum](#exponential-sum) have directions that reduce the [absolute value](real-analysis.md#absolute-value) of their [sum](arithmetic.md#sum). For example, the [orthogonality of roots of unity](algebra.md#orthogonality-of-roots-of-unity) makes $\sum_{a=0}^{p-1}e(a/p)=0$ for every [integer](number-theory.md#integer) $p>1$, despite all terms having [absolute value](real-analysis.md#absolute-value) one.

## Probabilistic number theory

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Probabilistic_number_theory)

[Probabilistic number theory](#probabilistic-number-theory) studies [arithmetic functions](number-theory.md#arithmetic-function) and integer sets through [probability distributions](probability-theory.md#probability-distribution), concentration, and limit theorems.

<h3 id="erdos-kac-theorem">Erdős-Kac theorem</h3>

↑ **Parent:** [Probabilistic number theory](#probabilistic-number-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Erdős-Kac_theorem)

For a real [strongly additive arithmetic function](number-theory.md#strongly-additive-arithmetic-function) with uniformly bounded values on [primes](number-theory.md#prime-number), put $A(x)=\sum_{p\le x}f(p)/p$ and $B(x)^2=\sum_{p\le x}f(p)^2/p$. If $B(x)\to\infty$, then $(f(n)-A(N))/B(N)$ under uniform sampling from $[N]$ converges to the [standard normal distribution](probability-theory.md#standard-normal-distribution). For the [prime omega function](number-theory.md#prime-omega-function), the mean and variance scales are $\log\log N$.

#### Centered moment comparison for additive arithmetic functions

↑ **Parent:** [Erdős-Kac theorem](#erdos-kac-theorem)

If a [strongly additive arithmetic function](number-theory.md#strongly-additive-arithmetic-function) $g$ is supported on [primes](number-theory.md#prime-number) up to $y$, its $j$th uniform [central moment](probability-theory.md#central-moment) differs from the independent [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) model with probabilities $1/p$ by $O(jy^j(\sum_{p\le y}|g(p)|)^j/N)$. Expansion of divisibility [indicator functions](measure-theory.md#indicator-function) reduces the comparison to $\lfloor N/d\rfloor/N=1/d+O(1/N)$.

<h3 id="cramer-model">Cramér model</h3>

↑ **Parent:** [Probabilistic number theory](#probabilistic-number-theory)

The [Cramér model](#cramer-model) selects integers $n\ge3$ independently with probability $1/\log n$, and conventionally sets $U_1=0$, $U_2=1$. It is a random model for the distribution of [primes](number-theory.md#prime-number), not an assertion of independence for actual [prime numbers](number-theory.md#prime-number).

<h4 id="cramer-model-prime-gap-upper-bound">Cramér model prime-gap upper bound</h4>

↑ **Parent:** [Cramér model](#cramer-model)

If $P_n$ are the increasing selected integers in the [Cramér model](#cramer-model), then [almost surely](convergence-of-random-variables.md#almost-sure-convergence) $\limsup_n(P_{n+1}-P_n)/(\log P_n)^2\le1$. A zero block of length $(1+\epsilon)(\log k)^2$ after $k$ has summable probability, so the [Borel-Cantelli first lemma](probability-theory.md#borel-cantelli-first-lemma) excludes these blocks eventually.

### Multiplication table problem

↑ **Parent:** [Probabilistic number theory](#probabilistic-number-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplication_table_problem)

The [multiplication table problem](#multiplication-table-problem) asks how many distinct integers occur as $ab$ with $1\le a,b\le N$. Counting the $N^2$ pairs greatly overcounts the distinct products.

#### Multiplication table bound from distinct prime factors

↑ **Parent:** [Multiplication table problem](#multiplication-table-problem)

Concentration of the [prime omega function](number-theory.md#prime-omega-function) near $\log\log N$, together with $\omega(ab)=\omega(a)+\omega(b)-\omega(\gcd(a,b))$ and the bounded mean of $\omega(\gcd(a,b))$, gives $M(N)\ll N^2/\log\log N$. This elementary argument uses only distinct [prime factors](number-theory.md#prime-factor).

<h3 id="turan-kubilius-inequality">Turán-Kubilius inequality</h3>

↑ **Parent:** [Probabilistic number theory](#probabilistic-number-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Turán-Kubilius_inequality)

For an [additive arithmetic function](number-theory.md#additive-function-number-theory) $f$, $N^{-1}\sum_{n\le N}|f(n)-A_f(N)|^2\ll B_f(N)^2$, where $A_f$ is the [mean of an additive arithmetic function](number-theory.md#mean-of-an-additive-arithmetic-function) and $B_f(N)^2=\sum_{p^k\le N}|f(p^k)|^2/p^k$. The implied constant is absolute.

## Landau theorem for a Dirichlet series with nonnegative coefficients

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

If a [Dirichlet series](#dirichlet-series) with nonnegative coefficients has finite abscissa of convergence $\sigma_c$, then the function it defines has a singularity at the real point $s=\sigma_c$. Consequently, if that function extends holomorphically across every real point, the original series converges for every real $s$.

## Nonvanishing of a nonprincipal Dirichlet L-function at one

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

For every nonprincipal [Dirichlet character](algebraic-number-theory.md#dirichlet-character), $L(1,\chi)\ne0$. A nonreal character is covered by [Euler product positivity for L-function nonvanishing](#euler-product-positivity-for-l-function-nonvanishing) at height zero, since its squared character is nonprincipal.

For a real character, suppose $L(1,\chi)=0$. The simple zeta pole would cancel, making $F(s)=\zeta(s)L(s,\chi)$ an [entire function](complex-analysis.md#entire-function). Its [nonnegative zeta-times-real-L coefficients](algebraic-number-theory.md#nonnegative-zeta-times-real-l-coefficients) satisfy $a_n\ge0$ and $a_{m^2}\ge1$. Termwise derivatives at two give $(-1)^kF^{(k)}(2)=\sum_na_n(\log n)^kn^{-2}$. The [Taylor series](calculus.md#taylor-series) of this entire function at two converges at zero. Every term there is nonnegative, and [Tonelli theorem](measure-theory.md#tonelli-theorem) identifies its sum as

$$
F(0)=\sum_{k\ge0}\frac{2^k}{k!}\sum_n\frac{a_n(\log n)^k}{n^2}=\sum_na_n.
$$

The last series diverges because all square coefficients are at least one. This contradiction proves the claim. It is the positive-coefficient mechanism behind the more general [Landau theorem for a Dirichlet series with nonnegative coefficients](#landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients).

## Chebyshev function in an arithmetic progression

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

For $(a,q)=1$,

$$
\psi(x;q,a)
=\sum_{\substack{n\leq x\\n\equiv a\pmod q}}\Lambda(n).
$$

The [Orthogonality of Dirichlet characters](algebraic-number-theory.md#orthogonality-of-dirichlet-characters) expresses it in terms of character-twisted [Von Mangoldt functions](number-theory.md#von-mangoldt-function).

## Classical zero-free region for Dirichlet L-functions

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

There is an absolute $c>0$ such that the [Dirichlet L-functions](algebraic-number-theory.md#dirichlet-l-function) modulo $q$ have no zero in

$$
\Re s\geq1-\frac{c}{\log(q(|\Im s|+2))}
$$

apart from at most one real simple zero belonging to a real nonprincipal character.

### Uniqueness of a possible exceptional real Dirichlet zero

↑ **Parent:** [Classical zero-free region for Dirichlet L-functions](#classical-zero-free-region-for-dirichlet-l-functions)

For primitive real [nonprincipal Dirichlet characters](algebraic-number-theory.md#nonprincipal-dirichlet-character), there is an absolute $c>0$ with at most one zero in this interval, counted with multiplicity. Positivity of $-\zeta'/\zeta-L'/L$ and the local partial fractions give $0\le1/(\sigma-1)+C\log q-\sum(\sigma-\beta)^{-1}$. Testing $\sigma=1+a/\log q$ with small fixed $a$ rules out two nearby real zeros. Any possible zero is consequently simple; existence is not asserted.

### Siegel zero

↑ **Parent:** [Classical zero-free region for Dirichlet L-functions](#classical-zero-free-region-for-dirichlet-l-functions)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Siegel_zero)

An exceptional zero is the possible real simple zero $\beta$ omitted from the otherwise uniform [classical zero-free region for Dirichlet L-functions](#classical-zero-free-region-for-dirichlet-l-functions). It belongs to a real nonprincipal primitive [Dirichlet character](algebraic-number-theory.md#dirichlet-character) and satisfies $\beta<1$.

#### Landau theorem for two real Dirichlet characters

↑ **Parent:** [Siegel zero](#siegel-zero)

For two real primitive nonprincipal [Dirichlet characters](algebraic-number-theory.md#dirichlet-character) with nonprincipal product, the real zeros in this interval are counted with multiplicity. The logarithmic-derivative coefficients of $\zeta L(\chi_1)L(\chi_2)L(\chi_1\chi_2)$ are $\Lambda(n)(1+\chi_1(n))(1+\chi_2(n))\geq0$. The [global partial-fraction expansion of a Dirichlet L-function logarithmic derivative](algebraic-number-theory.md#global-partial-fraction-expansion-of-a-dirichlet-l-function-logarithmic-derivative) therefore gives $0\leq1/(\sigma-1)-\sum_{j=1}^2(\sigma-\beta_j)^{-1}+C\log(q_1q_2)$ if two nearby real zeros exist. Put $\sigma=1+a/\log(q_1q_2)$, choose $a$ small, and test $1-\beta_j<a/(4\log(q_1q_2))$. The right side is negative, a contradiction.

// Target: analytic-number-theory.bigb

##### Sparse conductors of exceptional real Dirichlet zeros

↑ **Parent:** [Landau theorem for two real Dirichlet characters](#landau-theorem-for-two-real-dirichlet-characters)

Fix the exceptional-zero threshold $\beta>1-\eta/\log q$, with $\eta$ less than one third of the constant in [Landau theorem for two real Dirichlet characters](#landau-theorem-for-two-real-dirichlet-characters). If distinct primitive conductors satisfy $q_1<q_2\leq q_1^2$, then $\log(q_1q_2)\leq3\log q_1$; both exceptional zeros lie in the forbidden two-zero interval. Thus the conductors grow at least quadratically. The same argument with equal conductors proves at most one exceptional real primitive character for each modulus. Existence is not asserted, and a consistently sufficiently small threshold is essential.

// Target: number-theory.bigb

#### Prime number theorem in an arithmetic progression with an exceptional zero

↑ **Parent:** [Siegel zero](#siegel-zero)

Uniformly for $x\geq2$ and $(a,q)=1$,

$$
\psi(x;q,a)
=\frac{x}{\varphi(q)}
-\frac{\chi_1(a)x^\beta}{\beta\varphi(q)}
+O\left(
x(\log q)^2
\exp\left[-\frac{c\log x}{\log q+\sqrt{\log x}}\right]
\right),
$$

where the second term occurs only when a real character $\chi_1$ has an [exceptional zero](#siegel-zero) $\beta$.

##### Exceptional-zero bound from a uniform upper bound in arithmetic progressions

↑ **Parent:** [Prime number theorem in an arithmetic progression with an exceptional zero](#prime-number-theorem-in-an-arithmetic-progression-with-an-exceptional-zero)

If some $\epsilon>0$ satisfies

$$
\psi(x;q,a)\leq(2-\epsilon)\frac{x}{\varphi(q)}
\qquad(x\geq q^2)
$$

uniformly for sufficiently large $q$, then every [exceptional zero](#siegel-zero) modulo $q$ satisfies

$$
\beta\leq1-\frac{c_\epsilon}{(\log q)^2}.
$$

Choose $\chi_1(a)=-1$ and $x=\exp(A(\log q)^2)$ in the exceptional-zero asymptotic, with $A$ large in terms of $\epsilon$.

## Pretentious number theory

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pretentious_number_theory)

Pretentious number theory studies [multiplicative arithmetic functions](number-theory.md#multiplicative-function) by measuring how closely they imitate structured functions such as [Dirichlet characters](algebraic-number-theory.md#dirichlet-character) and [Archimedean characters](number-theory.md#archimedean-character).

## Normal order of an arithmetic function

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_order_of_an_arithmetic_function)

A positive function $g(n)$ is a normal order of an [arithmetic function](number-theory.md#arithmetic-function) $f(n)$ when, for every $\epsilon>0$, all but $o(x)$ integers $n\leq x$ satisfy $|f(n)-g(n)|<\epsilon g(n)$.

<h3 id="turan-normal-order-theorem-for-distinct-prime-divisors">Turán normal-order theorem for distinct prime divisors</h3>

↑ **Parent:** [Normal order of an arithmetic function](#normal-order-of-an-arithmetic-function)

The [prime omega function](number-theory.md#prime-omega-function) has normal order $\log\log n$. The elementary second-moment estimate

$$
\sum_{n\leq x}\bigl(\omega(n)-\log\log x\bigr)^2
\ll x\log\log x
$$

already proves concentration on every scale larger than $\sqrt{\log\log x}$.

<h2 id="dirichlet-s-theorem-on-arithmetic-progressions">Dirichlet's theorem on arithmetic progressions</h2>

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet's_theorem_on_arithmetic_progressions)

If $\gcd(a,m)=1$, infinitely many primes satisfy

$$
p\equiv a\pmod m.
$$

### Reciprocal primes in a fixed arithmetic progression

↑ **Parent:** [Dirichlet's theorem on arithmetic progressions](#dirichlet-s-theorem-on-arithmetic-progressions)

For fixed coprime integers $a,q$, the [Prime number theorem](#prime-number-theorem) in the [arithmetic progression](arithmetic.md#arithmetic-progression) gives $\pi(x;q,a)\sim x/(\varphi(q)\log x)$. [Partial summation](#abel-s-summation-formula) expresses the reciprocal-prime sum as $\pi(x;q,a)/x+\int_2^x\pi(t;q,a)t^{-2}\,dt$. The integral of the relative error is $o(\log\log x)$: fix a threshold beyond which that error is at most $\varepsilon$, bound its remaining integral by $\varepsilon\log\log x$, and then let $\varepsilon$ decrease to zero. The modulus is fixed in this statement.

<h3 id="siegel-walfisz-theorem">Siegel–Walfisz theorem</h3>

↑ **Parent:** [Dirichlet's theorem on arithmetic progressions](#dirichlet-s-theorem-on-arithmetic-progressions)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Siegel–Walfisz_theorem)

For fixed $A,C>0$,

$$
\psi(x;q,a)=\frac{x}{\phi(q)}+O_{A,C}\left(\frac{x}{\log^Ax}\right)
$$

uniformly for $q\leq\log^Cx$ and $(a,q)=1$. The implied constant may be ineffective. This small-modulus input complements the [large sieve](#large-sieve) in the proof of the [Bombieri–Vinogradov theorem](#bombieri-vinogradov-theorem).

#### Major-arc value of the prime exponential sum

↑ **Parent:** [Siegel–Walfisz theorem](#siegel-walfisz-theorem)

For $(a,q)=1$ and $q\le\log^A N$, apply the [Siegel–Walfisz theorem](#siegel-walfisz-theorem) to every reduced residue class with error exponent $A+B+2$. The main terms sum to $N c_q(a)/\varphi(q)$, where the [Ramanujan sum](algebra.md#ramanujan-sum) satisfies $c_q(a)=\mu(q)$ for coprime $a,q$. Nonunits with nonzero [Von Mangoldt function](number-theory.md#von-mangoldt-function) are powers of primes dividing $q$ and contribute at most $\omega(q)\log N$, which is absorbed by the error. For arbitrary $a$, the correct main term is $N c_q(a)/\varphi(q)$; the reduced numerator hypothesis cannot be omitted.

### Prime-character sum near one

↑ **Parent:** [Dirichlet's theorem on arithmetic progressions](#dirichlet-s-theorem-on-arithmetic-progressions)

For real $s>1$, the logarithm defined by the [Euler product](#euler-product) of a [Dirichlet L-function](algebraic-number-theory.md#dirichlet-l-function) differs from $F_\chi(s)$ by a quantity of absolute value at most $\sum_{n\geq2}1/(n(n-1))=1$. If $L(\chi,1)\ne0$, a local [holomorphic logarithm](complex-analysis.md#holomorphic-logarithm) differs from this continuous logarithm by one fixed multiple of $2\pi i$ on a short real interval, so $F_\chi(s)$ stays bounded as $s\downarrow1$. For the [principal Dirichlet character](algebraic-number-theory.md#principal-dirichlet-character), the pole of the [Riemann zeta function](#riemann-zeta-function) instead gives $F_{\chi_0}(s)=\log(1/(s-1))+O(1)$. [Orthogonality of Dirichlet characters](algebraic-number-theory.md#orthogonality-of-dirichlet-characters) then makes the sum over any reduced residue class diverge, proving infinitude of its [primes](number-theory.md#prime-number).

## Harmonic number

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Harmonic_number)

The $n$th harmonic number is $H_n=\sum_{k=1}^n1/k$. Its asymptotic expansion begins

$$
H_n=\log n+\gamma+\frac1{2n}+O(n^{-2}),
$$

where $\gamma$ is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant).

<h2 id="abel-s-summation-formula">Abel's summation formula</h2>

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abel's_summation_formula)

Partial summation is the discrete analogue of [integration by parts](calculus.md#integration-by-parts). If $A(x)=\sum_{n\leq x}a_n$ and $g$ is continuously differentiable, then

$$
\sum_{n\leq x}a_ng(n)=A(x)g(x)-\int_1^xA(t)g'(t)\,dt.
$$

### Reciprocal-sum convergence from a counting bound

↑ **Parent:** [Abel's summation formula](#abel-s-summation-formula)

If $A(x)$ counts a set of [positive integers](number-theory.md#positive-integer) and $\eta>0$, [Abel summation](#abel-s-summation-formula) gives $\sum_{n\in A,n\le X}1/n=A(X)/X+\int_1^X A(t)t^{-2}\,dt$. A bound $A(t)\ll t/(\log t)^{1+\eta}$ for $t\ge3$ makes the integral convergent, since the substitution $u=\log t$ gives $\int_{\log3}^\infty u^{-1-\eta}\,du<\infty$.

### Bounded-variation multipliers of a convergent series

↑ **Parent:** [Abel's summation formula](#abel-s-summation-formula)

If $\sum a_n$ converges and $b_n$ is bounded with $\sum|b_{n+1}-b_n|<\infty$, then $\sum a_nb_n$ converges. For $T_j=\sum_{k=m}^j a_k$, [summation by parts](#abel-s-summation-formula) gives

$$
\left|\sum_{j=m}^n a_jb_j\right|\leq\sup_{j\geq m}|T_j|\left(|b_n|+\sum_{j=m}^{n-1}|b_j-b_{j+1}|\right).
$$

The first factor tends uniformly to zero by the [Cauchy sequence](real-analysis.md#cauchy-sequence) criterion, and the second has a uniform bound. A bounded [monotone sequence](real-analysis.md#monotone-sequence) has finite total variation, so monotone multipliers are included. Eventual monotonicity also suffices, since finitely many initial terms do not affect convergence. Absolute convergence of $\sum a_n$ is unnecessary.

### Exponentially damped reciprocal-prime sum

↑ **Parent:** [Abel's summation formula](#abel-s-summation-formula)

For $3\leq z\leq D$, [prime-number estimates](#prime-number-theorem) and [partial summation](#abel-s-summation-formula) give, for an absolute $c>0$,

$$
\sum_{p\leq z}\frac{e^{-\frac12\log D/\log p}}{p(\log p)^3}
\ll\frac1{(\log D)^3}e^{-c\log D/\log z}.
$$

Indeed, comparison with the prime-density integral and the substitution $v=\log D/\log t$ reduce the left side to $(\log D)^{-3}\int_{\log D/\log z}^\infty v^2e^{-v/2}\,dv$.

## Reciprocal fractional-part sum near a rational

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

If $(a,q)=1$, $|\alpha-a/q|\leq q^{-2}$, and $M,R\geq2$, then uniformly in $m_0$,

$$
\sum_{m_0\leq m<m_0+M}\min(R,\|\alpha m\|^{-1})
\ll\log(2q)\left(\frac{MR}{q}+M+R+q\right).
$$

Split the interval into blocks of length at most $q/2$. Within a block the points $\alpha m$ are $\gg1/q$-separated modulo one; ordering their distances from the nearest integer gives $O(R+q\log q)$ per block.

## Bilinear quadratic exponential sum fourth-moment bound

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

Two applications of the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) give

$$
\left|\sum_{t,r}b_tc_re(\alpha r^2t^2)\right|
\leq\|b\|_2\|c\|_2
\left(\sum_{t_1,t_2,r_1,r_2}
e\bigl(\alpha(t_1^2-t_2^2)(r_1^2-r_2^2)\bigr)
\right)^{1/4}.
$$

The fourth moment exposes differences of squares that can be factored and estimated by one-dimensional geometric sums.

### Factorized fourth moment for a bilinear quadratic exponential sum

↑ **Parent:** [Bilinear quadratic exponential sum fourth-moment bound](#bilinear-quadratic-exponential-sum-fourth-moment-bound)

Factoring $r_1^2-r_2^2=(r_1-r_2)(r_1+r_2)$ and similarly in $t$ separates diagonal contributions from a geometric sum. Grouping the three fixed factors by their product $m$ bounds the off-diagonal fourth moment by

$$
\sum_{m\ll RT^2}\tau_4(m)\min(R,\|\alpha m\|^{-1}).
$$

#### Truncation of a divisor weight by its second moment

↑ **Parent:** [Factorized fourth moment for a bilinear quadratic exponential sum](#factorized-fourth-moment-for-a-bilinear-quadratic-exponential-sum)

If $\sum_{n\leq N}\tau_k(n)^2\ll N(\log N)^{O(1)}$, then for any $X\geq1$,

$$
\sum_{\substack{n\leq N\\\tau_k(n)\geq X}}\tau_k(n)
\leq X^{-1}\sum_{n\leq N}\tau_k(n)^2
\ll\frac{N(\log N)^{O(1)}}X.
$$

This separates a divisor-weighted exponential sum into a bounded-weight part and a sparse large-weight part.

## Bilinear sum

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)

A bilinear sum has the form $\sum_{m,n}a_mb_nK(m,n)$, with two independently controlled coefficient sequences. Cauchy-Schwarz, completion, and large-sieve estimates exploit this separation of variables.

<h3 id="vinogradov-type-i-ii-method">Vinogradov Type I–II method</h3>

↑ **Parent:** [Bilinear sum](#bilinear-sum)

This method uses cancellation in [Type I sums](#type-i-sum) and [Type II sums](#type-ii-sum) to control a sum weighted by the [Von Mangoldt function](number-theory.md#von-mangoldt-function). The [Vaughan identity](number-theory.md#vaughan-s-identity) separates the short-factor contributions from bilinear ones. [Fourier separation of interval cutoffs](#fourier-separation-of-interval-cutoffs) permits a hyperbolic product cutoff. [Ben Green's 2007 notes, Sections 2.3–2.4](https://arxiv.org/pdf/0710.0823) give a version adapted to binary digit sums.

#### Small Type I and Type II sums

↑ **Parent:** [Vinogradov Type I–II method](#vinogradov-type-i-ii-method)

Extend $f:[1,N]\cap\mathbb Z\to\mathbb C$ by zero, and assume $|f|\le1$. In one dyadic endpoint convention, [Type I sums](#type-i-sum) are $\delta$-small if $\sum_{M\le m<2M}|\sum_{n\in I_m}f(mn)|\le\delta N$ for every dyadic $M\le N^{1/100}$ and every choice of integer intervals $I_m\subset[K,2K)$, $MK\le N$. [Type II sums](#type-ii-sum) are $\delta$-small if $|\sum_{m\in[M,2M)}\sum_{n\in[K,2K)}a_mb_nf(mn)|\le\delta N$ for all dyadic $M,K\in[N^{1/100},N^{99/100}]$ and coefficients $|a_m|,|b_n|\le1$. Empty tails are handled by zero extension.

### Fourier separation of interval cutoffs

↑ **Parent:** [Bilinear sum](#bilinear-sum)

If $I_m$ is an integer interval inside $[1,N]$, discrete [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) gives the displayed identity. The [exponential geometric sum bound](real-analysis.md#exponential-geometric-sum-bound) gives a common envelope $H_N(\theta)\ll\min(N,\|\theta\|^{-1})$, whose integral is $O(\log(2N))$. At each frequency, $\widehat{1_{I_m}}(\theta)/H_N(\theta)$ is a bounded coefficient depending only on $m$, while $e(n\theta)$ depends only on $n$. A uniform bounded-coefficient [Type II sum](#type-ii-sum) estimate therefore survives an $m$-dependent interval cutoff at a cost of one logarithm. This is particularly useful for the condition $mn\le N$.

### Bilinear cancellation for badly approximable phases

↑ **Parent:** [Bilinear sum](#bilinear-sum)

Let $\alpha$ be a [badly approximable number](number-theory.md#badly-approximable-number), and sum $B=\sum_{D<d\leq2D}\sum_{W<w\leq2W,dw\leq X}a_db_we(\alpha dw)$ with $|a_d|\leq\tau(d)$ and $|b_w|\leq1$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), [divisor-square summatory bound](number-theory.md#divisor-square-summatory-bound) and geometric sums give $|B|^2\ll D\log^3X(DW+W\sum_{h\leq W}\min(D,\|h\alpha\|^{-1}))$. Separated rotations bound the last sum by $O_\alpha(W\log(2W))$, giving the displayed estimate. A hyperbolic cutoff remains valid because the allowed first-variable values after expansion form an interval.

### Type II sum

↑ **Parent:** [Bilinear sum](#bilinear-sum)

A Type II sum has the form $\sum_{d\sim D}\sum_{m\sim M}a_db_mf(dm)$ with two nontrivially weighted variables, both long enough for a [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and a [large sieve](#large-sieve) estimate. The [Vaughan identity](number-theory.md#vaughan-s-identity) supplies this bilinear structure for sums weighted by the [Von Mangoldt function](number-theory.md#von-mangoldt-function).

#### Rational-phase Type II estimate

↑ **Parent:** [Type II sum](#type-ii-sum)

Suppose $|a_u|\le\tau(u)$, $|b_d|\le\log(2N)$, $u,d>X\ge1$, $ud\le N$, and $|\theta-a/q|\le q^{-2}$ with $(a,q)=1$. A [dyadic decomposition](#dyadic-decomposition) reduces $S=\sum a_ub_de(\theta ud)$ to blocks $u\asymp U,d\asymp D$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality), [divisor-square summatory bound](number-theory.md#divisor-square-summatory-bound) and the [reciprocal fractional-part sum near a rational](#reciprocal-fractional-part-sum-near-a-rational) give

$$
|S_{U,D}|^2\ll UD\left(U+\frac{UD}{q}+q+D\right)\log^6(2N).
$$

The condition $ud\le N$ makes the allowed $u$ values for each pair $d_1,d_2$ an interval, so the [exponential geometric sum bound](real-analysis.md#exponential-geometric-sum-bound) applies despite the hyperbolic cutoff. Since $UD\le N$ and $U,D\gg X$, take square roots and sum the $O(\log^2(2N))$ blocks to get the displayed estimate.

### Type I sum

↑ **Parent:** [Bilinear sum](#bilinear-sum)

A Type I sum in [analytic number theory](analytic-number-theory.md) has the form $\sum_{d\leq U}a_d\sum_{m\in I_d}f(dm)$, with a short weighted variable and a relatively long inner sum whose coefficients are simple. The [Vaughan identity](number-theory.md#vaughan-s-identity) produces these sums when the [Möbius function](number-theory.md#mobius-function) is truncated.

### Dyadic decomposition

↑ **Parent:** [Bilinear sum](#bilinear-sum)

A dyadic decomposition partitions a positive range into intervals $(M,2M]$. It reduces a variable-length sum to $O(\log N)$ sums in which every variable has a fixed order of magnitude.

## Sieve theory

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sieve_theory)

Sieve theory estimates the number of integers that avoid specified residue classes modulo primes.

### Parity problem

↑ **Parent:** [Sieve theory](#sieve-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity_problem)

Divisibility information by small primes cannot by itself reliably distinguish integers with an odd or even total number of prime factors. Consequently an upper-bound [Selberg sieve](#selberg-sieve) can bound prime pairs and related sifted sets but does not supply a positive lower bound or the conjectured twin-prime asymptotic. This limitation concerns the information available to the sieve, not merely a choice of weight normalization.

// Target: number-theory.bigb

### Integers with all prime factors congruent to one modulo four

↑ **Parent:** [Sieve theory](#sieve-theory)

A [positive integer](number-theory.md#positive-integer) in this set has no [prime factor](number-theory.md#prime-factor) equal to two or congruent to three modulo four. Its [prime factors](number-theory.md#prime-factor) all lie in the [residue class](number-theory.md#residue-class) one modulo four. For example $5\cdot13=65$ belongs, while $3^2=9$ does not, even though $9$ itself is congruent to one modulo four. A [half-dimensional interval sieve](#half-dimensional-interval-sieve) bounds the count in an interval of length $z$ by $O(z/\sqrt{\log z})$.

### Large sieve

↑ **Parent:** [Sieve theory](#sieve-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Large_sieve)

The large sieve bounds how much an [exponential sum](#exponential-sum) can concentrate at separated points of the [circle group](lie-theory.md#circle-group). Its [variance form of the large sieve](#variance-form-of-the-large-sieve) also bounds simultaneous concentration in [residue classes](number-theory.md#residue-class) modulo many [primes](number-theory.md#prime-number).

#### Large sieve upper bound for sifted intervals

↑ **Parent:** [Large sieve](#large-sieve)

For an interval set avoiding one residue at each sieving [prime](number-theory.md#prime-number), the [Ramanujan sum](algebra.md#ramanujan-sum) at the forbidden [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) residue gives a linear combination of Fourier samples equal to $\mu(d)|S|$. [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) gives sample energy at least $|S|^2/\varphi(d)$ for each [squarefree](number-theory.md#squarefree-integer) modulus. Summing these energies and applying the [analytic large sieve inequality](#exponential-sum-large-sieve) gives the bound. If [primes](number-theory.md#prime-number) dividing $q$ are excluded, restrict the denominator to $(d,q)=1$; it is uniformly at least a constant times $(\varphi(q)/q)\log(2Q)$.

#### Character large sieve

↑ **Parent:** [Large sieve](#large-sieve)

For coefficients supported on $N$ consecutive [integers](number-theory.md#integer),

$$
\sum_{q\leq Q}\frac q{\phi(q)}\sum_{\chi\bmod q}^{*}\left|\sum_na_n\chi(n)\right|^2\leq(Q^2+2\pi N)\sum_n|a_n|^2.
$$

The star restricts to [primitive Dirichlet characters](algebraic-number-theory.md#primitive-dirichlet-character). Their [finite Fourier transform of a primitive Dirichlet character](algebraic-number-theory.md#finite-fourier-transform-of-a-primitive-dirichlet-character) has normalization of [absolute value](real-analysis.md#absolute-value) $\sqrt q$. [Orthogonality of Dirichlet characters](algebraic-number-theory.md#orthogonality-of-dirichlet-characters) therefore bounds the weighted contribution for one modulus by $\sum_{\substack{a\bmod q\\(a,q)=1}}|\sum_na_ne(an/q)|^2$. Sum over $q$ and use the [exponential-sum large sieve](#exponential-sum-large-sieve) on the distinct [reduced fractions](number-theory.md#reduced-fraction) of denominators at most $Q$.

#### Variance form of the large sieve

↑ **Parent:** [Large sieve](#large-sieve)

For coefficients $b_n$ supported on an interval of $H$ consecutive [integers](number-theory.md#integer), set $B=\sum b_n$ and $B_p(a)=\sum_{n\equiv a\pmod p}b_n$. Then

$$
\sum_{p\leq Q}p\sum_{a\bmod p}|B_p(a)-B/p|^2\leq(Q^2+2\pi H)\sum|b_n|^2.
$$

The [orthogonality of roots of unity](algebra.md#orthogonality-of-roots-of-unity) gives $p\sum_a|B_p(a)-B/p|^2=\sum_{r=1}^{p-1}|\sum_nb_ne(rn/p)|^2$. The distinct fractions $r/p$ have [circular spacing](#circular-spacing) at least $Q^{-2}$; now apply the [exponential-sum large sieve](#exponential-sum-large-sieve).

#### Exponential-sum large sieve

↑ **Parent:** [Large sieve](#large-sieve)

If $\theta_r$ have [circular spacing](#circular-spacing) at least $\delta$, then

$$
\sum_r\left|\sum_{M<n\leq M+N}a_ne(n\theta_r)\right|^2\leq(\delta^{-1}+2\pi N)\sum_{M<n\leq M+N}|a_n|^2.
$$

Multiply the [exponential sum](#exponential-sum) by $e(-Mt)$, apply the [Sobolev–Gallagher inequality](sobolev-space.md#sobolev-gallagher-inequality) on disjoint arcs of length $\delta$, and sum. The [finite-interval Parseval identities](fourier-analysis.md#finite-interval-parseval-identities) and [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound the derivative contribution by $2\pi N\sum|a_n|^2$.

<h5 id="fejer-kernel-proof-of-the-analytic-large-sieve">Fejér-kernel proof of the analytic large sieve</h5>

↑ **Parent:** [Exponential-sum large sieve](#exponential-sum-large-sieve)

A triangular taper majorizes a fixed fraction of the summation interval. Its Fourier kernel is the [Fejér kernel](fourier-series.md#fejer-kernel), bounded by $C\min(m,(m\|\theta\|^2)^{-1})$. For separated sample points, split each row sum at distance $1/m$: the plateau and square-decay tail each contribute $O(\delta^{-1})$, while the diagonal contributes $O(m)$. Bounding the resulting [quadratic form](linear-algebra.md#quadratic-form) proves the dual sieve with constant $C(N+\delta^{-1})$. [Operator norm duality](continuous-dual-space.md#operator-norm-duality) gives the primal sieve.

##### Local-multiplicity large sieve

↑ **Parent:** [Exponential-sum large sieve](#exponential-sum-large-sieve)

Let $K(\Delta)=\max_t\#\{r:\|\theta_r-t\|\leq\Delta/2\}$. Without a separation assumption,

$$
\sum_r|S(\theta_r)|^2\leq K(\Delta)(\Delta^{-1}+2\pi N)\sum|a_n|^2.
$$

For $0<\Delta\leq1$, each point belongs to at most $K(\Delta)$ integration arcs in the [Sobolev–Gallagher inequality](sobolev-space.md#sobolev-gallagher-inequality). For $\Delta\geq1$, $K(\Delta)$ is the total number of points, and the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) bound $|S|^2\leq N\sum|a_n|^2$ suffices.

###### Prime-denominator large sieve

↑ **Parent:** [Local-multiplicity large sieve](#local-multiplicity-large-sieve)

When $N\leq P$,

$$
\sum_{\substack{P\leq p\leq2P\\p\text{ prime}}}\sum_{a=1}^{p-1}\left|\sum_{M<n\leq M+N}a_ne(an/p)\right|^2\ll\frac{P^2}{\log P}\sum|a_n|^2.
$$

An arc of length $1/P$ contains at most three points of each grid of denominator $p\leq2P$. The [Chebyshev estimate](number-theory.md#chebyshev-estimate) gives $O(P/\log P)$ such [primes](number-theory.md#prime-number). Apply the [local-multiplicity large sieve](#local-multiplicity-large-sieve). Using only the separation of distinct [reduced fractions](number-theory.md#reduced-fraction) gives the weaker $O(P^2)\sum|a_n|^2$.

#### Circular spacing

↑ **Parent:** [Large sieve](#large-sieve)

Points $\theta_r$ have circular spacing at least $\delta$ when $\|\theta_r-\theta_s\|\geq\delta$ for distinct $r,s$, where $\|t\|=\min_{k\in\mathbb Z}|t-k|$. The distance is measured on the [circle group](lie-theory.md#circle-group) $\mathbb R/\mathbb Z$, so points near zero and one can be close.

### Buchstab function

↑ **Parent:** [Sieve theory](#sieve-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Buchstab_function)

The continuous [Buchstab function](#buchstab-function) satisfies $w(u)=1/u$ for $1\le u\le2$ and $\frac{d}{du}(u w(u))=w(u-1)$ for $u>2$. It describes the density of [rough numbers](#rough-number).

#### Oscillation of the Buchstab function

↑ **Parent:** [Buchstab function](#buchstab-function)

The [Buchstab function](#buchstab-function) takes values both above and below $e^{-\gamma}$ on every interval of length one in $[1,\infty)$. The equation $\frac{d}{du}(u(w(u)-e^{-\gamma}))=w(u-1)-e^{-\gamma}$ propagates any fixed sign forwards; the rapid decay to zero then forces an impossible identically zero tail.

#### Buchstab theorem

↑ **Parent:** [Buchstab function](#buchstab-function)

For each fixed $u>1$, the number $\Phi(z^u,z)$ of [z-sieved numbers](#rough-number) at most $z^u$ satisfies $\Phi(z^u,z)\sim z^u w(u)/\log z$ as $z\to\infty$. The fixed-$u$ asymptotic does not extend to $u=1$.

### Rough number

↑ **Parent:** [Sieve theory](#sieve-theory)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rough_number)

A $z$-rough integer has no [prime factor](number-theory.md#prime-factor) below $z$; $1$ is included. Some authors instead exclude [prime factors](number-theory.md#prime-factor) at most $z$, so the endpoint convention should be stated.

### Sifting function

↑ **Parent:** [Sieve theory](#sieve-theory)

For a finite integer set $A$ and a set of primes $\mathcal P$, the sifting function counts elements of $A$ divisible by no prime in $\mathcal P$ below $z$:

$$
S(A,\mathcal P,z)=\left|\left\{a\in A:\gcd(a,P(z))=1\right\}\right|,
\qquad
P(z)=\prod_{\substack{p\in\mathcal P\\p\leq z}}p.
$$

For a nonnegative weighted sequence $\mathcal A=(a_n)$, the same notation means $S(\mathcal A,\mathcal P,z)=\sum_{(n,P(z))=1}a_n$.

#### Sieve distribution

↑ **Parent:** [Sifting function](#sifting-function)

Put $|\mathcal A_d|=\sum_{d\mid n}a_n$. A nonnegative sequence has distribution $(X,P(z),g,(r_d))$ when $g$ is multiplicative on the squarefree divisors of $P(z)$, $0\leq g(p)<1$, and

$$
|\mathcal A_d|=Xg(d)+r_d
$$

for every $d\mid P(z)$.

#### Buchstab identity

↑ **Parent:** [Sifting function](#sifting-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Buchstab_identity)

If $w<z$, ordering the least prime factor gives

$$
S(\mathcal A,\mathcal P,z)
=S(\mathcal A,\mathcal P,w)
-\sum_{\substack{w\leq p<z\\p\in\mathcal P}}S(\mathcal A_p,\mathcal P,p),
$$

where $(\mathcal A_p)_n=a_{pn}$ in a set formulation, or equivalently $\mathcal A_p$ restricts the original sequence to terms divisible by $p$.

### Upper-bound sieve

↑ **Parent:** [Sieve theory](#sieve-theory)

An upper-bound sieve bounds the size of a sifted set from above. In a dimension-one problem with one forbidden class modulo each relevant prime $p$, its main density factor is comparable to $\prod_p(1-1/p)$.

<h4 id="brun-titchmarsh-theorem">Brun–Titchmarsh theorem</h4>

↑ **Parent:** [Upper-bound sieve](#upper-bound-sieve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brun–Titchmarsh_theorem)

For $x>q$ and $(a,q)=1$, the [prime-counting function](number-theory.md#prime-counting-function) in an [arithmetic progression](arithmetic.md#arithmetic-progression) satisfies

$$
\pi(x;q,a)\leq\frac{2x}{\phi(q)\log(x/q)}.
$$

The denominator involves the [Euler totient function](number-theory.md#euler-totient-function) and the length-to-modulus ratio. In particular, for $q\leq x^{1-\eta}$ with fixed $\eta>0$, this is $O_\eta(x/(\phi(q)\log x))$.

#### Selberg sieve

↑ **Parent:** [Upper-bound sieve](#upper-bound-sieve)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Selberg_sieve)

The Selberg sieve uses optimized quadratic weights to bound the size of a sifted set.

##### Selberg upper-bound sieve

↑ **Parent:** [Selberg sieve](#selberg-sieve)

Suppose $|\mathcal A_d|=Xg(d)+r_d$ for $d\mid P(z)$. If $\lambda_1=1$ and the real Selberg weights $\lambda_d$ vanish unless $d\mid P(z)$ and $d\leq D$, then

$$
S(\mathcal A,\mathcal P,z)
\leq X\sum_{d,e}\lambda_d\lambda_e g([d,e])
+\sum_{d,e}\lambda_d\lambda_e r_{[d,e]}.
$$

Optimizing the main quadratic form gives $X/G(D,z)$, where

$$
G(D,z)=\sum_{\substack{\ell\leq D\\\ell\mid P(z)}}
\prod_{p\mid\ell}\frac{g(p)}{1-g(p)},
$$

up to the harmless replacement of $D$ by $D^2$ under the alternative convention that $D$ denotes the level of the least common multiples.

###### Uniform interval bound from optimal Selberg weights

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

For all interval origins $a\ge0$, the number of multiples of any $d$ in $(a,a+x]$ is $x/d+O(1)$ with an absolute error bound. The [Selberg sieve diagonalization](#selberg-sieve-diagonalization) minimizes $\sum_{d,e\le z}\lambda_d\lambda_e/[d,e]$, subject to $\lambda_1=1$, at $1/G(z)$. The [optimal Selberg weights have modulus at most one](#optimal-selberg-weights-have-modulus-at-most-one), so the total remainder is $O(z^2)$. Restoring the at most $z$ small [primes](number-theory.md#prime-number) gives $\pi(a+x)-\pi(a)\le z+x/G(z)+O(z^2)$. Take $z=\lfloor\sqrt x/(\log x)^2\rfloor$ and use the [Selberg sieve denominator asymptotic](#selberg-sieve-denominator-asymptotic). The resulting $o(1)$ is independent of $a$.

###### Half-dimensional interval sieve

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

Sieve an interval of length $z$ by the [prime](number-theory.md#prime-number) two and the [primes](number-theory.md#prime-number) congruent to three modulo four, with local densities $g(p)=1/p$. Take $D=z^{1/2}$ and $L=\sqrt D$. The [truncated Euler-product lower bound](#truncated-euler-product-lower-bound), the [Mertens first theorem](#mertens-first-theorem) and the [reciprocal-prime sum in residue class one modulo four](#reciprocal-prime-sum-in-residue-class-one-modulo-four) give $J\gg\sqrt{\log z}$. The interval counts have bounded remainders, whose sum is $O(D\log^2D)$ by the [summatory bound for three to the prime omega](number-theory.md#summatory-bound-for-three-to-the-prime-omega). Hence the number surviving is $O(z/\sqrt{\log z})$, uniformly in the location of the interval.

###### Selberg sieve weights

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

For

$$
h(d)=\prod_{p\mid d}\frac{g(p)}{1-g(p)},\qquad
G(D,z)=\sum_{\substack{\ell<D\\\ell\mid P(z)}}h(\ell),
$$

define

$$
G_d(y,z)=
\sum_{\substack{\ell<y\\\ell\mid P(z)\\(\ell,d)=1}}h(\ell).
$$

The optimizing Selberg weights are

$$
\lambda_d=
\mu(d)\prod_{p\mid d}(1-g(p))^{-1}
\frac{G_d(D/d,z)}{G(D,z)}
$$

for $d<D$ dividing $P(z)$, and zero otherwise. They satisfy $\lambda_1=1$ and diagonalize the main quadratic form to $1/G(D,z)$.

###### Selberg sieve denominator asymptotic

↑ **Parent:** [Selberg sieve weights](#selberg-sieve-weights)

Put $g(n)=\mu(n)^2/\varphi(n)$. As a [Dirichlet convolution](number-theory.md#dirichlet-convolution), $g=h*(n\mapsto1/n)$, where $h$ is a [multiplicative arithmetic function](number-theory.md#multiplicative-function) with $h(p)=1/(p(p-1))$, $h(p^2)=-1/(p(p-1))$, and $h(p^j)=0$ for $j\ge3$. The local sums are one, so $\sum_nh(n)=1$. The series $\sum_n|h(n)|\log(2n)$ converges, since the prime-local errors are $O((\log p)/p^2)$. Consequently $G(z)=\sum_{d\le z}h(d)H_{\lfloor z/d\rfloor}=\log z+O(1)$ by the [harmonic number](#harmonic-number) estimate $H_m=\log m+O(1)$. This identifies the leading constant in the one-dimensional [Selberg upper-bound sieve](#selberg-upper-bound-sieve).

###### Selberg sieve diagonalization

↑ **Parent:** [Selberg sieve weights](#selberg-sieve-weights)

Put $L=\sqrt D$, $h(t)=\prod_{p\mid t}(g(p)^{-1}-1)$ and $y_t=\sum_{\substack{m\leq L\\t\mid m}}g(m)\rho_m$, where $g$ is a [multiplicative arithmetic function](number-theory.md#multiplicative-function) supported on [squarefree integers](number-theory.md#squarefree-integer). For [squarefree integers](number-theory.md#squarefree-integer) $m,n$,

$$
g([m,n])=g(m)g(n)\sum_{t\mid(m,n)}h(t).
$$

Thus the quadratic form is $\Sigma=\sum_{t\leq L}h(t)y_t^2$. [Möbius inversion](number-theory.md#mobius-inversion-formula) gives $g(d)\rho_d=\sum_{d\mid t\leq L}\mu(t/d)y_t$. On the permitted [squarefree integers](number-theory.md#squarefree-integer), the constraint $\rho_1=1$ becomes $\sum_t\mu(t)y_t=1$. The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) yields $\Sigma\geq1/J$, where $J=\sum_t1/h(t)$ over those integers; equality holds at $y_t=\mu(t)/(Jh(t))$.

###### Selberg least-common-multiple weights

↑ **Parent:** [Selberg sieve diagonalization](#selberg-sieve-diagonalization)

For real coefficients $\rho_1=1$ supported on permitted [divisors](number-theory.md#divisor) up to $L$, put $\lambda_d=\sum_{[u,v]=d}\rho_u\rho_v$. Then $\sum_{d\mid n}\lambda_d=(\sum_{d\mid n}\rho_d)^2$ is an upper bound for the [indicator function](measure-theory.md#indicator-function) of numbers free of the forbidden [prime factors](number-theory.md#prime-factor). Its support has $d\leq L^2$. If the coefficients vanish on non-[squarefree integers](number-theory.md#squarefree-integer) and satisfy $|\rho_d|\leq1$, then $|\lambda_d|\leq3^{\omega(d)}$: each [prime factor](number-theory.md#prime-factor) of $d$ occurs in $u$, in $v$, or in both.

###### Optimal Selberg weights have modulus at most one

↑ **Parent:** [Selberg sieve diagonalization](#selberg-sieve-diagonalization)

Let $k(d)=\prod_{p\mid d}g(p)/(1-g(p))$ on permitted [squarefree integers](number-theory.md#squarefree-integer). The [Selberg sieve weights](#selberg-sieve-weights) have

$$
|\rho_d|=\frac1{J\prod_{p\mid d}(1-g(p))}\sum_{\substack{v\leq L/d\\(v,d)=1}}k(v)\leq1.
$$

The numerator is the total weight of the distinct integers $ev\leq L$ with $e\mid d$ and $(v,d)=1$: [multiplicativity](number-theory.md#multiplicativity-of-an-arithmetic-function) gives $\sum_{e\mid d}k(e)=\prod_{p\mid d}(1-g(p))^{-1}$. They are a subset of the terms in $J$.

###### Polynomial root density in a sieve

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

For an integer polynomial $F$ and squarefree $d$, let $\rho_F(d)$ count the roots of $F$ modulo $d$. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) makes $\rho_F$ multiplicative, and

$$
\#\{m\leq X:d\mid F(m)\}=\frac{\rho_F(d)}dX+O(\rho_F(d)).
$$

Thus $g(d)=\rho_F(d)/d$ and $r_d=O(\rho_F(d))$ define a [sieve distribution](#sieve-distribution).

###### Elementary lower bound for the twin-prime sieve denominator

↑ **Parent:** [Polynomial root density in a sieve](#polynomial-root-density-in-a-sieve)

For the [polynomial](polynomial.md) $F(n)=n(n+2)$, take $\rho(2)=1$ and $\rho(p)=2$ at odd [primes](number-theory.md#prime-number). On odd [squarefree integers](number-theory.md#squarefree-integer), the summand is at least $2^{\omega(d)}/d$. Put $y=\sqrt z$ and $L(y)=\sum_{a\le y,\ a\text{ odd}}1/a=\tfrac12\log y+O(1)$. The weight of odd pairs $a,b\le y$ is $L(y)^2$. The pairs for which $a$ is not [squarefree](number-theory.md#squarefree-integer), $b$ is not [squarefree](number-theory.md#squarefree-integer), or $(a,b)>1$ each have weight at most $L(y)^2\sum_{p\text{ odd}}p^{-2}$. Indeed, the weighted count of multiples of an odd $p^k$ is $p^{-k}L(y/p^k)\le p^{-k}L(y)$. Moreover,

$$
\sum_{p\text{ odd}}p^{-2}\le\sum_{m\ge1}(2m+1)^{-2}\le\frac19+\int_1^\infty\frac{dt}{(2t+1)^2}=\frac5{18}.
$$

Hence the odd [coprime](number-theory.md#coprime-integers) [squarefree](number-theory.md#squarefree-integer) pairs have weight at least $L(y)^2/6$. Their products $d=ab\le z$ are [squarefree](number-theory.md#squarefree-integer), and $2^{\omega(d)}$ counts all ordered [coprime](number-theory.md#coprime-integers) factorizations of $d$. This proves the displayed lower bound needed for the [Selberg upper-bound sieve](#selberg-upper-bound-sieve).

###### Twin-prime upper bound from a quadratic sieve

↑ **Parent:** [Polynomial root density in a sieve](#polynomial-root-density-in-a-sieve)

For $F(n)=n(n+2)$, every odd [prime](number-theory.md#prime-number) has two forbidden [residue classes](number-theory.md#residue-class). Use [Selberg sieve weights](#selberg-sieve-weights) supported on odd [squarefree integers](number-theory.md#squarefree-integer) $d\le R=x^{1/8}$. Their main quadratic form is $1/J$, where $J=\sum_{d\le R}\prod_{p\mid d}2/(p-2)$. The [truncated Euler-product lower bound](#truncated-euler-product-lower-bound) applied to primes up to $R^{1/8}$ gives $J\gg\log^2R$: the mean logarithmic divisor size is $2\sum_{3\le p\le R^{1/8}}(\log p)/p<\frac12\log R$, by the [Mertens first theorem](#mertens-first-theorem), and the full product is $\asymp\log^2R$, by the [Mertens second theorem](#mertens-second-theorem). The [optimal Selberg weights have modulus at most one](#optimal-selberg-weights-have-modulus-at-most-one), so the remainder is at most $O(\sum_{d,e\le R}[d,e])=O(R^4)$. The finitely many possible pairs with $p\le R$ contribute $O(R)$. Thus the count is $O(x/J+R^4+R)$, proving the bound.

###### Prime-tuple upper bound from the Selberg sieve

↑ **Parent:** [Polynomial root density in a sieve](#polynomial-root-density-in-a-sieve)

For distinct natural numbers $h_1,\ldots,h_r$,

$$
\#\{n\leq x:n+h_1,\ldots,n+h_r\text{ are all prime}\}
\ll_{h_1,\ldots,h_r,r}\frac{x}{(\log x)^r}.
$$

Exclude the fixed primes dividing some $h_i-h_j$ so that the polynomial $\prod_i(n+h_i)$ has exactly $r$ roots modulo every remaining prime, then apply the [Selberg upper-bound sieve](#selberg-upper-bound-sieve) with level $x^{1/4}$.

###### Almost-primes from an upper-bound sieve and Buchstab identity

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

For a product of finitely many admissible linear forms, first omit a fixed finite set of locally obstructing primes. Apply the [Buchstab identity](#buchstab-identity) at a large fixed $w$, and bound each removed term by the [Selberg upper-bound sieve](#selberg-upper-bound-sieve). The convergent tail $\sum_{p\geq w}1/(p(\log p)^k)$ leaves a positive proportion with no prime divisor in $[w,X^\delta)$. Their distinct prime divisors below $w$ are finite in number, while those above $X^\delta$ number at most $O(1/\delta)$, producing infinitely many almost-prime values.

###### Fourier representation of a smooth Selberg weight

↑ **Parent:** [Selberg upper-bound sieve](#selberg-upper-bound-sieve)

If $f$ is smooth and supported on $[-1,1]$ and $g(t)=\int_{\mathbb R}e^xf(x)e(-tx)\,dx$, [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) gives

$$
f\left(\frac{\log d}{\log D}\right)
=\int_{\mathbb R}g(t)d^{-(1-2\pi it)/\log D}\,dt.
$$

Expanding the square of the resulting Möbius-weighted divisor sum turns its mean value into an Euler product controlled by zeta functions near their pole at one.

###### Smooth divisor-square sieve asymptotic

↑ **Parent:** [Fourier representation of a smooth Selberg weight](#fourier-representation-of-a-smooth-selberg-weight)

For a real [smooth](analysis.md#smooth-function) cutoff $\phi$ supported on $[-1/3,1/3]$ with $\phi(0)=1$, define $F_X(n)=(\sum_{d\mid n}\mu(d)\phi(\log d/\log X))^2$. Its sum over any interval of length $X$ is $c_\phi X/\log X+O_\phi(X/\log^2X+X^{2/3})$, uniformly in the interval location. Here $c_\phi$ is the [derivative energy constant for a smooth sieve cutoff](#derivative-energy-constant-for-a-smooth-sieve-cutoff). Expanding the square yields an interval-counting error $O(X^{2/3})$ and an [Euler product for a smoothed divisor-square correlation](#euler-product-for-a-smoothed-divisor-square-correlation); its [zeta function](#riemann-zeta-function) pole provides the main term. Every [prime](number-theory.md#prime-number) exceeding $X^{1/3}$ has weight one, giving the [short-interval prime upper bound from a smooth divisor weight](#short-interval-prime-upper-bound-from-a-smooth-divisor-weight).

###### Euler product for a smoothed divisor-square correlation

↑ **Parent:** [Smooth divisor-square sieve asymptotic](#smooth-divisor-square-sieve-asymptotic)

For $\operatorname{Re}z,\operatorname{Re}z'>0$, the series $\sum_{d,e}\mu(d)\mu(e)d^{-z}e^{-z'}/[d,e]$ has local factor $1-p^{-1-z}-p^{-1-z'}+p^{-1-z-z'}$. Dividing by the displayed [zeta function](#riemann-zeta-function) ratio leaves a [holomorphic function](complex-analysis.md#holomorphic-function) $H$ near zero with $H(0,0)=1$. The local factor of $H$ is $(1-a-b+c)(1-c)/((1-a)(1-b))$, where $a=p^{-1-z}$, $b=p^{-1-z'}$, $c=p^{-1-z-z'}$, and equals one exactly at zero. With $z=(1+it)/\log X$, the [zeta function](#riemann-zeta-function) poles produce the kernel $(1+it)(1+it')/((2+i(t+t'))\log X)$ that determines the [smooth divisor-square sieve asymptotic](#smooth-divisor-square-sieve-asymptotic).

###### Derivative energy constant for a smooth sieve cutoff

↑ **Parent:** [Smooth divisor-square sieve asymptotic](#smooth-divisor-square-sieve-asymptotic)

Write $e^u\phi(u)=\int\psi(t)e^{-iut}\,dt$. The double integral $\iint\psi(t)\psi(t')(1+it)(1+it')/(2+i(t+t'))\,dt\,dt'$ equals the displayed constant. Express the denominator as a Laplace integral and each differentiated Fourier factor as $-\phi'(u)$, then use [Fubini's theorem](measure-theory.md#fubini-s-theorem). For a real cutoff the resulting square is positive even though the [Fourier transform](analysis.md#fourier-transform) factors have no [complex conjugation](complex-analysis.md#complex-conjugation). The [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and $\phi(0)=1$, $\phi(1/3)=0$ give $c_\phi\geq3$.

###### Short-interval prime upper bound from a smooth divisor weight

↑ **Parent:** [Fourier representation of a smooth Selberg weight](#fourier-representation-of-a-smooth-selberg-weight)

For $Y\geq X\geq2$, a smooth Selberg divisor weight of level $D=X^{1/10}$ equals one on every prime in $(Y,Y+X]$. Its second moment can be expressed through an Euler product $H$ whose zeta-factor bound contributes $O(1/\log D)$ after integration against rapidly decreasing Fourier transforms. Consequently

$$
\pi(Y+X)-\pi(Y)\ll\frac X{\log X}.
$$

#### Dimension-three upper-bound sieve

↑ **Parent:** [Upper-bound sieve](#upper-bound-sieve)

If three nonproportional linear forms exclude three distinct residue classes modulo every sufficiently large prime, the upper-bound sieve has dimension three and gives an upper bound of order $x/(\log x)^3$.

## Mertens' theorems

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mertens'_theorems)

One form of Mertens' theorem is

$$
\prod_{p\leq x}\left(1-\frac1p\right)
\sim\frac{e^{-\gamma}}{\log x}.
$$

Taking a ratio gives $\prod_{w\leq p\leq z}(1-1/p)\ll\log w/\log z$ for $2\leq w\leq z$.

### Mertens first theorem

↑ **Parent:** [Mertens' theorems](#mertens-theorems)

The [prime sum](#prime-sum) $\sum_{p\leq y}(\log p)/p=\log y+O(1)$ is the first Mertens theorem. It controls the mean logarithmic size in a [truncated Euler-product lower bound](#truncated-euler-product-lower-bound).

#### Square-root logarithmic sum over primes

↑ **Parent:** [Mertens first theorem](#mertens-first-theorem)

Put $A(t)=\sum_{p\le t}(\log p)/p$. The [Mertens first theorem](#mertens-first-theorem) gives $A(t)=\log t+O(1)$. [Partial summation](#abel-s-summation-formula) yields

$$
\sum_{p\le x}\frac{\sqrt{\log p}}p
=\frac{A(x)}{\sqrt{\log x}}+\frac12\int_2^x\frac{A(t)}{t(\log t)^{3/2}}\,dt.
$$

The main terms sum to $2\sqrt{\log x}$ up to a constant. The error integral is bounded because $\int_2^\infty dt/(t(\log t)^{3/2})$ converges. Thus a [prime sum](#prime-sum) with a fractional logarithmic weight follows from an elementary bounded-error estimate, without the [Prime number theorem](#prime-number-theorem).

#### Positive logarithmic moments of reciprocal primes

↑ **Parent:** [Mertens first theorem](#mertens-first-theorem)

For fixed $\lambda>1$, integrate $(\log t)^{\lambda-1}$ against $A(t)=\sum_{p\le t}(\log p)/p$. The [Mertens first theorem](#mertens-first-theorem) gives $A(t)=\log t+O(1)$. [Partial summation](#abel-s-summation-formula) makes the main integral $(\log x)^\lambda/\lambda$; the bounded error in $A$ contributes at most a constant times $(\log x)^{\lambda-1}$. The restriction $\lambda>1$ ensures that integrating the derivative $(\lambda-1)(\log t)^{\lambda-2}/t$ has this bound.

#### Factorial proof of Mertens first theorem

↑ **Parent:** [Mertens first theorem](#mertens-first-theorem)

The [prime factorization](number-theory.md#fundamental-theorem-of-arithmetic) of $N!$ gives $\log N!=\sum_{p^j\le N}\lfloor N/p^j\rfloor\log p$. The [Chebyshev estimate](number-theory.md#chebyshev-estimate) bounds the error on replacing each floor by its argument by $O(N)$. Dividing by $N$ and using the [Stirling formula](real-analysis.md#stirling-formula) gives $\sum_{p^j\le N}(\log p)/p^j=\log N+O(1)$. The contribution of $j\ge2$ is bounded by the convergent series $\sum_{n\ge2}(\log n)/(n(n-1))$. This proves the [Mertens first theorem](#mertens-first-theorem) without the [Prime number theorem](#prime-number-theorem).

#### Logarithmically weighted reciprocal-prime tail

↑ **Parent:** [Mertens first theorem](#mertens-first-theorem)

For fixed $\delta>0$, the [Mertens first theorem](#mertens-first-theorem) and [partial summation](#abel-s-summation-formula) imply convergence of $\sum_p1/(p(\log p)^\delta)$ and, more precisely, the displayed tail asymptotic with error $O((\log x)^{-1-\delta})$. Write $A(t)=\sum_{p\le t}(\log p)/p=\log t+O(1)$ and integrate against $(\log t)^{-1-\delta}$. The boundary at infinity vanishes; combining the finite boundary with the integral gives the coefficient $1/\delta$.

### Mertens second theorem

↑ **Parent:** [Mertens' theorems](#mertens-theorems)

There is an absolute constant $B_1$, the Meissel–Mertens constant, such that

$$
\sum_{p\leq x}\frac1p
=\log\log x+B_1+O\left(\frac1{\log x}\right).
$$

#### Reciprocal-prime sum in residue class one modulo four

↑ **Parent:** [Mertens second theorem](#mertens-second-theorem)

The progression version of the [Mertens second theorem](#mertens-second-theorem) gives $\sum_{\substack{p\leq y\\p\equiv1\pmod4}}1/p=\tfrac12\log\log y+c+O(1/\log y)$. Subtracting from the all-[prime](number-theory.md#prime-number) sum shows that the forbidden [primes](number-theory.md#prime-number) $p\equiv3\pmod4$ contribute half the logarithmic density. This is the source of the square root in a [half-dimensional interval sieve](#half-dimensional-interval-sieve).

### Mertens third theorem

↑ **Parent:** [Mertens' theorems](#mertens-theorems)

There is a constant $C>0$ such that

$$
\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
=C\log x+O(1).
$$

Taking logarithms reduces the result to the [Mertens second theorem](#mertens-second-theorem), because the terms of order $p^{-2}$ and smaller form an absolutely convergent series.

#### Totient lower bound from the Mertens product

↑ **Parent:** [Mertens third theorem](#mertens-third-theorem)

If $C$ is the constant in the [Mertens third theorem](#mertens-third-theorem), then

$$
\varphi(n)\geq\left(C^{-1}+o(1)\right)\frac n{\log\log n}.
$$

Split the prime divisors of $n$ at $y=\log n/\sqrt{\log\log n}$. The small primes contribute at most $(C+o(1))\log\log n$ to $n/\varphi(n)$, while the large primes contribute a factor $1+o(1)$.

## Dirichlet series

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_series)

A Dirichlet series is a series of the form

$$
F(s)=\sum_{n=1}^{\infty}\frac{a_n}{n^s}.
$$

Multiplication of absolutely convergent Dirichlet series corresponds to [Dirichlet convolution](number-theory.md#dirichlet-convolution) of their coefficients.

### Holomorphy of a Dirichlet series from bounded partial sums

↑ **Parent:** [Dirichlet series](#dirichlet-series)

Writing $B(x)=\sum_{n\le x}b_n$, the [Abel summation formula](#abel-s-summation-formula) gives $\sum b_n n^{-s}=s\int_1^\infty B(x)x^{-s-1}\,dx$. If $B$ is bounded, the integral and its differentiated integrands converge uniformly on compact subsets of $\operatorname{Re}s>0$, giving a [holomorphic function](complex-analysis.md#holomorphic-function). A nonprincipal [Dirichlet character](algebraic-number-theory.md#dirichlet-character) has bounded partial sums because it is periodic and its sum over a period is zero.

// Target: algebra.bigb

### Epstein zeta function

↑ **Parent:** [Dirichlet series](#dirichlet-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Epstein_zeta_function)

For a full-rank [Euclidean lattice](fourier-analysis.md#euclidean-lattice) in $\mathbb R^n$, its Epstein zeta function is $E_\Lambda(s)=\sum_{0\ne x\in\Lambda}|x|^{-2s}$, initially convergent for $\operatorname{Re}s>n/2$. A [Mellin transform](analysis.md#mellin-transform) of its [theta function](modular-function.md#theta-function) gives its [completed Epstein zeta function](#completed-epstein-zeta-function) and a meromorphic continuation. Its sole pole has residue $\pi^{n/2}/[m(\Lambda)\Gamma(n/2)]$ at $s=n/2$.

#### Completed Epstein zeta function

↑ **Parent:** [Epstein zeta function](#epstein-zeta-function)

The completion $\mathcal E_\Lambda(s)=\pi^{-s}\Gamma(s)E_\Lambda(s)$ satisfies $\mathcal E_\Lambda(s)=m(\Lambda)^{-1}\mathcal E_{\Lambda^\vee}(n/2-s)$. Its simple poles at zero and $n/2$ have residues $-1$ and $m(\Lambda)^{-1}$. The [pole-subtracted theta integral for an Epstein zeta function](#pole-subtracted-theta-integral-for-an-epstein-zeta-function) gives both the continuation and this [dual lattice](fourier-analysis.md#dual-lattice) symmetry.

##### Pole-subtracted theta integral for an Epstein zeta function

↑ **Parent:** [Completed Epstein zeta function](#completed-epstein-zeta-function)

Put $a=n/2$, $m=m(\Lambda)$ and $A_\Lambda(s)=\int_1^\infty(\Theta_\Lambda(it)-1)t^{s-1}\,dt$, which is entire. Splitting the [Mellin transform](analysis.md#mellin-transform) at one and using the [lattice theta functional equation](modular-function.md#lattice-theta-functional-equation) gives $\mathcal E_\Lambda(s)=A_\Lambda(s)+m^{-1}A_{\Lambda^\vee}(a-s)+m^{-1}/(s-a)-1/s$. The two rational terms explicitly retain the contributions of the zero lattice vector.

### Dirichlet polynomial

↑ **Parent:** [Dirichlet series](#dirichlet-series)

A [Dirichlet polynomial](#dirichlet-polynomial) is a finite [Dirichlet series](#dirichlet-series), $A(s)=\sum_{n\le X}a_n n^{-s}$. Vertical integration separates equal product indices from oscillatory unequal ones.

#### Mean value of Dirichlet polynomials

↑ **Parent:** [Dirichlet polynomial](#dirichlet-polynomial)

For finite [Dirichlet polynomials](#dirichlet-polynomial), $\int_T^{2T}A(\sigma+it)\overline{B(\sigma+it)}\,dt$ has diagonal term $T\sum_n a_n\overline{b_n}/n^{2\sigma}$. Its off-diagonal error is bounded by $\sum_{m\ne n}|a_n b_m|/(n^\sigma m^\sigma|\log(m/n)|)$. A weighted row-sum estimate further bounds this by $\log(2X)\sum_{n\le X}n^{1-2\sigma}(|a_n|^2+|b_n|^2)$.

##### Odd moment of a prime cosine sum

↑ **Parent:** [Mean value of Dirichlet polynomials](#mean-value-of-dirichlet-polynomials)

For odd $j$, expanding $(\sum_{p\le X}p^{-\sigma}\cos(t\log p))^j$ gives products with different numbers of [prime factors](number-theory.md#prime-factor) on the two sides. [Unique prime factorization](number-theory.md#fundamental-theorem-of-arithmetic) rules out every diagonal equality. The integral over $[T,2T]$ is therefore $O_j(X^j(\sum_{n\le X^j}n^{-\sigma})^2)$.

### Euler product

↑ **Parent:** [Dirichlet series](#dirichlet-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_product)

An Euler product factors a [Dirichlet series](#dirichlet-series) into local factors indexed by [prime numbers](number-theory.md#prime-number). For a [multiplicative arithmetic function](number-theory.md#multiplicative-function) $f$ and in a half-plane of absolute convergence,

$$
\sum_{n\geq1}\frac{f(n)}{n^s}
=\prod_p\sum_{j\geq0}\frac{f(p^j)}{p^{js}}.
$$

#### Euler product positivity for L-function nonvanishing

↑ **Parent:** [Euler product](#euler-product)

For $\sigma>1$, logarithmic expansion of the [Euler product](#euler-product) reduces positivity to $3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2$. At [primes](number-theory.md#prime-number) dividing the modulus the zeta contribution is positive by itself. If the last factor is bounded at the line-one point, a zero of the middle factor would outweigh the zeta [pole](isolated-singularity.md#pole) and force this product to zero. This proves the relevant [nonvanishing of Dirichlet L-functions on the line one](algebraic-number-theory.md#nonvanishing-of-dirichlet-l-functions-on-the-line-one).

#### Truncated Euler-product lower bound

↑ **Parent:** [Euler product](#euler-product)

For a finite set of [primes](number-theory.md#prime-number) choose $0<g(p)<1$, put $k(p)=g(p)/(1-g(p))$, and let $W=\prod_p(1+k(p))$. Give each [squarefree integer](number-theory.md#squarefree-integer) $d$ on these primes probability $k(d)/W$. Inclusion of each [prime](number-theory.md#prime-number) is represented by a [Bernoulli random variable](discrete-probability-distribution.md#bernoulli-distribution) with parameter $g(p)$; these are [independent random variables](random-variable.md#independent-random-variables), so $\mathbb E[\log d]=\sum_pg(p)\log p$. If this is at most $\theta\log L$ with $0<\theta<1$, the [Markov inequality](probability-inequality.md#markov-inequality) gives

$$
\sum_{d\leq L}k(d)\geq(1-\theta)W.
$$

This turns a full [Euler product](#euler-product) into a lower bound for the truncated normalizing sum of a [Selberg sieve](#selberg-sieve).

#### Euler proof that the sum of reciprocals of primes diverges

↑ **Parent:** [Euler product](#euler-product)

For a finite set of primes,

$$
\prod_{p\leq x}\left(1-\frac1p\right)^{-1}
$$

expands as the sum of $1/n$ over positive integers whose prime factors are at most $x$. It contains every term with $n\leq x$, so these partial products dominate the [harmonic series](real-analysis.md#harmonic-series) and diverge. Since

$$
-\log(1-t)=t+O(t^2)
$$

uniformly for $0\leq t\leq1/2$, convergence of $\sum_p1/p$ would force convergence of the logarithms of these products, a contradiction.

##### Prime reciprocal lower bound

↑ **Parent:** [Euler proof that the sum of reciprocals of primes diverges](#euler-proof-that-the-sum-of-reciprocals-of-primes-diverges)

For $x\geq2$, the [harmonic number](#harmonic-number) $H_{\lfloor x\rfloor}$ exceeds $\log x$. The finite [Euler product](#euler-product) over the [primes](number-theory.md#prime-number) at most $x$ contains every summand of this [harmonic number](#harmonic-number). Taking [logarithms](calculus.md#logarithm) and applying the [geometric-series bound for the logarithmic remainder](calculus.md#geometric-series-bound-for-the-logarithmic-remainder) bounds the total remainder by $\frac12\sum_{n=2}^\infty[n(n-1)]^{-1}=1/2$, proving the displayed bound.

#### Three-four-one inequality for Euler products

↑ **Parent:** [Euler product](#euler-product)

For every complex number $z$ with $|z|\leq1$,

$$
3+4\Re z+\Re(z^2)\geq0.
$$

Applying this to each prime-power term in logarithms of Euler products proves that

$$
\zeta(\sigma)^3|D_f(\sigma+it)|^4|D_{f^2}(\sigma+2it)|\geq1
$$

for $\sigma>1$ and every completely multiplicative $f$ bounded by one.

<h3 id="perron-s-formula">Perron's formula</h3>

↑ **Parent:** [Dirichlet series](#dirichlet-series)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perron's_formula)

Perron's formula recovers a summatory arithmetic function from its [Dirichlet series](#dirichlet-series) by the inverse Mellin integral

$$
\sum_{n\leq x}a_n
=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
\left(\sum_{n\geq1}\frac{a_n}{n^s}\right)\frac{x^s}{s}\,ds,
$$

with the usual convergence and endpoint conventions.

#### Logarithmically smoothed Perron formula

↑ **Parent:** [Perron's formula](#perron-s-formula)

If the [Dirichlet series](#dirichlet-series) $F(s)=\sum_na_nn^{-s}$ is absolutely convergent at $\sigma>0$, then

$$
\sum_{n\le x}a_n\log(x/n)
=\frac1{2\pi i}\int_{\sigma-i\infty}^{\sigma+i\infty}\frac{F(s)x^s}{s^2}\,ds
=\frac1{2\pi}\int_{\mathbb R}\frac{F(\sigma+it)x^{\sigma+it}}{(\sigma+it)^2}\,dt.
$$

The scalar kernel is $(2\pi)^{-1}\int_{\mathbb R}e^{v(\sigma+it)}(\sigma+it)^{-2}dt=v_+$. This follows by [Fourier inversion](fourier-analysis.md#fourier-inversion-theorem) applied to $u e^{-\sigma u}\mathbf1_{u\ge0}$, whose [Fourier transform](analysis.md#fourier-transform) is $(\sigma+it)^{-2}$. Absolute convergence of the series and of $\int |\sigma+it|^{-2}dt$ justifies interchange. The factor $ds=i\,dt$ is essential.

##### Unsmoothing a logarithmically weighted sum

↑ **Parent:** [Logarithmically smoothed Perron formula](#logarithmically-smoothed-perron-formula)

Suppose $|a_n|\le(\log(2n))^k$ and $A(x)=\sum_{n\le x}a_n\log(x/n)=O(x(\log x)^\beta)$, with $0\le\beta\le k$. For $0<h\le1$, direct subtraction gives

$$
A(xe^h)-A(x)=h\sum_{n\le x}a_n+\sum_{x<n\le xe^h}a_n\log(xe^h/n).
$$

The last term has absolute value $O((xh^2+h)(\log x)^k)$. Choose $h=(\log x)^{(\beta-k)/2}$ to obtain the displayed bound, with an additional $O((\log x)^k)$ term harmless as $x\to\infty$ for fixed $k$. This elementary finite-difference argument converts a [logarithmically smoothed Perron formula](#logarithmically-smoothed-perron-formula) bound to cancellation in its original [partial sum](real-analysis.md#partial-sum).

#### Truncated Perron formula

↑ **Parent:** [Perron's formula](#perron-s-formula)

A truncated Perron integral over $c-iT$ to $c+iT$ recovers a summatory function with an error controlled by

$$
\sum_n |a_n|\left(\frac xn\right)^c
\min\left(1,\frac1{T|\log(x/n)|}\right).
$$

##### Short-interval Perron bound for the second Chebyshev function

↑ **Parent:** [Truncated Perron formula](#truncated-perron-formula)

For $c=1+1/\log x$, $1\le y\le x$ and $2\le T\le x$, apply the [truncated Perron formula](#truncated-perron-formula) with [Von Mangoldt function](number-theory.md#von-mangoldt-function) coefficients at both endpoints on the same vertical line. The difference kernel is $((x+y)^s-x^s)/s=\int_x^{x+y}u^{s-1}\,du$, of modulus $O(y)$. The usual near-integer error bound contributes $O(x\log^2x/T)$. The [logarithmic derivative](#logarithmic-derivative) on this line is finite because of the [Euler product](#euler-product).

##### Truncated Perron kernel estimate

↑ **Parent:** [Truncated Perron formula](#truncated-perron-formula)

For $v\ne1$, $K_T(v)$ differs from $1_{v>1}$ by $O(v^c\min(1,(T|\log v|)^{-1}))$. Close the contour to the left for $v>1$ and to the right for $v<1$; horizontal sides give the logarithmic denominator and the nearby transition is bounded. At $v=1$, direct integration gives $K_T(1)=\pi^{-1}\arctan(T/c)=1/2+O(c/T)$. This explains the half-weight endpoint in the [truncated Perron formula](#truncated-perron-formula). The constants may be taken uniform for $1\le c\le2$ and $T\ge2$.

## Riemann zeta function

↑ **Parent:** [Analytic number theory](analytic-number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_zeta_function)

$\zeta(s)=\sum_{n\ge1}n^{-s}$ for $\Re s>1$; its [Euler product](#euler-product) is $\prod_p(1-p^{-s})^{-1}$.

### Reciprocal Dirichlet-series bound on boundary-zero multiplicity

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

Absolute convergence of $1/\zeta(s)=\sum\mu(n)n^{-s}$ for $\operatorname{Re}s>1$ gives $|1/\zeta(\sigma+it)|\le\zeta(\sigma)=O((\sigma-1)^{-1})$ as $\sigma\downarrow1$. If $\zeta$ is holomorphic at $1+it_0$, a zero of order $m$ there would give reciprocal growth of order $(\sigma-1)^{-m}$ on the horizontal approach. Thus $m\le1$. This proves a multiplicity restriction, not existence of such a zero or a zero-free-line theorem.

### Reciprocal zeta bounds near the line one

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For $1<\sigma\le2$, the [three-four-one inequality for Euler products](#three-four-one-inequality-for-euler-products) gives $|1/\zeta(\sigma+it)|\le\zeta(\sigma)^{3/4}|\zeta(\sigma+2it)|^{1/4}$. For $|t|\ge1$, the [fractional-part continuation formula for the Riemann zeta function](#fractional-part-continuation-formula-for-the-riemann-zeta-function), truncated at $H\asymp2+|t|$, gives $\zeta^{(j)}(\sigma+it)=O_j(\log^{j+1}(2+|t|))$. Thus the reciprocal bound even holds with exponent $1/4$ instead of $1/2$ in this range. On bounded-height compact sets, [three-four-one product proof of zeta boundary nonvanishing](#three-four-one-product-proof-of-zeta-boundary-nonvanishing) and removal of the reciprocal's zero at the pole give uniform bounds. Differentiating $1/\zeta$ repeatedly yields

$$
\left|\left(\frac1\zeta\right)^{(k)}(\sigma+it)\right|
\ll_k(\sigma-1)^{-3(k+1)/4}\log^{3k+1}(2+|t|).
$$

The range restriction matters: $1/\zeta(\sigma)\to1$ as $\sigma\to\infty$, so the first displayed bound cannot hold uniformly for all $\sigma>1$. A global version replaces $(\sigma-1)^{-3/4}$ with $1+(\sigma-1)^{-3/4}$.

### Three-four-one product proof of zeta boundary nonvanishing

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For $\sigma>1$, the logarithm of the displayed product is a prime-power sum with coefficients $3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2\geq0$. A zero of order $a\geq1$ at $1+it$, with $t\neq0$, would make the product vanish like $O((\sigma-1)^{4a-3})$: the real factor has a pole of order three, and the third factor is bounded. This contradicts its lower bound one. Hence the [Riemann zeta function](#riemann-zeta-function) has no zeros on its line of real part one; its pole at one is not a zero.

<h3 id="lindelof-hypothesis">Lindelöf hypothesis</h3>

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lindelöf_hypothesis)

The hypothesis asks for growth smaller than every fixed positive power on the [critical line](#critical-line). The implied constant may depend on the chosen exponent. The [Riemann hypothesis implies the Lindelöf hypothesis](#riemann-hypothesis-implies-the-lindelof-hypothesis) through a smoothed explicit formula and strip convexity.

<h3 id="truncated-mobius-inverse-identity-for-the-riemann-zeta-function">Truncated Möbius inverse identity for the Riemann zeta function</h3>

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For $T/2\le\Im s\le T$ and $0<\Re s=\sigma\le1$, the [Hardy-Littlewood approximation to the Riemann zeta function](#hardy-littlewood-approximation-to-the-riemann-zeta-function) truncates zeta at $T$ with error $O(T^{-\sigma})$. Multiply the finite sums and use $a_n=\sum_{m\mid n,\ m\le M,\ n/m\le T}\mu(m)$. All coefficients with $1<n\le\min(M,T)$ vanish by the [Möbius divisor-sum identity](number-theory.md#mobius-divisor-sum-identity). The total error is bounded using $\sum_{m\le M}m^{-\sigma}\ll M^{1-\sigma}\log M$.

### Richert bound for the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For large positive $t$ and $0<\sigma\le1$, a fixed sufficiently large $C$ gives the displayed upper bound; to the right of one use $|\zeta(\sigma+it)|\ll\log^{2/3}t$. Its nonlinear dependence on $1-\sigma$ permits a wider [zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function) through the [Landau zero-free-region theorem](#landau-zero-free-region-theorem). Its proof uses estimates for [exponential sums](#exponential-sum); its use as an upper-bound input is separate from a proof of a zero-free region.

### Hardy-Littlewood approximation to the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For $s=\sigma+it$, $\sigma>0$, and $x\ge|t|/\pi$, the displayed approximation holds away from the [pole](isolated-singularity.md#pole). Apply the [Van der Corput sum-integral lemma](#van-der-corput-sum-integral-lemma) to $-t\log w/(2\pi)$ on $w\ge x$, where its derivative has modulus at most one half. [Abel summation](#abel-s-summation-formula) with $w^{-\sigma}$ converts the bounded unweighted discrepancy to $O(x^{-\sigma})$. [Locally uniform convergence](real-analysis.md#locally-uniform-convergence) of this weighted discrepancy extends the identity from $\sigma>1$ to $\sigma>0$. It turns estimates for finite [exponential sums](#exponential-sum) into estimates for the [Riemann zeta function](#riemann-zeta-function).

### Fractional-part continuation formula for the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

[Abel summation](#abel-s-summation-formula) applied to the counting function $\lfloor w\rfloor$ gives the displayed identity for $\Re s>1$ and every $x>0$. Since $0\le\{w\}<1$, the integral is [locally uniformly convergent](real-analysis.md#locally-uniform-convergence) and [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) for $\Re s>0$. This supplies a [meromorphic continuation](complex-analysis.md#meromorphic-continuation) of the [Riemann zeta function](#riemann-zeta-function) to that half-plane, with its sole [pole](isolated-singularity.md#pole) at one and [residue](analysis.md#residue) one. Keeping the fractional endpoint term makes the formula valid at noninteger cutoffs.

### Completed Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

The completed zeta function $\Lambda(s)=\pi^{-s/2}\Gamma(s/2)\zeta(s)$ satisfies $\Lambda(s)=\Lambda(1-s)$ and has poles at zero and one. It is also sometimes denoted $\xi(s)$; this differs from the entire xi function obtained by multiplying by $s(s-1)/2$. The distinction matters in the [constant term of a nonholomorphic Eisenstein series](modular-function.md#constant-term-of-a-nonholomorphic-eisenstein-series).

#### Riemann xi function

↑ **Parent:** [Completed Riemann zeta function](#completed-riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_xi_function)

Removing the completion's [poles](isolated-singularity.md#pole) produces an [entire function](complex-analysis.md#entire-function) with $\xi(0)=\xi(1)=1/2$ and $\xi(s)=\xi(1-s)$. Its zeros are the nontrivial zeros of the [Riemann zeta function](#riemann-zeta-function). Its finite order allows [Hadamard factorization](complex-analysis.md#hadamard-factorization-theorem), while the [xi modulus criterion for the Riemann hypothesis](#xi-modulus-criterion-for-the-riemann-hypothesis) characterizes their horizontal location.

##### Order-one growth of the Riemann xi function

↑ **Parent:** [Riemann xi function](#riemann-xi-function)

The [pole-subtracted theta integral for the completed zeta function](#pole-subtracted-theta-integral-for-the-completed-zeta-function) bounds the [Riemann xi function](#riemann-xi-function) on $|s|\leq R$ by a polynomial in $R$ times $\int_1^\infty e^{-\pi t}t^{(R+1)/2}\,dt$. The [Stirling formula](real-analysis.md#stirling-formula) gives logarithmic growth $O(R\log R)$. On the positive real axis, the definition and $\zeta(R)\geq1$ give $\log\xi(R)=\frac R2\log R+O(R)$. Thus its [order of an entire function](complex-analysis.md#order-of-an-entire-function) is exactly one.

// Target: analytic-number-theory.bigb

##### Real logarithmic derivative of Riemann xi

↑ **Parent:** [Riemann xi function](#riemann-xi-function)

Differentiate the genus-one [Hadamard factorization](complex-analysis.md#hadamard-factorization-theorem). Its complex difference terms converge as $O(|\rho|^{-2})$, and the individual real sums converge by the [absolute convergence of the real xi logarithmic derivative](#absolute-convergence-of-the-real-xi-logarithmic-derivative). The remaining constant is $\Re B+\sum\Re(1/\rho)$. On the [critical line](#critical-line) the xi [logarithmic derivative](#logarithmic-derivative) has zero real part, while the kernel terms cancel in pairs reflected across that line. Hence this constant vanishes and gives the displayed formula away from zeros.

###### Absolute convergence of the real xi logarithmic derivative

↑ **Parent:** [Real logarithmic derivative of Riemann xi](#real-logarithmic-derivative-of-riemann-xi)

The [Jensen zero-count bound](complex-analysis.md#jensen-zero-count-bound) gives $O(T\log T)$ zeros up to ordinate $T$. Since their real parts lie in $(0,1)$, a fixed-point real [logarithmic derivative](#logarithmic-derivative) summand is $O(|\Im\rho|^{-2})$. Dyadic ordinate bands then contribute $O(j2^{-j})$. This proves [absolute convergence](real-analysis.md#absolute-convergence) of the real sum, while the unpaired complex sum of reciprocals need not converge absolutely.

### Trivial zero of the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

The [trivial zeros of the Riemann zeta function](#trivial-zero-of-the-riemann-zeta-function) are $s=-2,-4,-6,\ldots$. The remaining zeros are the [Nontrivial zeros of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function).

### Fourth moment of the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

The [Riemann zeta function](#riemann-zeta-function) satisfies $\int_0^T|\zeta(1/2+it)|^4\,dt\ll T(\log T)^4$ for $T\ge2$. Squaring a short [Dirichlet polynomial](#dirichlet-polynomial) produces the [divisor function](number-theory.md#divisor-function); the [divisor-square summatory bound](number-theory.md#divisor-square-summatory-bound) controls the off-diagonal and diagonal terms.

### Bernoulli formula for zeta values at nonpositive integers

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For every integer $n\geq1$, the [Riemann zeta function](#riemann-zeta-function) satisfies $\zeta(1-n)=(-1)^{n-1}B_n/n$. One proof applies [meromorphic continuation of a Mellin transform from an asymptotic expansion](analysis.md#meromorphic-continuation-of-a-mellin-transform-from-an-asymptotic-expansion) to $(e^y-1)^{-1}$, whose transform is the [Bose integral](complex-analysis.md#bose-integral) $\Gamma(s)\zeta(s)$, and divides residues by the [residues of the Gamma function](complex-analysis.md#residues-of-the-gamma-function). The formula includes $\zeta(0)=-1/2$.

### Meromorphic continuation of the Riemann zeta function to the right half-plane

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

For $\Re s>0$,

$$
\zeta(s)=\frac{s}{s-1}
-s\int_1^\infty\frac{\{u\}}{u^{s+1}}\,du.
$$

The integral defines a [holomorphic function](complex-analysis.md#holomorphic-function) in that half-plane, so this continues $\zeta$ meromorphically across $\Re s=1$, with a simple pole of residue one at $s=1$.

### Basel problem

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Basel_problem)

The Basel problem asks for the exact value of $\zeta(2)$. Its answer is

$$
\sum_{n=1}^{\infty}\frac1{n^2}=\frac{\pi^2}{6}.
$$

### Functional equation of the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

The completed zeta function

$$
\xi(s)=\frac12s(s-1)\pi^{-s/2}\Gamma(s/2)\zeta(s)
$$

is an [entire function](complex-analysis.md#entire-function) satisfying $\xi(s)=\xi(1-s)$. Thus every nontrivial zero $\rho$ is accompanied by $1-\rho$, $\overline\rho$, and $1-\overline\rho$.

#### Mellin representation of the completed Riemann zeta function

↑ **Parent:** [Functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function)

For $\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}$ and initially $\Re s>1$,

$$
\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2}\frac{du}{u}.
$$

The [Poisson summation formula](fourier-analysis.md#poisson-summation-formula) gives $\Theta(u)=u^{-1/2}\Theta(1/u)$. Splitting the integral at one therefore continues it meromorphically and makes its invariance under $s\mapsto1-s$ visible.

##### Pole-subtracted theta integral for the completed zeta function

↑ **Parent:** [Mellin representation of the completed Riemann zeta function](#mellin-representation-of-the-completed-riemann-zeta-function)

Let $J(s)=\int_1^\infty(\theta(t)-1)t^{s/2-1}\,dt$, with $\theta(t)=\sum_{n\in\mathbb Z}e^{-\pi n^2t}$. Exponential decay makes $J$ an [entire function](complex-analysis.md#entire-function). The [Jacobi theta function](modular-function.md#jacobi-theta-function) transformation and a substitution in the [Mellin transform](analysis.md#mellin-transform) give

$$
\Lambda(s)=\frac1{s-1}-\frac1s+\frac12\bigl(J(s)+J(1-s)\bigr).
$$

This continues the completed [Riemann zeta function](#riemann-zeta-function) meromorphically, with residues $1$ and $-1$ at $1$ and $0$, and makes the [functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function) immediate. Dividing by the [Gamma function](complex-analysis.md#gamma-function) removes the apparent pole at zero from $\zeta(s)$.

#### Vertical-strip factor in the Riemann zeta functional equation

↑ **Parent:** [Functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function)

Writing

$$
\zeta(s)=\chi(s)\zeta(1-s),
\qquad
\chi(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s),
$$

the [Stirling formula](real-analysis.md#stirling-formula) gives, uniformly on every fixed vertical strip and for large $|t|$,

$$
|\chi(\sigma+it)|\asymp |t|^{1/2-\sigma}.
$$

### Euler-product nonvanishing of the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

Absolute convergence of the [Euler product](#euler-product) gives $\zeta(s)\ne0$ for $\Re s>1$. Equivalently,

$$
\frac1{\zeta(s)}=\sum_{n\geq1}\frac{\mu(n)}{n^s}
$$

converges absolutely there.

### Nontrivial zero of the Riemann zeta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)

A nontrivial zero of the [Riemann zeta function](#riemann-zeta-function) lies in the [critical strip](#critical-strip) $0<\Re s<1$. The [functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function) reflects such zeros across the [critical line](#critical-line) $\Re s=1/2$.

#### Critical strip

↑ **Parent:** [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_strip)

The critical strip for the [Riemann zeta function](#riemann-zeta-function) is $0<\Re s<1$.

##### Critical line

↑ **Parent:** [Critical strip](#critical-strip)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Critical_line)

The critical line is the symmetry line $\Re s=1/2$ inside the [critical strip](#critical-strip).

#### Riemann hypothesis

↑ **Parent:** [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann_hypothesis)

The Riemann hypothesis asserts that every [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) lies on the [critical line](#critical-line) $\Re s=1/2$.

<h5 id="riemann-hypothesis-implies-the-lindelof-hypothesis">Riemann hypothesis implies the Lindelöf hypothesis</h5>

↑ **Parent:** [Riemann hypothesis](#riemann-hypothesis)

The [subpower zeta bound to the right of the critical line](#subpower-zeta-bound-to-the-right-of-the-critical-line) gives an arbitrarily small exponent at $1/2+\delta$. The [functional equation](analysis.md#functional-equation) gives exponent $\delta+\varepsilon$ at $1/2-\delta$. The [Phragmén–Lindelöf principle](complex-analysis.md#phragmen-lindelof-principle) gives exponent $\delta/2+\varepsilon$ at the midpoint. Letting these fixed positive parameters be arbitrarily small proves the [Lindelöf hypothesis](#lindelof-hypothesis).

##### Subpower zeta bound to the right of the critical line

↑ **Parent:** [Riemann hypothesis](#riemann-hypothesis)

Under [Riemann hypothesis](#riemann-hypothesis), integrate a smoothed explicit formula from $1/2+\delta$ to two, taking $x=\log|t|$. The [prime](number-theory.md#prime-number) contribution is $O_\delta(x^{1-2\delta})$, while the local zero count bounds the zero contribution by $O_\delta(x^{-\delta}\log|t|/\log x)$. Both are $o(\log|t|)$ for fixed $0<\delta<1/4$, yielding the displayed bound; other fixed positive shifts follow by standard strip bounds and the [Euler product](#euler-product).

##### Xi modulus criterion for the Riemann hypothesis

↑ **Parent:** [Riemann hypothesis](#riemann-hypothesis)

[Riemann hypothesis](#riemann-hypothesis) is equivalent to monotonicity of $\sigma\mapsto|\xi(\sigma+it)|$ for every fixed $t$ on $\sigma\ge1/2$. Under [Riemann hypothesis](#riemann-hypothesis) the [real logarithmic derivative of Riemann xi](#real-logarithmic-derivative-of-riemann-xi) is positive for $\sigma>1/2$. Conversely a zero right of that line would force the nonnegative monotone modulus to vanish on an interval, contrary to the [identity theorem](complex-analysis.md#identity-theorem). Functional symmetry rules out zeros to the left.

##### Riemann hypothesis equivalence for the second Chebyshev function

↑ **Parent:** [Riemann hypothesis](#riemann-hypothesis)

The [Riemann hypothesis](#riemann-hypothesis) is equivalent to

$$
\psi(x)=x+O_\epsilon(x^{1/2+\epsilon})
$$

for every $\epsilon>0$. In fact, the hypothesis and the [Riemann–von Mangoldt explicit formula](number-theory.md#riemann-von-mangoldt-explicit-formula) give the stronger $O(x^{1/2}(\log x)^2)$ bound. Conversely, the stated error continues $-\zeta'/\zeta-s/(s-1)$ holomorphically to $\Re s>1/2$, excluding zeros there; the functional equation supplies the other half.

#### Zero-free region of the Riemann zeta function

↑ **Parent:** [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function)

The classical zero-free region asserts that for some $c>0$,

$$
\zeta(\sigma+it)\ne0
\quad\text{if}\quad
\sigma\geq1-\frac c{\log(|t|+3)}.
$$

Together with bounds for the [logarithmic derivative](#logarithmic-derivative), it permits contour arguments with exponentially small errors in $\sqrt{\log x}$.

##### Vinogradov-Korobov zero-free region

↑ **Parent:** [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)

For sufficiently large $|t|$, the [Riemann zeta function](#riemann-zeta-function) has no zeros in the displayed region, for a fixed positive $c$. To derive it from the [Richert bound for the Riemann zeta function](#richert-bound-for-the-riemann-zeta-function), take $\eta\asymp(\log\log t/\log t)^{2/3}$. The logarithm of the maximum on the two discs in the [Landau zero-free-region theorem](#landau-zero-free-region-theorem) is $O(\log\log t)$, as is $\log(1/\eta)$. Dividing $\eta$ by this logarithmic factor gives the displayed width.

##### Landau zero-free-region theorem

↑ **Parent:** [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)

For $t\ge2$ and $0<\eta\le1/4$, suppose $|\zeta|\le M$, $M\ge2$, on radius-$\eta$ discs centred at $1+\eta/4+it$ and $1+\eta/4+2it$. Every zero $\beta+it$ has the displayed gap. The reciprocal [Euler product](#euler-product) bounds both centre values below by a constant times $\eta$. The [local logarithmic-derivative lemma](#local-logarithmic-derivative-lemma) gives errors $B/\eta$, $B=1+\log(M/\eta)$. The [three-four-one zero-free-region argument](#three-four-one-zero-free-region-argument) then implies $4/(\sigma-\beta)-3/(\sigma-1)\ll B/\eta$. For a zero close to one, choose $\sigma=1+6(1-\beta)$, making the left side $1/(14(1-\beta))$. Zeros farther away already satisfy the bound. Thus a logarithmic upper bound for zeta translates into a quantitative zero-free width.

##### Weak logarithmic zero-free region for the Riemann zeta function

↑ **Parent:** [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)

The logarithm of the [Euler product](#euler-product) and $3+4\cos\theta+\cos2\theta\ge0$ give $\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1$. At $\sigma=1+a/\log^9|t|$, upper bounds $\zeta(\sigma)\ll\log^9|t|/a$ and $|\zeta(\sigma+2it)|\ll\log|t|$ imply the lower bound $|\zeta|\gg a^{3/4}\log^{-7}|t|$. The [Cauchy estimate for derivatives](analysis.md#cauchy-estimate) gives $|\zeta'|\ll\log^2|t|$ nearby, allowing a sufficiently small leftward displacement of order $\log^{-9}|t|$. This elementary region is weaker than the classical logarithmic region but gives an explicit reciprocal bound by simple estimates.

##### Three-four-one zero-free-region argument

↑ **Parent:** [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)

For $F=-\zeta'/\zeta$ and $\sigma>1$, positivity of

$$
3+4\cos\theta+\cos2\theta=2(1+\cos\theta)^2
$$

term by term in the [Euler product](#euler-product) gives

$$
3F(\sigma)+4\Re F(\sigma+it)+\Re F(\sigma+2it)\geq0.
$$

Comparing this with the pole of $F$ at one and the local poles of $\zeta'/\zeta$ at zeros proves the classical zero-free region.

##### Logarithmic derivative inside the zeta zero-free region

↑ **Parent:** [Zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function)

After shrinking the zero-free-region constant, one has

$$
\frac{\zeta'(\sigma+it)}{\zeta(\sigma+it)}\ll\log|t|
$$

in the half-width region $\sigma>1-c/(2\log|t|)$ for $|t|$ large. Compare the local partial-fraction expansion at $s$ with one at a point just to the right of one, where the [Euler product](#euler-product) controls the logarithmic derivative.

<h4 id="riemann-von-mangoldt-formula">Riemann–von Mangoldt formula</h4>

↑ **Parent:** [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Riemann–von_Mangoldt_formula)

If $N(T)$ counts the nontrivial zeta zeros $\rho=\beta+i\gamma$ with $0<\gamma\leq T$, including multiplicity, then

$$
N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}
-\frac{T}{2\pi}+O(\log T).
$$

In particular,

$$
\sum_{|\gamma|\leq T}\frac1{|\rho|}\ll(\log T)^2.
$$

##### Infinitely many reciprocal-logarithmic gaps between zeta zeros

↑ **Parent:** [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula)

List positive ordinates of [Nontrivial zeros of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) in nondecreasing order, including [multiplicity](polynomial.md#multiplicity-mathematics). If all sufficiently late gaps were at most $c/\log n$, summing would give $\gamma_n\le(c+o(1))n/\log n$, since $\sum_{j\le n}1/\log j\sim n/\log n$ with the sum starting at two. The [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula) would then give $n\le N(\gamma_n)\le(c/(2\pi)+o(1))n$, a contradiction when $c<2\pi$. The same argument applies when only distinct ordinates are listed, because $n\le N(\gamma_n)$ still holds.

##### Asymptotic inversion of the zeta zero count

↑ **Parent:** [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula)

List positive ordinates of [Nontrivial zeros of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) in nondecreasing order, including multiplicity. The [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula) gives $N(T)\sim T\log T/(2\pi)$. For each fixed $\varepsilon>0$, evaluate this at $T=(1\pm\varepsilon)2\pi n/\log n$ to bracket the $n$th ordinate. Letting $\varepsilon$ decrease to zero proves the displayed asymptotic without assuming simple zeros or distinct ordinates.

##### Local zero count for the Riemann zeta function

↑ **Parent:** [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula)

The number of [Nontrivial zeros of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) in a height interval of length one is $O(\log(|t|+3))$, including multiplicity and either endpoint. Subtract the [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula) at the endpoints and use conjugation at negative heights. Summing these counts with reciprocal-height weights gives $\sum_{|\Im\rho|\le T}1/|\rho|\ll\log^2(T+3)$.

###### Jensen disk proof of the zeta zero-count bound

↑ **Parent:** [Local zero count for the Riemann zeta function](#local-zero-count-for-the-riemann-zeta-function)

Put $F(s)=(s-1)\zeta(s)$. The [fractional-part continuation formula for the Riemann zeta function](#fractional-part-continuation-formula-for-the-riemann-zeta-function) gives $|F(s)|\ll(|s|+1)^2$ for $\operatorname{Re}s\geq1/4$. At $2+ij$, the reciprocal [Euler product](#euler-product) bounds $|\zeta(2+ij)|$ below by $1/\zeta(2)$. Applying the [Jensen zero-count bound](complex-analysis.md#jensen-zero-count-bound) with outer radius $7/4$ and inner radius $8/5$ gives $O(\log(|j|+2))$ zeros in the latter disk. Those disks cover the half-strip $1/2\leq\operatorname{Re}s\leq1$. Reflecting zeros using the [functional equation of the Riemann zeta function](#functional-equation-of-the-riemann-zeta-function) completes the $O(T\log T)$ bound without requiring left-half-plane growth estimates.

###### Smoothed zeta zero-count bound

↑ **Parent:** [Local zero count for the Riemann zeta function](#local-zero-count-for-the-riemann-zeta-function)

Evaluate the [real logarithmic derivative of Riemann xi](#real-logarithmic-derivative-of-riemann-xi) at real part two, where every summand is positive and comparable to this kernel. The gamma [logarithmic derivative](#logarithmic-derivative) and the bounded zeta [logarithmic derivative](#logarithmic-derivative) give the logarithmic bound. It implies the local unit-interval count, and conversely such local counts imply this smoothed bound by summing the decaying tails.

### Logarithmic derivative

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Logarithmic_derivative)

The logarithmic derivative of a nonzero differentiable function $f$ is $f'/f$. For $\Re s>1$, the [Euler product](#euler-product) for the [Riemann zeta function](#riemann-zeta-function) gives

$$
-\frac{\zeta'(s)}{\zeta(s)}
=\sum_{n\geq1}\frac{\Lambda(n)}{n^s}.
$$

#### Global partial-fraction expansion of the zeta logarithmic derivative

↑ **Parent:** [Logarithmic derivative](#logarithmic-derivative)

Here $\psi=\Gamma'/\Gamma$ is the [digamma function](complex-analysis.md#digamma-function), $B=\log2+\frac12\log\pi-1-\gamma/2$, and $\gamma$ is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant). The sum runs over [Nontrivial zeros of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) with multiplicities. Each displayed paired summand is $O_s(|\rho|^{-2})$, so it converges locally uniformly away from zeros. Differentiate the genus-one [Hadamard factorization](complex-analysis.md#hadamard-factorization-theorem) of the [Riemann xi function](#riemann-xi-function) and use the [Gamma function recurrence](complex-analysis.md#gamma-function-recurrence). Unlike an unpaired reciprocal-zero sum, this expression does not require an unstated summation convention.

#### Local logarithmic-derivative lemma

↑ **Parent:** [Logarithmic derivative](#logarithmic-derivative)

If $f$ is [holomorphic](complex-analysis.md#complex-differentiability-at-a-point) near the closed radius-$R$ disc, $f(z_0)\ne0$, and $|f|\le M$, the displayed estimate holds away from zeros for $|z-z_0|\le R/3$, counting zeros with multiplicity. Factoring local zeros isolates their poles; the remaining logarithm is controlled by disc estimates. If all zeros lie to the left of a point $z$ in real part, their real contributions are nonnegative. This is the disc estimate used by the [Landau zero-free-region theorem](#landau-zero-free-region-theorem); a version with general radius ratios is Lemma 24.17 in [Montgomery and Vaughan](https://personal.science.psu.edu/rcv4/Vol3/Vol3.pdf).

#### Local partial-fraction expansion of the Riemann zeta logarithmic derivative

↑ **Parent:** [Logarithmic derivative](#logarithmic-derivative)

Uniformly in a fixed bounded-width disk around height $t$,

$$
\frac{\zeta'(s)}{\zeta(s)}
=\sum_{\rho\text{ nearby}}\frac1{s-\rho}
+O(\log(|t|+3)).
$$

This follows by taking the logarithmic derivative of the Hadamard product for the completed zeta function and estimating the distant zeros.

#### Prime number theorem

↑ **Parent:** [Logarithmic derivative](#logarithmic-derivative)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_number_theorem)

The prime number theorem states that $\pi(x)\sim x/\log x$, equivalently $\sum_{n\leq x}\Lambda(n)\sim x$.

##### Prime number theorem error from a fixed zero-free strip

↑ **Parent:** [Prime number theorem](#prime-number-theorem)

If all nontrivial zeta zeros satisfy $\Re\rho\leq1-c$ with fixed $0<c<1/2$, the [Riemann–von Mangoldt formula](#riemann-von-mangoldt-formula) gives $\sum_{|\rho|<T}|\rho|^{-1}\ll\log^2T$. The [truncated explicit formula for the second Chebyshev function](number-theory.md#truncated-explicit-formula-for-the-second-chebyshev-function) then bounds the error by $O(x^{1-c}\log^2T+x\log^2x/T)$. Choosing $T=x^c$ gives the displayed bound and, for every positive $\varepsilon$, $O_\varepsilon(x^{1-c+\varepsilon})$.

// Target: number-theory.bigb

##### Prime number theorem error from a logarithmic zero-free region

↑ **Parent:** [Prime number theorem](#prime-number-theorem)

Suppose $A>0$ and every sufficiently high [Nontrivial zero of the Riemann zeta function](#nontrivial-zero-of-the-riemann-zeta-function) satisfies the displayed gap, with bounded heights also separated from one. The [truncated explicit formula for the second Chebyshev function](number-theory.md#truncated-explicit-formula-for-the-second-chebyshev-function) and the [local zero count for the Riemann zeta function](#local-zero-count-for-the-riemann-zeta-function) give errors $x\log^2x\exp(-c\log x/(\log T)^A)$ and $x\log^2x/T$. Balance them by $\log T\asymp(\log x)^{1/(A+1)}$. This explains how the width of a [zero-free region of the Riemann zeta function](#zero-free-region-of-the-riemann-zeta-function) determines the exponential scale in the [Prime number theorem](#prime-number-theorem) error.

##### Prime number theorem with classical zero-free-region error

↑ **Parent:** [Prime number theorem](#prime-number-theorem)

The classical zero-free region and a truncated Perron contour give

$$
\sum_{n\leq x}\Lambda(n)
=x+O\left(xe^{-c\sqrt{\log x}}\right)
$$

for some constant $c>0$.

##### Smoothed prime number theorem from a zero-free region

↑ **Parent:** [Prime number theorem](#prime-number-theorem)

For a smooth compactly supported $F:(0,\infty)\to\mathbb R$ whose [Mellin transform](analysis.md#mellin-transform) has suitable vertical decay, [Mellin inversion](analysis.md#mellin-inversion-theorem) and

$$
-\frac{\zeta'(s)}{\zeta(s)}=\sum_{n\geq1}\frac{\Lambda(n)}{n^s}
$$

give

$$
\sum_n\Lambda(n)F(n/X)
=\frac1{2\pi i}\int_{(2)}-\frac{\zeta'(s)}{\zeta(s)}\widetilde F(s)X^s\,ds.
$$

Moving the contour through the pole at $s=1$ and into the classical zero-free region gives main term $X\widetilde F(1)$ and error $O(X^{1-c/\log\log X})$ when $\widetilde F(\sigma+it)\ll e^{-|t|^{1/2}}$.

#### Twisted Von Mangoldt estimate implying the Riemann hypothesis

↑ **Parent:** [Logarithmic derivative](#logarithmic-derivative)

If, for some real $u$,

$$
\sum_{n\leq x}\Lambda(n)n^{iu}
=\frac{x^{1+iu}}{1+iu}+O\left(x^{1/2}(\log x)^2\right),
$$

then partial summation continues $-\zeta'(s-iu)/\zeta(s-iu)$ meromorphically to $\Re s>1/2$ with no pole except at $1+iu$. The zeta function has no zero to the right of the critical line, and its functional equation then implies the Riemann hypothesis.

### Dirichlet eta function

↑ **Parent:** [Riemann zeta function](#riemann-zeta-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_eta_function)

For $\Re s>0$, the alternating [Dirichlet series](#dirichlet-series)

$$
\eta(s)=\sum_{n=1}^\infty(-1)^{n-1}n^{-s}
$$

converges locally uniformly and defines a [holomorphic function](complex-analysis.md#holomorphic-function). For $\Re s>1$,

$$
\eta(s)=(1-2^{1-s})\zeta(s).
$$

#### Analytic continuation of the Riemann zeta function to the right half-plane

↑ **Parent:** [Dirichlet eta function](#dirichlet-eta-function)

The identity $\zeta(s)=\eta(s)/(1-2^{1-s})$ continues the [Riemann zeta function](#riemann-zeta-function) meromorphically to $\Re s>0$. Apparent singularities at nonreal zeros of $1-2^{1-s}$ are removable, as one sees by replacing $2$ with an integer $k$ for which $1-k^{1-s}\ne0$. At $s=1$, $\eta(1)=\log2$ and $1-2^{1-s}\sim(s-1)\log2$, so $\zeta$ has a simple pole of residue one.

## ↑ Ancestors (4)

1. [Number theory](number-theory.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)

## ← Incoming links (1)

- [Type I sum](#type-i-sum)
