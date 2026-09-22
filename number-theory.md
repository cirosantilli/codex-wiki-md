# Number theory

↑ **Parent:** [Area of mathematics](mathematics.md#area-of-mathematics)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Number_theory)

Number theory studies [integers](#integer), their [divisibility](#divisibility), and the patterns created by [prime numbers](#prime-number). Its questions often have short statements but rigid answers: which [integers](#integer) divide a given one, when does an [equation](algebra.md#equation) have integer solutions, and when can arithmetic with [congruence classes](#congruence-class) be reversed? The [Euclidean algorithm](#euclidean-algorithm) and [modular multiplicative inverses](#modular-multiplicative-inverse) connect these questions through explicit calculations.

For example, $252=2^2\cdot3^2\cdot7$ and $198=2\cdot3^2\cdot11$. Their shared [prime factors](#prime-factor) give [greatest common divisor](#greatest-common-divisor) $18$. The [Euclidean algorithm](#euclidean-algorithm) reaches that answer without finding either complete [prime factorization](#fundamental-theorem-of-arithmetic). It also produces $18=4\cdot252-5\cdot198$, an instance of [Bézout's identity](algebra.md#bezout-s-identity). This relation certifies every common [divisor](#divisor) at once and solves an associated [linear Diophantine equation](#linear-diophantine-equation).

[Modular arithmetic](#modular-arithmetic) retains only remainders, but the lost information can be surprisingly controlled. Multiplication by $5$ modulo $17$ is a [permutation](combinatorics.md#permutation) of all residue classes, because $5$ has [modular inverse](#modular-multiplicative-inverse) $7$. Multiplication by $5$ modulo $15$ collapses fifteen residue classes to three. Thus an apparently small change in the modulus changes whether a calculation can be reversed. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) explains another kind of compression: remainders modulo [coprime integers](#coprime-integers) can be combined into one remainder modulo their product.

Simple restrictions help reveal the structure without telling the whole story. Every [prime number](#prime-number) greater than three is congruent to $1$ or $5$ modulo $6$: the other four residue classes force [divisibility](#divisibility) by $2$ or $3$. The converse fails because $25$ and $35$ lie in those classes but are [composite numbers](#composite-number). Necessary conditions are useful filters, not substitutes for [primality testing](computer-science.md#primality-testing).

The subject's appeal lies partly in this tension: [prime factorization](#fundamental-theorem-of-arithmetic) gives a clean description of every positive [integer](#integer), while identifying factors and predicting their distribution lead to substantial further questions. [Analytic number theory](analytic-number-theory.md) uses tools from [analysis](analysis.md) to study global patterns, and [algebraic number theory](algebraic-number-theory.md) extends arithmetic into [number fields](algebraic-number-theory.md#number-field). Applications include [cryptography](computer-science.md#cryptography) and [error-correcting codes](coding-theory.md#error-correcting-code); MIT's discrete applied mathematics course develops modular structures for both purposes. [Ankur Moitra, MIT 18.200, Modular Arithmetic and Elementary Algebra, 2024, introduction](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

Euclid's _Elements_ already gives a greatest-common-measure construction in Book VII, Proposition 2, and the argument that a finite list cannot exhaust the [prime numbers](#prime-number) in Book IX, Proposition 20. These are documented ancient treatments, rather than evidence that all of number theory began with one author. [Euclid, Elements VII.2, translated text hosted by David Joyce](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII2.html) [Euclid, Elements IX.20, translated text hosted by David Joyce](https://mathcs.clarku.edu/~djoyce/java/elements/bookIX/propIX20.html)

**Table of contents**

- [Integer factorization](#integer-factorization)
  - [Factor base](#factor-base)
    - [Exponent vector](#exponent-vector)
  - [Odd part of a positive integer](#odd-part-of-a-positive-integer)
  - [Congruence of squares](#congruence-of-squares)
    - [Nontrivial square root of unity modulo an integer](#nontrivial-square-root-of-unity-modulo-an-integer)
- [Erdős-Turán inequality](#erdos-turan-inequality)
- [Fermat number](#fermat-number)
  - [Fermat number product identity](#fermat-number-product-identity)
    - [Distinct Fermat numbers are coprime](#distinct-fermat-numbers-are-coprime)
  - [Prime divisor of a Fermat number](#prime-divisor-of-a-fermat-number)
    - [Stronger prime-divisor congruence for Fermat numbers](#stronger-prime-divisor-congruence-for-fermat-numbers)
- [Bernoulli number](#bernoulli-number)
  - [Bernoulli polynomial](#bernoulli-polynomial)
    - [Integer power sum](#integer-power-sum)
      - [Bernoulli corrections for polynomial sums](#bernoulli-corrections-for-polynomial-sums)
  - [Hyperbolic cotangent generating function for Bernoulli numbers](#hyperbolic-cotangent-generating-function-for-bernoulli-numbers)
  - [Euler evaluation of even zeta values](#euler-evaluation-of-even-zeta-values)
  - [Generalized Bernoulli number](#generalized-bernoulli-number)
- [Normal number](#normal-number)
  - [Digit block frequency](#digit-block-frequency)
  - [Simply normal number](#simply-normal-number)
  - [Champernowne constant](#champernowne-constant)
  - [Normality and equidistribution under integer multiplication](#normality-and-equidistribution-under-integer-multiplication)
  - [Absolutely normal number](#absolutely-normal-number)
- [Natural density](#natural-density)
  - [Set without natural density](#set-without-natural-density)
  - [Upper asymptotic density](#upper-asymptotic-density)
  - [Full-density sequence](#full-density-sequence)
- [Lagrange's four-square theorem](#lagrange-s-four-square-theorem)
- [Arithmetic function](#arithmetic-function)
  - [Radical of an integer](#radical-of-an-integer)
    - [Prime support of an integer](#prime-support-of-an-integer)
  - [Total number of prime factors](#total-number-of-prime-factors)
    - [Excess prime-factor multiplicity](#excess-prime-factor-multiplicity)
  - [Additive function (number theory)](#additive-function-number-theory)
    - [Mean of an additive arithmetic function](#mean-of-an-additive-arithmetic-function)
    - [Strongly additive arithmetic function](#strongly-additive-arithmetic-function)
    - [Completely additive arithmetic function](#completely-additive-arithmetic-function)
  - [Multiplicative function](#multiplicative-function)
    - [Multiplicativity of an arithmetic function](#multiplicativity-of-an-arithmetic-function)
    - [Completely multiplicative function](#completely-multiplicative-function)
    - [Divisor sum](#divisor-sum)
      - [Sum-of-divisors function](#sum-of-divisors-function)
        - [Proper-divisor sum](#proper-divisor-sum)
    - [Pretentious distance](#pretentious-distance)
      - [Large Fourier coefficient criterion for pretentiousness](#large-fourier-coefficient-criterion-for-pretentiousness)
      - [Pretentious distance between one and the Möbius function](#pretentious-distance-between-one-and-the-mobius-function)
      - [Prime-restriction metric for pretentious distance](#prime-restriction-metric-for-pretentious-distance)
      - [Triangle inequality for pretentious distance](#triangle-inequality-for-pretentious-distance)
      - [Archimedean character](#archimedean-character)
      - [Halász theorem](#halasz-theorem)
      - [Strong aperiodicity of the Möbius function](#strong-aperiodicity-of-the-mobius-function)
  - [Pointwise product of arithmetic functions](#pointwise-product-of-arithmetic-functions)
  - [Dirichlet convolution](#dirichlet-convolution)
    - [Multiplicativity of Dirichlet convolution](#multiplicativity-of-dirichlet-convolution)
    - [Constant-one arithmetic function](#constant-one-arithmetic-function)
    - [Identity arithmetic function](#identity-arithmetic-function)
    - [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution)
    - [Dirichlet hyperbola method](#dirichlet-hyperbola-method)
      - [Divisor summatory function](#divisor-summatory-function)
      - [Asymmetric Dirichlet hyperbola split](#asymmetric-dirichlet-hyperbola-split)
      - [Arithmetic work of the Dirichlet hyperbola method](#arithmetic-work-of-the-dirichlet-hyperbola-method)
      - [Divisor summatory asymptotic](#divisor-summatory-asymptotic)
      - [Harmonic divisor sum](#harmonic-divisor-sum)
  - [Divisor function](#divisor-function)
    - [Subpower bound for the divisor function](#subpower-bound-for-the-divisor-function)
    - [Divisor-square summatory bound](#divisor-square-summatory-bound)
  - [Von Mangoldt function](#von-mangoldt-function)
    - [Selberg symmetry formula](#selberg-symmetry-formula)
    - [Von Mangoldt divisor identity](#von-mangoldt-divisor-identity)
    - [Chebyshev function](#chebyshev-function)
      - [Second Chebyshev function](#second-chebyshev-function)
        - [First integral of the Chebyshev function](#first-integral-of-the-chebyshev-function)
          - [Smoothed explicit formula for the Chebyshev function](#smoothed-explicit-formula-for-the-chebyshev-function)
        - [Integrated Chebyshev sum](#integrated-chebyshev-sum)
        - [Chebyshev estimate](#chebyshev-estimate)
          - [Chebyshev estimate from central binomial coefficients](#chebyshev-estimate-from-central-binomial-coefficients)
        - [Riemann–von Mangoldt explicit formula](#riemann-von-mangoldt-explicit-formula)
          - [Truncated explicit formula for the second Chebyshev function](#truncated-explicit-formula-for-the-second-chebyshev-function)
    - [Vaughan's identity](#vaughan-s-identity)
      - [Prime exponential-sum estimate from Vaughan identity](#prime-exponential-sum-estimate-from-vaughan-identity)
      - [Logarithmic coefficient bound in Vaughan identity](#logarithmic-coefficient-bound-in-vaughan-identity)
      - [Vaughan identity for the Möbius function](#vaughan-identity-for-the-mobius-function)
        - [Type I–type II inverse principle for Möbius correlation](#type-i-type-ii-inverse-principle-for-mobius-correlation)
      - [Vaughan identity proof](#vaughan-identity-proof)
  - [Prime omega function](#prime-omega-function)
    - [Three to the distinct-prime-factor count](#three-to-the-distinct-prime-factor-count)
      - [Summatory bound for three to the prime omega](#summatory-bound-for-three-to-the-prime-omega)
      - [Log-weighted convolution bound for three to the prime omega](#log-weighted-convolution-bound-for-three-to-the-prime-omega)
  - [Möbius function](#mobius-function)
    - [Möbius divisor-sum identity](#mobius-divisor-sum-identity)
    - [Möbius harmonic logarithmic moments](#mobius-harmonic-logarithmic-moments)
    - [Möbius inversion formula](#mobius-inversion-formula)
    - [Mertens function](#mertens-function)
      - [Prime number asymptotic from Mertens cancellation](#prime-number-asymptotic-from-mertens-cancellation)
      - [Mertens bound from a log-integrable Chebyshev error](#mertens-bound-from-a-log-integrable-chebyshev-error)
      - [Mertens function bound from the classical zeta zero-free region](#mertens-function-bound-from-the-classical-zeta-zero-free-region)
- [Analytic number theory](analytic-number-theory.md)
  - [Hardy-Littlewood circle method](analytic-number-theory.md#hardy-littlewood-circle-method)
    - [Vinogradov's three-primes theorem](analytic-number-theory.md#vinogradov-s-three-primes-theorem)
    - [Singular series](analytic-number-theory.md#singular-series)
    - [Minor arc](analytic-number-theory.md#minor-arc)
    - [Major arc](analytic-number-theory.md#major-arc)
  - [L-function](analytic-number-theory.md#l-function)
    - [Hasse–Weil zeta function](analytic-number-theory.md#hasse-weil-zeta-function)
    - [Hasse-Weil L-function](analytic-number-theory.md#hasse-weil-l-function)
    - [Hecke L-function](analytic-number-theory.md#hecke-l-function)
    - [p-adic L-function](analytic-number-theory.md#p-adic-l-function)
      - [Kubota-Leopoldt p-adic L-function](analytic-number-theory.md#kubota-leopoldt-p-adic-l-function)
        - [p-adic zeta pseudomeasure](analytic-number-theory.md#p-adic-zeta-pseudomeasure)
  - [Linnik's theorem](analytic-number-theory.md#linnik-s-theorem)
  - [Character sum](analytic-number-theory.md#character-sum)
    - [Pólya–Vinogradov inequality](analytic-number-theory.md#polya-vinogradov-inequality)
  - [Prime sum](analytic-number-theory.md#prime-sum)
  - [Bombieri–Vinogradov theorem](analytic-number-theory.md#bombieri-vinogradov-theorem)
    - [Weighted arithmetic-progression error bound](analytic-number-theory.md#weighted-arithmetic-progression-error-bound)
  - [Exponential sum](analytic-number-theory.md#exponential-sum)
    - [Weyl differencing](analytic-number-theory.md#weyl-differencing)
      - [Weyl inequality](analytic-number-theory.md#weyl-inequality)
      - [Cubic Weyl inequality](analytic-number-theory.md#cubic-weyl-inequality)
      - [Hua's lemma](analytic-number-theory.md#hua-s-lemma)
        - [Cubic eighth-moment proof by differencing](analytic-number-theory.md#cubic-eighth-moment-proof-by-differencing)
    - [Power Gauss sum over a prime field](analytic-number-theory.md#power-gauss-sum-over-a-prime-field)
      - [Three power summands over a large prime field](analytic-number-theory.md#three-power-summands-over-a-large-prime-field)
    - [Quadratic exponential sum](analytic-number-theory.md#quadratic-exponential-sum)
      - [Quadratic Weyl inequality](analytic-number-theory.md#quadratic-weyl-inequality)
    - [Vinogradov mean value](analytic-number-theory.md#vinogradov-mean-value)
      - [Vinogradov mean-value method for a bilinear exponential sum](analytic-number-theory.md#vinogradov-mean-value-method-for-a-bilinear-exponential-sum)
    - [Bilinear shift averaging for a logarithmic phase](analytic-number-theory.md#bilinear-shift-averaging-for-a-logarithmic-phase)
    - [Van der Corput sum-integral lemma](analytic-number-theory.md#van-der-corput-sum-integral-lemma)
    - [Cancellation in an exponential sum](analytic-number-theory.md#cancellation-in-an-exponential-sum)
  - [Probabilistic number theory](analytic-number-theory.md#probabilistic-number-theory)
    - [Erdős-Kac theorem](analytic-number-theory.md#erdos-kac-theorem)
      - [Centered moment comparison for additive arithmetic functions](analytic-number-theory.md#centered-moment-comparison-for-additive-arithmetic-functions)
    - [Cramér model](analytic-number-theory.md#cramer-model)
      - [Cramér model prime-gap upper bound](analytic-number-theory.md#cramer-model-prime-gap-upper-bound)
    - [Multiplication table problem](analytic-number-theory.md#multiplication-table-problem)
      - [Multiplication table bound from distinct prime factors](analytic-number-theory.md#multiplication-table-bound-from-distinct-prime-factors)
    - [Turán-Kubilius inequality](analytic-number-theory.md#turan-kubilius-inequality)
  - [Landau theorem for a Dirichlet series with nonnegative coefficients](analytic-number-theory.md#landau-theorem-for-a-dirichlet-series-with-nonnegative-coefficients)
  - [Nonvanishing of a nonprincipal Dirichlet L-function at one](analytic-number-theory.md#nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one)
  - [Chebyshev function in an arithmetic progression](analytic-number-theory.md#chebyshev-function-in-an-arithmetic-progression)
  - [Classical zero-free region for Dirichlet L-functions](analytic-number-theory.md#classical-zero-free-region-for-dirichlet-l-functions)
    - [Uniqueness of a possible exceptional real Dirichlet zero](analytic-number-theory.md#uniqueness-of-a-possible-exceptional-real-dirichlet-zero)
    - [Siegel zero](analytic-number-theory.md#siegel-zero)
      - [Landau theorem for two real Dirichlet characters](analytic-number-theory.md#landau-theorem-for-two-real-dirichlet-characters)
        - [Sparse conductors of exceptional real Dirichlet zeros](analytic-number-theory.md#sparse-conductors-of-exceptional-real-dirichlet-zeros)
      - [Prime number theorem in an arithmetic progression with an exceptional zero](analytic-number-theory.md#prime-number-theorem-in-an-arithmetic-progression-with-an-exceptional-zero)
        - [Exceptional-zero bound from a uniform upper bound in arithmetic progressions](analytic-number-theory.md#exceptional-zero-bound-from-a-uniform-upper-bound-in-arithmetic-progressions)
  - [Pretentious number theory](analytic-number-theory.md#pretentious-number-theory)
  - [Normal order of an arithmetic function](analytic-number-theory.md#normal-order-of-an-arithmetic-function)
    - [Turán normal-order theorem for distinct prime divisors](analytic-number-theory.md#turan-normal-order-theorem-for-distinct-prime-divisors)
  - [Dirichlet's theorem on arithmetic progressions](analytic-number-theory.md#dirichlet-s-theorem-on-arithmetic-progressions)
    - [Reciprocal primes in a fixed arithmetic progression](analytic-number-theory.md#reciprocal-primes-in-a-fixed-arithmetic-progression)
    - [Siegel–Walfisz theorem](analytic-number-theory.md#siegel-walfisz-theorem)
      - [Major-arc value of the prime exponential sum](analytic-number-theory.md#major-arc-value-of-the-prime-exponential-sum)
    - [Prime-character sum near one](analytic-number-theory.md#prime-character-sum-near-one)
  - [Harmonic number](analytic-number-theory.md#harmonic-number)
  - [Abel's summation formula](analytic-number-theory.md#abel-s-summation-formula)
    - [Reciprocal-sum convergence from a counting bound](analytic-number-theory.md#reciprocal-sum-convergence-from-a-counting-bound)
    - [Bounded-variation multipliers of a convergent series](analytic-number-theory.md#bounded-variation-multipliers-of-a-convergent-series)
    - [Exponentially damped reciprocal-prime sum](analytic-number-theory.md#exponentially-damped-reciprocal-prime-sum)
  - [Reciprocal fractional-part sum near a rational](analytic-number-theory.md#reciprocal-fractional-part-sum-near-a-rational)
  - [Bilinear quadratic exponential sum fourth-moment bound](analytic-number-theory.md#bilinear-quadratic-exponential-sum-fourth-moment-bound)
    - [Factorized fourth moment for a bilinear quadratic exponential sum](analytic-number-theory.md#factorized-fourth-moment-for-a-bilinear-quadratic-exponential-sum)
      - [Truncation of a divisor weight by its second moment](analytic-number-theory.md#truncation-of-a-divisor-weight-by-its-second-moment)
  - [Bilinear sum](analytic-number-theory.md#bilinear-sum)
    - [Vinogradov Type I–II method](analytic-number-theory.md#vinogradov-type-i-ii-method)
      - [Small Type I and Type II sums](analytic-number-theory.md#small-type-i-and-type-ii-sums)
    - [Fourier separation of interval cutoffs](analytic-number-theory.md#fourier-separation-of-interval-cutoffs)
    - [Bilinear cancellation for badly approximable phases](analytic-number-theory.md#bilinear-cancellation-for-badly-approximable-phases)
    - [Type II sum](analytic-number-theory.md#type-ii-sum)
      - [Rational-phase Type II estimate](analytic-number-theory.md#rational-phase-type-ii-estimate)
    - [Type I sum](analytic-number-theory.md#type-i-sum)
    - [Dyadic decomposition](analytic-number-theory.md#dyadic-decomposition)
  - [Sieve theory](analytic-number-theory.md#sieve-theory)
    - [Parity problem](analytic-number-theory.md#parity-problem)
    - [Integers with all prime factors congruent to one modulo four](analytic-number-theory.md#integers-with-all-prime-factors-congruent-to-one-modulo-four)
    - [Large sieve](analytic-number-theory.md#large-sieve)
      - [Large sieve upper bound for sifted intervals](analytic-number-theory.md#large-sieve-upper-bound-for-sifted-intervals)
      - [Character large sieve](analytic-number-theory.md#character-large-sieve)
      - [Variance form of the large sieve](analytic-number-theory.md#variance-form-of-the-large-sieve)
      - [Exponential-sum large sieve](analytic-number-theory.md#exponential-sum-large-sieve)
        - [Fejér-kernel proof of the analytic large sieve](analytic-number-theory.md#fejer-kernel-proof-of-the-analytic-large-sieve)
        - [Local-multiplicity large sieve](analytic-number-theory.md#local-multiplicity-large-sieve)
          - [Prime-denominator large sieve](analytic-number-theory.md#prime-denominator-large-sieve)
      - [Circular spacing](analytic-number-theory.md#circular-spacing)
    - [Buchstab function](analytic-number-theory.md#buchstab-function)
      - [Oscillation of the Buchstab function](analytic-number-theory.md#oscillation-of-the-buchstab-function)
      - [Buchstab theorem](analytic-number-theory.md#buchstab-theorem)
    - [Rough number](analytic-number-theory.md#rough-number)
    - [Sifting function](analytic-number-theory.md#sifting-function)
      - [Sieve distribution](analytic-number-theory.md#sieve-distribution)
      - [Buchstab identity](analytic-number-theory.md#buchstab-identity)
    - [Upper-bound sieve](analytic-number-theory.md#upper-bound-sieve)
      - [Brun–Titchmarsh theorem](analytic-number-theory.md#brun-titchmarsh-theorem)
      - [Selberg sieve](analytic-number-theory.md#selberg-sieve)
        - [Selberg upper-bound sieve](analytic-number-theory.md#selberg-upper-bound-sieve)
          - [Uniform interval bound from optimal Selberg weights](analytic-number-theory.md#uniform-interval-bound-from-optimal-selberg-weights)
          - [Half-dimensional interval sieve](analytic-number-theory.md#half-dimensional-interval-sieve)
          - [Selberg sieve weights](analytic-number-theory.md#selberg-sieve-weights)
            - [Selberg sieve denominator asymptotic](analytic-number-theory.md#selberg-sieve-denominator-asymptotic)
            - [Selberg sieve diagonalization](analytic-number-theory.md#selberg-sieve-diagonalization)
              - [Selberg least-common-multiple weights](analytic-number-theory.md#selberg-least-common-multiple-weights)
              - [Optimal Selberg weights have modulus at most one](analytic-number-theory.md#optimal-selberg-weights-have-modulus-at-most-one)
          - [Polynomial root density in a sieve](analytic-number-theory.md#polynomial-root-density-in-a-sieve)
            - [Elementary lower bound for the twin-prime sieve denominator](analytic-number-theory.md#elementary-lower-bound-for-the-twin-prime-sieve-denominator)
            - [Twin-prime upper bound from a quadratic sieve](analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve)
            - [Prime-tuple upper bound from the Selberg sieve](analytic-number-theory.md#prime-tuple-upper-bound-from-the-selberg-sieve)
          - [Almost-primes from an upper-bound sieve and Buchstab identity](analytic-number-theory.md#almost-primes-from-an-upper-bound-sieve-and-buchstab-identity)
          - [Fourier representation of a smooth Selberg weight](analytic-number-theory.md#fourier-representation-of-a-smooth-selberg-weight)
            - [Smooth divisor-square sieve asymptotic](analytic-number-theory.md#smooth-divisor-square-sieve-asymptotic)
              - [Euler product for a smoothed divisor-square correlation](analytic-number-theory.md#euler-product-for-a-smoothed-divisor-square-correlation)
              - [Derivative energy constant for a smooth sieve cutoff](analytic-number-theory.md#derivative-energy-constant-for-a-smooth-sieve-cutoff)
            - [Short-interval prime upper bound from a smooth divisor weight](analytic-number-theory.md#short-interval-prime-upper-bound-from-a-smooth-divisor-weight)
      - [Dimension-three upper-bound sieve](analytic-number-theory.md#dimension-three-upper-bound-sieve)
  - [Mertens' theorems](analytic-number-theory.md#mertens-theorems)
    - [Mertens first theorem](analytic-number-theory.md#mertens-first-theorem)
      - [Square-root logarithmic sum over primes](analytic-number-theory.md#square-root-logarithmic-sum-over-primes)
      - [Positive logarithmic moments of reciprocal primes](analytic-number-theory.md#positive-logarithmic-moments-of-reciprocal-primes)
      - [Factorial proof of Mertens first theorem](analytic-number-theory.md#factorial-proof-of-mertens-first-theorem)
      - [Logarithmically weighted reciprocal-prime tail](analytic-number-theory.md#logarithmically-weighted-reciprocal-prime-tail)
    - [Mertens second theorem](analytic-number-theory.md#mertens-second-theorem)
      - [Reciprocal-prime sum in residue class one modulo four](analytic-number-theory.md#reciprocal-prime-sum-in-residue-class-one-modulo-four)
    - [Mertens third theorem](analytic-number-theory.md#mertens-third-theorem)
      - [Totient lower bound from the Mertens product](analytic-number-theory.md#totient-lower-bound-from-the-mertens-product)
  - [Dirichlet series](analytic-number-theory.md#dirichlet-series)
    - [Holomorphy of a Dirichlet series from bounded partial sums](analytic-number-theory.md#holomorphy-of-a-dirichlet-series-from-bounded-partial-sums)
    - [Epstein zeta function](analytic-number-theory.md#epstein-zeta-function)
      - [Completed Epstein zeta function](analytic-number-theory.md#completed-epstein-zeta-function)
        - [Pole-subtracted theta integral for an Epstein zeta function](analytic-number-theory.md#pole-subtracted-theta-integral-for-an-epstein-zeta-function)
    - [Dirichlet polynomial](analytic-number-theory.md#dirichlet-polynomial)
      - [Mean value of Dirichlet polynomials](analytic-number-theory.md#mean-value-of-dirichlet-polynomials)
        - [Odd moment of a prime cosine sum](analytic-number-theory.md#odd-moment-of-a-prime-cosine-sum)
    - [Euler product](analytic-number-theory.md#euler-product)
      - [Euler product positivity for L-function nonvanishing](analytic-number-theory.md#euler-product-positivity-for-l-function-nonvanishing)
      - [Truncated Euler-product lower bound](analytic-number-theory.md#truncated-euler-product-lower-bound)
      - [Euler proof that the sum of reciprocals of primes diverges](analytic-number-theory.md#euler-proof-that-the-sum-of-reciprocals-of-primes-diverges)
        - [Prime reciprocal lower bound](analytic-number-theory.md#prime-reciprocal-lower-bound)
      - [Three-four-one inequality for Euler products](analytic-number-theory.md#three-four-one-inequality-for-euler-products)
    - [Perron's formula](analytic-number-theory.md#perron-s-formula)
      - [Logarithmically smoothed Perron formula](analytic-number-theory.md#logarithmically-smoothed-perron-formula)
        - [Unsmoothing a logarithmically weighted sum](analytic-number-theory.md#unsmoothing-a-logarithmically-weighted-sum)
      - [Truncated Perron formula](analytic-number-theory.md#truncated-perron-formula)
        - [Short-interval Perron bound for the second Chebyshev function](analytic-number-theory.md#short-interval-perron-bound-for-the-second-chebyshev-function)
        - [Truncated Perron kernel estimate](analytic-number-theory.md#truncated-perron-kernel-estimate)
  - [Riemann zeta function](analytic-number-theory.md#riemann-zeta-function)
    - [Reciprocal Dirichlet-series bound on boundary-zero multiplicity](analytic-number-theory.md#reciprocal-dirichlet-series-bound-on-boundary-zero-multiplicity)
    - [Reciprocal zeta bounds near the line one](analytic-number-theory.md#reciprocal-zeta-bounds-near-the-line-one)
    - [Three-four-one product proof of zeta boundary nonvanishing](analytic-number-theory.md#three-four-one-product-proof-of-zeta-boundary-nonvanishing)
    - [Lindelöf hypothesis](analytic-number-theory.md#lindelof-hypothesis)
    - [Truncated Möbius inverse identity for the Riemann zeta function](analytic-number-theory.md#truncated-mobius-inverse-identity-for-the-riemann-zeta-function)
    - [Richert bound for the Riemann zeta function](analytic-number-theory.md#richert-bound-for-the-riemann-zeta-function)
    - [Hardy-Littlewood approximation to the Riemann zeta function](analytic-number-theory.md#hardy-littlewood-approximation-to-the-riemann-zeta-function)
    - [Fractional-part continuation formula for the Riemann zeta function](analytic-number-theory.md#fractional-part-continuation-formula-for-the-riemann-zeta-function)
    - [Completed Riemann zeta function](analytic-number-theory.md#completed-riemann-zeta-function)
      - [Riemann xi function](analytic-number-theory.md#riemann-xi-function)
        - [Order-one growth of the Riemann xi function](analytic-number-theory.md#order-one-growth-of-the-riemann-xi-function)
        - [Real logarithmic derivative of Riemann xi](analytic-number-theory.md#real-logarithmic-derivative-of-riemann-xi)
          - [Absolute convergence of the real xi logarithmic derivative](analytic-number-theory.md#absolute-convergence-of-the-real-xi-logarithmic-derivative)
    - [Trivial zero of the Riemann zeta function](analytic-number-theory.md#trivial-zero-of-the-riemann-zeta-function)
    - [Fourth moment of the Riemann zeta function](analytic-number-theory.md#fourth-moment-of-the-riemann-zeta-function)
    - [Bernoulli formula for zeta values at nonpositive integers](analytic-number-theory.md#bernoulli-formula-for-zeta-values-at-nonpositive-integers)
    - [Meromorphic continuation of the Riemann zeta function to the right half-plane](analytic-number-theory.md#meromorphic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane)
    - [Basel problem](analytic-number-theory.md#basel-problem)
    - [Functional equation of the Riemann zeta function](analytic-number-theory.md#functional-equation-of-the-riemann-zeta-function)
      - [Mellin representation of the completed Riemann zeta function](analytic-number-theory.md#mellin-representation-of-the-completed-riemann-zeta-function)
        - [Pole-subtracted theta integral for the completed zeta function](analytic-number-theory.md#pole-subtracted-theta-integral-for-the-completed-zeta-function)
      - [Vertical-strip factor in the Riemann zeta functional equation](analytic-number-theory.md#vertical-strip-factor-in-the-riemann-zeta-functional-equation)
    - [Euler-product nonvanishing of the Riemann zeta function](analytic-number-theory.md#euler-product-nonvanishing-of-the-riemann-zeta-function)
    - [Nontrivial zero of the Riemann zeta function](analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function)
      - [Critical strip](analytic-number-theory.md#critical-strip)
        - [Critical line](analytic-number-theory.md#critical-line)
      - [Riemann hypothesis](analytic-number-theory.md#riemann-hypothesis)
        - [Riemann hypothesis implies the Lindelöf hypothesis](analytic-number-theory.md#riemann-hypothesis-implies-the-lindelof-hypothesis)
        - [Subpower zeta bound to the right of the critical line](analytic-number-theory.md#subpower-zeta-bound-to-the-right-of-the-critical-line)
        - [Xi modulus criterion for the Riemann hypothesis](analytic-number-theory.md#xi-modulus-criterion-for-the-riemann-hypothesis)
        - [Riemann hypothesis equivalence for the second Chebyshev function](analytic-number-theory.md#riemann-hypothesis-equivalence-for-the-second-chebyshev-function)
      - [Zero-free region of the Riemann zeta function](analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function)
        - [Vinogradov-Korobov zero-free region](analytic-number-theory.md#vinogradov-korobov-zero-free-region)
        - [Landau zero-free-region theorem](analytic-number-theory.md#landau-zero-free-region-theorem)
        - [Weak logarithmic zero-free region for the Riemann zeta function](analytic-number-theory.md#weak-logarithmic-zero-free-region-for-the-riemann-zeta-function)
        - [Three-four-one zero-free-region argument](analytic-number-theory.md#three-four-one-zero-free-region-argument)
        - [Logarithmic derivative inside the zeta zero-free region](analytic-number-theory.md#logarithmic-derivative-inside-the-zeta-zero-free-region)
      - [Riemann–von Mangoldt formula](analytic-number-theory.md#riemann-von-mangoldt-formula)
        - [Infinitely many reciprocal-logarithmic gaps between zeta zeros](analytic-number-theory.md#infinitely-many-reciprocal-logarithmic-gaps-between-zeta-zeros)
        - [Asymptotic inversion of the zeta zero count](analytic-number-theory.md#asymptotic-inversion-of-the-zeta-zero-count)
        - [Local zero count for the Riemann zeta function](analytic-number-theory.md#local-zero-count-for-the-riemann-zeta-function)
          - [Jensen disk proof of the zeta zero-count bound](analytic-number-theory.md#jensen-disk-proof-of-the-zeta-zero-count-bound)
          - [Smoothed zeta zero-count bound](analytic-number-theory.md#smoothed-zeta-zero-count-bound)
    - [Logarithmic derivative](analytic-number-theory.md#logarithmic-derivative)
      - [Global partial-fraction expansion of the zeta logarithmic derivative](analytic-number-theory.md#global-partial-fraction-expansion-of-the-zeta-logarithmic-derivative)
      - [Local logarithmic-derivative lemma](analytic-number-theory.md#local-logarithmic-derivative-lemma)
      - [Local partial-fraction expansion of the Riemann zeta logarithmic derivative](analytic-number-theory.md#local-partial-fraction-expansion-of-the-riemann-zeta-logarithmic-derivative)
      - [Prime number theorem](analytic-number-theory.md#prime-number-theorem)
        - [Prime number theorem error from a fixed zero-free strip](analytic-number-theory.md#prime-number-theorem-error-from-a-fixed-zero-free-strip)
        - [Prime number theorem error from a logarithmic zero-free region](analytic-number-theory.md#prime-number-theorem-error-from-a-logarithmic-zero-free-region)
        - [Prime number theorem with classical zero-free-region error](analytic-number-theory.md#prime-number-theorem-with-classical-zero-free-region-error)
        - [Smoothed prime number theorem from a zero-free region](analytic-number-theory.md#smoothed-prime-number-theorem-from-a-zero-free-region)
      - [Twisted Von Mangoldt estimate implying the Riemann hypothesis](analytic-number-theory.md#twisted-von-mangoldt-estimate-implying-the-riemann-hypothesis)
    - [Dirichlet eta function](analytic-number-theory.md#dirichlet-eta-function)
      - [Analytic continuation of the Riemann zeta function to the right half-plane](analytic-number-theory.md#analytic-continuation-of-the-riemann-zeta-function-to-the-right-half-plane)
- [Exponentiation by squaring](#exponentiation-by-squaring)
  - [Binary powering multiplication count](#binary-powering-multiplication-count)
  - [Modular exponentiation](#modular-exponentiation)
    - [Bit cost of modular exponentiation](#bit-cost-of-modular-exponentiation)
- [Integer](#integer)
  - [Repdigit](#repdigit)
  - [Euclidean division](#euclidean-division)
    - [Remainder](#remainder)
    - [Long division](#long-division)
  - [Integer interval](#integer-interval)
  - [Positional notation](#positional-notation)
    - [Decimal expansion](#decimal-expansion)
    - [Hereditary base representation](#hereditary-base-representation)
      - [Goodstein sequence](#goodstein-sequence)
        - [Goodstein's theorem](#goodstein-s-theorem)
        - [Ordinal rank of a Goodstein term](#ordinal-rank-of-a-goodstein-term)
        - [Goodstein function](#goodstein-function)
    - [Base-p expansion](#base-p-expansion)
    - [Binary numeral system](#binary-numeral-system)
      - [Binary digit](#binary-digit)
    - [Decimal](#decimal)
      - [Decimal representation](#decimal-representation)
        - [Terminating decimal](#terminating-decimal)
  - [Positive integer](#positive-integer)
    - [Power of two](#power-of-two)
    - [Perfect number](#perfect-number)
    - [Deficient number](#deficient-number)
    - [Abundant number](#abundant-number)
  - [Parity (mathematics)](#parity-mathematics)
    - [Odd integer](#odd-integer)
    - [Even number](#even-number)
    - [Odd number](#odd-number)
  - [Square-free integer](#square-free-integer)
  - [Powerful number](#powerful-number)
  - [Square number](#square-number)
- [Divisibility](#divisibility)
  - [Integer multiple](#integer-multiple)
  - [Divisor](#divisor)
    - [Proper divisor](#proper-divisor)
    - [Squarefree divisor](#squarefree-divisor)
  - [Greatest common divisor](#greatest-common-divisor)
    - [Scaling identity for greatest common divisors](#scaling-identity-for-greatest-common-divisors)
    - [Coprime integers](#coprime-integers)
      - [Pairwise coprimality](#pairwise-coprimality)
      - [Joint coprimality](#joint-coprimality)
  - [Least common multiple](#least-common-multiple)
- [Modular arithmetic](#modular-arithmetic)
  - [Modulus in modular arithmetic](#modulus-in-modular-arithmetic)
  - [Least nonnegative residue](#least-nonnegative-residue)
  - [Integer congruence](#integer-congruence)
  - [Wilson's theorem](#wilson-s-theorem)
    - [Wilson factorial congruence modulo a triangular number](#wilson-factorial-congruence-modulo-a-triangular-number)
    - [Odd-residue squared product modulo a prime](#odd-residue-squared-product-modulo-a-prime)
    - [Complementary factorial congruence](#complementary-factorial-congruence)
  - [Congruence class](#congruence-class)
  - [Modular congruence](#modular-congruence)
    - [Prime-power contraction under pth powers](#prime-power-contraction-under-pth-powers)
    - [Reduced residue system](#reduced-residue-system)
    - [Linear congruence](#linear-congruence)
    - [Residue class](#residue-class)
    - [Unit modulo n](#unit-modulo-n)
- [Prime number](#prime-number)
  - [Primality](#primality)
  - [Trial division](#trial-division)
  - [Sieve of Eratosthenes](#sieve-of-eratosthenes)
  - [Infinitely many primes congruent to one modulo six](#infinitely-many-primes-congruent-to-one-modulo-six)
  - [Infinitely many primes congruent to minus one modulo six](#infinitely-many-primes-congruent-to-minus-one-modulo-six)
  - [Bertrand's postulate](#bertrand-s-postulate)
  - [Twin prime](#twin-prime)
    - [Twin prime conjecture](#twin-prime-conjecture)
      - [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture)
      - [Twin-prime constant](#twin-prime-constant)
    - [Brun's theorem](#brun-s-theorem)
    - [Twin-prime upper bound using Bombieri–Vinogradov](#twin-prime-upper-bound-using-bombieri-vinogradov)
  - [Euclid's theorem](#euclid-s-theorem)
  - [Odd prime](#odd-prime)
  - [Fermat prime](#fermat-prime)
    - [Pépin's test](#pepin-s-test)
    - [Quadratic nonresidues modulo a Fermat prime](#quadratic-nonresidues-modulo-a-fermat-prime)
  - [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)
    - [Factorization tree](#factorization-tree)
  - [Prime factor](#prime-factor)
  - [Prime power](#prime-power)
- [Composite number](#composite-number)
  - [Semiprime](#semiprime)
- [Euler's theorem](#euler-s-theorem)
  - [Multiplication by a unit permutes reduced residues](#multiplication-by-a-unit-permutes-reduced-residues)
  - [Exponent reduction for units](#exponent-reduction-for-units)
  - [Generalized repunit pseudoprime construction](#generalized-repunit-pseudoprime-construction)
- [Fermat pseudoprime](#fermat-pseudoprime)
  - [Strong pseudoprime](#strong-pseudoprime)
    - [Strong-pseudoprime bases for a product of two primes with common predecessor divisor ten](#strong-pseudoprime-bases-for-a-product-of-two-primes-with-common-predecessor-divisor-ten)
- [Euler pseudoprime](#euler-pseudoprime)
  - [Euler witness](#euler-witness)
    - [Euler witnesses occupy at least half the unit bases](#euler-witnesses-occupy-at-least-half-the-unit-bases)
    - [Existence of an Euler witness for every odd composite integer](#existence-of-an-euler-witness-for-every-odd-composite-integer)
    - [Solovay-Strassen primality test](#solovay-strassen-primality-test)
- [P-adic valuation](#p-adic-valuation)
  - [p-adic integer](#p-adic-integer)
    - [Open subgroups of the p-adic integers](#open-subgroups-of-the-p-adic-integers)
    - [7-adic integer](#7-adic-integer)
    - [2-adic integer](#2-adic-integer)
    - [Topological generator of the additive group of p-adic integers](#topological-generator-of-the-additive-group-of-p-adic-integers)
  - [2-adic valuation](#2-adic-valuation)
  - [Legendre's formula](#legendre-s-formula)
  - [Base-p digit sum](#base-p-digit-sum)
    - [Subadditivity of the base-p digit sum](#subadditivity-of-the-base-p-digit-sum)
  - [Valuation of a near-central binomial coefficient](#valuation-of-a-near-central-binomial-coefficient)
- [Primorial](#primorial)
  - [Chebyshev theta function](#chebyshev-theta-function)
    - [Elementary lower bound for the Chebyshev theta function](#elementary-lower-bound-for-the-chebyshev-theta-function)
  - [Elementary primorial bound](#elementary-primorial-bound)
- [Decisive number](#decisive-number)
- [Prime-counting function](#prime-counting-function)
  - [Legendre prime-counting formula](#legendre-prime-counting-formula)
  - [Prime-counting upper bound from a primorial estimate](#prime-counting-upper-bound-from-a-primorial-estimate)
- [Primitive root modulo n](#primitive-root-modulo-n)
  - [Lifting a primitive root to odd prime powers](#lifting-a-primitive-root-to-odd-prime-powers)
  - [Primitive-root modulus classification](#primitive-root-modulus-classification)
- [Quadratic residue](#quadratic-residue)
  - [Square root of minus one modulo a prime](#square-root-of-minus-one-modulo-a-prime)
  - [Quadratic nonresidue](#quadratic-nonresidue)
    - [Least quadratic nonresidue](#least-quadratic-nonresidue)
      - [Large-sieve logarithmic exceptional-prime bound for least quadratic nonresidues](#large-sieve-logarithmic-exceptional-prime-bound-for-least-quadratic-nonresidues)
      - [Bounded exceptional primes for least quadratic nonresidues](#bounded-exceptional-primes-for-least-quadratic-nonresidues)
  - [Quadratic Gauss sum](#quadratic-gauss-sum)
    - [Quadratic periods modulo eleven](#quadratic-periods-modulo-eleven)
  - [Legendre symbol](#legendre-symbol)
    - [Multiplicativity of the Legendre symbol](#multiplicativity-of-the-legendre-symbol)
    - [Complete Legendre-symbol sum](#complete-legendre-symbol-sum)
    - [Quadratic Legendre-symbol correlation](#quadratic-legendre-symbol-correlation)
      - [Number of consecutive nonzero quadratic residues modulo an odd prime](#number-of-consecutive-nonzero-quadratic-residues-modulo-an-odd-prime)
    - [Euler's criterion](#euler-s-criterion)
      - [Primes congruent to five modulo eight from odd squares plus four](#primes-congruent-to-five-modulo-eight-from-odd-squares-plus-four)
    - [Gauss's lemma (number theory)](#gauss-s-lemma-number-theory)
    - [Euler criterion](#euler-criterion)
      - [First supplementary law for quadratic reciprocity](#first-supplementary-law-for-quadratic-reciprocity)
      - [Second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity)
        - [Euclid proof for infinitely many primes congruent to seven modulo eight](#euclid-proof-for-infinitely-many-primes-congruent-to-seven-modulo-eight)
        - [Elementary logarithmic lower bound for primes in the quadratic-residue classes of two](#elementary-logarithmic-lower-bound-for-primes-in-the-quadratic-residue-classes-of-two)
      - [Prime-power binomial congruence for a matrix](#prime-power-binomial-congruence-for-a-matrix)
    - [Weighted complete Legendre-symbol sum](#weighted-complete-legendre-symbol-sum)
    - [Lower-half quadratic-residue sum for primes congruent to seven modulo eight](#lower-half-quadratic-residue-sum-for-primes-congruent-to-seven-modulo-eight)
    - [Discriminant criterion for a quadratic congruence modulo an odd prime](#discriminant-criterion-for-a-quadratic-congruence-modulo-an-odd-prime)
- [Primitive-root lifting criterion](#primitive-root-lifting-criterion)
- [Jacobi symbol](#jacobi-symbol)
  - [Jacobi reciprocity law](#jacobi-reciprocity-law)
    - [Infinitely many prime quadratic nonresidues of a nonsquare integer](#infinitely-many-prime-quadratic-nonresidues-of-a-nonsquare-integer)
  - [Multiplicativity of the Jacobi symbol](#multiplicativity-of-the-jacobi-symbol)
- [Quadratic reciprocity](#quadratic-reciprocity)
  - [Computing Legendre symbols by quadratic reciprocity](#computing-legendre-symbols-by-quadratic-reciprocity)
  - [Lattice-point count for quadratic reciprocity](#lattice-point-count-for-quadratic-reciprocity)
  - [Quadratic character of minus three](#quadratic-character-of-minus-three)
    - [Cube roots of minus one modulo an odd prime](#cube-roots-of-minus-one-modulo-an-odd-prime)
- [Carmichael number](#carmichael-number)
  - [Korselt criterion](#korselt-criterion)
    - [Proof of Korselt criterion](#proof-of-korselt-criterion)
- [Perfect power](#perfect-power)
- [Smooth number](#smooth-number)
  - [Positive density of power-smooth integers](#positive-density-of-power-smooth-integers)
  - [B-smooth integer](#b-smooth-integer)
  - [S-smooth number](#s-smooth-number)
    - [Squarefree-part bound for smooth numbers](#squarefree-part-bound-for-smooth-numbers)
  - [Largest prime factor](#largest-prime-factor)
- [Diophantine equation](#diophantine-equation)
  - [Schinzel-Tijdeman exponent theorem](#schinzel-tijdeman-exponent-theorem)
  - [Local solubility](#local-solubility)
  - [Fermat last theorem](#fermat-last-theorem)
  - [abc conjecture](#abc-conjecture)
    - [Catalan power bound from abc](#catalan-power-bound-from-abc)
    - [Primitive Fermat bound from abc](#primitive-fermat-bound-from-abc)
  - [Thue theorem](#thue-theorem)
  - [Unit equation over a number field](#unit-equation-over-a-number-field)
  - [Infinite descent](#infinite-descent)
    - [Fourth-power sum cannot be a square](#fourth-power-sum-cannot-be-a-square)
- [Diophantine approximation](#diophantine-approximation)
  - [Transcendence theory](#transcendence-theory)
    - [Schneider-Lang theorem](#schneider-lang-theorem)
    - [Symmetric Hermite integral obstruction](#symmetric-hermite-integral-obstruction)
    - [Gelfond–Schneider theorem](#gelfond-schneider-theorem)
      - [Schneider lattice proof of the Gelfond–Schneider theorem](#schneider-lattice-proof-of-the-gelfond-schneider-theorem)
    - [Mahler method](#mahler-method)
      - [Fredholm lacunary series](#fredholm-lacunary-series)
        - [Roth criterion for rational Fredholm values](#roth-criterion-for-rational-fredholm-values)
        - [Auxiliary-value height argument for the Fredholm series](#auxiliary-value-height-argument-for-the-fredholm-series)
    - [E-function](#e-function)
      - [Addition closure of Siegel E-functions](#addition-closure-of-siegel-e-functions)
      - [Siegel–Shidlovsky theorem](#siegel-shidlovsky-theorem)
    - [Lindemann–Weierstrass theorem](#lindemann-weierstrass-theorem)
      - [Hermite auxiliary-polynomial proof for pi](#hermite-auxiliary-polynomial-proof-for-pi)
  - [Badly approximable number](#badly-approximable-number)
    - [Diophantine bound for the square root of two](#diophantine-bound-for-the-square-root-of-two)
  - [Diophantine frequency vector](#diophantine-frequency-vector)
    - [Small divisor](#small-divisor)
  - [Quantitative quadratic recurrence](#quantitative-quadratic-recurrence)
  - [Distance to the nearest integer](#distance-to-the-nearest-integer)
    - [Separated reciprocal-distance sum](#separated-reciprocal-distance-sum)
  - [Dirichlet's approximation theorem](#dirichlet-s-approximation-theorem)
  - [Best rational approximation](#best-rational-approximation)
  - [Schmidt subspace theorem](#schmidt-subspace-theorem)
    - [Roth's theorem](#roth-s-theorem)
    - [Ridout theorem](#ridout-theorem)
  - [Linear form in logarithms of algebraic numbers](#linear-form-in-logarithms-of-algebraic-numbers)
    - [Baker's theorem](#baker-s-theorem)
    - [General lower bound for a linear form in logarithms](#general-lower-bound-for-a-linear-form-in-logarithms)
    - [Baker lower bound for a homogeneous linear form in logarithms](#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms)
      - [Exponent bound for a binomial power equation](#exponent-bound-for-a-binomial-power-equation)
      - [Effective norm-form height estimate](#effective-norm-form-height-estimate)
  - [Siegel's lemma](#siegel-s-lemma)
    - [Pigeonhole proof of integer Siegel lemma](#pigeonhole-proof-of-integer-siegel-lemma)
    - [Normalized derivative of a polynomial](#normalized-derivative-of-a-polynomial)
    - [Thue-Siegel auxiliary polynomial](#thue-siegel-auxiliary-polynomial)
      - [Rational multiplicity bound for a linear auxiliary polynomial](#rational-multiplicity-bound-for-a-linear-auxiliary-polynomial)
      - [Thue-Siegel rational approximation bound](#thue-siegel-rational-approximation-bound)
  - [Pell equation](#pell-equation)
    - [Unit reduction for quadratic norm equations](#unit-reduction-for-quadratic-norm-equations)
    - [Generalized Pell equation](#generalized-pell-equation)
  - [Continued fraction](#continued-fraction)
    - [Continued fraction of the square root of nineteen](#continued-fraction-of-the-square-root-of-nineteen)
    - [Negative continued fraction](#negative-continued-fraction)
    - [Simple continued fraction](#simple-continued-fraction)
    - [Gauss continued-fraction map](#gauss-continued-fraction-map)
      - [Natural extension of the continued-fraction Gauss map](#natural-extension-of-the-continued-fraction-gauss-map)
      - [Bounded distortion of continued-fraction cylinders](#bounded-distortion-of-continued-fraction-cylinders)
      - [Gauss measure](#gauss-measure)
    - [Complete quotient](#complete-quotient)
    - [Continued-fraction algorithm](#continued-fraction-algorithm)
      - [Termination criterion for a simple continued fraction](#termination-criterion-for-a-simple-continued-fraction)
    - [Continued fraction convergent](#continued-fraction-convergent)
      - [Small norm residues from square-root continued fractions](#small-norm-residues-from-square-root-continued-fractions)
      - [Best approximation of the second kind](#best-approximation-of-the-second-kind)
      - [Continued-fraction matrix](#continued-fraction-matrix)
        - [Continued-fraction tail formula](#continued-fraction-tail-formula)
        - [Reversal identity for a finite continued fraction](#reversal-identity-for-a-finite-continued-fraction)
    - [Positive generalized continued fraction](#positive-generalized-continued-fraction)
      - [Convergence of a positive simple continued fraction](#convergence-of-a-positive-simple-continued-fraction)
        - [All-one continued fraction and Fibonacci ratios](#all-one-continued-fraction-and-fibonacci-ratios)
    - [Lagrange theorem on continued fractions](#lagrange-theorem-on-continued-fractions)
    - [Periodic continued fraction of a quadratic irrational](#periodic-continued-fraction-of-a-quadratic-irrational)
      - [Purely periodic continued fraction](#purely-periodic-continued-fraction)
        - [Reversed-period identity for a purely periodic continued fraction](#reversed-period-identity-for-a-purely-periodic-continued-fraction)
      - [Continued fraction of the square root of three](#continued-fraction-of-the-square-root-of-three)
      - [Continued fraction of the square root of eleven](#continued-fraction-of-the-square-root-of-eleven)
        - [Alternating multiplier recurrence for convergents of the square root of eleven](#alternating-multiplier-recurrence-for-convergents-of-the-square-root-of-eleven)
        - [Pell-type norm from a periodic continued fraction](#pell-type-norm-from-a-periodic-continued-fraction)
  - [Liouville approximation theorem](#liouville-approximation-theorem)
    - [Unbounded continued-fraction coefficients exclude quadratic irrationality](#unbounded-continued-fraction-coefficients-exclude-quadratic-irrationality)
    - [Proof of Liouville approximation theorem](#proof-of-liouville-approximation-theorem)
    - [Separation of distinct reduced fractions](#separation-of-distinct-reduced-fractions)
    - [Transcendental subseries of a positive rational convergent series](#transcendental-subseries-of-a-positive-rational-convergent-series)
- [Binary quadratic form](#binary-quadratic-form)
  - [Primes represented by x squared plus three y squared](#primes-represented-by-x-squared-plus-three-y-squared)
  - [Prime representation via an ideal class](#prime-representation-via-an-ideal-class)
  - [Discriminant criterion for prime representation by a binary quadratic form](#discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form)
  - [Proper equivalence of binary quadratic forms](#proper-equivalence-of-binary-quadratic-forms)
  - [Primitive binary quadratic form](#primitive-binary-quadratic-form)
  - [Discriminant of a binary quadratic form](#discriminant-of-a-binary-quadratic-form)
  - [Reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form)
    - [Reduction algorithm for a positive definite binary quadratic form](#reduction-algorithm-for-a-positive-definite-binary-quadratic-form)
    - [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)
      - [Reduced positive definite binary quadratic forms of discriminant minus thirty-nine](#reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-nine)
      - [Reduced forms of discriminant minus thirty-two](#reduced-forms-of-discriminant-minus-thirty-two)
      - [Class number one for discriminant minus sixty-seven](#class-number-one-for-discriminant-minus-sixty-seven)
      - [Reduced forms of discriminant minus forty-four](#reduced-forms-of-discriminant-minus-forty-four)
      - [Reduced positive definite binary quadratic forms of discriminant minus thirty-five](#reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-five)
        - [Primitive representation criterion at discriminant minus thirty-five](#primitive-representation-criterion-at-discriminant-minus-thirty-five)
    - [Class number problem](#class-number-problem)
      - [Class number of a negative discriminant](#class-number-of-a-negative-discriminant)
        - [Two distinguished classes of discriminant minus eight q](#two-distinguished-classes-of-discriminant-minus-eight-q)
          - [Prime representation when h of minus eight q equals two](#prime-representation-when-h-of-minus-eight-q-equals-two)
        - [Coprime-factorization lower bound for a quadratic-form class number](#coprime-factorization-lower-bound-for-a-quadratic-form-class-number)
  - [Unimodular reduction of a discriminant-minus-four form to two squares](#unimodular-reduction-of-a-discriminant-minus-four-form-to-two-squares)
- [Euclid's lemma](#euclid-s-lemma)
- [Prime valuation](#prime-valuation)
- [Euler totient function](#euler-totient-function)
  - [Totient divisor-sum identity](#totient-divisor-sum-identity)
  - [Sum of reduced residues](#sum-of-reduced-residues)
  - [Integers whose totient divides them](#integers-whose-totient-divides-them)
  - [Totient divisibility along divisors](#totient-divisibility-along-divisors)
  - [Rosser–Schoenfeld totient bound](#rosser-schoenfeld-totient-bound)
  - [Elementary totient-ratio lower bound](#elementary-totient-ratio-lower-bound)
  - [Euler theorem](#euler-theorem)
  - [Multiplicativity of the Euler totient function](#multiplicativity-of-the-euler-totient-function)
  - [Finite fibres of the Euler totient function](#finite-fibres-of-the-euler-totient-function)
- [Jordan's totient function](#jordan-s-totient-function)
- [Fermat little theorem](#fermat-little-theorem)
- [Squarefree integer](#squarefree-integer)
- [Square factor](#square-factor)
- [Difference of two squares](#difference-of-two-squares)
  - [Fermat's factorization method](#fermat-s-factorization-method)
- [Rational number](#rational-number)
  - [Fraction](#fraction)
    - [Numerator](#numerator)
    - [Denominator](#denominator)
  - [Farey sequence](#farey-sequence)
    - [Farey fraction](#farey-fraction)
  - [Reduced fraction](#reduced-fraction)
  - [Density of the rational numbers](#density-of-the-rational-numbers)
  - [Repeating decimal](#repeating-decimal)
    - [Decimal preperiod](#decimal-preperiod)
  - [Eventually periodic positional expansion of a rational number](#eventually-periodic-positional-expansion-of-a-rational-number)
- [Modular multiplicative inverse](#modular-multiplicative-inverse)
- [Carmichael function](#carmichael-function)
- [Multiplicative order](#multiplicative-order)
  - [Decimal period from multiplicative order](#decimal-period-from-multiplicative-order)
  - [Cyclic decimal divisibility](#cyclic-decimal-divisibility)
  - [Periodic modular exponentiation](#periodic-modular-exponentiation)
    - [Order as the exact period of modular exponentiation](#order-as-the-exact-period-of-modular-exponentiation)
  - [Order verification from divisors](#order-verification-from-divisors)
- [Euclidean algorithm](#euclidean-algorithm)
  - [Extended Euclidean algorithm](#extended-euclidean-algorithm)
  - [Linear Diophantine equation](#linear-diophantine-equation)
    - [All solutions of a linear Diophantine equation](#all-solutions-of-a-linear-diophantine-equation)
    - [Linear Diophantine equation solvability criterion](#linear-diophantine-equation-solvability-criterion)
- [Sum of two squares theorem](#sum-of-two-squares-theorem)
  - [Congruence lattice proof of the prime sum of two squares](#congruence-lattice-proof-of-the-prime-sum-of-two-squares)
- [Modular function](modular-function.md)
  - [Modular lambda function](modular-function.md#modular-lambda-function)
    - [Universal covering by the modular lambda function](modular-function.md#universal-covering-by-the-modular-lambda-function)
  - [Modular curve](modular-function.md#modular-curve)
    - [Elliptic point of a modular curve](modular-function.md#elliptic-point-of-a-modular-curve)
    - [Modular symbol](modular-function.md#modular-symbol)
      - [Manin symbol](modular-function.md#manin-symbol)
    - [X0 2 modular curve](modular-function.md#x0-2-modular-curve)
      - [Discriminant-ratio coordinate on X0 2](modular-function.md#discriminant-ratio-coordinate-on-x0-2)
    - [Compactified modular curve](modular-function.md#compactified-modular-curve)
    - [Level-two modular curve](modular-function.md#level-two-modular-curve)
    - [Genus formula for a modular curve](modular-function.md#genus-formula-for-a-modular-curve)
      - [Principal congruence modular curve genus](modular-function.md#principal-congruence-modular-curve-genus)
        - [Elliptic and cusp ramification for principal level](modular-function.md#elliptic-and-cusp-ramification-for-principal-level)
      - [Modular curve X0 3](modular-function.md#modular-curve-x0-3)
  - [Cusp of a modular group](modular-function.md#cusp-of-a-modular-group)
    - [Width of a cusp](modular-function.md#width-of-a-cusp)
    - [Holomorphic at a cusp](modular-function.md#holomorphic-at-a-cusp)
      - [Cusp holomorphy under rational slash operators](modular-function.md#cusp-holomorphy-under-rational-slash-operators)
  - [Modular form](modular-function.md#modular-form)
    - [Weight of a modular form](modular-function.md#weight-of-a-modular-form)
    - [Mellin continuation of a noncuspidal modular form](modular-function.md#mellin-continuation-of-a-noncuspidal-modular-form)
    - [Dimension of level-one modular forms](modular-function.md#dimension-of-level-one-modular-forms)
      - [Polynomial ring of level-one modular forms](modular-function.md#polynomial-ring-of-level-one-modular-forms)
        - [Graded weights separate analytic polynomial relations](modular-function.md#graded-weights-separate-analytic-polynomial-relations)
        - [Rational structure of level-one modular forms](modular-function.md#rational-structure-of-level-one-modular-forms)
    - [Modular forms as meromorphic differentials on X(1)](modular-function.md#modular-forms-as-meromorphic-differentials-on-x-1)
    - [Integral triangular basis of level-one modular forms](modular-function.md#integral-triangular-basis-of-level-one-modular-forms)
    - [Modular form on a finite-index subgroup](modular-function.md#modular-form-on-a-finite-index-subgroup)
      - [Nebentypus character](modular-function.md#nebentypus-character)
      - [Coset norm of a modular form](modular-function.md#coset-norm-of-a-modular-form)
    - [Serre derivative](modular-function.md#serre-derivative)
      - [First Rankin-Cohen bracket](modular-function.md#first-rankin-cohen-bracket)
    - [Oldform by argument dilation](modular-function.md#oldform-by-argument-dilation)
      - [Prime stabilization of an oldform](modular-function.md#prime-stabilization-of-an-oldform)
      - [Weight-four modular forms on Gamma 0 3](modular-function.md#weight-four-modular-forms-on-gamma-0-3)
    - [Weak modular form](modular-function.md#weak-modular-form)
      - [Derivative transformation of a weak modular form](modular-function.md#derivative-transformation-of-a-weak-modular-form)
        - [Bol identity for modular forms](modular-function.md#bol-identity-for-modular-forms)
    - [Fricke involution](modular-function.md#fricke-involution)
      - [Fricke sign from a nonvanishing fixed-point value](modular-function.md#fricke-sign-from-a-nonvanishing-fixed-point-value)
    - [Modular group](modular-function.md#modular-group)
      - [Modular-invariant function](modular-function.md#modular-invariant-function)
      - [Rational conjugation of finite-index modular subgroups](modular-function.md#rational-conjugation-of-finite-index-modular-subgroups)
      - [Standard fundamental domain of the modular group](modular-function.md#standard-fundamental-domain-of-the-modular-group)
        - [Fundamental region of a modular subgroup](modular-function.md#fundamental-region-of-a-modular-subgroup)
        - [Elliptic stabilizers of the modular group](modular-function.md#elliptic-stabilizers-of-the-modular-group)
        - [Reduction to the standard modular region](modular-function.md#reduction-to-the-standard-modular-region)
    - [Slash operator for modular forms](modular-function.md#slash-operator-for-modular-forms)
      - [Double-coset operator on modular forms](modular-function.md#double-coset-operator-on-modular-forms)
      - [Hecke-normalized rational slash operator](modular-function.md#hecke-normalized-rational-slash-operator)
      - [Determinant-normalized slash operator](modular-function.md#determinant-normalized-slash-operator)
      - [Automorphy factor](modular-function.md#automorphy-factor)
    - [Fourier expansion of a modular form](modular-function.md#fourier-expansion-of-a-modular-form)
      - [Cusp form](modular-function.md#cusp-form)
        - [Old subspace of cusp forms](modular-function.md#old-subspace-of-cusp-forms)
          - [Degeneracy map for cusp forms](modular-function.md#degeneracy-map-for-cusp-forms)
            - [Prime-level cusp orders of discriminant degeneracy forms](modular-function.md#prime-level-cusp-orders-of-discriminant-degeneracy-forms)
          - [Prime-power old block at a bad prime](modular-function.md#prime-power-old-block-at-a-bad-prime)
        - [New subspace of cusp forms](modular-function.md#new-subspace-of-cusp-forms)
          - [Newform](modular-function.md#newform)
            - [Bad-prime eigenvalue of a trivial-character newform](modular-function.md#bad-prime-eigenvalue-of-a-trivial-character-newform)
            - [Newform multiplicity-one theorem](modular-function.md#newform-multiplicity-one-theorem)
        - [L-function of a cusp form](modular-function.md#l-function-of-a-cusp-form)
          - [Additive twist of a cusp-form L-function](modular-function.md#additive-twist-of-a-cusp-form-l-function)
            - [Functional equation of an additive cusp-form twist](modular-function.md#functional-equation-of-an-additive-cusp-form-twist)
            - [Rational-cusp inversion of a level-one cusp form](modular-function.md#rational-cusp-inversion-of-a-level-one-cusp-form)
        - [Character twist by rational translations of a cusp form](modular-function.md#character-twist-by-rational-translations-of-a-cusp-form)
          - [Primitive twist at coprime level](modular-function.md#primitive-twist-at-coprime-level)
            - [Fricke transform of a primitive coprime twist](modular-function.md#fricke-transform-of-a-primitive-coprime-twist)
        - [Invariant norm of a modular form](modular-function.md#invariant-norm-of-a-modular-form)
          - [Bounded invariant norm characterization of cusp forms](modular-function.md#bounded-invariant-norm-characterization-of-cusp-forms)
          - [Fourier coefficient bound for a cusp form](modular-function.md#fourier-coefficient-bound-for-a-cusp-form)
        - [Fourier coefficient growth criterion for a level-one cusp form](modular-function.md#fourier-coefficient-growth-criterion-for-a-level-one-cusp-form)
        - [Dimension of level-one cusp forms](modular-function.md#dimension-of-level-one-cusp-forms)
        - [Mellin transform of a cusp-form L-function](modular-function.md#mellin-transform-of-a-cusp-form-l-function)
          - [Phase-normalized Fricke functional equation](modular-function.md#phase-normalized-fricke-functional-equation)
        - [Modular discriminant](modular-function.md#modular-discriminant)
          - [Multiplication by the modular discriminant](modular-function.md#multiplication-by-the-modular-discriminant)
          - [Weight-two discriminant root at level eleven](modular-function.md#weight-two-discriminant-root-at-level-eleven)
          - [Integrality identity for the modular discriminant](modular-function.md#integrality-identity-for-the-modular-discriminant)
          - [Ramanujan tau function](modular-function.md#ramanujan-tau-function)
            - [Ramanujan tau congruence modulo five](modular-function.md#ramanujan-tau-congruence-modulo-five)
            - [Ramanujan congruence modulo 691](modular-function.md#ramanujan-congruence-modulo-691)
          - [Mellin transform of the modular discriminant](modular-function.md#mellin-transform-of-the-modular-discriminant)
        - [Petersson inner product](modular-function.md#petersson-inner-product)
          - [Hecke operators are self-adjoint for the Petersson inner product](modular-function.md#hecke-operators-are-self-adjoint-for-the-petersson-inner-product)
          - [Rankin–Selberg method](modular-function.md#rankin-selberg-method)
            - [Rankin–Selberg integral for holomorphic cusp forms](modular-function.md#rankin-selberg-integral-for-holomorphic-cusp-forms)
              - [Positive unfolding of a cusp-form square](modular-function.md#positive-unfolding-of-a-cusp-form-square)
                - [Absolute convergence of cusp-form L-series from square coefficients](modular-function.md#absolute-convergence-of-cusp-form-l-series-from-square-coefficients)
            - [Rankin–Selberg convolution](modular-function.md#rankin-selberg-convolution)
              - [Euler factor of a coefficientwise product of Hecke eigenforms](modular-function.md#euler-factor-of-a-coefficientwise-product-of-hecke-eigenforms)
              - [Zeta-completed Rankin-Selberg coefficient series](modular-function.md#zeta-completed-rankin-selberg-coefficient-series)
              - [Rankin–Selberg unfolding identity for a holomorphic Eisenstein series](modular-function.md#rankin-selberg-unfolding-identity-for-a-holomorphic-eisenstein-series)
    - [Eisenstein series](modular-function.md#eisenstein-series)
      - [Lattice Eisenstein sum](modular-function.md#lattice-eisenstein-sum)
        - [A complex lattice is determined by its fourth and sixth Eisenstein sums](modular-function.md#a-complex-lattice-is-determined-by-its-fourth-and-sixth-eisenstein-sums)
      - [Weight-four Eisenstein basis at level two](modular-function.md#weight-four-eisenstein-basis-at-level-two)
      - [Character-twisted Eisenstein series](modular-function.md#character-twisted-eisenstein-series)
        - [Fourier expansion of a character-twisted Eisenstein series](modular-function.md#fourier-expansion-of-a-character-twisted-eisenstein-series)
      - [Fourier expansion of a normalized Eisenstein series](modular-function.md#fourier-expansion-of-a-normalized-eisenstein-series)
        - [Divisor-sum convolution identity of weights four and eight](modular-function.md#divisor-sum-convolution-identity-of-weights-four-and-eight)
      - [Integral echelon basis of level-one modular forms](modular-function.md#integral-echelon-basis-of-level-one-modular-forms)
        - [Eisenstein congruence from a denominator prime](modular-function.md#eisenstein-congruence-from-a-denominator-prime)
          - [Weight-sixteen Eisenstein congruence](modular-function.md#weight-sixteen-eisenstein-congruence)
      - [Congruence-class Eisenstein series](modular-function.md#congruence-class-eisenstein-series)
      - [Orthogonality of cusp forms and holomorphic Eisenstein series](modular-function.md#orthogonality-of-cusp-forms-and-holomorphic-eisenstein-series)
      - [Eisenstein series of weight two](modular-function.md#eisenstein-series-of-weight-two)
        - [Almost holomorphic weight-two Eisenstein series](modular-function.md#almost-holomorphic-weight-two-eisenstein-series)
          - [Weight-two transformation from an invariant Eisenstein limit](modular-function.md#weight-two-transformation-from-an-invariant-eisenstein-limit)
          - [Cancellation of weight-two Eisenstein anomalies](modular-function.md#cancellation-of-weight-two-eisenstein-anomalies)
        - [Iterated Eisenstein summation in weight two](modular-function.md#iterated-eisenstein-summation-in-weight-two)
      - [Nonholomorphic Eisenstein series](modular-function.md#nonholomorphic-eisenstein-series)
        - [Completed nonholomorphic Eisenstein series](modular-function.md#completed-nonholomorphic-eisenstein-series)
          - [Kronecker limit formula](modular-function.md#kronecker-limit-formula)
        - [Primitive real-analytic Eisenstein series](modular-function.md#primitive-real-analytic-eisenstein-series)
        - [Constant term of a nonholomorphic Eisenstein series](modular-function.md#constant-term-of-a-nonholomorphic-eisenstein-series)
        - [Hecke eigenvalue of a nonholomorphic Eisenstein series](modular-function.md#hecke-eigenvalue-of-a-nonholomorphic-eisenstein-series)
      - [Weight-k real-analytic Eisenstein series](modular-function.md#weight-k-real-analytic-eisenstein-series)
        - [Analytic continuation of a weight-k real-analytic Eisenstein series](modular-function.md#analytic-continuation-of-a-weight-k-real-analytic-eisenstein-series)
        - [Absolute convergence of a weight-k real-analytic Eisenstein series](modular-function.md#absolute-convergence-of-a-weight-k-real-analytic-eisenstein-series)
        - [Invariant product with a weight-k real-analytic Eisenstein series](modular-function.md#invariant-product-with-a-weight-k-real-analytic-eisenstein-series)
    - [Hecke operator](modular-function.md#hecke-operator)
      - [Modular Hecke algebra](modular-function.md#modular-hecke-algebra)
        - [Eisenstein ideal](modular-function.md#eisenstein-ideal)
      - [Hecke eigenform](modular-function.md#hecke-eigenform)
        - [Prime-power coefficients of a level-one eigenform are often large and positive](modular-function.md#prime-power-coefficients-of-a-level-one-eigenform-are-often-large-and-positive)
        - [Euler product of a Hecke eigenform](modular-function.md#euler-product-of-a-hecke-eigenform)
        - [Hecke eigenvalues are algebraic integers](modular-function.md#hecke-eigenvalues-are-algebraic-integers)
      - [Hecke multiplication relations](modular-function.md#hecke-multiplication-relations)
        - [Hecke prime-power recurrence from q-shift operators](modular-function.md#hecke-prime-power-recurrence-from-q-shift-operators)
      - [Noncuspidal level-one Hecke eigenform](modular-function.md#noncuspidal-level-one-hecke-eigenform)
      - [Integral Hecke algebra of level-one cusp forms](modular-function.md#integral-hecke-algebra-of-level-one-cusp-forms)
        - [Perfect integral Hecke pairing](modular-function.md#perfect-integral-hecke-pairing)
      - [Fourier coefficients of a composite-index Hecke operator](modular-function.md#fourier-coefficients-of-a-composite-index-hecke-operator)
      - [Determinant-n matrix representatives for Hecke operators](modular-function.md#determinant-n-matrix-representatives-for-hecke-operators)
      - [Finite Hecke orbit criterion for holomorphy at a cusp](modular-function.md#finite-hecke-orbit-criterion-for-holomorphy-at-a-cusp)
    - [Meromorphic modular form](modular-function.md#meromorphic-modular-form)
      - [Cusp-form divisor presentation](modular-function.md#cusp-form-divisor-presentation)
      - [Regular-cusp valence formula on a torsion-free modular curve](modular-function.md#regular-cusp-valence-formula-on-a-torsion-free-modular-curve)
      - [Valence formula for the modular group](modular-function.md#valence-formula-for-the-modular-group)
        - [Vanishing of weight-fourteen level-one cusp forms](modular-function.md#vanishing-of-weight-fourteen-level-one-cusp-forms)
        - [Vanishing of weight-two level-one modular forms](modular-function.md#vanishing-of-weight-two-level-one-modular-forms)
        - [Dimension bound for modular forms on a finite-index subgroup](modular-function.md#dimension-bound-for-modular-forms-on-a-finite-index-subgroup)
      - [Klein j-invariant](modular-function.md#klein-j-invariant)
        - [Klein j-invariant classifies complex lattice homothety](modular-function.md#klein-j-invariant-classifies-complex-lattice-homothety)
        - [Level-two modular ratio of Klein j-invariants](modular-function.md#level-two-modular-ratio-of-klein-j-invariants)
    - [Theta function](modular-function.md#theta-function)
      - [Riemann theta function](modular-function.md#riemann-theta-function)
      - [Gaussian theta sum](modular-function.md#gaussian-theta-sum)
        - [Theta series of a Euclidean lattice](modular-function.md#theta-series-of-a-euclidean-lattice)
        - [Small-parameter asymptotic of a lattice theta sum](modular-function.md#small-parameter-asymptotic-of-a-lattice-theta-sum)
        - [Covolume-one theta function of a fractional ideal](modular-function.md#covolume-one-theta-function-of-a-fractional-ideal)
      - [Lattice theta functional equation](modular-function.md#lattice-theta-functional-equation)
        - [Anisotropic theta functional equation](modular-function.md#anisotropic-theta-functional-equation)
      - [Jacobi theta function](modular-function.md#jacobi-theta-function)
        - [Jacobi derivative formula](modular-function.md#jacobi-derivative-formula)
        - [Theta function with characteristics](modular-function.md#theta-function-with-characteristics)
          - [Theta constant](modular-function.md#theta-constant)
          - [Period lattice of theta3 over theta4](modular-function.md#period-lattice-of-theta3-over-theta4)
          - [Jacobi theta duplication identity](modular-function.md#jacobi-theta-duplication-identity)
          - [Modular transformations of theta characteristics](modular-function.md#modular-transformations-of-theta-characteristics)
          - [Heat equation for theta functions with characteristics](modular-function.md#heat-equation-for-theta-functions-with-characteristics)
          - [Zeros of theta functions with characteristics](modular-function.md#zeros-of-theta-functions-with-characteristics)
        - [Jacobi abstruse identity](modular-function.md#jacobi-abstruse-identity)
        - [Theta-constant inversion and translation laws](modular-function.md#theta-constant-inversion-and-translation-laws)
        - [Theta series of integer squares](modular-function.md#theta-series-of-integer-squares)
          - [Eight-square representation formula](modular-function.md#eight-square-representation-formula)
        - [Jacobi triple product](modular-function.md#jacobi-triple-product)
          - [Jacobi cubic product identity](modular-function.md#jacobi-cubic-product-identity)
          - [Euler pentagonal identity](modular-function.md#euler-pentagonal-identity)
        - [Theta group](modular-function.md#theta-group)
        - [Nonvanishing of the Jacobi theta function](modular-function.md#nonvanishing-of-the-jacobi-theta-function)
    - [Lattice model of a modular form](modular-function.md#lattice-model-of-a-modular-form)
      - [Gamma 1 level structure on a complex lattice](modular-function.md#gamma-1-level-structure-on-a-complex-lattice)
        - [Diamond operator](modular-function.md#diamond-operator)
        - [Hecke operator on marked lattices](modular-function.md#hecke-operator-on-marked-lattices)
          - [Good-prime and bad-prime Hecke coefficient formula](modular-function.md#good-prime-and-bad-prime-hecke-coefficient-formula)
        - [Marked-lattice model of a modular form](modular-function.md#marked-lattice-model-of-a-modular-form)
        - [Prime-index overlattices preserving a Gamma 1 level structure](modular-function.md#prime-index-overlattices-preserving-a-gamma-1-level-structure)
      - [Weighted Gaussian theta sum of a complex lattice](modular-function.md#weighted-gaussian-theta-sum-of-a-complex-lattice)
      - [Hecke operator on lattice functions](modular-function.md#hecke-operator-on-lattice-functions)

## Integer factorization

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer_factorization)

Integer factorization seeks the [prime factorization](#fundamental-theorem-of-arithmetic) of a positive [integer](#integer) $N$. For $N>1$, this means identifying its [prime factors](#prime-factor) and their multiplicities; one has the empty [prime factorization](#fundamental-theorem-of-arithmetic). Finding one proper [divisor](#divisor) $1<d<N$ is useful progress, but need not finish the job: factor $d$ and $N/d$ further until all factors are [prime numbers](#prime-number).

For example, $77=7\cdot11$ is a [semiprime](#semiprime), whereas $231=3\cdot7\cdot11$ has three [prime factors](#prime-factor). [Primality testing](computer-science.md#primality-testing) asks whether a proposed [integer](#integer) is prime; it need not return a factor when the answer is no. [Trial division](#trial-division) is a direct factoring method: try division by small [prime numbers](#prime-number) until a [divisor](#divisor) is found. More elaborate methods obtain a proper [divisor](#divisor) through a [greatest common divisor](#greatest-common-divisor) of $N$ with a specially constructed [integer](#integer).

The beautiful trick in [congruence of squares](#congruence-of-squares) is that two [integers](#integer) with equal squares modulo $N$ can reveal different factors through their sum and difference. In the worked $N=77$ example, $20^2\equiv13^2\pmod{77}$ gives $\gcd(20-13,77)=7$ and $\gcd(20+13,77)=11$. Computing those [greatest common divisors](#greatest-common-divisor) uses the [Euclidean algorithm](#euclidean-algorithm); it does not require trying every potential factor. A [factor base](#factor-base) supplies a systematic way to construct useful equal-square relations. [Ben Lynn, Factoring and Discrete Logarithms: congruent squares and the linear-algebra step](https://crypto.stanford.edu/pbc/notes/crypto/factoring.html).

This connection is useful in [cryptography](computer-science.md#cryptography) because recovering the factors of an [RSA cryptosystem](algebra.md#rsa-cryptosystem) modulus defeats the factoring assumption behind its construction. That application concerns large, carefully chosen inputs; the small examples here explain the arithmetic mechanism and are not benchmarks or estimates of present cryptographic security.

### Factor base

↑ **Parent:** [Integer factorization](#integer-factorization)

A factor base is a finite [set](set.md) of small [prime numbers](#prime-number) over which selected auxiliary [integers](#integer) are completely factored. Some methods also record a sign coordinate for $-1$, which is not a [prime number](#prime-number). A positive [integer](#integer) supported entirely on the chosen [factor base](#factor-base) gives an [exponent vector](#exponent-vector); reducing that vector modulo two records which [prime exponents](#p-adic-valuation) are [odd integers](#odd-integer). The product is a [square of a number](arithmetic.md#square-of-a-number) precisely when every prime exponent is an [even integer](#even-number).

For the original toy $N=77$, use [factor base](#factor-base) $\{2,3,5\}$ and the two relations

$$
13^2\equiv15=3\cdot5\pmod{77},\qquad
40^2\equiv60=2^2\cdot3\cdot5\pmod{77}.
$$

The residues have exponent vectors $(0,1,1)$ and $(2,1,1)$ in the order $(2,3,5)$. Adding the two vectors modulo two gives $(0,0,0)$, so multiplying the residues gives $15\cdot60=900=30^2$. Consequently

$$
(13\cdot40)^2\equiv30^2\pmod{77},\qquad
X=13\cdot40\bmod77=58,\quad Y=30,
$$

and **$\gcd(X-Y,77)=7$ and $\gcd(X+Y,77)=11$**. Neither individual residue was a square; combining the relations made all exponents even.

<a id="image-a-factor-base-turns-two-smooth-relations-into-a-congruence-of-squares-through-exponent-parity"></a>
![](factor-base-parity-to-square-congruence.png)

**[Figure 1](#image-a-factor-base-turns-two-smooth-relations-into-a-congruence-of-squares-through-exponent-parity). A factor base turns two smooth relations into a congruence of squares through exponent parity**. The original $N=77$ example uses the ordered [factor base](#factor-base) $(2,3,5)$. The rows $(0,1,1)$ and $(2,1,1)$ add to zero modulo two, giving residue product $900=30^2$. The product of the original inputs is $520\equiv58\pmod{77}$; [greatest common divisor](#greatest-common-divisor) calculations then extract seven and eleven.

In a larger collection, choose relations $x_i^2\equiv r_i\pmod N$ with positive residues $r_i=\prod_{j=1}^B p_j^{e_{ji}}$. If a nonempty selection $I$ has an even sum in every exponent coordinate, set

$$
X=\prod_{i\in I}x_i\bmod N,\qquad
Y=\prod_{j=1}^B p_j^{\frac12\sum_{i\in I}e_{ji}}\bmod N.
$$

Then $X^2\equiv Y^2\pmod N$. Finding such a selection is a [linear dependence](vector-space.md#linear-dependence) problem over the [finite field](algebra.md#finite-field) $\mathbb F_2$: the indicator vector of the chosen relations belongs to the [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) given by the parity matrix. This is why a problem about [prime factors](#prime-factor) recruits [linear algebra](linear-algebra.md). The final [congruence of squares](#congruence-of-squares) may still be trivial, so another selection can be needed. [Ben Lynn, Factoring and Discrete Logarithms, Dixon's Algorithm: exponent matrix and kernel](https://crypto.stanford.edu/pbc/notes/crypto/factoring.html).

There is a tradeoff: a small [factor base](#factor-base) gives a smaller parity matrix, but fewer auxiliary [integers](#integer) factor completely over it. A larger [factor base](#factor-base) accepts more relations but makes the [linear algebra](linear-algebra.md) larger. Negative auxiliary values need an additional sign coordinate, and a selected product needs even sign parity as well as even prime exponents. Pomerance's account explains this balance and the historical development of combining smooth relations; the toy example omits algorithm-specific sieving and running-time claims. [Carl Pomerance, A Tale of Two Sieves (1996), pp. 1475–1476: exponent parity, factor bases and signs](https://math.dartmouth.edu/~carlp/PDF/paper109.pdf).

#### Exponent vector

↑ **Parent:** [Factor base](#factor-base)

Relative to an ordered [factor base](#factor-base) $(p_1,\ldots,p_B)$, a positive [integer](#integer) $r=\prod_jp_j^{e_j}$ has exponent vector $(e_1,\ldots,e_B)$. [Multiplication](arithmetic.md#multiplication) of such [integers](#integer) adds their exponent vectors. Reducing every coordinate modulo two gives the parity vector used to find [congruences of squares](#congruence-of-squares). The ordering and any sign coordinate must be used consistently across all rows.

### Odd part of a positive integer

↑ **Parent:** [Integer factorization](#integer-factorization)

The odd part of a positive [integer](#integer) $n$ is the unique odd positive [integer](#integer) $d$ obtained by repeatedly dividing $n$ by two. The process terminates because the positive [integers](#integer) decrease. If $2^r d=2^s e$ with $d,e$ odd, then $r>s$ would make $e$ even and $s>r$ would make $d$ even; hence $r=s$ and $d=e$. Two positive [integers](#integer) have the same odd part exactly when their ratio is an integral power of two. The odd positive [integers](#integer) therefore give representatives for the resulting [equivalence classes](set-theory.md#equivalence-class).

### Congruence of squares

↑ **Parent:** [Integer factorization](#integer-factorization)

A congruence of squares says that two [integers](#integer) $a,b$ have the same square modulo a positive [integer](#integer) $N$. Factoring their difference of squares gives

$$
a^2\equiv b^2\pmod N\quad\Longrightarrow\quad N\mid(a-b)(a+b).
$$

A useful [integer factorization](#integer-factorization) results when $\gcd(a-b,N)$ or $\gcd(a+b,N)$ is a proper [divisor](#divisor) of $N$. Divisibility of a product does not generally force divisibility of either factor by all of $N$: different [prime factors](#prime-factor) of $N$ can divide different parts of that product.

For $N=77$, $20^2-13^2=231=3\cdot77$. Therefore

$$
\gcd(20-13,77)=\gcd(7,77)=7,\qquad
\gcd(20+13,77)=\gcd(33,77)=11.
$$

**Thus $77=7\cdot11$.** The prime seven divides the difference, while eleven divides the sum. These computations already give a complete [prime factorization](#fundamental-theorem-of-arithmetic) because seven and eleven are [prime numbers](#prime-number).

The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) explains the hidden sign choices. The four [congruence classes](#congruence-class) solving $z^2\equiv15\pmod{77}$ have representatives $13,20,57,64$. Modulo seven each is $1$ or $-1$; modulo eleven each is $2$ or $-2$. Two independent sign choices produce four roots. The inputs thirteen and twenty agree modulo seven and disagree by sign modulo eleven, allowing their sum and difference to separate the two [prime factors](#prime-factor).

<a id="image-the-chinese-remainder-theorem-exposes-four-sign-choices-behind-one-square-residue-modulo-77"></a>
![](square-congruence-chinese-remainder-signs.png)

**[Figure 2](#image-the-chinese-remainder-theorem-exposes-four-sign-choices-behind-one-square-residue-modulo-77). The Chinese remainder theorem exposes four sign choices behind one square residue modulo $77$**. Each cell gives the unique residue modulo $77$ with its indicated residues modulo seven and eleven. Relative to input thirteen, input twenty agrees modulo seven and has the opposite sign modulo eleven. The resulting [greatest common divisors](#greatest-common-divisor) are seven and eleven. Diagonal all-same or all-opposite choices give only the trivial factors one and $77$.

For distinct odd [prime numbers](#prime-number) $p,q$, $N=pq$ and $\gcd(b,N)=1$, a solution $a^2\equiv b^2\pmod N$ with $a\not\equiv b$ and $a\not\equiv-b$ modulo $N$ yields both proper factors by the two [greatest common divisors](#greatest-common-divisor). For a general composite [integer](#integer), a proper [divisor](#divisor) need not itself be prime; further factoring can remain. If $a\equiv b$ or $a\equiv-b\pmod N$ in the coprime case, the two calculations return $N$ and one instead. A [factor base](#factor-base) helps generate relations, but does not ensure every resulting relation is useful.

For historical context, Pomerance describes Kraitchik's 1920s enhancement of the difference-of-squares approach associated with Fermat: seek a difference that is a multiple of $N$, rather than exactly $N$. His account also notes antecedents in Gauss and Seelhoff, so this is not an attribution of the whole idea to a single inventor. [Carl Pomerance, A Tale of Two Sieves (1996), pp. 1474–1475: difference-of-squares and congruent squares](https://math.dartmouth.edu/~carlp/PDF/paper109.pdf).

#### Nontrivial square root of unity modulo an integer

↑ **Parent:** [Congruence of squares](#congruence-of-squares)

For an odd [integer](#integer) $N>1$, a nontrivial square root of unity modulo $N$ is a residue $z$ with $z^2\equiv1\pmod N$ and $z\not\equiv\pm1\pmod N$. Then both $\gcd(z-1,N)$ and $\gcd(z+1,N)$ are proper [divisors](#divisor). For $N=77$, $z=34$ works: $34^2\equiv1\pmod{77}$, $\gcd(33,77)=11$, and $\gcd(35,77)=7$.

A [congruence of squares](#congruence-of-squares) with $\gcd(b,N)=1$ converts to this form by $z\equiv a b^{-1}\pmod N$, using a [modular multiplicative inverse](#modular-multiplicative-inverse). In the $a=20,b=13$ example, $13^{-1}\equiv6\pmod{77}$, so $z\equiv20\cdot6\equiv43\pmod{77}$. It yields $\gcd(42,77)=7$ and $\gcd(44,77)=11$. Nontriviality requires mixed sign choices across prime factors, which an odd [prime number](#prime-number) modulus cannot provide.

<h2 id="erdos-turan-inequality">Erdős-Turán inequality</h2>

↑ **Parent:** [Number theory](number-theory.md)

The Erdős-Turán inequality bounds discrepancy of a finite sequence on the circle by a smoothing error and exponential sums of its low Fourier modes.

## Fermat number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_number)

A [Fermat number](#fermat-number) is the [positive integer](#positive-integer) $F_n=2^{2^n}+1$, indexed by a [nonnegative integer](arithmetic.md#natural-number) $n$. The first five are $3,5,17,257,65537$, all [prime numbers](#prime-number); the next is **the [composite number](#composite-number) $F_5=4294967297=641\cdot6700417$**. This family offers a compact lesson in [number theory](number-theory.md): a very persuasive finite pattern can fail, while an exact [divisibility](#divisibility) relation settles a gigantic case with little computation.

<a id="image-exact-fermat-numbers-five-initial-primes-a-composite-sixth-term-and-rapidly-increasing-decimal-lengths"></a>
![](fermat-numbers-growth-and-first-factors.png)

**[Figure 3](#image-exact-fermat-numbers-five-initial-primes-a-composite-sixth-term-and-rapidly-increasing-decimal-lengths). Exact Fermat numbers: five initial primes, a composite sixth term, and rapidly increasing decimal lengths**.

Why does the exponent itself have the form $2^n$? Suppose $m=ab$ is a [positive integer](#positive-integer) with an [odd integer](#odd-integer) factor $b>1$. The [polynomial factorization](polynomial.md#factorization-of-polynomials) $x^b+1=(x+1)(x^{b-1}-x^{b-2}+\cdots-x+1)$ shows that $2^a+1$ is a proper [divisor](#divisor) of $2^m+1$. Consequently, if $2^m+1$ is a [prime number](#prime-number), $m$ must be a [power of two](#power-of-two). That is a necessary condition, rather than a promise that the surviving candidates are prime.

The [Fermat number product identity](#fermat-number-product-identity) makes distinct [Fermat numbers](#fermat-number) [coprime integers](#coprime-integers). Thus every term has a [prime factor](#prime-factor) absent from all earlier terms, whether or not that term is itself a [prime number](#prime-number). This gives an explicit route to infinitely many different [prime numbers](#prime-number), without establishing that infinitely many terms of this particular [sequence](real-analysis.md#sequence) are prime. Meanwhile the [prime divisor of a Fermat number](#prime-divisor-of-a-fermat-number) criterion filters possible factors through a small [multiplicative order](#multiplicative-order) calculation.

The family also links arithmetic to [Euclidean geometry](geometry-and-topology.md#euclidean-geometry): a [constructible regular polygon](straightedge-and-compass-construction.md#constructible-regular-polygon) can have a number of sides equal to a [power of two](#power-of-two) times a product of distinct [Fermat primes](#fermat-prime). The [Gauss-Wantzel theorem](straightedge-and-compass-construction.md#gauss-wantzel-theorem) gives the precise criterion. For instance, $15=3\cdot5$ and $17$ qualify, but $9=3^2$ does not. The word "distinct" matters. [Carl Pomerance](mathematics-author.md#carl-pomerance) describes this connection in [Primality testing: then and now by Carl Pomerance](mathematics-bibliography.md#primality-testing-then-and-now-by-carl-pomerance) (slide 18).

Historically, [Leonhard Euler](mathematics.md#leonhard-euler) records [Pierre de Fermat](mathematics.md#pierre-de-fermat)'s proposed primality pattern, then refutes it by finding the factor $641$ of $F_5$. His paper was presented in 1732 and published in 1738; those are different events, not competing dates for one publication.[pp. 1–2 and the publication note](mathematics-bibliography.md#observations-on-a-certain-theorem-of-fermat-and-on-others-concerning-prime-numbers-by-leonhard-euler)

A short modern check needs only two representations of $641$:

$$
641=5\cdot2^7+1=5^4+2^4.
$$

In [modular arithmetic](#modular-arithmetic) these give $5^4 2^{28}\equiv1$ and $5^4\equiv-2^4\pmod{641}$. Substitution yields $2^{32}\equiv-1\pmod{641}$, so $641\mid F_5$. This verifies the factor directly; it does not claim to reconstruct Euler's search process.

### Fermat number product identity

↑ **Parent:** [Fermat number](#fermat-number)

For each [positive integer](#positive-integer) $n$, the product of the preceding [Fermat numbers](#fermat-number) is two less than the next:

$$
\prod_{j=0}^{n-1}F_j=2^{2^n}-1=F_n-2.
$$

For example, $3\cdot5\cdot17=255=257-2$. The identity telescopes by repeated [difference of squares](#difference-of-two-squares): $(2^{2^j}-1)(2^{2^j}+1)=2^{2^{j+1}}-1$. Its usefulness is that a huge [integer](#integer) product exposes a tiny difference, two, from the next term.

#### Distinct Fermat numbers are coprime

↑ **Parent:** [Fermat number product identity](#fermat-number-product-identity)

If $m<n$, a common [divisor](#divisor) of $F_m$ and $F_n$ divides both $F_n-2$, by the [Fermat number product identity](#fermat-number-product-identity), and $F_n$. It therefore divides two. Both [Fermat numbers](#fermat-number) are [odd integers](#odd-integer), so their [greatest common divisor](#greatest-common-divisor) is one. Each term's [prime factors](#prime-factor) are consequently different from the [prime factors](#prime-factor) of every other term.

### Prime divisor of a Fermat number

↑ **Parent:** [Fermat number](#fermat-number)

For a [prime number](#prime-number) $p$, the exact criterion is

$$
p\mid F_n\quad\Longleftrightarrow\quad\operatorname{ord}_p(2)=2^{n+1},\qquad n\geq0,
$$

where $p$ must be different from two and $\operatorname{ord}_p(2)$ is the [multiplicative order](#multiplicative-order) of two modulo $p$. If $p\mid F_n$, then $2^{2^n}\equiv-1\pmod p$: the order divides $2^{n+1}$ but not $2^n$, so it is exactly $2^{n+1}$. Conversely, that order makes $2^{2^n}$ a [square root of unity](algebra.md#square-root-of-unity) different from one in the [prime field](algebra.md#prime-field) $\mathbb F_p$; it must be $-1$, because $(x-1)(x+1)=0$ has no other roots in a [field](algebra.md#field).

<a id="image-exact-modular-powers-distinguish-fermat-divisors-from-the-prime-thirteen-whose-multiplicative-order-is-twelve"></a>
![](fermat-prime-divisors-modular-orders.png)

**[Figure 4](#image-exact-modular-powers-distinguish-fermat-divisors-from-the-prime-thirteen-whose-multiplicative-order-is-twelve). Exact modular powers distinguish Fermat divisors from the prime thirteen, whose multiplicative order is twelve**.

For example, modulo seventeen the powers of two are $2,4,8,16,15,13,9,1$. Their first return to one occurs after eight steps. The half-way value is $16=-1\pmod{17}$, proving that $17\mid F_2$. Likewise, $\operatorname{ord}_{641}(2)=64$ identifies $641$ as a [prime factor](#prime-factor) of $F_5$. These are statements about [divisibility](#divisibility), not evidence that the entire [Fermat number](#fermat-number) is prime.

The [multiplicative order](#multiplicative-order) always divides $p-1$, by [Fermat's little theorem](#fermat-little-theorem), so $p\equiv1\pmod{2^{n+1}}$. In particular, for $n\geq1$ every [prime divisor of a Fermat number](#prime-divisor-of-a-fermat-number) is one modulo four. That weaker [modular congruence](#modular-congruence) is insufficient: thirteen is one modulo four, but $\operatorname{ord}_{13}(2)=12$, which is not a [power of two](#power-of-two). It divides no [Fermat number](#fermat-number) at any index. The exact order criterion explains the whole family, instead of testing finitely many terms.

#### Stronger prime-divisor congruence for Fermat numbers

↑ **Parent:** [Prime divisor of a Fermat number](#prime-divisor-of-a-fermat-number)

For $n\geq2$, the first order bound already gives $p\equiv1\pmod8$. The [second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity) says that two is then a [quadratic residue](#quadratic-residue) modulo $p$. [Euler's criterion](#euler-s-criterion) gives $2^{(p-1)/2}\equiv1$, so its [multiplicative order](#multiplicative-order) $2^{n+1}$ divides $(p-1)/2$. Thus $2^{n+2}\mid p-1$, further reducing the candidate factors. At $n=5$, $641=5\cdot128+1$ meets this bound. The restriction matters: $F_1=5$ has factor five, which is not one modulo eight.

## Bernoulli number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_number)

The [Bernoulli numbers](#bernoulli-number) are a [sequence](real-analysis.md#sequence) of [rational numbers](#rational-number) that turns [integer power sums](#integer-power-sum) into exact [polynomials](polynomial.md). The same numbers describe corrections when a discrete [summation](arithmetic.md#summation) is compared with an [integral](calculus.md#integral). For example, the [sum of squares](arithmetic.md#sum-of-squares) $1^2+\cdots+N^2$ is $N^3/3+N^2/2+N/6$: the leading term is an [integral](calculus.md#integral), while the last two terms repair the difference between area and sampled values.

We use **$B_1=-\tfrac12$ throughout**. The defining [exponential generating function](real-analysis.md#exponential-generating-function) is

$$
\frac{t}{e^t-1}=\sum_{n=0}^{\infty}B_n\frac{t^n}{n!}
=1-\frac t2+\frac{t^2}{12}-\frac{t^4}{720}+\frac{t^6}{30240}-\cdots.
$$

Here $e^t$ is the [exponential function](calculus.md#exponential-function) and $n!$ is a [factorial](combinatorics.md#factorial); in particular, the [coefficient](vector-space.md#coefficient) of $t^2$ is $B_2/2!$, rather than $B_2$. At $t=0$ the quotient has limiting value one. The identity can be read algebraically as a [formal power series](commutative-algebra.md#formal-power-series), or as a [convergent series](real-analysis.md#convergent-series) for $|t|<2\pi$.[Karl Dilcher, Chapter 24, §24.2(i), equation 24.2.1: defining generating function and convergence domain](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

To compute the numbers, multiply by $e^t-1$ and compare [coefficients](vector-space.md#coefficient). The resulting [recurrence relation](real-analysis.md#recurrence-relation), with [binomial coefficients](combinatorics.md#binomial-coefficient), is

$$
B_0=1,\qquad \sum_{k=0}^{m}\binom{m+1}{k}B_k=0\quad(m\geq1),\qquad
B_m=-\frac{1}{m+1}\sum_{k=0}^{m-1}\binom{m+1}{k}B_k.
$$

Thus $1+2B_1=0$, $1+3B_1+3B_2=0$, and $1+4B_1+6B_2+4B_3=0$ give $B_1=-1/2$, $B_2=1/6$, and $B_3=0$. Continuing gives

$$
\begin{array}{c|rrrrrrrrrrr}
n&0&1&2&3&4&5&6&7&8&9&10\\\hline
B_n&1&-\tfrac12&\tfrac16&0&-\tfrac1{30}&0&\tfrac1{42}&0&-\tfrac1{30}&0&\tfrac5{66}
\end{array}
$$

The [recurrence relation](real-analysis.md#recurrence-relation) agrees with equation 24.5.3 after replacing its index $n$ by $m+1$.[Karl Dilcher, Chapter 24, §24.5(i), equation 24.5.3; first values also in Table 24.2.1](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

Why do so many values vanish? Put $F(t)=t/(e^t-1)$. Direct substitution gives $F(-t)=F(t)+t$, so $F(t)+t/2$ is an [even function](calculus.md#even-function). Its odd [power series](real-analysis.md#power-series) [coefficients](vector-space.md#coefficient) vanish: $B_{2r+1}=0$ for every [positive integer](#positive-integer) $r$. The exception $B_1$ matters. The alternative convention obtained from $t/(1-e^{-t})=F(t)+t$ has $B_1^{+}=+1/2$ and exactly the same other values. A formula copied between conventions must also retain its summation endpoints.

Historically, [integer power sums](#integer-power-sum) were studied before the modern [Bernoulli number](#bernoulli-number) notation. A historical study examines formulas published in 1631 and distinguishes those separate formulas from encoding all exponents using one [sequence](real-analysis.md#sequence) of constants. This is a useful motivation for the [generating function](real-analysis.md#generating-function), without assigning all discovery to a single moment. [Donald E. Knuth, Johann Faulhaber and sums of powers, 1992 preprint, pp. 2 and 14: the 1631 power-sum formulas and the uniform Bernoulli-number formula](mathematics-bibliography.md#johann-faulhaber-and-sums-of-powers-by-donald-e-knuth)

### Bernoulli polynomial

↑ **Parent:** [Bernoulli number](#bernoulli-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Bernoulli_polynomial)

The [Bernoulli polynomials](#bernoulli-polynomial) extend the [Bernoulli numbers](#bernoulli-number) by inserting the [exponential function](calculus.md#exponential-function) $e^{xt}$ into their [exponential generating function](real-analysis.md#exponential-generating-function):

$$
\frac{te^{xt}}{e^t-1}=\sum_{n=0}^{\infty}B_n(x)\frac{t^n}{n!},\qquad
B_n(x)=\sum_{j=0}^{n}\binom nj B_jx^{n-j},\qquad B_n(0)=B_n.
$$

For example, $B_0(x)=1$, $B_1(x)=x-1/2$, $B_2(x)=x^2-x+1/6$, and $B_3(x)=x^3-3x^2/2+x/2$.[Karl Dilcher, Chapter 24, equations 24.2.3–24.2.5 and Table 24.2.2](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

Their crucial property is a [finite difference](finite-difference.md) identity:

$$
B_n(x+1)-B_n(x)=nx^{n-1}\quad(n\geq1).
$$

Indeed, subtracting the two [exponential generating functions](real-analysis.md#exponential-generating-function) cancels $e^t-1$ and leaves $te^{xt}$. Thus $B_{p+1}(x)/(p+1)$ plays for discrete [summation](arithmetic.md#summation) the role that $x^{p+1}/(p+1)$ plays for [integration](calculus.md#integral): taking a unit [finite difference](finite-difference.md) recovers $x^p$.[Karl Dilcher, Chapter 24, §24.4(i), equation 24.4.1](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

#### Integer power sum

↑ **Parent:** [Bernoulli polynomial](#bernoulli-polynomial)

An integer power sum adds a fixed nonnegative [integer](#integer) power of consecutive [integers](#integer). Let $N$ be a [nonnegative integer](arithmetic.md#natural-number) and $p$ a [nonnegative integer](arithmetic.md#natural-number). For $p=0$, use the constant [polynomial](polynomial.md) $x^0=1$, including at zero, so $S_0(N)=N$. Summing the [Bernoulli polynomial](#bernoulli-polynomial) [finite difference](finite-difference.md) identity makes the intermediate terms cancel and gives

$$
S_p(N)=\sum_{k=0}^{N-1}k^p
=\frac{B_{p+1}(N)-B_{p+1}(0)}{p+1}
=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_jN^{p+1-j}.
$$

The sum is empty when $N=0$. For the endpoints $1,\ldots,N$, the formula valid also at $p=0$ is instead

$$
\sum_{k=1}^{N}k^p=\frac{B_{p+1}(N+1)-B_{p+1}(1)}{p+1}.
$$

For $p\geq1$, $B_{p+1}(1)=B_{p+1}(0)$, and this becomes the standard positive-endpoint formula. The exception at $p=0$ is essential: $B_1(1)-B_1(0)=1$.[Karl Dilcher, Chapter 24, equations 24.4.1 and 24.4.7; the displayed equation 24.4.7 needs the endpoint adjustment at exponent zero](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

For $p\geq1$, adding $N^p$ to $S_p(N)$ changes the $B_1$ contribution from $-N^p/2$ to $+N^p/2$. Equivalently,

$$
\sum_{k=1}^{N}k^p=\frac{1}{p+1}\sum_{j=0}^{p}\binom{p+1}{j}B_j^{+}N^{p+1-j}\quad(p\geq1),
$$

where only $B_1^{+}$ differs from our [Bernoulli numbers](#bernoulli-number). A quick endpoint check is $p=1$: the sums over $0,\ldots,N-1$ and $1,\ldots,N$ are $N(N-1)/2$ and $N(N+1)/2$, respectively. The latter is a [triangular number](arithmetic.md#triangular-number).

##### Bernoulli corrections for polynomial sums

↑ **Parent:** [Integer power sum](#integer-power-sum)

For a concrete comparison, take $f(x)=x^2$ on $[0,6]$. The [integral](calculus.md#integral) is $I=\int_0^6x^2\,dx=72$, whereas the unit-width left and right [Riemann sums](real-analysis.md#riemann-sum) are $L=55$ and $R=91$. The exact [integer power sum](#integer-power-sum) formula gives

$$
L=I-\frac{6^2}{2}+\frac66=55,\qquad
R=I+\frac{6^2}{2}+\frac66=91.
$$

The endpoint choice explains the opposite signs of the $18$ correction. The remaining correction is one in both cases.

<a id="image-left-and-right-riemann-sums-for-x-2-differ-from-its-integral-by-exact-bernoulli-number-corrections"></a>
![](bernoulli-square-sums-versus-integral.png)

**[Figure 5](#image-left-and-right-riemann-sums-for-x-2-differ-from-its-integral-by-exact-bernoulli-number-corrections). Left and right Riemann sums for $x^2$ differ from its integral by exact Bernoulli number corrections**. Six rectangles of width one sample $x^2$ at $0,\ldots,5$ on the left and $1,\ldots,6$ on the right. Their areas are $55$ and $91$; the smooth area is $72$. The endpoint terms are $-18$ and $+18$, while the $B_2$ correction adds one in each case.

The same method is useful far beyond [squares of numbers](arithmetic.md#square-of-a-number). Substituting $B_0$, $B_1$, $B_2$ and $B_4$ into the [integer power sum](#integer-power-sum) formula gives the exact fourth-power result

$$
\sum_{k=1}^{N}k^4=\frac{N^5}{5}+\frac{N^4}{2}+\frac{N^3}{3}-\frac{N}{30}.
$$

At $N=10$, this is

$$
\underbrace{20000}_{\text{integral}}+\underbrace{5000}_{\text{endpoint}}+
\underbrace{\frac{1000}{3}}_{B_2\text{ term}}-
\underbrace{\frac13}_{B_4\text{ term}}=25333.
$$

Thus a finite [polynomial](polynomial.md) calculation replaces ten additions, or a million additions if $N$ is a million. Although the individual corrections can be [rational numbers](#rational-number), the result is the exact [integer](#integer) sum.

<a id="image-exact-bernoulli-number-corrections-turn-an-integral-into-the-fourth-power-sum-1-4-plus-cdots-plus-10-4"></a>
![](bernoulli-fourth-power-exact-corrections.png)

**[Figure 6](#image-exact-bernoulli-number-corrections-turn-an-integral-into-the-fourth-power-sum-1-4-plus-cdots-plus-10-4). Exact Bernoulli number corrections turn an integral into the fourth-power sum $1^4+\cdots+10^4$**. The first panel builds the sum from integral $20000$, endpoint term $5000$, and $B_2$ term $1000/3$. The enlarged second panel resolves the final $B_4$ correction $-1/3$, reaching $25333$, checked independently by direct addition.

There is also a useful [numerical integration](numerical-analysis.md#numerical-integration) interpretation. The average of the left and right [Riemann sums](real-analysis.md#riemann-sum) is the composite [trapezoidal rule](numerical-analysis.md#trapezoidal-rule). For $x^2$, the endpoint corrections cancel but its value is $73$, one above the true [integral](calculus.md#integral). Subtracting the $B_2$ correction makes this particular [polynomial](polynomial.md) example exact. For $f(x)=x^4$, the two interior corrections above can be written $B_2(f'(N)-f'(0))/2!$ and $B_4(f'''(N)-f'''(0))/4!$. These are exact identities for these [polynomials](polynomial.md); extending such corrections to general [functions](function.md) requires a separate error analysis.

### Hyperbolic cotangent generating function for Bernoulli numbers

↑ **Parent:** [Bernoulli number](#bernoulli-number)

The defining generating function of the [Bernoulli numbers](#bernoulli-number), with $B_1=-1/2$, gives this identity of formal [Laurent series](analysis.md#laurent-series) by $\coth z=1+2/(e^{2z}-1)$. Therefore $a\coth(az)-\coth z$ is regular and odd. Integrating it gives the even formal logarithm of $\sinh(az)/(a\sinh z)$. Its even derivatives of order $k$ at zero are $2^k(a^k-1)B_k/k$, while the odd derivatives vanish. This computes the [cyclotomic higher logarithmic derivatives](algebraic-number-theory.md#cyclotomic-higher-logarithmic-derivative) of symmetric [cyclotomic units](galois-theory.md#cyclotomic-unit) without introducing a spurious linear term.

### Euler evaluation of even zeta values

↑ **Parent:** [Bernoulli number](#bernoulli-number)

Expand the [cotangent partial-fraction expansion](geometry-and-topology.md#cotangent-partial-fraction-expansion) at zero to obtain $\pi\cot(\pi z)=z^{-1}-2\sum_{r\geq1}\zeta(2r)z^{2r-1}$. Substituting $t=2\pi iz$ in the generating function of the [Bernoulli numbers](#bernoulli-number) gives the same [Laurent series](analysis.md#laurent-series) as $z^{-1}+\sum_{r\geq1}B_{2r}(2\pi i)^{2r}z^{2r-1}/(2r)!$. Equality of [Laurent coefficients](analysis.md#laurent-coefficient) proves the formula.

### Generalized Bernoulli number

↑ **Parent:** [Bernoulli number](#bernoulli-number)

For a [Dirichlet character](algebraic-number-theory.md#dirichlet-character) $\chi$ of conductor $f$, define the generalized Bernoulli numbers by

$$
\sum_{a=1}^{f}\chi(a)\frac{z e^{az}}{e^{fz}-1}
=\sum_{k\geq0}B_{k,\chi}\frac{z^k}{k!}.
$$

They express special values of [Dirichlet L-functions](algebraic-number-theory.md#dirichlet-l-function) at nonpositive integers and occur in the interpolation formula for [Kubota-Leopoldt p-adic L-functions](analytic-number-theory.md#kubota-leopoldt-p-adic-l-function).

## Normal number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Normal_number)

A [real number](arithmetic.md#real-number) is normal in an [integer](#integer) base $K\geq2$ when every finite [word](foundations-of-mathematics.md#string) of digits occurs in its [positional notation](#positional-notation) with the same limiting [digit block frequency](#digit-block-frequency) as every other [word](foundations-of-mathematics.md#string) of the same length. Write its [fractional part](calculus.md#fractional-part) as $x=0.d_1d_2\ldots$ in base $K$, using the expansion that is not eventually all $K-1$ digits when two expansions are possible. For every length $r\geq1$ and every [word](foundations-of-mathematics.md#string) $w\in\{0,\ldots,K-1\}^r$, the requirement is

$$
\lim_{N\to\infty}\frac{\left|\{1\leq j\leq N-r+1:(d_j,\ldots,d_{j+r-1})=w\}\right|}{N-r+1}=K^{-r}.
$$

Occurrences overlap: the [word](foundations-of-mathematics.md#string) $11$ occurs twice in $111$. There are $K^r$ possible [words](foundations-of-mathematics.md#string) of length $r$, so $K^{-r}$ is the equal share for each. In a [decimal representation](#decimal-representation), this means frequency $1/10$ for each digit, $1/100$ for each pair, and $1/1000$ for each triple, continuing through every finite length. The definition agrees with that used by Copeland and Erdős in their work on explicit [normal numbers](#normal-number). [Arthur H. Copeland and Paul Erdős, Note on Normal Numbers, 1946, opening definition](https://users.renyi.hu/~p_erdos/1946-01.pdf)

The appeal is that a precise, deterministic [real number](arithmetic.md#real-number) can have the same limiting [digit block frequencies](#digit-block-frequency) as repeated draws from a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution), with [independence](random-variable.md#independent-random-variables) between draws. [Champernowne constant](#champernowne-constant) is an explicit example. Normality is useful for studying digit distribution, but balanced digits alone establish only a [simply normal number](#simply-normal-number), and a finite sample cannot establish any of these infinite [limits](calculus.md#limit-of-a-function).

Émile Borel introduced [normal numbers](#normal-number) and established their prevalence in his 1909 paper applying [probability](probability-theory.md#probability) to [number theory](number-theory.md); the stronger all-base statement is discussed under [absolutely normal number](#absolutely-normal-number). [Émile Borel, Les probabilités dénombrables et leurs applications arithmétiques, Rendiconti del Circolo Matematico di Palermo 27, 247–271, 1909](https://doi.org/10.1007/BF03019651)

### Digit block frequency

↑ **Parent:** [Normal number](#normal-number)

For a finite prefix of $N\geq r$ digits in [positional notation](#positional-notation), the digit block frequency $F_N(w)$ of a length-$r$ [word](foundations-of-mathematics.md#string) $w$ is its number of overlapping occurrences divided by $N-r+1$, the number of available starting positions. All such [digit block frequencies](#digit-block-frequency) sum to one. The infinite [limit](calculus.md#limit-of-a-function) used for a [normal number](#normal-number) can instead divide counts by $N$: the factor $(N-r+1)/N$ tends to one for fixed $r$.

For the six [binary digits](#binary-digit) $010101$, the single-digit counts are three zeros and three ones. Its five adjacent pairs are $01,10,01,10,01$, giving

$$
F_6(00)=F_6(11)=0,\qquad F_6(01)=\frac35,\qquad F_6(10)=\frac25.
$$

This example explains both the overlapping convention and the end correction in a finite sample. The corresponding infinite [binary expansion](arithmetic.md#binary-expansion) has pair frequencies $0,1/2,1/2,0$, rather than the four values $1/4$ required of a [normal number](#normal-number) in base two.

### Simply normal number

↑ **Parent:** [Normal number](#normal-number)

A [real number](arithmetic.md#real-number) is simply normal in base $K$ if each individual digit in its [positional notation](#positional-notation) has limiting [digit block frequency](#digit-block-frequency) $1/K$. This is the length-one part of the definition of a [normal number](#normal-number). It places no equal-frequency requirement on longer [words](foundations-of-mathematics.md#string).

For example, $x=0.010101\ldots_2=1/3$ is a [simply normal number](#simply-normal-number) in base two: each [binary digit](#binary-digit) has frequency $1/2$. But $00$ and $11$ never occur, and $01$ and $10$ each have frequency $1/2$. Thus $x$ is not a [normal number](#normal-number) in base two. Even a [sequence](real-analysis.md#sequence) that looks more complicated, such as the deterministic [Thue–Morse sequence](real-analysis.md#thue-morse-sequence), must be tested against the actual [digit block frequency](#digit-block-frequency) definition; visual complexity is no substitute for it.

The [decimal representation](#decimal-representation) $y=0.01234567890123456789\ldots$ makes the same point in base ten. Every digit has frequency $1/10$, yet the only adjacent pairs are

$$
01,12,23,34,45,56,67,78,89,90.
$$

Each has limiting [digit block frequency](#digit-block-frequency) $1/10$; the other ninety pairs have frequency zero. A [normal number](#normal-number) in base ten requires $1/100$ for every one of the hundred pairs. This [rational number](#rational-number) is a [simply normal number](#simply-normal-number) in base ten, but it is not a [normal number](#normal-number) in that base.

### Champernowne constant

↑ **Parent:** [Normal number](#normal-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Champernowne_constant)

Form [Champernowne constant](#champernowne-constant) by using [concatenation](foundations-of-mathematics.md#concatenation) to join the [decimal representations](#decimal-representation) of the [positive integers](#positive-integer) $1,2,3,\ldots$ after the decimal point. Champernowne proved in 1933 that this particular [real number](arithmetic.md#real-number) is a [normal number](#normal-number) in base ten. The construction is striking because its rule is completely explicit, while all finite [words](foundations-of-mathematics.md#string) have the prescribed limiting [digit block frequencies](#digit-block-frequency). [D. G. Champernowne, The Construction of Decimals Normal in the Scale of Ten, Journal of the London Mathematical Society 8, 254–260, 1933](https://doi.org/10.1112/jlms/s1-8.4.254) Copeland and Erdős explicitly recall this result at the start of their own paper. [Copeland and Erdős, Note on Normal Numbers, 1946, first paragraph](https://users.renyi.hu/~p_erdos/1946-01.pdf)

The first $100000$ digits of [Champernowne constant](#champernowne-constant) have the following exact counts, in digit order $0,1,\ldots,9$:

$$
(8642,19753,11111,8642,8642,8642,8642,8642,8642,8642).
$$

For the $99999$ adjacent pairs fully inside that prefix, the [words](foundations-of-mathematics.md#string) $00,01,12,99$ occur $642,1753,2088,753$ times respectively. Thus, for example, $F_{100000}(12)=2088/99999$, which is about $0.02088$, rather than $0.01$. The prefix ends partway through the [decimal representation](#decimal-representation) of $22222$; the many leading ones in earlier [positive integers](#positive-integer) help explain the visible imbalance.

<a id="image-exact-digit-and-adjacent-pair-frequencies-in-two-prefixes-of-100000-decimal-digits"></a>
![](digit-block-frequency-comparison.png)

**[Figure 7](#image-exact-digit-and-adjacent-pair-frequencies-in-two-prefixes-of-100000-decimal-digits). Exact digit and adjacent-pair frequencies in two prefixes of 100000 decimal digits**. The upper panels compare single-digit frequencies and list exact counts. The lower panels show all hundred overlapping pair frequencies, each with denominator $99999$, on the same vertical scale. The dashed $1/100$ line is the limiting reference for a [normal number](#normal-number) in base ten. In the periodic prefix, pairs $01$ through $89$ occur $10000$ times each and $90$ occurs $9999$ times; all other pairs are absent.

These are finite counts, not a proof of the [normal number](#normal-number) theorem: a finite prefix can be followed by an all-zero tail. The theorem for [Champernowne constant](#champernowne-constant) concerns the infinite [limit](calculus.md#limit-of-a-function), and establishes base-ten normality, rather than [absolute normality](#absolutely-normal-number). Nor do computations prove normality for familiar constants: the normality of [Pi](topology.md#pi) and [Euler's number](calculus.md#e-mathematical-constant) remains unproved, as discussed by Bailey and Borwein. [David H. Bailey and Jonathan M. Borwein, Normal Numbers and Pseudorandom Generators, author manuscript, 2011, introduction](https://www.davidhbailey.com/dhbpapers/normal-pseudo.pdf)

### Normality and equidistribution under integer multiplication

↑ **Parent:** [Normal number](#normal-number)

A [real number](arithmetic.md#real-number) $x$ is a [normal number](#normal-number) in base $K$ exactly when its iterates under the [integer multiplication map on the circle](measure-theory.md#integer-multiplication-map-on-the-circle), $T_K(x)=\{Kx\}$, form an [equidistributed sequence](measure-theory.md#equidistributed-sequence). Braces denote the [fractional part](calculus.md#fractional-part). Multiplication by $K$ shifts the [positional notation](#positional-notation) one digit to the left:

$$
T_K^n(x)=\{K^nx\}=0.d_{n+1}d_{n+2}\ldots\quad\text{in base }K.
$$

A length-$r$ [word](foundations-of-mathematics.md#string) with base-$K$ [integer](#integer) value $a$ specifies the half-open [interval](real-analysis.md#interval-mathematics) $[a/K^r,(a+1)/K^r)$, whose length is $K^{-r}$. Visiting that [interval](real-analysis.md#interval-mathematics) is exactly encountering that [word](foundations-of-mathematics.md#string) at the next digit position. These digit [intervals](real-analysis.md#interval-mathematics) form arbitrarily fine grids, so their correct limiting visiting frequencies imply [equidistribution](measure-theory.md#equidistributed-sequence) on every [interval](real-analysis.md#interval-mathematics). This converts a question about digits into one about a [dynamical system](dynamical-systems.md#dynamical-system). Bailey and Crandall develop this connection using [equidistribution](measure-theory.md#equidistributed-sequence) of the [fractional parts](calculus.md#fractional-part) of $K^nx$. [David H. Bailey and Richard E. Crandall, Random Generators and Normal Numbers, 2003 author manuscript, Section 2](https://www.davidhbailey.com/dhbpapers/bcnormal.pdf)

In base ten the [word](foundations-of-mathematics.md#string) $12$ corresponds to $[0.12,0.13)$. For [Champernowne constant](#champernowne-constant), counting the visits $T_{10}^n(x)$ for $0\leq n\leq99998$ gives precisely the $2088$ occurrences of $12$ in its first $100000$ digits. For $x=1/3$, the base-two [integer multiplication map on the circle](measure-theory.md#integer-multiplication-map-on-the-circle) instead alternates between $1/3$ and $2/3$; it never visits $[0,1/4)$, the [interval](real-analysis.md#interval-mathematics) for $00$. This two-point [orbit](dynamical-systems.md#orbit-dynamical-system) is not an [equidistributed sequence](measure-theory.md#equidistributed-sequence).

### Absolutely normal number

↑ **Parent:** [Normal number](#normal-number)

An absolutely normal number is a [normal number](#normal-number) in every [integer](#integer) base $K\geq2$. This requires every finite [word](foundations-of-mathematics.md#string) in every such [positional notation](#positional-notation) to have its appropriate limiting [digit block frequency](#digit-block-frequency). Knowing base-ten normality alone does not establish [absolute normality](#absolutely-normal-number); the base is part of the statement.

Borel's 1909 result says that [absolute normality](#absolutely-normal-number) holds [almost everywhere](measure-theory.md#almost-everywhere) for [Lebesgue measure](measure-theory.md#lebesgue-measure): within $[0,1)$ the exceptions form a [Lebesgue null set](measure-theory.md#lebesgue-null-set). In particular, the [set](set.md) of [absolutely normal numbers](#absolutely-normal-number) has [Lebesgue measure](measure-theory.md#lebesgue-measure) one there. This is a statement about the size of an exceptional [set](set.md), not a test for a specified constant. [Émile Borel, Les probabilités dénombrables et leurs applications arithmétiques, 1909](https://doi.org/10.1007/BF03019651) [Bailey and Borwein, Normal Numbers and Pseudorandom Generators, 2011, introduction: simultaneous normality in all integer bases](https://www.davidhbailey.com/dhbpapers/normal-pseudo.pdf)

A modern route uses the [Birkhoff ergodic theorem](measure-theory.md#birkhoff-ergodic-theorem) and [ergodicity of integer multiplication on the circle](measure-theory.md#ergodicity-of-integer-multiplication-on-the-circle). For each fixed base and digit [interval](real-analysis.md#interval-mathematics), the time proportion equals its [Lebesgue measure](measure-theory.md#lebesgue-measure) [almost everywhere](measure-theory.md#almost-everywhere). The bases and finite [words](foundations-of-mathematics.md#string) form [countable sets](set-theory.md#countable-set), so a [countable intersection](set.md#countable-intersection) of these measure-one [sets](set.md) still has [Lebesgue measure](measure-theory.md#lebesgue-measure) one. For an [absolutely normal number](#absolutely-normal-number), the [word](foundations-of-mathematics.md#string) $11$ therefore has frequency $1/4$ in base two, $1/9$ in base three, and $1/100$ in base ten. The same symbols represent different [intervals](real-analysis.md#interval-mathematics) in different bases.

## Natural density

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Natural_density)

For a [set](set.md) $S$ of [nonnegative integers](arithmetic.md#natural-number), its natural density is the limiting proportion of the first $N$ [nonnegative integers](arithmetic.md#natural-number) that belong to $S$:

$$
d(S)=\lim_{N\to\infty}\frac{|S\cap\{0,\ldots,N-1\}|}{N},
$$

provided this [limit](calculus.md#limit-of-a-function) exists. Write $C_S(N)=|S\cap\{0,\ldots,N-1\}|$ for the counting [function](function.md). The numerator is a finite [cardinality](set-theory.md#cardinality); the denominator is exactly $N$, including zero. Every existing [natural density](#natural-density) lies between zero and one.

For the even [nonnegative integers](arithmetic.md#natural-number) $E=\{0,2,4,\ldots\}$, there are $m$ elements below $N=2m$ and $m+1$ below $N=2m+1$. Thus $C_E(N)=\lceil N/2\rceil$ using the [ceiling function](calculus.md#ceiling-function), and $d(E)=1/2$. For the [square numbers](#square-number) $Q=\{0,1,4,9,\ldots\}$, the exact count for $N\geq1$ is

$$
C_Q(N)=\lfloor\sqrt{N-1}\rfloor+1,\qquad d(Q)=0.
$$

The [floor function](calculus.md#floor-function) counts the allowed indices $1,\ldots,\lfloor\sqrt{N-1}\rfloor$, and the extra one counts zero. At $N=10$, the [square numbers](#square-number) below ten are $0,1,4,9$, so the proportion is $4/10$; at $N=100$, it is $10/100$. The count grows like the [square root](algebra.md#square-root) of $N$, while the denominator grows like $N$.

The [prime numbers](#prime-number) also have [natural density](#natural-density) zero. If $P$ is their [set](set.md), the [Prime number theorem](analytic-number-theory.md#prime-number-theorem) gives $C_P(N)\sim N/\log N$, hence $C_P(N)/N\to0$. The [Prime number theorem](analytic-number-theory.md#prime-number-theorem) is a substantial result about the count, rather than a consequence of the fact that there are infinitely many [prime numbers](#prime-number). [Andrew V. Sutherland, MIT 18.785 lecture 16, Riemann's zeta function and the prime number theorem, 2025](https://math.mit.edu/classes/18.785/2025/LectureNotes16.pdf)

Why use [natural density](#natural-density) when [cardinality](set-theory.md#cardinality) already measures size? The even [nonnegative integers](arithmetic.md#natural-number), the [square numbers](#square-number), and the [prime numbers](#prime-number) all have the same countably infinite [cardinality](set-theory.md#cardinality), yet their proportions among large initial [integer intervals](#integer-interval) differ. [Natural density](#natural-density) distinguishes frequent membership from sparse membership. Equivalently, under a [uniform distribution on a finite set](discrete-probability-distribution.md#discrete-uniform-distribution) of $N$ possible [nonnegative integers](arithmetic.md#natural-number), $C_S(N)/N$ is the [probability](probability-theory.md#probability) of landing in $S$. A [set without natural density](#set-without-natural-density) shows why this limiting proportion need not exist.

<a id="image-exact-proportions-below-n-even-integers-squares-and-an-alternating-block-set"></a>
![](natural-density-samples.png)

**[Figure 8](#image-exact-proportions-below-n-even-integers-squares-and-an-alternating-block-set). Exact proportions below N: even integers, squares, and an alternating-block set**. Every point uses the count in $\{0,\ldots,N-1\}$ divided by $N$, with zero included among the even [integers](#integer) and [square numbers](#square-number). The right panel marks exact block-boundary counts for a [set without natural density](#set-without-natural-density). Its low and high proportions approach $1/3$ and $2/3$ along different [subsequences](real-analysis.md#subsequence).

### Set without natural density

↑ **Parent:** [Natural density](#natural-density)

Include the positive [integers](#integer) in $[1,2),[4,8),[16,32),[64,128),\ldots$, and exclude the intervening [integer intervals](#integer-interval) and zero. Equivalently, include $[2^{2k},2^{2k+1})\cap\mathbb Z$ for $k\geq0$. Each included block is large enough to raise the running proportion; the following excluded block lowers it again.

With $C_A(N)=|A\cap\{0,\ldots,N-1\}|$, the exact boundary counts follow from a [geometric series](real-analysis.md#geometric-series):

$$
C_A(4^k)=\sum_{j=0}^{k-1}4^j=\frac{4^k-1}{3},\qquad C_A(2\cdot4^k)=\sum_{j=0}^k4^j=\frac{4^{k+1}-1}{3}.
$$

The first sum is empty at $k=0$. Dividing by the corresponding boundary, rather than using one denominator for both, gives

$$
\frac{C_A(4^k)}{4^k}=\frac13-\frac{1}{3\cdot4^k},\qquad\frac{C_A(2\cdot4^k)}{2\cdot4^k}=\frac23-\frac{1}{6\cdot4^k}.
$$

For example, $C_A(16)=1+4=5$, whereas $C_A(32)=1+4+16=21$, yielding proportions $5/16$ and $21/32$. For $4^k\leq N\leq2\cdot4^k$, the exact count is $(4^k-1)/3+N-4^k$; for $2\cdot4^k\leq N\leq4^{k+1}$ it stays $(4^{k+1}-1)/3$. Hence the proportion increases through each included block and decreases through each excluded block. These boundary [subsequences](real-analysis.md#subsequence) give the actual [limit inferior](real-analysis.md#limit-inferior) and [limit superior](real-analysis.md#limit-superior):

$$
\liminf_{N\to\infty}\frac{C_A(N)}N=\frac13,\qquad\limsup_{N\to\infty}\frac{C_A(N)}N=\frac23.
$$

Since these differ, $A$ has no [natural density](#natural-density). Its [upper asymptotic density](#upper-asymptotic-density) still records its largest limiting proportion.

### Upper asymptotic density

↑ **Parent:** [Natural density](#natural-density)

For a [subset](set.md#subset) $A$ of the [positive integers](#positive-integer), its upper asymptotic density is

$$
\overline d(A)=\limsup_{N\to\infty}\frac{|A\cap\{1,\ldots,N\}|}{N}.
$$

The [limit superior](real-analysis.md#limit-superior) keeps the largest limiting proportion even when the running proportions oscillate. Because they lie in $[0,1]$, this [limit superior](real-analysis.md#limit-superior) always exists in $[0,1]$. If [natural density](#natural-density) exists, [upper asymptotic density](#upper-asymptotic-density) equals it.

The convention here uses $1,\ldots,N$, while [natural density](#natural-density) above uses $0,\ldots,N-1$. Replacing one interval by the other changes a count by at most one, so the proportions differ by at most $1/N$ and have the same [limit superior](real-analysis.md#limit-superior). For the [set without natural density](#set-without-natural-density) above, the count in $\{1,\ldots,16\}$ is six rather than five, because $16$ is included and zero is absent. Nevertheless its [upper asymptotic density](#upper-asymptotic-density) is exactly $2/3$. The even [positive integers](#positive-integer) have [upper asymptotic density](#upper-asymptotic-density) $1/2$ and the [prime numbers](#prime-number) have [upper asymptotic density](#upper-asymptotic-density) zero.

The useful feature is that a large proportion along arbitrarily large initial [integer intervals](#integer-interval) already supplies structure. The [Szemerédi theorem](probabilistic-combinatorics.md#szemeredi-s-theorem) says that positive [upper asymptotic density](#upper-asymptotic-density) forces [arithmetic progressions](arithmetic.md#arithmetic-progression) of every finite length, with positive common difference, even without an existing [natural density](#natural-density). Szemerédi's 1975 paper resolved this general finite-length problem; it makes density a bridge from counting to additive structure. [Endre Szemerédi, On sets of integers containing k elements in arithmetic progression, Acta Arithmetica 27, 199–245, 1975](https://doi.org/10.4064/aa-27-1-199-245)

### Full-density sequence

↑ **Parent:** [Natural density](#natural-density)

An increasing sequence of integers has full density when its range has [natural density](#natural-density) one. [Convergence in density of a sequence](measure-theory.md#convergence-in-density-of-a-sequence) means that, for each fixed tolerance, the exceptional indices have [natural density](#natural-density) zero.

<h2 id="lagrange-s-four-square-theorem">Lagrange's four-square theorem</h2>

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Lagrange's_four-square_theorem)

**Every [nonnegative integer](arithmetic.md#natural-number) is a [sum of squares](arithmetic.md#sum-of-squares) with four terms, with zero terms allowed.** Precisely, for every [integer](#integer) $n\geq0$, there exist [nonnegative integers](arithmetic.md#natural-number) $a,b,c,d$ such that

$$
n=a^2+b^2+c^2+d^2.
$$

Allowing arbitrary [integer](#integer) roots gives the same statement: changing a root to its [absolute value](real-analysis.md#absolute-value) leaves the resulting [square number](#square-number) unchanged. Four is a uniform upper bound on the number of nonzero terms, rather than a demand for four positive terms. Repeated [square numbers](#square-number) are allowed. Conrad states the positive case and explicitly explains the role of zero terms; $n=0$ follows by taking all four roots zero. [Keith Conrad, Proofs by Descent, Section 6, opening paragraph and Theorem 6.6](https://kconrad.math.uconn.edu/blurbs/ugradnumthy/descent.pdf)

The small cases make the convention visible:

$$
\begin{aligned}
0&=0^2+0^2+0^2+0^2,\\
1&=1^2+0^2+0^2+0^2,\\
2&=1^2+1^2+0^2+0^2,\\
3&=1^2+1^2+1^2+0^2,\\
7&=2^2+1^2+1^2+1^2.
\end{aligned}
$$

In particular, $1$ could not be a [sum of squares](arithmetic.md#sum-of-squares) with four strictly positive roots, since each term would be at least one. Geometrically, a [square](geometry-and-topology.md#square) of [integer](#integer) side length $a$ has [area](differential-geometry.md#surface-area) $a^2$: the theorem says that any nonnegative whole-number total area can be split into at most four such square areas. It does not assert that those [squares](geometry-and-topology.md#square) tile one larger [square](geometry-and-topology.md#square) or a prescribed [rectangle](geometry-and-topology.md#rectangle).

<a id="image-four-square-representations-as-areas-counted-in-unit-cells"></a>
![](four-square-areas.png)

**[Figure 9](#image-four-square-representations-as-areas-counted-in-unit-cells). Four-square representations as areas counted in unit cells**. The roots for $7,23,28,31$ were found by enumerating nonnegative four-tuples. Each panel has the same unit length, and each little cell has [area](differential-geometry.md#surface-area) one. The four separate [squares](geometry-and-topology.md#square) illustrate addition of areas, with no claim about tiling a prescribed shape. These are exact arithmetic examples, not measured data.

Why does the fourth term matter? Two [square numbers](#square-number) do not suffice for $3$: in [modular arithmetic](#modular-arithmetic), a [square number](#square-number) has [remainder](#remainder) zero or one modulo four, so their sum cannot be three modulo four. The [sum of two squares theorem](#sum-of-two-squares-theorem) gives a complete criterion for the positive [integers](#integer) representable with two terms. Even three terms leave gaps. A [square number](#square-number) has [remainder](#remainder) $0,1,$ or $4$ modulo eight; adding three of these, with repetition allowed, never gives seven modulo eight. Thus $7,15,23,31,\ldots$ cannot be sums of three [square numbers](#square-number), although [Lagrange's four-square theorem](#lagrange-s-four-square-theorem) represents all of them with four. This also proves that the bound four cannot be reduced to three.

The modulo-eight obstruction is not the only way that three terms can fail. For example, $28$ needs four: if three [square numbers](#square-number) added to $28$, their [remainders](#remainder) modulo four would force all three roots even. Dividing by four would then express $7$ as a sum of three [square numbers](#square-number), contradicting the preceding calculation. These short checks explain the examples without requiring a full classification of sums of three [square numbers](#square-number).

<a id="image-minimum-number-of-nonzero-square-terms-for-integers-from-one-to-one-hundred"></a>
![](four-square-minima.png)

**[Figure 10](#image-minimum-number-of-nonzero-square-terms-for-integers-from-one-to-one-hundred). Minimum number of nonzero square terms for integers from one to one hundred**. Each cell is labelled by the [positive integer](#positive-integer) being represented; its colour records the least number of nonzero [square numbers](#square-number) whose sum equals it. Direct enumeration gives $10$ requiring one term, $33$ two, $42$ three, and $15$ four. Zero is omitted from the grid and requires no nonzero terms. Zero padding converts every representation into four slots. This finite computation illustrates [Lagrange's four-square theorem](#lagrange-s-four-square-theorem); it does not prove its assertion for all [nonnegative integers](arithmetic.md#natural-number).

The practical benefit of [Lagrange's four-square theorem](#lagrange-s-four-square-theorem) is an existence guarantee for a family of [Diophantine equations](#diophantine-equation): for every [nonnegative integer](arithmetic.md#natural-number) $n$, the displayed [equation](algebra.md#equation) has an [integer](#integer) solution. It does not specify a unique solution. For instance, $65=8^2+1^2+0^2+0^2=7^2+4^2+0^2+0^2=6^2+4^2+3^2+2^2$. To find a representation by a finite search, enumerate $0\leq d\leq c\leq b\leq a\leq\lfloor\sqrt n\rfloor$ and test the sum. The [floor function](calculus.md#floor-function) supplies a finite bound because no single term can exceed $n$, and sorting roots removes duplicate orderings without discarding any possible sum. The theorem guarantees that the search succeeds.

A [greedy algorithm](computer-science.md#greedy-algorithm) that repeatedly subtracts the largest available [square number](#square-number) need not find four terms: for $23$ it chooses $16+4+1+1+1$, while $23=9+9+4+1$ uses four. The appeal of the theorem is this gap between local choices and a global promise: individual [square numbers](#square-number) become farther apart, and two or three terms leave arithmetic obstructions, yet four terms cover every [nonnegative integer](arithmetic.md#natural-number).

For historical orientation, Conrad dates [Lagrange's four-square theorem](#lagrange-s-four-square-theorem) to $1770$ and identifies the memoir as _Démonstration d'un théorème d'arithmétique_: it appeared in the Berlin Academy's volume for the year $1770$, published in $1772$, pages $123$–$133$. Keeping the volume year and publication year distinct avoids an apparent conflict between dates. [Keith Conrad, Proofs by Descent, Theorem 6.6 and reference 11](https://kconrad.math.uconn.edu/blurbs/ugradnumthy/descent.pdf)

## Arithmetic function

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Arithmetic_function)

An [arithmetic function](#arithmetic-function) is a [function](function.md) whose [domain of a function](function.md#domain-of-a-function) is the [positive integers](#positive-integer), usually taking values in the [complex numbers](complex-analysis.md#complex-number). Thus $f(1),f(2),\ldots$ are its values; $f(0)$ is outside this [domain of a function](function.md#domain-of-a-function). Examples include the [divisor function](#divisor-function), with $\tau(12)=6$, and the [sum-of-divisors function](#sum-of-divisors-function), with $\sigma_1(12)=28$. Studying an [arithmetic function](#arithmetic-function) packages a question about each [positive integer](#positive-integer) into one object whose values can be combined using [Dirichlet convolution](#dirichlet-convolution). [Darij Grinberg, MIT 18.781 lecture notes, Section 2.1: arithmetic functions](https://darijgrinberg.gitlab.io/floor.pdf)

### Radical of an integer

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Radical_of_an_integer)

The [radical of an integer](#radical-of-an-integer) $n>0$ is the [product](arithmetic.md#product-of-numbers) of its distinct [prime factors](#prime-factor), each included exactly once. If the [prime factorization](#fundamental-theorem-of-arithmetic) is $n=p_1^{a_1}\cdots p_r^{a_r}$ with distinct [prime numbers](#prime-number) $p_i$ and positive [integer](#integer) exponents $a_i$, then

$$
\operatorname{rad}(n)=p_1\cdots p_r=\prod_{p\mid n}p.
$$

Thus the [radical of an integer](#radical-of-an-integer) remembers which [prime factors](#prime-factor) occur and forgets their [prime valuations](#prime-valuation). At $n=1$, the [empty product](arithmetic.md#empty-product) gives $\operatorname{rad}(1)=1$. The [domain of a function](function.md#domain-of-a-function) here is the [positive integers](#positive-integer); zero is excluded. [Jan-Hendrik Evertse, Diophantine approximation, Homework IV, Exercise 20: definition of the integer radical](https://pub.math.leidenuniv.nl/~evertsejh/dio12-ex4.pdf)

For example, $72=2^3\cdot3^2$ has distinct [prime factors](#prime-factor) $2,3$, so $\operatorname{rad}(72)=2\cdot3=6$. Similarly,

$$
\operatorname{rad}(30)=30,\qquad
\operatorname{rad}(32)=2,\qquad
\operatorname{rad}(36)=6,
$$

using the [prime factorizations](#fundamental-theorem-of-arithmetic) $30=2\cdot3\cdot5$, $32=2^5$ and $36=2^2\cdot3^2$. The [prime omega function](#prime-omega-function) counts the retained [prime factors](#prime-factor), while the [total number of prime factors](#total-number-of-prime-factors) counts their occurrences before repetitions are removed.

The [radical of an integer](#radical-of-an-integer) is its largest [squarefree divisor](#squarefree-divisor). Indeed, a [squarefree divisor](#squarefree-divisor) chooses at most one copy of each [prime factor](#prime-factor), so it divides $\operatorname{rad}(n)$; the [radical of an integer](#radical-of-an-integer) itself is a [squarefree divisor](#squarefree-divisor). Consequently,

$$
\operatorname{rad}(n)\mid n,\qquad
\operatorname{rad}(n)\le n,\qquad
\operatorname{rad}(n)=n\ \Longleftrightarrow\ n\text{ is squarefree}.
$$

The last statement follows because every nonzero [prime valuation](#prime-valuation) is then one. It includes $n=1$, a [squarefree integer](#squarefree-integer). Applying the [radical of an integer](#radical-of-an-integer) twice also changes nothing: $\operatorname{rad}(\operatorname{rad}(n))=\operatorname{rad}(n)$.

<a id="image-the-radical-of-an-integer-for-1-le-n-le60-squarefree-integers-lie-on-the-diagonal-and-horizontal-families-share-their-prime-support-of-an-integer"></a>
![](integer-radicals-prime-support.png)

**[Figure 11](#image-the-radical-of-an-integer-for-1-le-n-le60-squarefree-integers-lie-on-the-diagonal-and-horizontal-families-share-their-prime-support-of-an-integer). The radical of an integer for $1\le n\le60$: squarefree integers lie on the diagonal, and horizontal families share their prime support of an integer**.

For any [positive integers](#positive-integer) $a,b$, the exact [product](arithmetic.md#product-of-numbers) rule is

$$
\operatorname{rad}(ab)=\frac{\operatorname{rad}(a)\operatorname{rad}(b)}{\operatorname{rad}(\gcd(a,b))}.
$$

To prove it, a [prime factor](#prime-factor) dividing just one input occurs once in the numerator and not in the denominator. A [prime factor](#prime-factor) dividing both occurs twice in the numerator and once in the denominator, since it divides their [greatest common divisor](#greatest-common-divisor). Each [prime factor](#prime-factor) of $ab$ therefore remains exactly once. For [coprime integers](#coprime-integers), the denominator is $\operatorname{rad}(1)=1$, proving the [radical of an integer](#radical-of-an-integer) is a [multiplicative function](#multiplicative-function). It is not a [completely multiplicative function](#completely-multiplicative-function): $\operatorname{rad}(4)=2\ne4=\operatorname{rad}(2)^2$.

For a worked example with shared [prime factors](#prime-factor), take $a=12$ and $b=18$. Their [greatest common divisor](#greatest-common-divisor) is $6$, and $ab=216=2^3\cdot3^3$, so

$$
\operatorname{rad}(216)=\frac{6\cdot6}{6}=6.
$$

This explains why [prime support of an integer](#prime-support-of-an-integer) is useful: questions about the presence of [prime factors](#prime-factor) can discard their multiplicities. For example, the [squarefree divisors](#squarefree-divisor) of $72$ are exactly the [integer divisors](#divisor) of $\operatorname{rad}(72)=6$, namely $1,2,3,6$. Also $\gcd(m,n)=1$ if and only if $\gcd(m,\operatorname{rad}(n))=1$, because [coprimality](#coprime-integers) depends only on shared [prime factors](#prime-factor).

A further characterization uses mutual [divisibility](#divisibility) of powers: for [positive integers](#positive-integer) $a,b$,

$$
\operatorname{rad}(a)=\operatorname{rad}(b)
\quad\Longleftrightarrow\quad
\text{there exist }k,\ell\ge1\text{ with }a\mid b^k\text{ and }b\mid a^\ell.
$$

If their [prime supports of an integer](#prime-support-of-an-integer) agree, sufficiently large $k,\ell$ make all the required [prime valuations](#prime-valuation) large enough. Conversely, these two [divisibility](#divisibility) relations force each [prime factor](#prime-factor) of either input to divide the other. For $72$ and $36$, one can take $k=2$ and $\ell=1$: $72\mid36^2$ and $36\mid72$.

#### Prime support of an integer

↑ **Parent:** [Radical of an integer](#radical-of-an-integer)

The [prime support of an integer](#prime-support-of-an-integer) $n>0$ is the [finite set](set.md#finite-set) of its distinct [prime factors](#prime-factor). For example, $P(72)=P(36)=\{2,3\}$, $P(30)=\{2,3,5\}$ and $P(1)$ is the [empty set](set.md#empty-set). Its [cardinality](set-theory.md#cardinality) is the [prime omega function](#prime-omega-function) $\omega(n)$, and the [product](arithmetic.md#product-of-numbers) of its elements is the [radical of an integer](#radical-of-an-integer) $\operatorname{rad}(n)$. These are two different ways to summarize the same [finite set](set.md#finite-set): a count and a [product](arithmetic.md#product-of-numbers).

### Total number of prime factors

↑ **Parent:** [Arithmetic function](#arithmetic-function)

The [total number of prime factors](#total-number-of-prime-factors) $\Omega(n)$ counts every occurrence of a [prime factor](#prime-factor) in the [prime factorization](#fundamental-theorem-of-arithmetic) of a [positive integer](#positive-integer) $n$. Equivalently, it adds the [prime valuations](#prime-valuation):

$$
n=p_1^{a_1}\cdots p_r^{a_r}
\quad\Longrightarrow\quad
\Omega(n)=a_1+\cdots+a_r=\sum_{p\mid n}v_p(n).
$$

One may also write $\Omega(n)=\sum_p v_p(n)$ over all [prime numbers](#prime-number), since only finitely many [prime valuations](#prime-valuation) are nonzero. The [empty sum](arithmetic.md#empty-sum) gives $\Omega(1)=0$. By contrast, the [prime omega function](#prime-omega-function) has $\omega(n)=r$ and counts distinct [prime factors](#prime-factor). [Darij Grinberg, MIT 18.781, Floor and arithmetic functions, Definition 2.1.2: the two prime-factor counts](https://darijgrinberg.gitlab.io/floor.pdf)

Expanding $72=2^3\cdot3^2$ into $2\cdot2\cdot2\cdot3\cdot3$ shows $\Omega(72)=3+2=5$, whereas $\omega(72)=2$ and $\operatorname{rad}(72)=6$. The same calculation for the comparison examples gives

$$
\begin{array}{c|c|c|c|c}
n&\text{prime factorization}&\operatorname{rad}(n)&\omega(n)&\Omega(n)\\\hline
1&\text{empty product}&1&0&0\\
72&2^3\cdot3^2&6&2&5\\
30&2\cdot3\cdot5&30&3&3\\
32&2^5&2&1&5\\
36&2^2\cdot3^2&6&2&4
\end{array}
$$

The [total number of prime factors](#total-number-of-prime-factors) agrees for $72$ and $32$, although their [prime supports of an integer](#prime-support-of-an-integer) differ. Meanwhile $72$ and $36$ have the same [radical of an integer](#radical-of-an-integer) and [prime omega function](#prime-omega-function), but different values of the [total number of prime factors](#total-number-of-prime-factors). These examples show exactly which information each [arithmetic function](#arithmetic-function) forgets.

<a id="image-one-box-per-prime-factor-occurrence-the-total-number-of-prime-factors-counts-boxes-the-prime-omega-function-counts-groups-and-the-radical-of-an-integer-multiplies-one-prime-number-from-each-group"></a>
![](prime-factor-multiplicity-comparison.png)

**[Figure 12](#image-one-box-per-prime-factor-occurrence-the-total-number-of-prime-factors-counts-boxes-the-prime-omega-function-counts-groups-and-the-radical-of-an-integer-multiplies-one-prime-number-from-each-group). One box per prime factor occurrence: the total number of prime factors counts boxes, the prime omega function counts groups, and the radical of an integer multiplies one prime number from each group**.

The [total number of prime factors](#total-number-of-prime-factors) is a [completely additive arithmetic function](#completely-additive-arithmetic-function):

$$
\Omega(ab)=\Omega(a)+\Omega(b)\qquad(a,b\ge1).
$$

The proof is that [multiplication](arithmetic.md#multiplication) adds each [prime valuation](#prime-valuation), $v_p(ab)=v_p(a)+v_p(b)$, and summing preserves that equality. No [coprimality](#coprime-integers) condition is needed. For example, $12=2^2\cdot3$ and $18=2\cdot3^2$ both have [total number of prime factors](#total-number-of-prime-factors) three; their [product](arithmetic.md#product-of-numbers) $216=2^3\cdot3^3$ has six. By comparison, the [prime omega function](#prime-omega-function) is only an [additive arithmetic function](#additive-function-number-theory): here $\omega(216)=2\ne4=\omega(12)+\omega(18)$.

There is a useful way to see the [total number of prime factors](#total-number-of-prime-factors) as a count of elementary building blocks: any expression of $n$ as a [product](arithmetic.md#product-of-numbers) of [prime numbers](#prime-number) has exactly $\Omega(n)$ factors, by the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). Equivalently, every [factorization tree](#factorization-tree) for $n>1$ has $\Omega(n)$ leaves. Repeated [prime factors](#prime-factor) increase this count without introducing new kinds of [prime number](#prime-number). The difference is the existing [excess prime-factor multiplicity](#excess-prime-factor-multiplicity):

$$
\Omega(n)-\omega(n)=\sum_{p\mid n}\bigl(v_p(n)-1\bigr)\ge0.
$$

Every summand is nonnegative, so $\Omega(n)=\omega(n)$ if and only if $n$ is a [squarefree integer](#squarefree-integer), including $n=1$. In particular, a [prime power](#prime-power) $p^k$ with $k\ge1$ has $\Omega(p^k)=k$, $\omega(p^k)=1$ and $\operatorname{rad}(p^k)=p$.

Historically, Hardy and Ramanujan's 1917 paper explicitly separated the [prime omega function](#prime-omega-function) from the [total number of prime factors](#total-number-of-prime-factors), writing them as $f(n)$ and $F(n)$, respectively. Their example $2^3\cdot3^2\cdot5$ has counts three and six. That distinction let them compare two measures of how an [integer](#integer) is built from [prime factors](#prime-factor). [G. H. Hardy and S. Ramanujan, The normal number of prime factors of a number n, Quarterly Journal of Mathematics 48 (1917), 76–92, Section 1.2, transcribed original text](https://ramanujan.sirinudi.org/Volumes/published/ram35.html)

#### Excess prime-factor multiplicity

↑ **Parent:** [Total number of prime factors](#total-number-of-prime-factors)

The nonnegative [arithmetic function](#arithmetic-function) $\Omega(n)-\omega(n)$ counts the repeated occurrences beyond the first of each [prime factor](#prime-factor). Its [expectation](probability-theory.md#expected-value) under uniform sampling from $[N]$ is bounded by $\sum_p1/(p(p-1))\le1$, independently of $N$.

### Additive function (number theory)

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Additive_function)

An [arithmetic function](#arithmetic-function) $f$ is additive when $f(mn)=f(m)+f(n)$ for [coprime integers](#coprime-integers) $m,n$. Equivalently, $f(n)=\sum_{p^k\parallel n}f(p^k)$. This concerns multiplication of integers, and differs from an [additive function](analysis.md#additive-function) on a vector space.

#### Mean of an additive arithmetic function

↑ **Parent:** [Additive function (number theory)](#additive-function-number-theory)

For an [additive arithmetic function](#additive-function-number-theory), the model mean is $A_f(x)=\sum_{p^k\le x}f(p^k)(1-1/p)/p^k$. The exact uniform [expectation](probability-theory.md#expected-value) differs by $O(x^{-1}\sum_{p^k\le x}|f(p^k)|)$.

#### Strongly additive arithmetic function

↑ **Parent:** [Additive function (number theory)](#additive-function-number-theory)

A [strongly additive arithmetic function](#strongly-additive-arithmetic-function) satisfies $f(p^k)=f(p)$ for every [prime](#prime-number) $p$ and $k\ge1$, so $f(n)=\sum_{p\mid n}f(p)$. The [prime omega function](#prime-omega-function) is an example.

#### Completely additive arithmetic function

↑ **Parent:** [Additive function (number theory)](#additive-function-number-theory)

A [completely additive arithmetic function](#completely-additive-arithmetic-function) satisfies $f(mn)=f(m)+f(n)$ for all positive $m,n$, equivalently $f(p^k)=k f(p)$. The [total number of prime factors](#total-number-of-prime-factors) is an example.

### Multiplicative function

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplicative_function)

An [arithmetic function](#arithmetic-function) $f$ is a [multiplicative function](#multiplicative-function) when $f(1)=1$ and $f(mn)=f(m)f(n)$ for all [coprime integers](#coprime-integers) $m,n>0$, meaning their [greatest common divisor](#greatest-common-divisor) is $1$. The condition $f(1)=1$ excludes the identically zero [function](function.md). This definition makes no assertion about a pair whose [greatest common divisor](#greatest-common-divisor) exceeds $1$. [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.2.1](https://darijgrinberg.gitlab.io/floor.pdf)

For the [divisor function](#divisor-function), the [integer divisors](#divisor) of $2$ are $1,2$, those of $3$ are $1,3$, and those of $6$ are $1,2,3,6$. Hence

$$
\tau(6)=4=\tau(2)\tau(3)=2\cdot2.
$$

Here $2$ and $3$ are [coprime integers](#coprime-integers). In contrast, $\tau(4)=3\ne4=\tau(2)^2$, because the [integer divisors](#divisor) of $4$ are $1,2,4$. Thus the [divisor function](#divisor-function) is a [multiplicative function](#multiplicative-function) but not a [completely multiplicative function](#completely-multiplicative-function).

The practical gain is that [prime factorization](#fundamental-theorem-of-arithmetic) reduces all values to values at [prime powers](#prime-power). For distinct [prime numbers](#prime-number) $p_1,\ldots,p_r$ and positive exponents $a_1,\ldots,a_r$,

$$
n=\prod_{k=1}^r p_k^{a_k}\quad\Longrightarrow\quad f(n)=\prod_{k=1}^r f(p_k^{a_k}).
$$

For instance, $f(12)=f(4)f(3)$ since $4$ and $3$ are [coprime integers](#coprime-integers); replacing $f(4)$ by $f(2)^2$ additionally requires a [completely multiplicative function](#completely-multiplicative-function). The short proof repeatedly applies the defining rule to [prime powers](#prime-power) belonging to different [prime numbers](#prime-number), which are [coprime integers](#coprime-integers).

#### Multiplicativity of an arithmetic function

↑ **Parent:** [Multiplicative function](#multiplicative-function)

For an [arithmetic function](#arithmetic-function), [multiplicativity](#multiplicativity-of-an-arithmetic-function) means $f(1)=1$ and $f(mn)=f(m)f(n)$ whenever $m,n$ are positive [coprime integers](#coprime-integers). It allows values of an [arithmetic function](#arithmetic-function) to be assembled from its values on [prime powers](#prime-power), as explained under [multiplicative function](#multiplicative-function).

#### Completely multiplicative function

↑ **Parent:** [Multiplicative function](#multiplicative-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Completely_multiplicative_function)

An [arithmetic function](#arithmetic-function) $f$ is a [completely multiplicative function](#completely-multiplicative-function) when $f(1)=1$ and $f(mn)=f(m)f(n)$ for every pair of [positive integers](#positive-integer) $m,n$. In particular $f(p^a)=f(p)^a$ for every [prime number](#prime-number) $p$ and every nonnegative exponent $a$. Both the [constant-one arithmetic function](#constant-one-arithmetic-function) and the [identity arithmetic function](#identity-arithmetic-function) are [completely multiplicative functions](#completely-multiplicative-function): $\mathbf1(mn)=1=1\cdot1$ and $\operatorname{id}(mn)=mn=\operatorname{id}(m)\operatorname{id}(n)$. The [divisor function](#divisor-function) fails this stronger condition at $m=n=2$.

#### Divisor sum

↑ **Parent:** [Multiplicative function](#multiplicative-function)

The [divisor sum](#divisor-sum) of an [arithmetic function](#arithmetic-function) $f$ assigns to each [positive integer](#positive-integer) $n$ the [sum](arithmetic.md#sum)

$$
F(n)=\sum_{d\mid n}f(d).
$$

Only positive [integer divisors](#divisor) are included, so $F(1)=f(1)$. The weights $f(d)$ can count the [integer divisors](#divisor), measure their sizes, or record other arithmetic information: the [constant-one arithmetic function](#constant-one-arithmetic-function) gives the [divisor function](#divisor-function), whereas the [identity arithmetic function](#identity-arithmetic-function) gives the [sum-of-divisors function](#sum-of-divisors-function).

Equivalently, $F=f*\mathbf1$, where $*$ is [Dirichlet convolution](#dirichlet-convolution) and $\mathbf1$ is the [constant-one arithmetic function](#constant-one-arithmetic-function). If $f$ is a [multiplicative function](#multiplicative-function), then $F$ is a [multiplicative function](#multiplicative-function) by [Multiplicativity of Dirichlet convolution](#multiplicativity-of-dirichlet-convolution). [Darij Grinberg, MIT 18.781 notes on floor and arithmetic functions, Proposition 2.4.2 and Theorem 2.6.1](https://darijgrinberg.gitlab.io/floor.pdf)

Here is the mechanism. For positive [coprime integers](#coprime-integers) $m,n$, every positive [integer divisor](#divisor) of $mn$ has a unique form $ab$ with $a\mid m$ and $b\mid n$; moreover, $a,b$ are [coprime integers](#coprime-integers). Thus a [multiplicative function](#multiplicative-function) satisfies

$$
F(mn)=\sum_{a\mid m}\sum_{b\mid n}f(a)f(b)=F(m)F(n).
$$

At a [prime power](#prime-power), the [divisor sum](#divisor-sum) becomes $F(p^a)=f(1)+f(p)+\cdots+f(p^a)$. This turns a calculation over many [integer divisors](#divisor) into short local calculations at [prime powers](#prime-power).

##### Sum-of-divisors function

↑ **Parent:** [Divisor sum](#divisor-sum)

The [sum-of-divisors function](#sum-of-divisors-function) adds all positive [integer divisors](#divisor) of a [positive integer](#positive-integer), including the number itself:

$$
\sigma(n)=\sigma_1(n)=\sum_{d\mid n}d,\qquad \sigma(1)=1.
$$

It is the [divisor sum](#divisor-sum) of the [identity arithmetic function](#identity-arithmetic-function) $\operatorname{id}(n)=n$, so $\sigma=\operatorname{id}*\mathbf1$ under [Dirichlet convolution](#dirichlet-convolution). Both factors are [multiplicative functions](#multiplicative-function), hence so is the [sum-of-divisors function](#sum-of-divisors-function). The notation $\sigma_1$ distinguishes it from other weighted [divisor sums](#divisor-sum). [Darij Grinberg, MIT 18.781 notes, Definition 2.1.2 and Proposition 2.2.2(e)](https://darijgrinberg.gitlab.io/floor.pdf)

For a [prime number](#prime-number) $p$ and a nonnegative exponent $a$, the positive [integer divisors](#divisor) of the [prime power](#prime-power) $p^a$ are precisely $1,p,\ldots,p^a$. Their [finite geometric series](real-analysis.md#finite-geometric-series) gives

$$
\sigma(p^a)=1+p+\cdots+p^a=\frac{p^{a+1}-1}{p-1}.
$$

For example, $\sigma(8)=1+2+4+8=15=(2^4-1)/(2-1)$. For a [prime factorization](#fundamental-theorem-of-arithmetic) $n=\prod_{k=1}^r p_k^{a_k}$ with distinct [prime numbers](#prime-number) $p_k$ and positive exponents $a_k$, [multiplicativity](#multiplicativity-of-an-arithmetic-function) gives

$$
\sigma(n)=\prod_{k=1}^r(1+p_k+\cdots+p_k^{a_k})=\prod_{k=1}^r\frac{p_k^{a_k+1}-1}{p_k-1}.
$$

For $n=1$, this is an [empty product](arithmetic.md#empty-product), equal to $1$. [Darij Grinberg, MIT 18.781 notes, Theorem 2.1.8 with k equal to one](https://darijgrinberg.gitlab.io/floor.pdf)

The [distributive property](algebra.md#distributive-property) makes the formula especially beautiful: choosing one term from each factor produces each positive [integer divisor](#divisor) exactly once, by the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). For $12=4\cdot3=2^2\cdot3$, the choices form a three-by-two grid with entries $2^i3^j$, where $0\le i\le2$ and $0\le j\le1$. Adding its rows gives

$$
\sigma(12)=(1+2+4)+(3+6+12)=(1+2+4)(1+3)=7\cdot4=28.
$$

The [divisor function](#divisor-function) counts six cells; the [sum-of-divisors function](#sum-of-divisors-function) adds their six values. Once the [prime factorization](#fundamental-theorem-of-arithmetic) is known, the product formula avoids testing every candidate [integer divisor](#divisor). Shared [prime factors](#prime-factor) require care: $\sigma(4)=7\ne9=\sigma(2)^2$, so the [sum-of-divisors function](#sum-of-divisors-function) is not a [completely multiplicative function](#completely-multiplicative-function).

<a id="image-the-sum-of-divisors-function-for-12-each-grid-entry-is-a-positive-integer-divisor-and-the-weighted-total-is-1-plus-2-plus-4-1-plus-3-28"></a>
![](divisor-sum-prime-factor-grid.png)

**[Figure 13](#image-the-sum-of-divisors-function-for-12-each-grid-entry-is-a-positive-integer-divisor-and-the-weighted-total-is-1-plus-2-plus-4-1-plus-3-28). The sum-of-divisors function for $12$: each grid entry is a positive integer divisor, and the weighted total is $(1+2+4)(1+3)=28$**.

Subtracting the number itself gives the [proper-divisor sum](#proper-divisor-sum) $s(n)=\sigma(n)-n$. Comparing $s(n)$ with $n$ distinguishes [perfect numbers](#perfect-number), [deficient numbers](#deficient-number), and [abundant numbers](#abundant-number). For $6$, $s(6)=1+2+3=6$; for $28$, $s(28)=1+2+4+7+14=28$. Both are [perfect numbers](#perfect-number). The calculation $s(8)=1+2+4=7<8$ makes $8$ a [deficient number](#deficient-number), while $s(12)=1+2+3+4+6=16>12$ makes $12$ an [abundant number](#abundant-number). These comparisons turn the sizes of [integer divisors](#divisor) into a classification of [positive integers](#positive-integer). [Western Carolina University, Challenge Problem: Perfect Numbers, hosted by MIT OpenCourseWare](https://ocw.mit.edu/courses/ec-s01-internet-technology-in-local-and-global-communities-spring-2005-summer-2005/aac0b504648aff57a83daec957da3a58_MITEC_S01S05_perf_numb.pdf)

<a id="image-the-proper-divisor-sum-for-1-le-n-le30-perfect-numbers-lie-on-s-n-n-deficient-numbers-below-it-and-abundant-numbers-above-it"></a>
![](proper-divisor-sum-classification.png)

**[Figure 14](#image-the-proper-divisor-sum-for-1-le-n-le30-perfect-numbers-lie-on-s-n-n-deficient-numbers-below-it-and-abundant-numbers-above-it). The proper-divisor sum for $1\le n\le30$: perfect numbers lie on $s(n)=n$, deficient numbers below it, and abundant numbers above it**.

This connection is ancient: [Euclid's Elements](geometry-and-topology.md#euclid-s-elements), Book IX, Proposition 36, constructs a [perfect number](#perfect-number) by multiplying the last term of $1,2,\ldots,2^{k-1}$ by their [sum](arithmetic.md#sum), when that [sum](arithmetic.md#sum) is a [prime number](#prime-number). In modern notation, put $q=2^k-1$ and $N=2^{k-1}q$, with $k\ge2$ and $q$ a [prime number](#prime-number). The [sum-of-divisors function](#sum-of-divisors-function) proves the construction immediately:

$$
\sigma(N)=(2^k-1)(1+q)=q\,2^k=2N.
$$

Consequently the [proper-divisor sum](#proper-divisor-sum) is $s(N)=N$. Taking $k=2,3$ produces the [perfect numbers](#perfect-number) $6,28$. [Euclid, Elements IX.36, translated text and commentary by David Joyce](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX36.html)

###### Proper-divisor sum

↑ **Parent:** [Sum-of-divisors function](#sum-of-divisors-function)

The [proper-divisor sum](#proper-divisor-sum), or [aliquot sum](#proper-divisor-sum), adds the positive [proper divisors](#proper-divisor):

$$
s(n)=\sum_{\substack{d\mid n\\d<n}}d=\sigma(n)-n.
$$

In particular $s(1)=0$, an [empty sum](arithmetic.md#empty-sum). Removing $n$ from the [sum-of-divisors function](#sum-of-divisors-function) is essential: $\sigma(6)=12$, but its [proper-divisor sum](#proper-divisor-sum) is $6$.

#### Pretentious distance

↑ **Parent:** [Multiplicative function](#multiplicative-function)

For multiplicative functions bounded by one, the pretentious distance up to $x$ is defined by

$$
\mathbb D(f,g;x)^2
=\sum_{p\leq x}\frac{1-\Re(f(p)\overline{g(p)})}{p}.
$$

It measures how similarly $f$ and $g$ behave on primes.

##### Large Fourier coefficient criterion for pretentiousness

↑ **Parent:** [Pretentious distance](#pretentious-distance)

Let $X\geq3$, and let $f$ be a normalized [multiplicative arithmetic function](#multiplicative-function) supported on [squarefree integers](#squarefree-integer), with $|f(p)|\leq1$. Form the [finite measure](measure-theory.md#finite-measure) $\nu=\sum_n f(n)n^{-1-1/\log X}\delta_{\log n}$ using [Dirac measures](measure-theory.md#dirac-measure). Under the transform convention $\widehat\nu(t)=\int e^{-itu}\,d\nu(u)$, its [Euler product](analytic-number-theory.md#euler-product) is $\prod_p(1+f(p)p^{-1-1/\log X-it})$. Expanding its logarithmic modulus, and replacing the damped [prime](#prime-number) weights by $1/p$ up to $X$ with [Mertens first theorem](analytic-number-theory.md#mertens-first-theorem), gives the displayed absolute bound, uniformly in real $t$. Hence $|\widehat\nu(t)|\geq\delta\log X$ forces $D(f,n^{it};X)^2\leq\log(C/\delta)$. The distance expression still defines a nonnegative pretentious score for [prime](#prime-number) values bounded by one; its actual [metric](topological-analysis.md#metric) interpretation uses unit-modulus values.

<h5 id="pretentious-distance-between-one-and-the-mobius-function">Pretentious distance between one and the Möbius function</h5>

↑ **Parent:** [Pretentious distance](#pretentious-distance)

Because $\mu(p)=-1$, the squared [pretentious distance](#pretentious-distance) from one to the [Möbius function](#mobius-function) is twice the reciprocal-prime sum. The [Mertens second theorem](analytic-number-theory.md#mertens-second-theorem) therefore gives $D(1,\mu;X)^2=2\log\log X+2B_1+o(1)$. In particular the distance diverges, illustrating that a multiplicative function can be far from the constant function even though both have unit-modulus [prime](#prime-number) values.

##### Prime-restriction metric for pretentious distance

↑ **Parent:** [Pretentious distance](#pretentious-distance)

For unit-modulus [prime](#prime-number) values, [pretentious distance](#pretentious-distance) is the Euclidean [metric](topological-analysis.md#metric) on the finite vectors $(f(p)/\sqrt{2p})_{p\leq X}$. On whole [arithmetic functions](#arithmetic-function) it is only a [pseudometric](topological-analysis.md#pseudometric): it sees neither values on [prime powers](#prime-power) nor [primes](#prime-number) above the cutoff. Even for every cutoff, the functions one and $\mu^2$ have distance zero but differ on nonsquarefree integers. The [norm](functional-analysis.md#norm) representation proves the [triangle inequality](topological-analysis.md#triangle-inequality) and identifies exactly the quotient on which separation holds.

##### Triangle inequality for pretentious distance

↑ **Parent:** [Pretentious distance](#pretentious-distance)

The pretentious distance obeys

$$
\mathbb D(f_1f_2,g_1g_2;x)
\leq\mathbb D(f_1,g_1;x)+\mathbb D(f_2,g_2;x).
$$

##### Archimedean character

↑ **Parent:** [Pretentious distance](#pretentious-distance)

An Archimedean character on the positive integers is the completely multiplicative function $n\mapsto n^{it}$ for a real parameter $t$.

<h5 id="halasz-theorem">Halász theorem</h5>

↑ **Parent:** [Pretentious distance](#pretentious-distance)

Halász's theorem bounds the mean of a bounded [multiplicative arithmetic function](#multiplicative-function) in terms of its least [pretentious distance](#pretentious-distance) from an [Archimedean character](#archimedean-character). A large mean can occur only when this distance is small.

<h5 id="strong-aperiodicity-of-the-mobius-function">Strong aperiodicity of the Möbius function</h5>

↑ **Parent:** [Pretentious distance](#pretentious-distance)

The Möbius function stays far in [pretentious distance](#pretentious-distance) from every [Archimedean character](#archimedean-character). One useful uniform form is

$$
\inf_{|t|\leq2(\log x)^{1/10}}
\mathbb D(\mu,n^{it};x)^2\longrightarrow\infty.
$$

This follows by estimating the prime sum $\sum_{p\leq x}(1+\cos(t\log p))/p$.

### Pointwise product of arithmetic functions

↑ **Parent:** [Arithmetic function](#arithmetic-function)

The [pointwise product of arithmetic functions](#pointwise-product-of-arithmetic-functions) multiplies two [arithmetic functions](#arithmetic-function) at the same input: $(f\cdot g)(n)=f(n)g(n)$. Thus $(\mathbf1\cdot\mathbf1)(12)=1$ and $(\operatorname{id}\cdot\mathbf1)(12)=12$, using the [constant-one arithmetic function](#constant-one-arithmetic-function) and the [identity arithmetic function](#identity-arithmetic-function). These differ from the corresponding [Dirichlet convolution](#dirichlet-convolution) values $6$ and $28$, because [Dirichlet convolution](#dirichlet-convolution) sums over every positive [integer divisor](#divisor).

### Dirichlet convolution

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_convolution)

The [Dirichlet convolution](#dirichlet-convolution) of [arithmetic functions](#arithmetic-function) $f,g$ is the [arithmetic function](#arithmetic-function)

$$
(f*g)(n)=\sum_{d\mid n}f(d)g(n/d)=\sum_{\substack{a,b>0\\ab=n}}f(a)g(b),\qquad n>0.
$$

In the first sum, $d$ runs over the positive [integer divisors](#divisor) of $n$; the second uses [ordered pairs](set.md#ordered-pair) of [positive integers](#positive-integer) whose product is $n$. Both sums are finite. Each pair contributes one weight from $f$ and one from $g$, so [Dirichlet convolution](#dirichlet-convolution) combines information attached to complementary factors. It turns a [divisor sum](#divisor-sum) into an operation on [arithmetic functions](#arithmetic-function). [Darij Grinberg, MIT 18.781 lecture notes, Sections 2.3 and 2.4: Dirichlet convolution and examples](https://darijgrinberg.gitlab.io/floor.pdf)

For $n=12$ the six [ordered pairs](set.md#ordered-pair) are $(1,12),(2,6),(3,4),(4,3),(6,2),(12,1)$. The [constant-one arithmetic function](#constant-one-arithmetic-function) gives one per pair, while the [identity arithmetic function](#identity-arithmetic-function) weights the first factor by its size:

$$
\begin{aligned}
\tau&=\mathbf1*\mathbf1,&\tau(12)&=1+1+1+1+1+1=6,\\
\sigma_1&=\operatorname{id}*\mathbf1,&\sigma_1(12)&=1+2+3+4+6+12=28.
\end{aligned}
$$

Here $\tau$ is the [divisor function](#divisor-function) and $\sigma_1$ is the [sum-of-divisors function](#sum-of-divisors-function). By comparison, the [pointwise product of arithmetic functions](#pointwise-product-of-arithmetic-functions) gives $(\mathbf1\cdot\mathbf1)(12)=1$ and $(\operatorname{id}\cdot\mathbf1)(12)=12$.

<a id="image-six-ordered-pairs-of-positive-integers-with-product-12-contribute-to-dirichlet-convolution-one-per-pair-for-the-divisor-function-or-the-first-factor-for-the-sum-of-divisors-function"></a>
![](dirichlet-convolution-factor-pairs.png)

**[Figure 15](#image-six-ordered-pairs-of-positive-integers-with-product-12-contribute-to-dirichlet-convolution-one-per-pair-for-the-divisor-function-or-the-first-factor-for-the-sum-of-divisors-function). Six ordered pairs of positive integers with product 12 contribute to Dirichlet convolution: one per pair for the divisor function, or the first factor for the sum-of-divisors function**.

[Commutativity](algebra.md#commutativity) follows by swapping the two entries of every [ordered pair](set.md#ordered-pair). [Associativity](algebra.md#associative-property) follows by reindexing either grouping over the same ordered [tuples](set-theory.md#finite-tuple) of three [positive integers](#positive-integer):

$$
((f*g)*h)(n)=\sum_{\substack{a,b,c>0\\abc=n}}f(a)g(b)h(c)=(f*(g*h))(n).
$$

For example, $((\mathbf1*\mathbf1)*\mathbf1)(12)$ counts ordered [tuples](set-theory.md#finite-tuple) of three [positive integers](#positive-integer) with product $12$. Distribute the two occurrences of the [prime factor](#prime-factor) $2$ among three entries in $\binom{2+2}{2}=6$ ways, and the one occurrence of the [prime factor](#prime-factor) $3$ in $\binom{1+2}{2}=3$ ways. These [binomial coefficients](combinatorics.md#binomial-coefficient) are the [stars and bars](combinatorics.md#stars-and-bars-combinatorics) counts of exponent choices in the [nonnegative integers](arithmetic.md#natural-number); [prime factorization](#fundamental-theorem-of-arithmetic) therefore gives $6\cdot3=18$ such [tuples](set-theory.md#finite-tuple). Directly, the same [Dirichlet convolution](#dirichlet-convolution) is $\sum_{d\mid12}\tau(d)=1+2+2+3+4+6=18$.

The [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution) is $\varepsilon$, and the [Möbius function](#mobius-function) reverses a [divisor sum](#divisor-sum) because $\mu*\mathbf1=\varepsilon$. This makes [Dirichlet convolution](#dirichlet-convolution) useful both for counting factorizations and for recovering an [arithmetic function](#arithmetic-function) from its [divisor sum](#divisor-sum).

#### Multiplicativity of Dirichlet convolution

↑ **Parent:** [Dirichlet convolution](#dirichlet-convolution)

The [Dirichlet convolution](#dirichlet-convolution) of two [multiplicative functions](#multiplicative-function) is a [multiplicative function](#multiplicative-function). For positive [coprime integers](#coprime-integers) $m,n$, every positive [integer divisor](#divisor) of $mn$ has a unique form $de$ with $d\mid m$ and $e\mid n$, by [prime factorization](#fundamental-theorem-of-arithmetic). The pairs $d,e$ and $m/d,n/e$ are each [coprime integers](#coprime-integers), so the defining rules for the two [multiplicative functions](#multiplicative-function) separate the sum:

$$
(f*g)(mn)=\sum_{d\mid m}\sum_{e\mid n}f(d)f(e)g(m/d)g(n/e)=(f*g)(m)(f*g)(n).
$$

Also $(f*g)(1)=f(1)g(1)=1$. This short argument proves [multiplicativity](#multiplicativity-of-an-arithmetic-function) of both the [divisor function](#divisor-function) $\mathbf1*\mathbf1$ and the [sum-of-divisors function](#sum-of-divisors-function) $\operatorname{id}*\mathbf1$. The result need not be a [completely multiplicative function](#completely-multiplicative-function), even when both inputs are: $\mathbf1*\mathbf1=\tau$ fails at $2\cdot2$. [Darij Grinberg, MIT 18.781 lecture notes, Theorem 2.6.1](https://darijgrinberg.gitlab.io/floor.pdf)

#### Constant-one arithmetic function

↑ **Parent:** [Dirichlet convolution](#dirichlet-convolution)

The [constant-one arithmetic function](#constant-one-arithmetic-function) has $\mathbf1(n)=1$ for every [positive integer](#positive-integer) $n$, including $\mathbf1(1)=\mathbf1(12)=1$. It is a [completely multiplicative function](#completely-multiplicative-function). Its [Dirichlet convolution](#dirichlet-convolution) with an [arithmetic function](#arithmetic-function) $f$ is the [divisor sum](#divisor-sum) $(\mathbf1*f)(n)=\sum_{d\mid n}f(d)$. Thus $\mathbf1*\mathbf1=\tau$, the [divisor function](#divisor-function). Its [pointwise product of arithmetic functions](#pointwise-product-of-arithmetic-functions) with $f$ is $f$ itself; its [Dirichlet convolution](#dirichlet-convolution) with $f$ generally is not. The [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution) is instead $\varepsilon$.

#### Identity arithmetic function

↑ **Parent:** [Dirichlet convolution](#dirichlet-convolution)

The [identity arithmetic function](#identity-arithmetic-function) is $\operatorname{id}(n)=n$ on the [positive integers](#positive-integer), for example $\operatorname{id}(1)=1$ and $\operatorname{id}(12)=12$. It is a [completely multiplicative function](#completely-multiplicative-function) and gives the [sum-of-divisors function](#sum-of-divisors-function) through $\operatorname{id}*\mathbf1=\sigma_1$ under [Dirichlet convolution](#dirichlet-convolution). It is distinct from the [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution) $\varepsilon$. The identity $\operatorname{id}=\mathbf1*\varphi$, where $\varphi$ is [Euler's totient function](#euler-totient-function), is equivalent to $\sum_{d\mid n}\varphi(d)=n$.

#### Identity for Dirichlet convolution

↑ **Parent:** [Dirichlet convolution](#dirichlet-convolution)

The [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution) is the [arithmetic function](#arithmetic-function)

$$
\varepsilon(n)=\begin{cases}1&n=1,\\0&n>1.\end{cases}
$$

For every [arithmetic function](#arithmetic-function) $f$, it satisfies $f*\varepsilon=\varepsilon*f=f$. Indeed, in $(f*\varepsilon)(n)=\sum_{d\mid n}f(d)\varepsilon(n/d)$, only $d=n$ survives. For example,

$$
(f*\varepsilon)(12)=f(1)0+f(2)0+f(3)0+f(4)0+f(6)0+f(12)1=f(12).
$$

At $n=1$ the sole term is $f(1)\varepsilon(1)=f(1)$. This gives a useful way to check [Dirichlet convolution](#dirichlet-convolution) calculations: inserting $\varepsilon$ leaves every value unchanged. The three [arithmetic functions](#arithmetic-function) $\mathbf1$, $\operatorname{id}$, and $\varepsilon$ all take value $1$ at $1$, but at $12$ the [constant-one arithmetic function](#constant-one-arithmetic-function), the [identity arithmetic function](#identity-arithmetic-function), and the [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution) take values $1$, $12$, and $0$, respectively. [Darij Grinberg, MIT 18.781 lecture notes, Theorem 2.3.4](https://darijgrinberg.gitlab.io/floor.pdf)

The [Möbius function](#mobius-function) is the inverse of the [constant-one arithmetic function](#constant-one-arithmetic-function) under [Dirichlet convolution](#dirichlet-convolution), meaning $\mu*\mathbf1=\mathbf1*\mu=\varepsilon$. The [Möbius divisor-sum identity](#mobius-divisor-sum-identity) gives a short proof: for $n>1$ the nonzero terms expand $\prod_{p\mid n}(1-1)=0$, while at $1$ the sum is $\mu(1)=1$. At $12$, the computation is

$$
(\mu*\mathbf1)(12)=\mu(1)+\mu(2)+\mu(3)+\mu(4)+\mu(6)+\mu(12)=1-1-1+0+1+0=0=\varepsilon(12).
$$

The zeros occur because $4$ and $12$ are divisible by the square of the [prime number](#prime-number) $2$. Consequently, if $F=f*\mathbf1$ is a [divisor sum](#divisor-sum), then [associativity](algebra.md#associative-property) gives $F*\mu=f*(\mathbf1*\mu)=f*\varepsilon=f$: this is [Möbius inversion](#mobius-inversion-formula).

#### Dirichlet hyperbola method

↑ **Parent:** [Dirichlet convolution](#dirichlet-convolution)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet_hyperbola_method)

The [Dirichlet hyperbola method](#dirichlet-hyperbola-method) turns a long [summation](arithmetic.md#summation) over a [Dirichlet convolution](#dirichlet-convolution) into two short ones by covering the [lattice points](quantum-mechanics.md#lattice-point) below a [hyperbola](geometry-and-topology.md#hyperbola) with two overlapping strips. Its simplest application is an exact count: for a [positive integer](#positive-integer) $N$, every positive [integer divisor](#divisor) $a$ of $n\le N$ corresponds to the [ordered pair](set.md#ordered-pair) $(a,n/a)$. Thus the [divisor summatory function](#divisor-summatory-function) counts precisely the [ordered pairs](set.md#ordered-pair) of [positive integers](#positive-integer) with $ab\le N$:

$$
D(N)=\sum_{n=1}^N\tau(n)
=\#\{(a,b)\in\mathbb Z_{>0}^2:ab\le N\}
=\sum_{a=1}^N\left\lfloor\frac Na\right\rfloor.
$$

Here $\tau$ is the [divisor function](#divisor-function), and the [floor function](calculus.md#floor-function) gives the number of allowed values of $b$ for each $a$. The axes are excluded, while points on $ab=N$ are included.

Set $r=\lfloor\sqrt N\rfloor$, using the [floor function](calculus.md#floor-function) and the positive [square root](algebra.md#square-root). **Every counted pair has $a\le r$ or $b\le r$.** Otherwise $ab\ge(r+1)^2>N$. The first strip contains $\sum_{a=1}^r\lfloor N/a\rfloor$ points; swapping the two coordinates gives the same count for the second. Their overlap contains all $r^2$ pairs with $1\le a,b\le r$, since $r^2\le N$. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) therefore gives the exact identity

$$
\boxed{D(N)=2\sum_{a=1}^r\left\lfloor\frac Na\right\rfloor-r^2,
\qquad r=\lfloor\sqrt N\rfloor.}
$$

The subtraction is for the whole overlap square, rather than only the diagonal. The same [Dirichlet hyperbola method](#dirichlet-hyperbola-method) identity holds for real $x\ge1$, with $D(x)=\sum_{n\le x}\tau(n)$ and $r=\lfloor\sqrt x\rfloor$. [Andrew Granville and K. Soundararajan, Multiplicative number theory: The pretentious approach, §1.1.4, pp. 7–8: divisor pairing and the hyperbola split](mathematics-bibliography.md#multiplicative-number-theory-the-pretentious-approach-by-andrew-granville-and-k-soundararajan)

<a id="image-the-dirichlet-hyperbola-method-counts-35-positive-lattice-points-with-ab-le12-two-strips-of-22-points-overlap-in-a-square-of-nine-points"></a>
![](dirichlet-hyperbola-lattice-split.png)

**[Figure 16](#image-the-dirichlet-hyperbola-method-counts-35-positive-lattice-points-with-ab-le12-two-strips-of-22-points-overlap-in-a-square-of-nine-points). The Dirichlet hyperbola method counts 35 positive lattice points with $ab\le12$: two strips of 22 points overlap in a square of nine points**.

##### Divisor summatory function

↑ **Parent:** [Dirichlet hyperbola method](#dirichlet-hyperbola-method)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisor_summatory_function)

The [divisor summatory function](#divisor-summatory-function) adds the [divisor function](#divisor-function) up to a cutoff $x\ge1$. It counts all [ordered pairs](set.md#ordered-pair) of [positive integers](#positive-integer) whose product is at most $x$. For $N=12$, the twelve individual [divisor function](#divisor-function) values are

$$
(\tau(1),\ldots,\tau(12))=(1,2,2,3,2,4,2,4,3,4,2,6),
\qquad D(12)=35.
$$

Counting columns of [lattice points](quantum-mechanics.md#lattice-point) instead gives $12+6+4+3+2+2+1+1+1+1+1+1=35$. The [Dirichlet hyperbola method](#dirichlet-hyperbola-method) needs only the first three column counts:

$$
D(12)=2(12+6+4)-3^2=44-9=35.
$$

The [arithmetic work of the Dirichlet hyperbola method](#arithmetic-work-of-the-dirichlet-hyperbola-method) is much smaller even though the answer is identical.

This is useful for elementary averages: individual [divisor function](#divisor-function) values fluctuate, but their [summation](arithmetic.md#summation) has the regular behavior given by the [divisor summatory asymptotic](#divisor-summatory-asymptotic). Dividing that estimate by a [positive integer](#positive-integer) $N$ gives

$$
\frac1N\sum_{n=1}^N\tau(n)
=\log N+2\gamma-1+O(N^{-1/2})\qquad(N\longrightarrow\infty),
$$

where $\log$ is the [natural logarithm](calculus.md#natural-logarithm), $\gamma$ is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant), and $O$ uses [big O notation](real-analysis.md#big-o-notation). This describes an average, rather than an estimate for every individual [divisor function](#divisor-function) value. [§1.1.4, p. 8, equation (1.1.13): the divisor summatory asymptotic](mathematics-bibliography.md#multiplicative-number-theory-the-pretentious-approach-by-andrew-granville-and-k-soundararajan)

##### Asymmetric Dirichlet hyperbola split

↑ **Parent:** [Dirichlet hyperbola method](#dirichlet-hyperbola-method)

A balanced [Dirichlet hyperbola method](#dirichlet-hyperbola-method) split takes real thresholds $A=B=\sqrt N$. An asymmetric split takes $1\le A\le N$ and $B=N/A$. Every [lattice point](quantum-mechanics.md#lattice-point) with $ab\le N$ then has $a\le A$ or $b\le B$, and every point in their overlap rectangle is allowed because $AB=N$. For [arithmetic functions](#arithmetic-function) $f,g$, define their [partial sums](real-analysis.md#partial-sum) by $F(t)=\sum_{a\le t}f(a)$ and $G(t)=\sum_{b\le t}g(b)$, always over [positive integers](#positive-integer). The same [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle), now with weight $f(a)g(b)$, yields

$$
\sum_{n\le N}(f*g)(n)
=\sum_{a\le A}f(a)G(N/a)
+\sum_{b\le B}g(b)F(N/b)-F(A)G(B),
\qquad AB=N.
$$

No [multiplicativity](#multiplicativity-of-an-arithmetic-function) assumption is needed: this is a finite rearrangement of [Dirichlet convolution](#dirichlet-convolution). The [constant-one arithmetic function](#constant-one-arithmetic-function) in both positions recovers the [divisor summatory function](#divisor-summatory-function). For $N=12$, $A=2$, $B=6$ gives

$$
D(12)=(12+6)+(12+6+4+3+2+2)-2\cdot6=18+29-12=35.
$$

It uses two columns and six rows, with a twelve-point overlap.

For general positive real thresholds, **$AB\ge N$ is sufficient for coverage**, since $a>A$ and $b>B$ would imply $ab>AB\ge N$. If $AB>N$, however, the overlap can include points above the [hyperbola](geometry-and-topology.md#hyperbola). The correct subtraction is then $\sum_{a\le A,\ b\le B,\ ab\le N}f(a)g(b)$; the product $F(A)G(B)$ is justified only when the whole integer rectangle lies below it. For example, $N=12$, $A=B=4$ covers every allowed pair, but its rectangle contains the forbidden pair $(4,4)$, so subtracting all sixteen points would give $34$ instead of $35$.

Conversely, the balanced integer thresholds $r,r$ have $r^2\le N$ and still cover every allowed pair because $(r+1)^2>N$. More generally, positive integer thresholds $U,V$ give coverage exactly when $(U+1)(V+1)>N$, and their overlap is a full rectangle exactly when $UV\le N$. These discrete conditions explain why the square-root identity works even when $r^2<N$.

##### Arithmetic work of the Dirichlet hyperbola method

↑ **Parent:** [Dirichlet hyperbola method](#dirichlet-hyperbola-method)

The direct [divisor summatory function](#divisor-summatory-function) formula evaluates $N$ floor divisions. Its balanced [Dirichlet hyperbola method](#dirichlet-hyperbola-method) formula evaluates $r=\lfloor\sqrt N\rfloor$ floor divisions and reuses their [sum](arithmetic.md#sum) for the other strip, followed by doubling and square-overlap subtraction. Thus it uses $O(\sqrt N)$ [arithmetic operations](numerical-analysis.md#arithmetic-operation), with [big O notation](real-analysis.md#big-o-notation), in a model that counts each division, addition and multiplication as one operation. At $N=10^6$, the division counts for these two formulas are $10^6$ and $10^3$.

<a id="image-the-balanced-dirichlet-hyperbola-method-reduces-floor-divisions-from-n-to-lfloor-sqrt-n-rfloor-for-n-12-two-sequences-of-partial-sums-reach-the-same-exact-answer-35"></a>
![](dirichlet-hyperbola-work-and-partial-sums.png)

**[Figure 17](#image-the-balanced-dirichlet-hyperbola-method-reduces-floor-divisions-from-n-to-lfloor-sqrt-n-rfloor-for-n-12-two-sequences-of-partial-sums-reach-the-same-exact-answer-35). The balanced Dirichlet hyperbola method reduces floor divisions from $N$ to $\lfloor\sqrt N\rfloor$; for $N=12$, two sequences of partial sums reach the same exact answer 35**.

For a general [Dirichlet convolution](#dirichlet-convolution), the asymmetric formula has $\lfloor A\rfloor+\lfloor B\rfloor$ outer terms; evaluating $F$ and $G$ has an additional cost. Under $AB=N$, equal thresholds minimize $A+B$, but an asymmetric split can be useful if the two [partial sums](real-analysis.md#partial-sum) have different evaluation costs. The balanced [divisor summatory function](#divisor-summatory-function) gains the further reuse because its two [arithmetic functions](#arithmetic-function) are identical.

These are [arithmetic operation](numerical-analysis.md#arithmetic-operation) counts, rather than counts of elementary operations on [binary digits](#binary-digit): the [integers](#integer) grow with $N$, and division of longer [integers](#integer) costs more in that model of [computational complexity theory](computer-science.md#computational-complexity-theory). Computing $r$ also requires an exact integer [square root](algebra.md#square-root), or checking and correcting a numerical [square root](algebra.md#square-root) until $r^2\le N<(r+1)^2$ holds.

##### Divisor summatory asymptotic

↑ **Parent:** [Dirichlet hyperbola method](#dirichlet-hyperbola-method)

The [Dirichlet hyperbola method](#dirichlet-hyperbola-method) gives $D(x)=2\sum_{a\le r}\lfloor x/a\rfloor-r^2$, where $r=\lfloor\sqrt x\rfloor$. The [harmonic number](analytic-number-theory.md#harmonic-number) estimate $H_r=\log r+\gamma+O(1/r)$, with $\gamma$ the [Euler's constant](complex-analysis.md#euler-s-constant), yields $D(x)=2x(\log r+\gamma)-r^2+O(x/r+r)$. Substitution of $r=\sqrt x+O(1)$ gives the displayed [asymptotic expansion](analysis.md#asymptotic-expansion). Comparison of $\sum_{n\le x}\log n$ with its integral consequently gives $\sum_{n\le N}(\tau(n)-\log n-2\gamma)=O(\sqrt N)$ for integer $N$.

##### Harmonic divisor sum

↑ **Parent:** [Dirichlet hyperbola method](#dirichlet-hyperbola-method)

Write $B(t)=\sum_{n\leq t}\tau(n)/n$ and $r=\lfloor\sqrt t\rfloor$. The weighted [Dirichlet hyperbola method](#dirichlet-hyperbola-method) gives

$$
B(t)=2\sum_{a\leq r}\frac{H_{\lfloor t/a\rfloor}}a-H_r^2
=\tfrac12\log^2t+2\gamma\log t+c+O\left(\frac{\log(2t)}{\sqrt t}\right).
$$

Indeed, use $H_{\lfloor u\rfloor}=\log u+\gamma+O(1/u)$ and $\sum_{a\leq r}(\log a)/a=\tfrac12\log^2r+c\prime+O(\log(2r)/r)$. The latter follows by comparing each summand with the integral on its unit interval: the derivative of $(\log t)/t$ has an integrable tail. Since $r=\sqrt t+O(1)$, substitution yields the expansion. Here $H_n$ is the [harmonic number](analytic-number-theory.md#harmonic-number) and $\gamma$ the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant).

### Divisor function

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisor_function)

The [divisor function](#divisor-function) $\tau(n)=\sum_{d\mid n}1$ counts the positive [integer divisors](#divisor) of a [positive integer](#positive-integer) $n$. In particular $\tau(1)=1$, because $1$ has just one positive [integer divisor](#divisor). More generally the notation $\sigma_k(n)=\sum_{d\mid n}d^k$ gives $\tau=\sigma_0$ and the [sum-of-divisors function](#sum-of-divisors-function) $\sigma_1$. Thus the [divisor function](#divisor-function) counts the positive [integer divisors](#divisor), while $\sigma_1$ adds their sizes. [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.1.2 and Theorem 2.1.6](https://darijgrinberg.gitlab.io/floor.pdf)

If the [prime factorization](#fundamental-theorem-of-arithmetic) is $n=\prod_{k=1}^r p_k^{a_k}$ with distinct [prime numbers](#prime-number) $p_k$ and positive exponents $a_k$, then

$$
\tau(n)=\prod_{k=1}^r(a_k+1).
$$

The short proof is a count: each positive [integer divisor](#divisor) has a unique form $\prod_{k=1}^r p_k^{b_k}$, where $0\le b_k\le a_k$. There are $a_k+1$ choices at each [prime number](#prime-number), and choosing them gives every positive [integer divisor](#divisor) exactly once. For $n=1$ there are no [prime factors](#prime-factor) and the product is $1$.

For $12=2^2\cdot3$, choose $i\in\{0,1,2\}$ and $j\in\{0,1\}$ to obtain $2^i3^j$. The six values are $1,2,4,3,6,12$; sorted, the positive [integer divisors](#divisor) are $1,2,3,4,6,12$. Therefore $\tau(12)=(2+1)(1+1)=6$. The diagram makes the independent exponent choices visible.

<a id="image-the-prime-factorization-12-2-2-cdot3-gives-a-three-by-two-array-of-positive-integer-divisors-2-i3-j-so-the-divisor-function-has-tau-12-6"></a>
![](divisor-count-prime-exponents.png)

**[Figure 18](#image-the-prime-factorization-12-2-2-cdot3-gives-a-three-by-two-array-of-positive-integer-divisors-2-i3-j-so-the-divisor-function-has-tau-12-6). The prime factorization $12=2^2\cdot3$ gives a three-by-two array of positive integer divisors $2^i3^j$, so the divisor function has $\tau(12)=6$**.

This count is useful because a known [prime factorization](#fundamental-theorem-of-arithmetic) gives $\tau(n)$ without testing every smaller [positive integer](#positive-integer) for [divisibility](#divisibility). It also proves the [divisor function](#divisor-function) is a [multiplicative function](#multiplicative-function): [coprime integers](#coprime-integers) have disjoint [prime factors](#prime-factor), so their exponent choices combine. For example $\tau(6)=4=\tau(2)\tau(3)$, but $\tau(4)=3\ne4=\tau(2)^2$, so it is not a [completely multiplicative function](#completely-multiplicative-function). Equivalently, $\tau=\mathbf1*\mathbf1$ under [Dirichlet convolution](#dirichlet-convolution), counting [ordered pairs](set.md#ordered-pair) of [positive integers](#positive-integer) whose product is $n$.

#### Subpower bound for the divisor function

↑ **Parent:** [Divisor function](#divisor-function)

For each $\eta>0$, the [divisor function](#divisor-function) satisfies the displayed bound. Write $n=\prod p^{a_p}$, so $\tau(n)=\prod(a_p+1)$. For all sufficiently large [primes](#prime-number), $a+1\le2^a\le p^{\eta a}$ for every $a\ge0$. For each of the finitely many smaller [primes](#prime-number), $\sup_{a\ge0}(a+1)p^{-\eta a}$ is finite. Multiplying these finitely many constants proves the bound. Products of a fixed number of divisor functions obey the same conclusion after reducing $\eta$.

#### Divisor-square summatory bound

↑ **Parent:** [Divisor function](#divisor-function)

The [divisor function](#divisor-function) satisfies $\sum_{n\le X}d(n)^2\ll X\log^3(2X)$. [Partial summation](analytic-number-theory.md#abel-s-summation-formula) consequently gives $\sum_{n\le X}d(n)^2/n\ll\log^4(2X)$.

### Von Mangoldt function

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Von_Mangoldt_function)

The [Von Mangoldt function](#von-mangoldt-function) assigns a [natural logarithm](calculus.md#natural-logarithm) weight to each positive power of a [prime number](#prime-number). For a [positive integer](#positive-integer) $n$,

$$
\Lambda(n)=\begin{cases}
\log p,&n=p^k,\quad p\text{ prime},\ k\geq1,\\
0,&\text{otherwise}.
\end{cases}
$$

Here and throughout the [Chebyshev functions](#chebyshev-function), **$\log$ means the [natural logarithm](calculus.md#natural-logarithm)**. In particular, $\Lambda(1)=0$: the exponent must be positive, even though the convention in [prime power](#prime-power) allows exponent zero. The [support of a function](function.md#support) of $\Lambda$ therefore consists precisely of the [prime powers](#prime-power) greater than one. [254A, Notes 1: Elementary multiplicative number theory](mathematics-bibliography.md#254a-analytic-prime-number-theory/254a-notes-1-elementary-multiplicative-number-theory)

For example, $\Lambda(2)=\Lambda(4)=\Lambda(8)=\log2$ and $\Lambda(3)=\Lambda(9)=\log3$, whereas $\Lambda(6)=\Lambda(12)=0$. A [composite number](#composite-number) can have a nonzero weight: $8$ has just one distinct [prime factor](#prime-factor). But $12=2^2\cdot3$ has two distinct [prime factors](#prime-factor), so its weight is zero. At $p^k$ the weight is **$\log p$, not $\log(p^k)=k\log p$**. This choice lets successive powers record successive copies of the same [prime factor](#prime-factor) in the [Von Mangoldt divisor identity](#von-mangoldt-divisor-identity).

The [Von Mangoldt function](#von-mangoldt-function) is useful because it connects two views of the [prime numbers](#prime-number): the [prime factorization](#fundamental-theorem-of-arithmetic) of an individual [integer](#integer), through a [divisor sum](#divisor-sum), and the accumulated weights below a cutoff, through the [Second Chebyshev function](#second-chebyshev-function). The latter turns questions about the distribution of [prime numbers](#prime-number) into questions about a [partial sum](real-analysis.md#partial-sum) of an [arithmetic function](#arithmetic-function).

#### Selberg symmetry formula

↑ **Parent:** [Von Mangoldt function](#von-mangoldt-function)

The elementary Selberg symmetry formula can be written

$$
\psi(x)+\frac1{\log x}\sum_{n\leq x}\Lambda(n)\psi(x/n)=2x+O\left(\frac{x}{\log x}\right).
$$

Use the weights $\lambda_d=\mu(d)\log(x/d)/\log x$. Their [divisor sum](#divisor-sum) is $1_{n=1}+\Lambda(n)/\log x$. Apply them to the [integrated Chebyshev sum](#integrated-chebyshev-sum), then use the [Möbius harmonic logarithmic moments](#mobius-harmonic-logarithmic-moments). The [Chebyshev estimate](#chebyshev-estimate) shows this is equivalent, with an $O(x)$ error, to $\sum_{n\leq x}\Lambda(n)\log n+\sum_{mn\leq x}\Lambda(m)\Lambda(n)=2x\log x+O(x)$.

#### Von Mangoldt divisor identity

↑ **Parent:** [Von Mangoldt function](#von-mangoldt-function)

For every [positive integer](#positive-integer) $n$, the [divisor sum](#divisor-sum) of its [Von Mangoldt function](#von-mangoldt-function) weights recovers its [natural logarithm](calculus.md#natural-logarithm):

$$
\sum_{d\mid n}\Lambda(d)=\log n.
$$

The sum runs over the positive [integer divisors](#divisor) of $n$. For $n=1$, its only term is $\Lambda(1)=0=\log1$. Equivalently, if $L(n)=\log n$ and $\mathbf1$ is the [constant-one arithmetic function](#constant-one-arithmetic-function), then $\mathbf1*\Lambda=L$, where $*$ is [Dirichlet convolution](#dirichlet-convolution). [254A, Notes 1: Elementary multiplicative number theory](mathematics-bibliography.md#254a-analytic-prime-number-theory/254a-notes-1-elementary-multiplicative-number-theory)

For $12=2^2\cdot3$, the positive [integer divisors](#divisor) are $1,2,3,4,6,12$. Only $2,3,4$ contribute:

$$
\Lambda(1)+\Lambda(2)+\Lambda(3)+\Lambda(4)+\Lambda(6)+\Lambda(12)
=0+\log2+\log3+\log2+0+0
=\log12.
$$

Thus the vanishing of $\Lambda(12)$ loses no information here: the [divisor sum](#divisor-sum) retrieves both copies of the [prime factor](#prime-factor) $2$ from the [integer divisors](#divisor) $2$ and $4$.

<a id="image-von-mangoldt-divisor-contributions"></a>
![](von-mangoldt-divisor-contributions.png)

**[Figure 19](#image-von-mangoldt-divisor-contributions). The Von Mangoldt divisor identity assembles $\log12$ from three nonzero divisor weights**. The six positive [integer divisors](#divisor) of $12$ appear in increasing order. Blue bars contribute $\log2$ at $2$ and $4$; the orange bar contributes $\log3$ at $3$. The remaining three weights are zero. The adjacent stacked bar shows the total $2\log2+\log3=\log12$.

Proof outline: by the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic), write $n=\prod_{i=1}^r p_i^{a_i}$ with distinct [prime numbers](#prime-number) $p_i$ and positive exponents $a_i$. Among the positive [integer divisors](#divisor), the ones with nonzero [Von Mangoldt function](#von-mangoldt-function) weights are exactly $p_i,p_i^2,\ldots,p_i^{a_i}$. Consequently

$$
\sum_{d\mid n}\Lambda(d)=\sum_{i=1}^r\sum_{j=1}^{a_i}\log p_i
=\sum_{i=1}^r a_i\log p_i
=\log\!\left(\prod_{i=1}^r p_i^{a_i}\right)=\log n.
$$

The [natural logarithm](calculus.md#natural-logarithm) turns the [prime factorization](#fundamental-theorem-of-arithmetic) product into a sum, and the [prime powers](#prime-power) greater than one supply exactly the required multiplicities.

#### Chebyshev function

↑ **Parent:** [Von Mangoldt function](#von-mangoldt-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chebyshev_function)

The two [Chebyshev functions](#chebyshev-function) measure the total [natural logarithm](calculus.md#natural-logarithm) weight of [prime numbers](#prime-number) or of [prime powers](#prime-power) greater than one below a real cutoff $x\geq0$:

$$
\vartheta(x)=\sum_{p\leq x}\log p,
\qquad
\psi(x)=\sum_{n\leq x}\Lambda(n)
=\sum_{\substack{p^k\leq x\\k\geq1}}\log p.
$$

Here $p$ ranges over [prime numbers](#prime-number), $n$ over [positive integers](#positive-integer), and $k$ over [positive integers](#positive-integer). The [Chebyshev theta function](#chebyshev-theta-function) $\vartheta$, also written $\theta$, weights each [prime number](#prime-number) once. The [Second Chebyshev function](#second-chebyshev-function) $\psi$ weights every positive power of each [prime number](#prime-number) separately. Both vanish for $0\leq x<2$; the inclusive cutoff makes them [right-continuous functions](calculus.md#right-continuous-function) and [nondecreasing functions](calculus.md#nondecreasing-function), constant between their jumps. [7.2: Chebyshev's Functions](mathematics-bibliography.md#elementary-number-theory/7-2-chebyshev-s-functions)

At $x=10$, the [prime numbers](#prime-number) are $2,3,5,7$, while the extra [prime powers](#prime-power) greater than one are $4,8,9$. Exactly,

$$
\begin{aligned}
\vartheta(10)&=\log2+\log3+\log5+\log7=\log210,\\
\psi(10)&=3\log2+2\log3+\log5+\log7=\log2520,\\
\psi(10)-\vartheta(10)&=2\log2+\log3=\log12.
\end{aligned}
$$

At each [prime number](#prime-number) $p$, both [Chebyshev functions](#chebyshev-function) jump by $\log p$. At a [prime power](#prime-power) $p^k$ with $k\geq2$, only the [Second Chebyshev function](#second-chebyshev-function) jumps, by $\log p$. At $6$ and $10$ neither jumps. Notice that the gap is already positive at $5$ and $7$: a shared jump does not remove the earlier contribution from $4$.

<a id="image-chebyshev-prime-power-staircases"></a>
![](chebyshev-prime-power-staircases.png)

**[Figure 20](#image-chebyshev-prime-power-staircases). The Chebyshev functions separate at the extra prime powers $4$, $8$, and $9$**. The upper panel compares $\vartheta(x)$ and $\psi(x)$ for $0\leq x\leq10$. Solid endpoints include the jump at each contributing [integer](#integer); open endpoints show the preceding value. The lower panel isolates $\psi(x)-\vartheta(x)$, which jumps by $\log2$ at $4$ and $8$ and by $\log3$ at $9$, reaching $\log12$. All logarithms are [natural logarithms](calculus.md#natural-logarithm).

Grouping the [prime powers](#prime-power) by their exponent gives, for $x\geq2$,

$$
\psi(x)=\sum_{k=1}^{\lfloor\log x/\log2\rfloor}\vartheta(x^{1/k}),
\qquad
\psi(x)-\vartheta(x)=\sum_{k=2}^{\lfloor\log x/\log2\rfloor}\vartheta(x^{1/k}).
$$

The [floor function](calculus.md#floor-function) cutoff is exact: $p\geq2$ forces $2^k\leq x$ whenever $p^k\leq x$. For each exponent, $p^k\leq x$ is equivalent to $p\leq x^{1/k}$. An upper cutoff smaller than the lower one means an empty sum. [7.2: Chebyshev's Functions](mathematics-bibliography.md#elementary-number-theory/7-2-chebyshev-s-functions)

##### Second Chebyshev function

↑ **Parent:** [Chebyshev function](#chebyshev-function)

The [Second Chebyshev function](#second-chebyshev-function) is the [partial sum](real-analysis.md#partial-sum) of the [Von Mangoldt function](#von-mangoldt-function) up to a real cutoff $x\geq0$:

$$
\psi(x)=\sum_{1\leq n\leq x}\Lambda(n).
$$

For example, $\psi(3)=\log6$, $\psi(4)=\log12$, and $\psi(4.5)=\log12$. At $4=2^2$ the jump has size $\log2$; between $4$ and $5$ no new [prime power](#prime-power) greater than one enters the sum. In contrast, the [Chebyshev theta function](#chebyshev-theta-function) stays at $\vartheta(4)=\log6$.

There is also an exact connection with the [least common multiple](#least-common-multiple). For $N=\lfloor x\rfloor\geq1$, each [prime number](#prime-number) $p\leq N$ occurs to the highest exponent $k$ for which $p^k\leq N$, both in that [least common multiple](#least-common-multiple) and in the accumulated [Von Mangoldt function](#von-mangoldt-function) weights. Thus

$$
\psi(x)=\log\operatorname{lcm}(1,2,\ldots,N).
$$

This explains the $\log2520$ value at $x=10$: the [least common multiple](#least-common-multiple) is $2^3\cdot3^2\cdot5\cdot7$. The [Chebyshev theta function](#chebyshev-theta-function) instead gives the [natural logarithm](calculus.md#natural-logarithm) of the [primorial](#primorial) $2\cdot3\cdot5\cdot7=210$. The additional [prime powers](#prime-power) retain the highest required multiplicities.

Why is this useful for the distribution of [prime numbers](#prime-number)? The [Prime number theorem](analytic-number-theory.md#prime-number-theorem) has the equivalent forms

$$
\pi(x)\sim\frac{x}{\log x},\qquad\vartheta(x)\sim x,\qquad\psi(x)\sim x
\quad(x\longrightarrow\infty),
$$

where $\pi$ is the [prime-counting function](#prime-counting-function) and $\sim$ denotes [asymptotic equivalence](real-analysis.md#asymptotic-equivalence). Thus an [arithmetic function](#arithmetic-function) defined using [prime factorization](#fundamental-theorem-of-arithmetic) has average weight tending to one over long initial intervals of the [positive integers](#positive-integer). These are substantive [asymptotic equivalences](real-analysis.md#asymptotic-equivalence), not consequences of the definitions or the [Von Mangoldt divisor identity](#von-mangoldt-divisor-identity) alone. [254A, Notes 2: Complex-analytic multiplicative number theory](mathematics-bibliography.md#254a-analytic-prime-number-theory/254a-notes-2-complex-analytic-multiplicative-number-theory)

The elementary reason the two [Chebyshev functions](#chebyshev-function) have the same leading behavior is that their difference is small compared with $x$. Every additional [prime power](#prime-power) has base $p\leq\sqrt x$, and for each such [prime number](#prime-number) its total extra weight is at most $\log x$. There are at most $\lfloor\sqrt x\rfloor$ such bases, so

$$
0\leq\psi(x)-\vartheta(x)\leq\lfloor\sqrt x\rfloor\log x,
\qquad
\frac{\psi(x)-\vartheta(x)}x\longrightarrow0.
$$

This transfers $\psi(x)\sim x$ to $\vartheta(x)\sim x$, or conversely, once either is established. [Partial summation](analytic-number-theory.md#abel-s-summation-formula) then relates the [Chebyshev theta function](#chebyshev-theta-function) to the [prime-counting function](#prime-counting-function). The estimate controls the extra [prime powers](#prime-power); proving the leading value itself is the harder [Prime number theorem](analytic-number-theory.md#prime-number-theorem) problem.

###### First integral of the Chebyshev function

↑ **Parent:** [Second Chebyshev function](#second-chebyshev-function)

For the [Second Chebyshev function](#second-chebyshev-function), finite summation gives $\Psi_1(x)=\sum_{n\le x}(x-n)\Lambda(n)$. For $c>1$, Mellin inversion of the kernel $1/(s(s+1))$ gives

$$
\Psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds.
$$

The extra denominator makes this smoothing useful: the resulting sum over [Nontrivial zeros of the Riemann zeta function](analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) is absolutely convergent. This integral differs from the [integrated Chebyshev sum](#integrated-chebyshev-sum), which denotes a sum of the values $\psi(x/n)$.

###### Smoothed explicit formula for the Chebyshev function

↑ **Parent:** [First integral of the Chebyshev function](#first-integral-of-the-chebyshev-function)

For $x>1$, moving the Mellin contour past the [pole](isolated-singularity.md#pole) at one, the [Nontrivial zeros of the Riemann zeta function](analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function), and the remaining poles gives

$$
\Psi_1(x)=\frac{x^2}{2}-\sum_\rho\frac{x^{\rho+1}}{\rho(\rho+1)}-x\log(2\pi)+\frac{\zeta'(-1)}{\zeta(-1)}-\sum_{k\ge1}\frac{x^{1-2k}}{2k(2k-1)}.
$$

Zeros are included with multiplicity. The [Riemann–von Mangoldt formula](analytic-number-theory.md#riemann-von-mangoldt-formula) makes the zero sum absolutely convergent. If every nontrivial zero has real part below one, division by $x^2$ and [dominated convergence](measure-theory.md#dominated-convergence-theorem) give $\Psi_1(x)\sim x^2/2$. Monotonicity of $\psi$ then recovers $\psi(x)\sim x$ by upper and lower difference quotients.

###### Integrated Chebyshev sum

↑ **Parent:** [Second Chebyshev function](#second-chebyshev-function)

For $\psi(t)=\sum_{m\leq t}\Lambda(m)$, finite rearrangement and the [Von Mangoldt divisor identity](#von-mangoldt-divisor-identity) give

$$
T(x)=\sum_{n\leq x}\psi(x/n)=\sum_{m\leq x}\log m=\log(\lfloor x\rfloor!).
$$

The [Stirling formula](real-analysis.md#stirling-formula), or integral comparison for the [logarithm](calculus.md#logarithm), gives $T(x)=x\log x-x+O(\log(x+1))$ for real $x\geq1$.

###### Chebyshev estimate

↑ **Parent:** [Second Chebyshev function](#second-chebyshev-function)

The Chebyshev estimate is

$$
\psi(x)\asymp x.
$$

It gives upper and lower bounds of the correct linear order without asserting the [Prime number theorem](analytic-number-theory.md#prime-number-theorem) asymptotic $\psi(x)\sim x$.

###### Chebyshev estimate from central binomial coefficients

↑ **Parent:** [Chebyshev estimate](#chebyshev-estimate)

The central [binomial coefficient](combinatorics.md#binomial-coefficient) satisfies $4^m/(2m+1)\leq\binom{2m}{m}\leq4^m$. Prime factors between $m$ and $2m$ give a dyadic upper bound for the [Chebyshev theta function](#chebyshev-theta-function). The prime-power exponents in the factorial quotient are sums of zeros and ones, so the central coefficient gives a linear lower bound for the [Second Chebyshev function](#second-chebyshev-function). Higher prime powers contribute only $O(\sqrt x\log x)$; hence the prime-counting function has upper and lower bounds of order $x/\log x$.

<h6 id="riemann-von-mangoldt-explicit-formula">Riemann–von Mangoldt explicit formula</h6>

↑ **Parent:** [Second Chebyshev function](#second-chebyshev-function)

For $x>1$ away from a jump of $\psi$,

$$
\psi(x)=x-\sum_\rho\frac{x^\rho}{\rho}
-\log(2\pi)-\frac12\log(1-x^{-2}),
$$

where the sum over [Nontrivial zeros of the Riemann zeta function](analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) is taken symmetrically. A finite-height version has an explicit truncation error controlled by $x/T$ and the distance from $x$ to the nearest prime power.

###### Truncated explicit formula for the second Chebyshev function

↑ **Parent:** [Riemann–von Mangoldt explicit formula](#riemann-von-mangoldt-explicit-formula)

For $2\le T\le x$, the [truncated Perron formula](analytic-number-theory.md#truncated-perron-formula) and a contour shift give the displayed form of the [Riemann–von Mangoldt explicit formula](#riemann-von-mangoldt-explicit-formula). The [pole](isolated-singularity.md#pole) at one contributes $x$ and the [Nontrivial zeros of the Riemann zeta function](analytic-number-theory.md#nontrivial-zero-of-the-riemann-zeta-function) contribute the finite sum. One can choose a separated height in $[T,T+1]$ and then restore $T$ using the [local zero count for the Riemann zeta function](analytic-number-theory.md#local-zero-count-for-the-riemann-zeta-function). The error absorbs the half-weight discrepancy at a prime power. Outside this range of $T$, one needs the fuller error with the near-integer terms retained.

<h4 id="vaughan-s-identity">Vaughan's identity</h4>

↑ **Parent:** [Von Mangoldt function](#von-mangoldt-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Vaughan's_identity)

For thresholds $U,V$, write $\mu_{\leq U}(d)=\mu(d)1_{d\leq U}$ and similarly for the other truncations. Vaughan's identity is

$$
\Lambda
=\Lambda_{\leq V}
+\mu_{\leq U}*\log
-\mu_{\leq U}*\Lambda_{\leq V}*1
+\mu_{>U}*\Lambda_{>V}*1.
$$

It decomposes a sum weighted by $\Lambda$ into short, Type I, and Type II bilinear sums.

##### Prime exponential-sum estimate from Vaughan identity

↑ **Parent:** [Vaughan's identity](#vaughan-s-identity)

For reduced $a/q$ with $|\alpha-a/q|\leq q^{-2}$ and $1\leq q\leq N$, the displayed bound follows by splitting [Vaughan identity](#vaughan-s-identity) with parameters $U=V=N^{2/5}$. [Type I sums](analytic-number-theory.md#type-i-sum) use short geometric-sum bounds; [type II sums](analytic-number-theory.md#type-ii-sum) use the [Cauchy-Schwarz inequality](probability-and-statistics.md#cauchy-schwarz-inequality) and rational spacing to control bilinear cancellation. A [badly approximable number](#badly-approximable-number) has a Dirichlet approximant with $q\asymp N^{1/2}$, yielding $O(N^{4/5}\log^4N)$ and hence $O(N^{9/10})$.

// Target: analytic-number-theory.bigb

##### Logarithmic coefficient bound in Vaughan identity

↑ **Parent:** [Vaughan's identity](#vaughan-s-identity)

The [Von Mangoldt function](#von-mangoldt-function) is nonnegative and satisfies $\sum_{d\mid m}\Lambda(d)=\log m$. Therefore the middle short-divisor coefficient in the [Vaughan identity](#vaughan-s-identity) has the displayed pointwise bound. Grouping its long-divisor term as $\mu_{>U}(m)b(n)$, with $b(n)=\sum_{d\mid n,d>V}\Lambda(d)$, gives $0\le b(n)\le\log n$. This grouping permits bounded-coefficient [Type II sums](analytic-number-theory.md#type-ii-sum) after division by $\log N$.

<h5 id="vaughan-identity-for-the-mobius-function">Vaughan identity for the Möbius function</h5>

↑ **Parent:** [Vaughan's identity](#vaughan-s-identity)

The displayed identity is exact for all positive integers and all positive cutoffs. Expand $(\mu-\mu_{\leq U})*(\mu-\mu_{\leq V})*\mathbf1$ and use $\mu*\mathbf1=\varepsilon$. The two truncated terms are short sums; the negative term is a [type I sum](analytic-number-theory.md#type-i-sum) over [divisors](#divisor) at most $UV$; the last term is a [type II sum](analytic-number-theory.md#type-ii-sum) with both factor variables larger than a cutoff. This form of the [Vaughan identity](#vaughan-s-identity) is specific to Möbius weights.

<h6 id="type-i-type-ii-inverse-principle-for-mobius-correlation">Type I–type II inverse principle for Möbius correlation</h6>

↑ **Parent:** [Vaughan identity for the Möbius function](#vaughan-identity-for-the-mobius-function)

For $|f|\leq1$, if $|\sum_{n\leq X}\mu(n)f(n)|\geq\delta X$ and $U+V\leq\delta X/2$, the [Vaughan identity for the Möbius function](#vaughan-identity-for-the-mobius-function) gives a [type I sum](analytic-number-theory.md#type-i-sum) or a [type II sum](analytic-number-theory.md#type-ii-sum) of modulus at least $\delta X/4$. The first is $\sum_{d\leq UV}c_d\sum_{k\leq X/d}f(dk)$, with $c_d=\sum_{bc=d,b\leq U,c\leq V}\mu(b)\mu(c)$. The second is $\sum_{d>V,w>U,dw\leq X}a_d\mu(w)f(dw)$, with $a_d=\sum_{c\mid d,c>V}\mu(c)$. Both coefficient sequences are bounded by the [divisor function](#divisor-function). Thus correlation forces either detection by small-modulus periodic indicators or a large multiplicatively organized [bilinear sum](analytic-number-theory.md#bilinear-sum), without claiming that $f$ itself is literally periodic or multiplicative.

##### Vaughan identity proof

↑ **Parent:** [Vaughan's identity](#vaughan-s-identity)

For [Dirichlet convolution](#dirichlet-convolution), let $\mathbf1(n)=1$ and $\epsilon(n)=1_{n=1}$. [Prime factorization](#fundamental-theorem-of-arithmetic) gives $\mu*\mathbf1=\epsilon$ and $\Lambda*\mathbf1=\log$. With subscripts denoting truncation at $U,V$,

$$
\begin{aligned}
\mu*\log&=\Lambda,\\
\mu_{>U}*\mathbf1*\Lambda_{>V}
&=(\epsilon-\mu_{\leq U}*\mathbf1)*\Lambda_{>V}\\
&=\Lambda_{>V}-\mu_{\leq U}*\log+\mu_{\leq U}*\mathbf1*\Lambda_{\leq V}.
\end{aligned}
$$

Rearranging proves the [Vaughan identity](#vaughan-s-identity).

### Prime omega function

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_omega_function)

The [prime omega function](#prime-omega-function) $\omega(n)$ counts the distinct [prime factors](#prime-factor) of a [positive integer](#positive-integer) $n$, so it is the [cardinality](set-theory.md#cardinality) of the [prime support of an integer](#prime-support-of-an-integer) $P(n)$. For a [prime factorization](#fundamental-theorem-of-arithmetic) with distinct [prime numbers](#prime-number) $p_1,\ldots,p_r$ and positive exponents,

$$
n=p_1^{a_1}\cdots p_r^{a_r}\quad\Longrightarrow\quad
\omega(n)=r=\sum_{p\mid n}1.
$$

At $n=1$ there are no [prime factors](#prime-factor), so the [empty sum](arithmetic.md#empty-sum) gives $\omega(1)=0$. The [total number of prime factors](#total-number-of-prime-factors) instead gives $\Omega(n)=\sum_i a_i$. [Darij Grinberg, MIT 18.781, Floor and arithmetic functions, Definition 2.1.2: distinct and repeated prime factors](https://darijgrinberg.gitlab.io/floor.pdf)

For $72=2^3\cdot3^2$, the [prime support of an integer](#prime-support-of-an-integer) is $\{2,3\}$ and $\omega(72)=2$. The comparison examples give $\omega(30)=3$, $\omega(32)=1$ and $\omega(36)=2$. Raising an existing [prime factor](#prime-factor) to a higher power does not affect the [prime omega function](#prime-omega-function): $\omega(p^k)=1$ for a [prime number](#prime-number) $p$ and $k\ge1$. Thus the [prime omega function](#prime-omega-function) is a [strongly additive arithmetic function](#strongly-additive-arithmetic-function), with

$$
\omega(ab)=\omega(a)+\omega(b)\quad\text{if }\gcd(a,b)=1.
$$

The reason is that [coprime integers](#coprime-integers) have disjoint [prime supports of an integer](#prime-support-of-an-integer). For arbitrary [positive integers](#positive-integer), their [prime support of an integer](#prime-support-of-an-integer) combines by [set union](set.md#set-union), and the shared [prime factors](#prime-factor) are exactly those of the [greatest common divisor](#greatest-common-divisor). Counting this [set union](set.md#set-union) gives the more general identity

$$
\omega(ab)=\omega(a)+\omega(b)-\omega(\gcd(a,b)).
$$

For $a=12$, $b=18$, both [prime supports of an integer](#prime-support-of-an-integer) are $\{2,3\}$ and $\gcd(a,b)=6$, so $\omega(216)=2+2-2=2$. In particular $\omega(4)=1\ne2=\omega(2)+\omega(2)$: the [prime omega function](#prime-omega-function) is not a [completely additive arithmetic function](#completely-additive-arithmetic-function).

The [prime omega function](#prime-omega-function) is useful for counting choices involving distinct [prime factors](#prime-factor). Every [squarefree divisor](#squarefree-divisor) of $n$ chooses a [subset](set.md#subset) of its [prime support of an integer](#prime-support-of-an-integer), so there are $2^{\omega(n)}$ [squarefree divisors](#squarefree-divisor). For $72$, this gives $2^2=4$, namely $1,2,3,6$. Also $\omega(\operatorname{rad}(n))=\omega(n)$, because the [radical of an integer](#radical-of-an-integer) keeps exactly that [prime support of an integer](#prime-support-of-an-integer). The [total number of prime factors](#total-number-of-prime-factors) records what this count discards, and the two counts agree exactly on [squarefree integers](#squarefree-integer).

#### Three to the distinct-prime-factor count

↑ **Parent:** [Prime omega function](#prime-omega-function)

The [multiplicative arithmetic function](#multiplicative-function) $f(n)=3^{\omega(n)}$ counts assignments of three labels to each distinct [prime factor](#prime-factor). It also counts pairs of [squarefree divisors](#squarefree-divisor) whose [least common multiple](#least-common-multiple) is the [radical of an integer](#radical-of-an-integer) $n$.

##### Summatory bound for three to the prime omega

↑ **Parent:** [Three to the distinct-prime-factor count](#three-to-the-distinct-prime-factor-count)

The [Euler product](analytic-number-theory.md#euler-product) and [Mertens second theorem](analytic-number-theory.md#mertens-second-theorem) give $\sum_{n\leq D}3^{\omega(n)}/n\ll\log^3D$. The [log-weighted convolution bound for three to the prime omega](#log-weighted-convolution-bound-for-three-to-the-prime-omega), with the [Chebyshev estimate](#chebyshev-estimate) $\psi(y)\ll y$, then gives $\sum_{\sqrt D\leq n\leq D}3^{\omega(n)}\ll D\log^2D$. A direct bound for the full range follows from $3^{\omega(n)}\leq\tau_3(n)$, where $\tau_3(n)=\#\{(a,b,c):abc=n\}$:

$$
\sum_{n\leq D}3^{\omega(n)}\leq\sum_{abc\leq D}1\leq D\sum_{a\leq D}\frac1a\sum_{b\leq D}\frac1b\ll D\log^2D.
$$

##### Log-weighted convolution bound for three to the prime omega

↑ **Parent:** [Three to the distinct-prime-factor count](#three-to-the-distinct-prime-factor-count)

For $f(n)=3^{\omega(n)}$,

$$
f(n)\log n\leq3(f*\Lambda)(n).
$$

If $p^a\Vert n$, its contribution to $(f*\Lambda)(n)$ is $f(n)(a-1+1/3)\log p$. Since $3(a-1+1/3)\geq a$, summing over the [prime factors](#prime-factor) proves the bound. Here $*$ is [Dirichlet convolution](#dirichlet-convolution) and $\Lambda$ is the [Von Mangoldt function](#von-mangoldt-function).

<h3 id="mobius-function">Möbius function</h3>

↑ **Parent:** [Arithmetic function](#arithmetic-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Möbius_function)

The [Möbius function](#mobius-function) assigns a cancellation weight to each [positive integer](#positive-integer):

$$
\mu(n)=\begin{cases}
1&n=1,\\
(-1)^r&n=p_1\cdots p_r\text{ with distinct primes }p_1,\ldots,p_r,\\
0&p^2\mid n\text{ for some prime }p.
\end{cases}
$$

Thus a [squarefree integer](#squarefree-integer) contributes a sign determined by its number of distinct [prime factors](#prime-factor); a repeated [prime factor](#prime-factor) makes the weight zero. This packages the alternating signs of [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle) into an [arithmetic function](#arithmetic-function). [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.1.2](https://darijgrinberg.gitlab.io/floor.pdf)

For example, $\mu(2)=\mu(3)=-1$, $\mu(6)=1$, and $\mu(30)=(-1)^3=-1$, since $30=2\cdot3\cdot5$. In contrast, $\mu(4)=\mu(12)=\mu(60)=0$: all three have the square of the [prime number](#prime-number) $2$ as a [divisor](#divisor). On [prime powers](#prime-power), $\mu(p)=-1$ and $\mu(p^a)=0$ for $a\geq2$.

The [Möbius function](#mobius-function) is a [multiplicative function](#multiplicative-function): for [coprime integers](#coprime-integers), their [prime factors](#prime-factor) are disjoint, so either a squared [prime factor](#prime-factor) forces both sides of $\mu(mn)=\mu(m)\mu(n)$ to vanish, or the counts of distinct [prime factors](#prime-factor) add and their signs multiply. It is not a [completely multiplicative function](#completely-multiplicative-function), since $\mu(4)=0\ne1=\mu(2)^2$. Its [Möbius divisor-sum identity](#mobius-divisor-sum-identity) makes it the inverse of the [constant-one arithmetic function](#constant-one-arithmetic-function) under [Dirichlet convolution](#dirichlet-convolution): $\mu*\mathbf1=\varepsilon$, the [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution). This is why the small set of weights $-1,0,1$ can undo an entire [divisor sum](#divisor-sum).

<h4 id="mobius-divisor-sum-identity">Möbius divisor-sum identity</h4>

↑ **Parent:** [Möbius function](#mobius-function)

For every [positive integer](#positive-integer) $n$, the [divisor sum](#divisor-sum) of the [Möbius function](#mobius-function) is

$$
\sum_{d\mid n}\mu(d)=\begin{cases}1&n=1,\\0&n>1.\end{cases}
$$

The sum includes all positive [integer divisors](#divisor), but only [squarefree divisors](#squarefree-divisor) contribute. Equivalently, $\mu*\mathbf1=\varepsilon$ under [Dirichlet convolution](#dirichlet-convolution), where $\mathbf1$ is the [constant-one arithmetic function](#constant-one-arithmetic-function) and $\varepsilon$ is the [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution). [Darij Grinberg, MIT 18.781 lecture notes, Propositions 2.4.6 and 2.4.7](https://darijgrinberg.gitlab.io/floor.pdf)

Each [squarefree divisor](#squarefree-divisor) chooses a [subset](set.md#subset) of the distinct [prime factors](#prime-factor) of $n$, contributing $(-1)^r$ when that [subset](set.md#subset) has $r$ elements. Expanding a product therefore gives

$$
\sum_{d\mid n}\mu(d)=\prod_{p\mid n}(1-1).
$$

For $n>1$ at least one [prime factor](#prime-factor) occurs, so the product is zero. At $n=1$ it is an [empty product](arithmetic.md#empty-product), equal to one. This is the same alternating cancellation that drives [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle).

For $30=2\cdot3\cdot5$, all eight positive [integer divisors](#divisor) are [squarefree integers](#squarefree-integer), giving

$$
\mu(1)+\mu(2)+\mu(3)+\mu(5)+\mu(6)+\mu(10)+\mu(15)+\mu(30)
=1-1-1-1+1+1+1-1=0.
$$

Pair each [subset](set.md#subset) not containing $2$ with the [subset](set.md#subset) obtained by inserting $2$: $(1,2),(3,6),(5,10),(15,30)$. Each pair cancels. The same nonzero terms occur for $60$, because its [squarefree divisors](#squarefree-divisor) are still the [integer divisors](#divisor) of $30$; its other [integer divisors](#divisor) have [Möbius function](#mobius-function) value zero.

<a id="image-the-eight-integer-divisors-of-30-form-a-cube-of-subsets-of-its-prime-factors-adding-one-prime-factor-reverses-the-mobius-function-sign-and-all-contributions-cancel"></a>
![](mobius-divisor-cancellation.png)

**[Figure 21](#image-the-eight-integer-divisors-of-30-form-a-cube-of-subsets-of-its-prime-factors-adding-one-prime-factor-reverses-the-mobius-function-sign-and-all-contributions-cancel). The eight integer divisors of 30 form a cube of subsets of its prime factors; adding one prime factor reverses the Möbius function sign, and all contributions cancel**.

The [Möbius divisor-sum identity](#mobius-divisor-sum-identity) is the cancellation behind [Möbius inversion](#mobius-inversion-formula) and reciprocal [Dirichlet series](analytic-number-theory.md#dirichlet-series): aggregation over [integer divisors](#divisor) has an exact inverse.

<h4 id="mobius-harmonic-logarithmic-moments">Möbius harmonic logarithmic moments</h4>

↑ **Parent:** [Möbius function](#mobius-function)

Put $A_j(x)=\sum_{d\leq x}\mu(d)\log^j(x/d)/d$. The elementary estimates are

$$
A_0(x)=O(1),\qquad A_1(x)=O(1),\qquad A_2(x)=2\log x+O(1).
$$

The identities $\sum_d\mu(d)\lfloor x/d\rfloor=1$ and $\sum_d\mu(d)H_{\lfloor x/d\rfloor}/d=1$ give the first two bounds. Convolve the [harmonic divisor sum](#harmonic-divisor-sum) with $\mu(d)/d$: because $\mu*\tau=\mathbf1$, its left side is $H_{\lfloor x\rfloor}$. Thus $\tfrac12A_2+2\gamma A_1+cA_0=\log x+O(1)$. The summed error is $O(x^{-1/2}\sum_{d\leq x}d^{-1/2}\log(2x/d))=O(1)$.

This elementary smoothing argument is used in [Selberg's original proof](https://www.math.lsu.edu/~mahlburg/teaching/handouts/2014-7230/Selberg-ElemPNT1949.pdf) and [Ramaré's sieve lectures, Lemma 4.2](https://ramare-olivier.github.io/Maths/LecturesEasyChennai.pdf).

<h4 id="mobius-inversion-formula">Möbius inversion formula</h4>

↑ **Parent:** [Möbius function](#mobius-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Möbius_inversion_formula)

[Möbius inversion](#mobius-inversion-formula) recovers an [arithmetic function](#arithmetic-function) from its [divisor sum](#divisor-sum). For [arithmetic functions](#arithmetic-function) $f,g$, the following statements are equivalent, with each equality required for every [positive integer](#positive-integer) $n$:

$$
g(n)=\sum_{d\mid n}f(d)
\quad\Longleftrightarrow\quad
f(n)=\sum_{d\mid n}\mu(d)g(n/d).
$$

Here $d$ ranges over positive [integer divisors](#divisor) of $n$ and $\mu$ is the [Möbius function](#mobius-function). No [multiplicativity](#multiplicativity-of-an-arithmetic-function) assumption is needed, and both sums are finite. The right side can also be written $\sum_{d\mid n}\mu(n/d)g(d)$ by exchanging complementary [integer divisors](#divisor). [Darij Grinberg, MIT 18.781 lecture notes, Theorem 2.5.1 and Proposition 2.5.2](https://darijgrinberg.gitlab.io/floor.pdf)

The [divisor sum](#divisor-sum) $g(n)$ bundles $f(n)$ together with values at smaller [integer divisors](#divisor). [Möbius inversion](#mobius-inversion-formula) subtracts aggregates indexed by one distinct [prime factor](#prime-factor), adds those indexed by two, and continues with the alternating signs of [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle). A [divisor](#divisor) containing a squared [prime factor](#prime-factor) receives weight zero. The [Möbius divisor-sum identity](#mobius-divisor-sum-identity) ensures that every unwanted contribution cancels exactly.

In [Dirichlet convolution](#dirichlet-convolution) notation, $g=f*\mathbf1$ and $\mu*\mathbf1=\varepsilon$, where $\mathbf1$ is the [constant-one arithmetic function](#constant-one-arithmetic-function) and $\varepsilon$ is the [Identity for Dirichlet convolution](#identity-for-dirichlet-convolution). [Associativity](algebra.md#associative-property) and [commutativity](algebra.md#commutativity) give the short proof:

$$
\mu*g=\mu*(\mathbf1*f)=(\mu*\mathbf1)*f=\varepsilon*f=f.
$$

Convolving $f=\mu*g$ with $\mathbf1$ proves the reverse implication. At $n=1$, the formula reduces to $f(1)=g(1)$ because $\mu(1)=1$.

For a worked example, take $f(n)=\varphi(n)$, [Euler's totient function](#euler-totient-function). The [totient divisor-sum identity](#totient-divisor-sum-identity) says that $g(n)=n$, the [identity arithmetic function](#identity-arithmetic-function):

$$
g(12)=\varphi(1)+\varphi(2)+\varphi(3)+\varphi(4)+\varphi(6)+\varphi(12)
=1+1+2+2+2+4=12.
$$

This identity comes from classifying the [integers](#integer) $1,\ldots,n$ by their [greatest common divisor](#greatest-common-divisor) with $n$: the group with $\gcd(j,n)=h$ has $\varphi(n/h)$ members, since $j/h$ and $n/h$ are [coprime integers](#coprime-integers). Summing the group sizes gives $n$, as detailed under [totient divisor-sum identity](#totient-divisor-sum-identity).

Now undo this aggregation with the [Möbius function](#mobius-function):

$$
\begin{aligned}
\varphi(12)&=\mu(1)12+\mu(2)6+\mu(3)4+\mu(4)3+\mu(6)2+\mu(12)1\\
&=12-6-4+0+2+0=4.
\end{aligned}
$$

The nonzero terms use $d=1,2,3,6$; $d=4,12$ vanish because they contain the square of the [prime number](#prime-number) $2$. The four surviving [integers](#integer) [coprime](#coprime-integers) to $12$ are $1,5,7,11$.

<a id="image-a-divisor-sum-aggregates-euler-s-totient-function-values-to-12-while-mobius-inversion-recovers-the-four-integers-coprime-to-12"></a>
![](mobius-inversion-totient.png)

**[Figure 22](#image-a-divisor-sum-aggregates-euler-s-totient-function-values-to-12-while-mobius-inversion-recovers-the-four-integers-coprime-to-12). A divisor sum aggregates Euler's totient function values to 12, while Möbius inversion recovers the four integers coprime to 12**.

This example also reveals why [Möbius inversion](#mobius-inversion-formula) is useful: it turns an easy count of all objects into a count satisfying a [coprimality](#coprime-integers) restriction. Expanding over [subsets](set.md#subset) of distinct [prime factors](#prime-factor) gives

$$
\varphi(n)=\sum_{d\mid n}\mu(d)\frac nd
=n\prod_{p\mid n}\left(1-\frac1p\right).
$$

The product is [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle) over multiples of the [prime factors](#prime-factor). For $12$, it gives $12(1-1/2)(1-1/3)=4$. More generally, whenever a counting problem produces a [divisor sum](#divisor-sum), [Möbius inversion](#mobius-inversion-formula) lets that aggregate be reversed without solving a new system of [equations](algebra.md#equation).

#### Mertens function

↑ **Parent:** [Möbius function](#mobius-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Mertens_function)

The Mertens function is the summatory [Möbius function](#mobius-function)

$$
M(x)=\sum_{n\leq x}\mu(n).
$$

##### Prime number asymptotic from Mertens cancellation

↑ **Parent:** [Mertens function](#mertens-function)

Let $\Delta(N)=\sum_{n\le N}(\tau(n)-\log n-2\gamma)$. The [Möbius divisor-sum identity](#mobius-divisor-sum-identity) and the [Von Mangoldt divisor identity](#von-mangoldt-divisor-identity) give $\mu*\tau=\mathbf1$ and $\mu*\log=\Lambda$, so

$$
\psi(N)=N-2\gamma-\sum_{d\le N}\mu(d)\Delta(\lfloor N/d\rfloor).
$$

Here $*$ is [Dirichlet convolution](#dirichlet-convolution). The [divisor summatory asymptotic](#divisor-summatory-asymptotic) bounds the terms with $d\le N/K$ in absolute value by $O(N/\sqrt K)$. For $d>N/K$, group by $j=\lfloor N/d\rfloor<K$: the remaining sum is $\sum_{j<K}\Delta(j)(M(N/j)-M(N/(j+1)))=o_K(N)$. First let $N$ tend to infinity, then $K$ tend to infinity. This proves the [Second Chebyshev function](#second-chebyshev-function) asymptotic from cancellation of the [Mertens function](#mertens-function).

##### Mertens bound from a log-integrable Chebyshev error

↑ **Parent:** [Mertens function](#mertens-function)

Suppose $\Psi(x)=x+O(xE(x))$ and $\sum_{j\geq0}\sup_{2^j\leq u<2^{j+1}}|E(u)|<\infty$. The [Möbius divisor-sum identity](#mobius-divisor-sum-identity) gives $\sum_{d\leq x}\mu(d)/d=O(1)$. The exact [Dirichlet convolution](#dirichlet-convolution) identity $\mu\log=-\mu*\Lambda$ then gives $\sum_{n\leq x}\mu(n)\log n=O(x)$, because its error is a convergent dyadic harmonic sum. Since $\sum_{n\leq x}\log(x/n)=O(x)$, the displayed [Mertens function](#mertens-function) bound follows. The classical [Prime number theorem](analytic-number-theory.md#prime-number-theorem) error $E(x)=e^{-c\sqrt{\log x}}$ meets the summability condition. This is a deduction from the Chebyshev error itself, without a separate estimate for the reciprocal [zeta function](analytic-number-theory.md#riemann-zeta-function).

##### Mertens function bound from the classical zeta zero-free region

↑ **Parent:** [Mertens function](#mertens-function)

The classical [zero-free region of the Riemann zeta function](analytic-number-theory.md#zero-free-region-of-the-riemann-zeta-function) and a [truncated Perron formula](analytic-number-theory.md#truncated-perron-formula) give

$$
M(x)\ll x\exp(-c\sqrt{\log x})
$$

for some absolute constant $c>0$. Take contour height $T=\exp(\sqrt{\log x})$ and move the Perron contour to $\Re s=1-c_1/\log T$.

## Analytic number theory

↑ **Parent:** [Number theory](number-theory.md)

[This section is present in another page, follow this link to view it.](analytic-number-theory.md)

## Exponentiation by squaring

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exponentiation_by_squaring)

Exponentiation by squaring computes an [integer](#integer) power by reading the exponent's [binary expansion](arithmetic.md#binary-expansion). Appending a [binary digit](#binary-digit) $b$ to a prefix of value $p$ replaces $p$ by $2p+b$, so the corresponding power changes by

$$
a^{2p+b}=(a^p)^2a^b,\qquad b\in\{0,1\}.
$$

Each new digit requires one squaring and, only for digit one, one further [multiplication](arithmetic.md#multiplication). The number of digits grows with the [logarithm](calculus.md#logarithm) of the exponent, making this useful for [modular exponentiation](#modular-exponentiation), [primality testing](computer-science.md#primality-testing), and powers of [matrices](vector-space.md#matrix) using [matrix multiplication](vector-space.md#matrix-multiplication).[Section 3.4, pp. 65–66: binary-prefix recurrence and repeated-squaring algorithm; p. 67: primality-testing application](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

For a concrete calculation, $13=(1101)_2=8+4+1$, so $3^{13}=3^8\cdot3^4\cdot3$. The **optimized left-to-right [algorithm](computer-science.md#algorithm) used here** instead keeps one accumulated power: initialize $r=3$ from the leading digit one, then process only the remaining digits $1,0,1$:

$$
\begin{aligned}
1&:\quad r=3,\\
11&:\quad r=3^2\cdot3=27,\\
110&:\quad r=27^2=729,\\
1101&:\quad r=729^2\cdot3=531441\cdot3=1594323.
\end{aligned}
$$

Thus **$3^{13}=1594323$**, using three squarings and two further [multiplications](arithmetic.md#multiplication), instead of twelve successive [multiplications](arithmetic.md#multiplication) starting at $3$.

<a id="image-reading-the-same-binary-expansion-computes-3-13-and-2-13-bmod17"></a>
![](binary-powering-prefix-and-modular-trace.png)

**[Figure 23](#image-reading-the-same-binary-expansion-computes-3-13-and-2-13-bmod17). Reading the same binary expansion computes $3^{13}$ and $2^{13}\bmod17$**. Each appended [binary digit](#binary-digit) changes the prefix value by $p\mapsto2p+b$. The ordinary-power row grows to $1594323$; the [modular exponentiation](#modular-exponentiation) row stores only remainders $2,8,13,15$. Both traces use three squarings and two further [multiplications](arithmetic.md#multiplication).

For a general positive [integer](#integer) $n=(b_{\ell-1}\cdots b_0)_2$ with leading digit $b_{\ell-1}=1$, set $r=a$ and, for $i=\ell-2,\ldots,0$, first replace $r$ by $r^2$, then multiply it by $a$ if $b_i=1$. Return $r$. This explicitly skips the leading digit's otherwise unnecessary operations on one. [A Computational Introduction to Number Theory and Algebra by Victor Shoup](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup) (Section 3.4, pp. 65–66) presents the version initialized at one and processing every digit; the optimization here makes the counting convention unambiguous.

The [loop invariant](computer-science.md#loop-invariant) is **$r=a^p$, where $p$ is the value of the digits already read**. Initially $p=1$ and $r=a$. If the next digit is $b$, then squaring and optionally multiplying give $r'=a^{2p+b}$, exactly the next prefix. At termination $p=n$. This proof uses [associativity](algebra.md#associative-property) of [multiplication](arithmetic.md#multiplication); it works in any [monoid](algebra.md#monoid), including [matrices](vector-space.md#matrix) with the [identity matrix](vector-space.md#identity-matrix) as [identity element](algebra.md#identity-element), and needs no [commutativity](algebra.md#commutativity) between different bases.

For $n=0$, return the [identity element](algebra.md#identity-element) without performing a [multiplication](arithmetic.md#multiplication). This is the empty-product convention $a^0=1$; if $a=0$, the [algorithm](computer-science.md#algorithm) therefore returns one for $0^0$ by convention, rather than resolving its meaning in every mathematical setting. Negative [integer](#integer) exponents require an [inverse element](algebra.md#inverse-element): compute $(a^{-1})^{-n}$, counting the inversion separately. Over the [integers](#integer), such an inverse generally leaves the [integers](#integer), and a zero base has no inverse.

### Binary powering multiplication count

↑ **Parent:** [Exponentiation by squaring](#exponentiation-by-squaring)

For the optimized left-to-right [exponentiation by squaring](#exponentiation-by-squaring) [algorithm](computer-science.md#algorithm), let $\ell=\lfloor\log_2 n\rfloor+1$ be the length of the [binary expansion](arithmetic.md#binary-expansion) of a positive [integer](#integer) $n$, and let $w=\operatorname{wt}(n)$ be its [Hamming weight](coding-theory.md#hamming-weight), the number of digits equal to one. There are exactly $\ell-1$ digits after the leading one, and exactly $w-1$ remaining ones. Therefore the count is

$$
S(n)=\ell-1,\qquad T(n)=w-1,\qquad C(n)=S(n)+T(n)=\ell+w-2.
$$

Here $S$ counts squarings and $T$ counts further [multiplications](arithmetic.md#multiplication) by the base; **every squaring counts as one [multiplication](arithmetic.md#multiplication) in $C$**. Assignment, digit reading, and any inversion are outside this count. The formula includes $n=1$, which requires zero [multiplications](arithmetic.md#multiplication); define $C(0)=0$ separately.

For a fixed length $\ell$, the bounds are $\ell-1\leq C(n)\leq2\ell-2$. A [power of two](#power-of-two) reaches the lower bound because its [Hamming weight](coding-theory.md#hamming-weight) is one; $n=2^\ell-1$ reaches the upper bound because all digits are one. For $n=13$, $\ell=4$ and $w=3$, giving $C(13)=5$. Thus the [arithmetic operation](numerical-analysis.md#arithmetic-operation) count is $O(\log(n+1))$ in [Big O notation](real-analysis.md#big-o-notation), but inputs of similar magnitude can have different counts.

<a id="image-exact-multiplication-counts-for-optimized-exponentiation-by-squaring-depend-on-binary-length-and-hamming-weight"></a>
![](binary-powering-multiplication-count.png)

**[Figure 24](#image-exact-multiplication-counts-for-optimized-exponentiation-by-squaring-depend-on-binary-length-and-hamming-weight). Exact multiplication counts for optimized exponentiation by squaring depend on binary length and Hamming weight**. For positive exponents through $63$, dots show $C(n)=\ell+\operatorname{wt}(n)-2$, including each squaring. The dashed curves bound all counts at each binary length. Successive multiplication needs $n-1$ operations. The second panel compares squarings and further [multiplications](arithmetic.md#multiplication) for exponents $8,13,15,16,31$. These are exact counts, not timing measurements.

This is a count for the specified [algorithm](computer-science.md#algorithm), not a claim that it always minimizes [multiplications](arithmetic.md#multiplication) among all methods. For instance, at $n=15$ the count is six, but the powers with exponents $1,2,3,6,12,15$ can be built in five [multiplications](arithmetic.md#multiplication): square, multiply by $a$, square, square, then multiply by the already stored $a^3$. Saving operations this way uses a different schedule and stored intermediate powers.

### Modular exponentiation

↑ **Parent:** [Exponentiation by squaring](#exponentiation-by-squaring)

Modular exponentiation computes the [remainder](#remainder) $a^n\bmod m$ for an [integer](#integer) base $a$, a [nonnegative integer](arithmetic.md#natural-number) exponent $n$, and, here, an [integer](#integer) modulus $m\geq2$. It applies [exponentiation by squaring](#exponentiation-by-squaring) while reducing after **each** [multiplication](arithmetic.md#multiplication), including each squaring. The result is the unique representative in $\{0,\ldots,m-1\}$. There is no requirement that the base be [coprime](#coprime-integers) to the modulus when the exponent is nonnegative.[Section 3.4, pp. 64–66: canonical representatives, modular products, and nonnegative-exponent repeated squaring](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

Take $a=2$, $n=13=(1101)_2$, and $m=17$. Initialize $r=2$; the remaining digits give

$$
\begin{aligned}
11&:\quad 2^2\bmod17=4,\quad4\cdot2\bmod17=8,\\
110&:\quad 8^2\bmod17=64\bmod17=13,\\
1101&:\quad13^2\bmod17=169\bmod17=16,\quad16\cdot2\bmod17=15.
\end{aligned}
$$

Hence **$2^{13}\bmod17=15$**. The final operation multiplies $16$ by $2$, since the preceding square has already been reduced. The computation never needs to construct $2^{13}=8192$.

In general reduce the base first, $x=a\bmod m$. For $n>0$, initialize $r=x$ and process the remaining [binary digits](#binary-digit) with $r\leftarrow r^2\bmod m$, followed, for a digit one, by $r\leftarrow rx\bmod m$. The [loop invariant](computer-science.md#loop-invariant) is

$$
0\leq r<m,\qquad r\equiv a^p\pmod m,
$$

where $p$ is the processed prefix value. The congruence is preserved because [modular arithmetic](#modular-arithmetic) respects [multiplication](arithmetic.md#multiplication): if $u\equiv v\pmod m$, then $u^2\equiv v^2$ and $ux\equiv va\pmod m$. Thus changing representatives never changes the final [congruence class](#congruence-class).

Both factors in every product are less than $m$, so the unreduced product is less than $m^2$, and the stored result is again less than $m$. The same bounds hold for a gigantic exponent, such as $n=2^{1000}$: there are $1000$ squarings, each on bounded-size residues. For base two, the corresponding ordinary power would have $2^{1000}+1$ [binary digits](#binary-digit). The benefit is avoiding the huge ordinary power altogether, rather than constructing it and taking one final [remainder](#remainder). Initial reduction is essential when the supplied base is much larger than the modulus.

For $n=0$, return $1$ under the same empty-product convention as [exponentiation by squaring](#exponentiation-by-squaring). For $n=-k<0$, require $\gcd(a,m)=1$, find the [modular multiplicative inverse](#modular-multiplicative-inverse) $a^{-1}\bmod m$, and compute $(a^{-1})^k\bmod m$; the [extended Euclidean algorithm](#extended-euclidean-algorithm) can find that inverse. Its cost is separate from the positive-exponent [binary powering multiplication count](#binary-powering-multiplication-count). For example, $2^{-1}\equiv9\pmod{17}$, while $2^{-1}\bmod4$ is undefined because $2$ and $4$ are not [coprime](#coprime-integers).

A [reversible computation](computer-science.md#reversible-computation) gives the coherent [quantum modular exponentiation](quantum-theory.md#quantum-modular-exponentiation) used in [quantum order finding](quantum-theory.md#quantum-order-finding) and [discrete-logarithm Fourier sampling](quantum-theory.md#discrete-logarithm-fourier-sampling).

#### Bit cost of modular exponentiation

↑ **Parent:** [Modular exponentiation](#modular-exponentiation)

The [binary powering multiplication count](#binary-powering-multiplication-count) counts [arithmetic operations](numerical-analysis.md#arithmetic-operation). The [time complexity](computer-science.md#time-complexity) measured in operations on individual [bits](information-theory.md#bit) also depends on operand lengths. Put $L=\lfloor\log_2m\rfloor+1$, the binary length of the modulus, and let $\ell$ be the positive exponent's binary length. Stored residues use at most $L$ [bits](information-theory.md#bit), and an unreduced product uses at most $2L$ [bits](information-theory.md#bit).

With ordinary long [multiplication](arithmetic.md#multiplication) and [division with remainder](#euclidean-division), one modular product costs $O(L^2)$ operations on [bits](information-theory.md#bit). Combining that cost with $O(\ell)$ modular products gives

$$
\text{bit cost of the powering loop}=O(\ell L^2).
$$

This bound includes reductions in the loop, and assumes the base has already been reduced and the exponent is available as a [binary expansion](arithmetic.md#binary-expansion). Reading the exponent takes $O(\ell)$ additional work; initial reduction of a very long base depends on its input length, and an inverse for a negative exponent adds further work. More generally, if a modular product costs $R(L)$ operations on [bits](information-theory.md#bit), the powering loop costs $O(\ell R(L))$. Faster [multiplication](arithmetic.md#multiplication) and reduction methods can improve the quadratic bound.[Section 3.3.5, pp. 62–63, Theorem 3.3: operand-length costs; Section 3.4, p. 65: modular multiplication and powering bounds; Section 3.5, pp. 69–71: faster arithmetic](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

For ordinary [integer](#integer) powers with $|a|\geq2$, the output itself has $\lfloor n\log_2|a|\rfloor+1$ [binary digits](#binary-digit). Even writing it takes work proportional to that length. Consequently $O(\log(n+1))$ [multiplications](arithmetic.md#multiplication) does not imply $O(\log(n+1))$ operations on [bits](information-theory.md#bit): the operands grow during ordinary [exponentiation by squaring](#exponentiation-by-squaring), whereas [modular exponentiation](#modular-exponentiation) keeps them bounded by the modulus. A squaring or multiplication by a small fixed base can also cost less than a general product, so equal counts need not mean equal running times.

## Integer

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Integer)

An integer is a whole number, positive, negative, or zero.

### Repdigit

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Repdigit)

A [repdigit](#repdigit) is a positive integer whose base-$b$ expansion repeats one nonzero digit $d$. For $b\ge2$, $1\le d<b$ and $n\ge1$, the [finite geometric series](real-analysis.md#finite-geometric-series) gives $R_n=d(1+b+\cdots+b^{n-1})=d(b^n-1)/(b-1)$. For example, $5(10^n-1)/9$ has $n$ decimal digits, all equal to five.

Every [prime number](#prime-number) not dividing $b$ divides infinitely many such [repdigits](#repdigit). If it divides $d$, every length works. Otherwise, if it does not divide $b-1$, the [Fermat little theorem](#fermat-little-theorem) gives divisibility for lengths that are multiples of $p-1$, and division by $b-1$ is justified by its [modular inverse](#modular-multiplicative-inverse). If $p\mid b-1$, the sum is congruent to $dn$ modulo $p$, so lengths divisible by $p$ work instead. A prime dividing $b$ but not $d$ divides none, since $R_n\equiv d\pmod p$. This distinction prevents invalid cancellation of the geometric-sum denominator.

### Euclidean division

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_division)

For an [integer](#integer) $a$ and positive [integer](#integer) $b$, Euclidean division writes $a=bq+r$ with unique integer quotient $q$ and remainder $0\le r<b$. For $a\ge0$, repeated quotient-and-remainder steps yield the digits of a [base-p expansion](#base-p-expansion) when $b=p$. The uniqueness follows because the difference of two permitted remainders cannot be a nonzero multiple of $b$.

#### Remainder

↑ **Parent:** [Euclidean division](#euclidean-division)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Remainder)

For an [integer](#integer) $a$ and positive [integer](#integer) $b$, the remainder in [Euclidean division](#euclidean-division) is the unique [integer](#integer) $r$ in $0\leq r<b$ for which $a=bq+r$ with an [integer](#integer) $q$. It is not the full [quotient](arithmetic.md#quotient) $a/b$.

#### Long division

↑ **Parent:** [Euclidean division](#euclidean-division)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Long_division)

Repeated [division with remainder](#euclidean-division) that determines successive digits of a [quotient](arithmetic.md#quotient). To generate the fractional digits in base $b$, multiply the current [remainder](#remainder) by $b$, divide by the [denominator](#denominator), and keep the resulting [remainder](#remainder) for the next step.

### Integer interval

↑ **Parent:** [Integer](#integer)

A finite [integer interval](#integer-interval) is a set $\{a,a+1,\ldots,b\}$ with [integers](#integer) $a\leq b$. Its length is $b-a+1$. Infinite [integer intervals](#integer-interval) can also be defined by allowing one or both endpoints to be infinite; a bounded-gaps condition on words always quantifies over finite [integer intervals](#integer-interval).

### Positional notation

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positional_notation)

In positional notation of base $b$, a digit string $d_nd_{n-1}\cdots d_0$ represents $\sum_{j=0}^nd_jb^j$.

#### Decimal expansion

↑ **Parent:** [Positional notation](#positional-notation)

A nonnegative integer's [decimal expansion](#decimal-expansion) uses digits $0\leq a_i\leq9$. Testing divisibility reduces this polynomial in ten modulo the divisor: for example $10\equiv-1\pmod{11}$ makes divisibility by eleven equivalent to vanishing of the alternating digit sum.

#### Hereditary base representation

↑ **Parent:** [Positional notation](#positional-notation)

A [hereditary base representation](#hereditary-base-representation) expands not only the number in base $b$, but also every exponent recursively in that same base. Changing the base at every depth defines the Goodstein base-change operation; replacing it by omega defines an [ordinal rank of a Goodstein term](#ordinal-rank-of-a-goodstein-term).

##### Goodstein sequence

↑ **Parent:** [Hereditary base representation](#hereditary-base-representation)

Start at base two. At each nonzero step, change every base occurrence in the [hereditary base representation](#hereditary-base-representation) to the next base and subtract one. Although the natural-number terms can grow, their [ordinal ranks of a Goodstein term](#ordinal-rank-of-a-goodstein-term) decrease strictly. Keep zero fixed once it is reached.

<h6 id="goodstein-s-theorem">Goodstein's theorem</h6>

↑ **Parent:** [Goodstein sequence](#goodstein-sequence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Goodstein's_theorem)

Every [Goodstein sequence](#goodstein-sequence) reaches zero. Before zero, the [ordinal rank of a Goodstein term](#ordinal-rank-of-a-goodstein-term) of each step is strictly smaller than the preceding one. An infinite [sequence](real-analysis.md#sequence) would contradict [well-foundedness](set-theory.md#well-founded-relation) of the [ordinals](set-theory.md#ordinal) below [epsilon zero](set-theory.md#epsilon-zero).

###### Ordinal rank of a Goodstein term

↑ **Parent:** [Goodstein sequence](#goodstein-sequence)

Replacing every base occurrence by omega in a [hereditary base representation](#hereditary-base-representation) gives a [Cantor normal form](set-theory.md#cantor-normal-form) below [epsilon zero](set-theory.md#epsilon-zero). Hereditary base change preserves this [ordinal](set-theory.md#ordinal) expression, and subtraction of one lowers it strictly. The [ordinal](set-theory.md#ordinal) is a termination measure even when the natural-number value increases.

###### Goodstein function

↑ **Parent:** [Goodstein sequence](#goodstein-sequence)

The [Goodstein function](#goodstein-function) records the least step at which the [Goodstein sequence](#goodstein-sequence) from a given initial number reaches zero. With the initial step numbered zero, its values on $0,1,2,3$ are $0,1,3,5$. [Goodstein's theorem](#goodstein-s-theorem) makes this effective termination-time [function](function.md) total.

#### Base-p expansion

↑ **Parent:** [Positional notation](#positional-notation)

For an integer base $p\ge2$, a nonnegative [integer](#integer) has a finite positional representation with digits $k_i\in\{0,\ldots,p-1\}$. Repeated [Euclidean division](#euclidean-division) gives the digits uniquely; appending zero high-place digits has no effect. The base need not be prime for uniqueness, but a prime base is useful in [Lucas theorem](combinatorics.md#lucas-s-theorem) and modular [binomial coefficients](combinatorics.md#binomial-coefficient).

#### Binary numeral system

↑ **Parent:** [Positional notation](#positional-notation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_numeral_system)

The binary numeral system is [positional notation](#positional-notation) of base two, using the digits zero and one.

##### Binary digit

↑ **Parent:** [Binary numeral system](#binary-numeral-system)

A [binary digit](#binary-digit) is a zero or one in the base-two positional representation of an [integer](#integer). The sum $s_2(n)=\sum_jb_j$ determines the [Thue–Morse sequence](real-analysis.md#thue-morse-sequence) and is the [Hamming weight](coding-theory.md#hamming-weight) of the binary representation.

#### Decimal

↑ **Parent:** [Positional notation](#positional-notation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Decimal)

The decimal numeral system is [positional notation](#positional-notation) in base ten.

##### Decimal representation

↑ **Parent:** [Decimal](#decimal)

A decimal representation is a [positional notation](#positional-notation) of base ten.

###### Terminating decimal

↑ **Parent:** [Decimal representation](#decimal-representation)

A [decimal representation](#decimal-representation) with only finitely many nonzero fractional digits. A [reduced fraction](#reduced-fraction) has this property exactly when its [denominator](#denominator) has no [prime factors](#prime-factor) other than two and five. The zero tail is distinguished from the genuine repeating block measured by [decimal period from multiplicative order](#decimal-period-from-multiplicative-order).

### Positive integer

↑ **Parent:** [Integer](#integer)

A positive integer is an [integer](#integer) greater than zero.

#### Power of two

↑ **Parent:** [Positive integer](#positive-integer)

In this [positive integer](#positive-integer) context, a [power of two](#power-of-two) is $2^k$ for a [nonnegative integer](arithmetic.md#natural-number) $k$, giving $1,2,4,8,\ldots$. Allowing negative or real [exponents](arithmetic.md#exponent) gives a broader meaning of [exponentiation](arithmetic.md#exponentiation), which is not intended in the integer divisibility criteria here.

#### Perfect number

↑ **Parent:** [Positive integer](#positive-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_number)

A [positive integer](#positive-integer) whose [proper-divisor sum](#proper-divisor-sum) equals itself; equivalently, its [sum-of-divisors function](#sum-of-divisors-function) satisfies $\sigma(n)=2n$. For example, $28=1+2+4+7+14$.

#### Deficient number

↑ **Parent:** [Positive integer](#positive-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Deficient_number)

A [positive integer](#positive-integer) whose [proper-divisor sum](#proper-divisor-sum) is smaller than itself; equivalently, its [sum-of-divisors function](#sum-of-divisors-function) satisfies $\sigma(n)<2n$. For example, $s(8)=7<8$; also $s(1)=0<1$.

#### Abundant number

↑ **Parent:** [Positive integer](#positive-integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Abundant_number)

A [positive integer](#positive-integer) whose [proper-divisor sum](#proper-divisor-sum) exceeds itself; equivalently, its [sum-of-divisors function](#sum-of-divisors-function) satisfies $\sigma(n)>2n$. For example, $s(12)=16>12$.

### Parity (mathematics)

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity_(mathematics))

The parity of an [integer](#integer) records whether it is divisible by two.

#### Odd integer

↑ **Parent:** [Parity (mathematics)](#parity-mathematics)

An odd integer is not divisible by two; equivalently, it has the form $2k+1$.

#### Even number

↑ **Parent:** [Parity (mathematics)](#parity-mathematics)

An integer is even when it is divisible by two.

#### Odd number

↑ **Parent:** [Parity (mathematics)](#parity-mathematics)

An integer is odd when it is not divisible by two.

### Square-free integer

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square-free_integer)

A [positive integer](#positive-integer) $n$ is **square-free** when no [square number](#square-number) greater than one is a [divisor](#divisor) of $n$. It suffices to exclude squares of [prime numbers](#prime-number); equivalently, every [prime valuation](#prime-valuation) is zero or one:

$$
n\text{ is square-free}\quad\Longleftrightarrow\quad
p^2\nmid n\text{ for every prime }p
\quad\Longleftrightarrow\quad v_p(n)\in\{0,1\}\text{ for every prime }p.
$$

Thus the [prime factorization](#fundamental-theorem-of-arithmetic) of a [square-free integer](#square-free-integer) is a [product](arithmetic.md#product-of-numbers) of distinct [prime factors](#prime-factor), with no repetitions. One is included: its [prime factorization](#fundamental-theorem-of-arithmetic) is an [empty product](arithmetic.md#empty-product) and all its [prime valuations](#prime-valuation) are zero. These equivalent tests are stated in Grinberg's notes. [Darij Grinberg, MIT 18.781, Floor and arithmetic functions, Definition 2.1.2 and footnote 6](https://darijgrinberg.gitlab.io/floor.pdf)

For signed [integers](#integer), extend the definition by requiring $|n|$ to be a [square-free integer](#square-free-integer), where $|n|$ denotes [absolute value](real-analysis.md#absolute-value). Hence $-30$ and both $1,-1$ qualify. Zero does not: every [prime number](#prime-number) has its square as a [divisor](#divisor) of zero. The [Möbius function](#mobius-function) and [radical of an integer](#radical-of-an-integer) below use their existing [positive integer](#positive-integer) domains, so apply them to $|n|$ when handling a negative [integer](#integer).

For example, $30=2\cdot3\cdot5$ is a [square-free integer](#square-free-integer), whereas $12=2^2\cdot3$ is not, because $4\mid12$ and $v_2(12)=2$. Being a [composite number](#composite-number) causes no problem: $6,10,15$ are all [square-free integers](#square-free-integer). A [square-free integer](#square-free-integer) need not be [coprime](#coprime-integers) to another [integer](#integer): $6$ and $10$ are both [square-free integers](#square-free-integer) but have [greatest common divisor](#greatest-common-divisor) two. In fact the only signed [integers](#integer) [coprime](#coprime-integers) to every [integer](#integer) are $1,-1$, since $\gcd(n,n)=|n|$.

<a id="image-exact-square-free-integer-classification-of-the-integers-from-one-to-sixty"></a>
![](coprime-squarefree-integers-square-sieve.png)

**[Figure 25](#image-exact-square-free-integer-classification-of-the-integers-from-one-to-sixty). Exact square-free integer classification of the integers from one to sixty**. Green cells are [square-free integers](#square-free-integer); each red cell displays a [prime number](#prime-number) square that divides its label, choosing the smallest such [prime number](#prime-number). Only $4,9,25,49$ need testing in this range. There are $37$ green cells. This original finite arithmetic diagram is an exact enumeration, not a measurement or an assertion about a limiting frequency.

For [positive integers](#positive-integer) $a,b$, the useful [product](arithmetic.md#product-of-numbers) criterion is

$$
ab\text{ is square-free}\quad\Longleftrightarrow\quad
a,b\text{ are square-free and }\gcd(a,b)=1.
$$

The proof outline is just [addition](arithmetic.md#addition) of [prime valuations](#prime-valuation): $v_p(ab)=v_p(a)+v_p(b)$ can stay at most one only if neither input repeats a [prime factor](#prime-factor) and no [prime factor](#prime-factor) occurs in both. Thus $6\cdot5=30$ is a [square-free integer](#square-free-integer), but $6\cdot10=60$ is not. An equivalent characterization is that **every** factorization $n=ab$ into [positive integers](#positive-integer) has [coprime](#coprime-integers) factors. If $p^2\mid n$, the factorization $n=p(n/p)$ supplies two factors sharing $p$; conversely, a shared [prime factor](#prime-factor) forces its square to divide $n$. For $30$, the unordered factor pairs $(1,30),(2,15),(3,10),(5,6)$ all have [greatest common divisor](#greatest-common-divisor) one; for $12$, the pair $(2,6)$ fails.

Two existing [arithmetic functions](#arithmetic-function) turn the definition into practical tests:

$$
\operatorname{rad}(n)=n\quad\Longleftrightarrow\quad n\text{ is square-free},\qquad
\mu(n)^2=\begin{cases}1&n\text{ is square-free},\\0&\text{otherwise},\end{cases}\qquad n>0.
$$

The [radical of an integer](#radical-of-an-integer) keeps one copy of each [prime factor](#prime-factor), so it changes precisely the [integers](#integer) with a repeated [prime factor](#prime-factor). Its definition is given in Evertse's exercise sheet. [Jan-Hendrik Evertse, Diophantine approximation, Homework IV, Exercise 20](https://pub.math.leidenuniv.nl/~evertsejh/dio12-ex4.pdf) The [Möbius function](#mobius-function) assigns $(-1)^r$ to a [square-free integer](#square-free-integer) with $r$ distinct [prime factors](#prime-factor) and zero otherwise; squaring forgets the sign. Consequently $\sum_{n=1}^{60}\mu(n)^2=37$ counts exactly the green cells. This connects a restriction on repeated [prime factors](#prime-factor) with weighted counting and [inclusion-exclusion](combinatorics.md#inclusion-exclusion-principle). [Darij Grinberg, MIT 18.781, Definition 2.1.2: the Möbius function](https://darijgrinberg.gitlab.io/floor.pdf)

### Powerful number

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Powerful_number)

A positive integer is squarefull when every [prime](#prime-number) dividing it also divides it to at least the second power. Thus $n$ is not squarefull as soon as some prime $p$ satisfies $p\mid n$ but $p^2\nmid n$.

### Square number

↑ **Parent:** [Integer](#integer)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_number)

A square number is an [integer](#integer) of the form $n^2$ for some integer $n$. Consecutive nonnegative squares differ by $(n+1)^2-n^2=2n+1$.

## Divisibility

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisibility)

For [integers](#integer) $d,n$, **$d$ divides $n$** when [multiplication](arithmetic.md#multiplication) by some [integer](#integer) $k$ takes $d$ to $n$:

$$
d\mid n\quad\Longleftrightarrow\quad \text{there exists }k\in\mathbb Z\text{ such that }n=dk.
$$

Then $d$ is a [divisor](#divisor) of $n$, and $n$ is an [integer multiple](#integer-multiple) of $d$. The notation $d\nmid n$ means that no such [integer](#integer) $k$ exists. For $d\ne0$, this is equivalent to saying that the [quotient](arithmetic.md#quotient) $n/d$ is an [integer](#integer), or that [Euclidean division](#euclidean-division) by $|d|$ leaves [remainder](#remainder) zero.

For example, $3\mid12$ because $12=3\cdot4$, whereas $5\nmid12$ because $12=5\cdot2+2$. Signs do not change [divisibility](#divisibility): $-3\mid12$ because $12=(-3)(-4)$, and $3\mid-12$ because $-12=3(-4)$. In general, changing the sign of either input preserves the relation.

The definition here permits zero as either input. Every [integer](#integer) divides zero, since $0=d\cdot0$. In particular, **$0\mid0$**; however, $0\nmid n$ whenever $n\ne0$, since $0k$ is always zero. This is a statement about [multiplication](arithmetic.md#multiplication), and assigns no meaning to [division](arithmetic.md#division-mathematics) by zero: $0/0$ remains undefined.

Two useful properties come directly from the defining [multiplication](arithmetic.md#multiplication). [Divisibility](#divisibility) is a [reflexive relation](set-theory.md#reflexive-relation), since $n=n\cdot1$, and a [transitive relation](set-theory.md#transitive-relation): if $b=ar$ and $c=bs$, then $c=a(rs)$. Moreover, a shared [divisor](#divisor) divides every [integer](#integer) [linear combination](vector-space.md#linear-combination):

$$
d\mid a,\quad d\mid b\quad\Longrightarrow\quad d\mid(ax+by)\qquad(x,y\in\mathbb Z).
$$

Indeed, writing $a=du$ and $b=dv$ gives $ax+by=d(ux+vy)$. For example, $6\mid12$ and $6\mid18$ imply $6\mid(18-12)$. This small observation explains why the [Euclidean algorithm](#euclidean-algorithm) preserves common [divisors](#divisor), and why [Bézout's identity](algebra.md#bezout-s-identity) can certify a [greatest common divisor](#greatest-common-divisor).

On the [positive integers](#positive-integer), [divisibility](#divisibility) is a [partial order](set.md#partially-ordered-set): if $a\mid b$ and $b\mid a$, then $a=b$. The restriction matters, since $3\mid-3$ and $-3\mid3$ although $3\ne-3$. The [prime factorization](#fundamental-theorem-of-arithmetic) viewpoint makes this order concrete: $d\mid n$ exactly when every [prime valuation](#prime-valuation) of $d$ is at most the corresponding [prime valuation](#prime-valuation) of $n$. Thus one relation connects equal grouping, [prime factorization](#fundamental-theorem-of-arithmetic), and [modular arithmetic](#modular-arithmetic).

Book VII, definitions 3 and 5 of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements) describe the corresponding positive-number relation through one number measuring another and through [integer multiples](#integer-multiple). The sign and zero conventions above belong to the present [integer](#integer) formulation, rather than to those ancient definitions. [Euclid, Elements VII, definitions 3 and 5, T. L. Heath translation](https://geometor.github.io/euclid/heath/VII/index.html)

### Integer multiple

↑ **Parent:** [Divisibility](#divisibility)

An integer multiple of an [integer](#integer) $d$ is a [product](arithmetic.md#product-of-numbers) $dk$ with $k$ an [integer](#integer); equivalently, $d$ is a [divisor](#divisor) of that [product](arithmetic.md#product-of-numbers). The [integer multiples](#integer-multiple) of $12$ are $\ldots,-24,-12,0,12,24,\ldots$. Zero is an [integer multiple](#integer-multiple) of every [integer](#integer), and the only [integer multiple](#integer-multiple) of zero is zero. Shared positive [integer multiples](#integer-multiple) lead to the [least common multiple](#least-common-multiple).

### Divisor

↑ **Parent:** [Divisibility](#divisibility)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Divisor)

A divisor of an [integer](#integer) $n$ is an [integer](#integer) $d$ satisfying the [divisibility](#divisibility) relation $d\mid n$. Equivalently, $n=dk$ for some [integer](#integer) $k$. The word **positive** matters when listing or counting [divisors](#divisor): unless signs are restricted, both $d$ and $-d$ qualify.

The positive [divisors](#divisor) of $12$ are

$$
1,2,3,4,6,12.
$$

Their negatives are also [divisors](#divisor) of $12$, giving twelve [integer divisors](#divisor) altogether. The same list of positive [divisors](#divisor) works for $-12$. One has only the positive [divisor](#divisor) $1$, while zero has every [integer](#integer) as a [divisor](#divisor), including zero under our [divisibility](#divisibility) convention. A nonzero [integer](#integer) never has zero as a [divisor](#divisor).

For a [positive integer](#positive-integer) $n$, the positive [divisors](#divisor) come in pairs $(d,n/d)$ whose [product](arithmetic.md#product-of-numbers) is $n$. For $12$, the pairs are $(1,12)$, $(2,6)$ and $(3,4)$. Each pair contains a [divisor](#divisor) at most $\sqrt n$, so searching through candidate [divisors](#divisor) up to the [square root](algebra.md#square-root) suffices to find all pairs. A pair repeats its own member only when $n$ is a [perfect square](#square-number); for $36$, the middle pair is $(6,6)$. Consequently a [positive integer](#positive-integer) has an odd number of positive [divisors](#divisor) exactly when it is a [perfect square](#square-number).

The [prime factorization](#fundamental-theorem-of-arithmetic) gives another complete description. Since $12=2^2\cdot3$, its positive [divisors](#divisor) are precisely $2^i3^j$ with $0\leq i\leq2$ and $0\leq j\leq1$. These independent choices give $(2+1)(1+1)=6$ positive [divisors](#divisor), the value of the [divisor function](#divisor-function) $\tau(12)$. A [prime factor](#prime-factor) is one particular kind of [divisor](#divisor); $4$, $6$ and $12$ show that [divisors](#divisor) need not be [prime numbers](#prime-number).

Thinking in pairs connects exact grouping with [integer factorization](#integer-factorization): twelve objects can form three groups of four or four groups of three. Thinking in shared [divisors](#divisor) gives the [greatest common divisor](#greatest-common-divisor); for $12$ and $18$, the positive common [divisors](#divisor) are $1,2,3,6$, and the largest is $6$.

#### Proper divisor

↑ **Parent:** [Divisor](#divisor)

Here a [proper divisor](#proper-divisor) of a [positive integer](#positive-integer) $n$ means a positive [integer divisor](#divisor) other than $n$ itself. Thus $1$ has no [proper divisors](#proper-divisor), and the [proper divisors](#proper-divisor) of $12$ are $1,2,3,4,6$.

#### Squarefree divisor

↑ **Parent:** [Divisor](#divisor)

A squarefree divisor of an [integer](#integer) $n$ is a [divisor](#divisor) $d\mid n$ that is a [squarefree integer](#squarefree-integer). It is specified by choosing a subset of the distinct [prime factors](#prime-factor) of $n$.

### Greatest common divisor

↑ **Parent:** [Divisibility](#divisibility)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Greatest_common_divisor)

For [integers](#integer) $a,b$ not both zero, their greatest common divisor is the largest positive [integer](#integer) dividing both. It is unchanged by replacing either input by its negative. The convention $\gcd(0,0)=0$ is useful, but this exceptional value is not a largest positive common [divisor](#divisor). For positive inputs, the [Euclidean algorithm](#euclidean-algorithm) computes the answer, and [Bézout's identity](algebra.md#bezout-s-identity) expresses it as an integer [linear combination](vector-space.md#linear-combination) of the inputs.

For $12=2^2\cdot3$ and $18=2\cdot3^2$, a common [divisor](#divisor) can contain at most one copy of the [prime number](#prime-number) two and one of the [prime number](#prime-number) three. Taking the smaller [prime valuation](#prime-valuation) at each [prime number](#prime-number) therefore gives

$$
\gcd(12,18)=2^{\min(2,1)}3^{\min(1,2)}=2\cdot3=6.
$$

The check $6=18-12$ is also a [Bézout's identity](algebra.md#bezout-s-identity): every common [divisor](#divisor) divides this difference, and six itself divides both inputs. More generally, every common [divisor](#divisor) divides the [greatest common divisor](#greatest-common-divisor), a stronger statement than merely being no larger than it. The companion [least common multiple](#least-common-multiple) takes the larger [prime valuations](#prime-valuation), as the diagram there illustrates. For an application, divide the [numerator](#numerator) and [denominator](#denominator) of the [fraction](#fraction) $12/18$ by six to obtain $2/3$; these remaining [integers](#integer) are [coprime](#coprime-integers).

#### Scaling identity for greatest common divisors

↑ **Parent:** [Greatest common divisor](#greatest-common-divisor)

For positive integers $m,n,k$, the [greatest common divisor](#greatest-common-divisor) scales by the common multiplier $k$. If $d=\gcd(m,n)$, then $kd$ is a common divisor of $km,kn$. Meanwhile [Bézout's identity](algebra.md#bezout-s-identity) expresses $kd$ as an integer linear combination of $km,kn$, so their [greatest common divisor](#greatest-common-divisor) divides $kd$. These two comparisons prove the identity without prime factorization.

#### Coprime integers

↑ **Parent:** [Greatest common divisor](#greatest-common-divisor)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coprime_integers)

Two [integers](#integer) $a,b$ are **coprime** when their [greatest common divisor](#greatest-common-divisor) is one:

$$
a,b\text{ are coprime}\quad\Longleftrightarrow\quad\gcd(a,b)=1.
$$

For [positive integers](#positive-integer), this says that the only positive common [divisor](#divisor) is one. For signed [integers](#integer), use $\gcd(a,b)=\gcd(|a|,|b|)$, with [absolute values](real-analysis.md#absolute-value); changing either sign leaves [coprimality](#coprime-integers) unchanged. With the convention $\gcd(0,0)=0$, zero is [coprime](#coprime-integers) precisely to $1,-1$, because $\gcd(a,0)=|a|$. Both $1,-1$ are [coprime](#coprime-integers) to every [integer](#integer). [Darij Grinberg, MIT 18.781, Section 1.2: greatest common divisors and coprimality](https://darijgrinberg.gitlab.io/floor.pdf)

The word concerns shared [prime factors](#prime-factor), not whether either input is a [prime number](#prime-number). For instance $8=2^3$ and $9=3^2$ are [coprime](#coprime-integers) [composite numbers](#composite-number), even though neither is a [square-free integer](#square-free-integer). Conversely, $6=2\cdot3$ and $10=2\cdot5$ are [square-free integers](#square-free-integer) but are not [coprime](#coprime-integers). Consecutive [integers](#integer) are always [coprime](#coprime-integers): any common [divisor](#divisor) of $n,n+1$ divides their difference one. Thus $14,15$ provide another pair of [coprime](#coprime-integers) [composite numbers](#composite-number).

For [positive integers](#positive-integer), let $P(n)$ be the [prime support of an integer](#prime-support-of-an-integer). The equivalent test is

$$
\gcd(a,b)=1\quad\Longleftrightarrow\quad P(a)\cap P(b)=\varnothing.
$$

The [set intersection](set.md#set-intersection) of the two [prime supports of an integer](#prime-support-of-an-integer) must be the [empty set](set.md#empty-set). Indeed, any positive common [divisor](#divisor) greater than one has a [prime factor](#prime-factor), and any shared [prime factor](#prime-factor) is a common [divisor](#divisor) greater than one. Hence [coprimality](#coprime-integers) depends on which [prime factors](#prime-factor) occur, rather than on their [prime valuations](#prime-valuation); replacing either input by its [radical of an integer](#radical-of-an-integer) preserves [coprimality](#coprime-integers).

For a list of at least two [integers](#integer), distinguish [pairwise coprimality](#pairwise-coprimality), requiring every pair to be [coprime](#coprime-integers), from [joint coprimality](#joint-coprimality), requiring only the [greatest common divisor](#greatest-common-divisor) of the entire list to be one. For example,

$$
\gcd(6,10,15)=1,\qquad
\gcd(6,10)=2,\quad\gcd(6,15)=3,\quad\gcd(10,15)=5.
$$

No [prime factor](#prime-factor) belongs to all three [prime supports of an integer](#prime-support-of-an-integer), yet each pair shares one. By contrast, $4,9,25$ have [pairwise coprimality](#pairwise-coprimality). The distinction is presented by Poritz under the names pairwise and mutually relatively prime. [Jonathan A. Poritz, Yet Another Introductory Number Theory Textbook, Section 1.5](https://math.libretexts.org/Bookshelves/Combinatorics_and_Discrete_Mathematics/Yet_Another_Introductory_Number_Theory_Textbook_-_Cryptology_Emphasis_(Poritz)/01:_Well-Ordering_and_Division/1.05:_The_Greatest_Common_Divisor)

<a id="image-prime-support-of-an-integer-distinguishes-coprime-pairs-joint-coprimality-and-pairwise-coprimality"></a>
![](coprime-squarefree-integers-prime-sharing.png)

**[Figure 26](#image-prime-support-of-an-integer-distinguishes-coprime-pairs-joint-coprimality-and-pairwise-coprimality). Prime support of an integer distinguishes coprime pairs, joint coprimality and pairwise coprimality**. Filled cells mark membership in the [prime support of an integer](#prime-support-of-an-integer); empty cells mean the [prime number](#prime-number) does not divide the row label. The first panel has two [coprime integers](#coprime-integers); the middle has [joint coprimality](#joint-coprimality) but fails [pairwise coprimality](#pairwise-coprimality); the last has [pairwise coprimality](#pairwise-coprimality). The columns exhaust all [prime factors](#prime-factor) of these eight row entries. This original finite arithmetic diagram shows exact [divisibility](#divisibility), not sampled probabilities.

One use is simplifying [fractions](#fraction). For a [fraction](#fraction) $a/b$ with [integer](#integer) entries and $b>0$, divide its [numerator](#numerator) and [denominator](#denominator) by $d=\gcd(a,b)$ to obtain a [reduced fraction](#reduced-fraction) with [coprime](#coprime-integers) entries. For example, $42/30=7/5$ since $d=6$, and $-42/30=-7/5$ uses the same $d$. A further common [divisor](#divisor) would make $d$ too small, so the reduction is complete. In particular, the [reduced fraction](#reduced-fraction) for zero is $0/1$.

Another use is reversible [modular arithmetic](#modular-arithmetic): for an [integer modulus](#modulus-in-modular-arithmetic) $m>1$, an [integer](#integer) $a$ has a [modular inverse](#modular-multiplicative-inverse) precisely when $a,m$ are [coprime](#coprime-integers). The proof outline uses [Bézout's identity](algebra.md#bezout-s-identity): $ua+vm=1$ makes $u$ a [modular inverse](#modular-multiplicative-inverse), and any inverse relation $ua-km=1$ forces every common [divisor](#divisor) to divide one. For example, $3\cdot5-2\cdot7=1$ gives $5^{-1}\equiv3\pmod7$, whereas $6$ has no [modular inverse](#modular-multiplicative-inverse) modulo $10$. Thus [coprimality](#coprime-integers) is the exact condition allowing division by a residue in [modular arithmetic](#modular-arithmetic). [Ankur Moitra, MIT 18.200, Lecture 15, Lemmas 1–2 and modular inverses](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

##### Pairwise coprimality

↑ **Parent:** [Coprime integers](#coprime-integers)

A list of [integers](#integer) $a_1,\ldots,a_r$, with $r\ge2$, has [pairwise coprimality](#pairwise-coprimality) when every two entries in distinct positions are [coprime](#coprime-integers). This implies [joint coprimality](#joint-coprimality). For [positive integers](#positive-integer), it means no [prime factor](#prime-factor) occurs in two different entries. For example, $4,9,25$ satisfy this condition.

##### Joint coprimality

↑ **Parent:** [Coprime integers](#coprime-integers)

A list of [integers](#integer) $a_1,\ldots,a_r$, with $r\ge2$, has [joint coprimality](#joint-coprimality) when its [greatest common divisor](#greatest-common-divisor) is one; define that [greatest common divisor](#greatest-common-divisor) by repeated application of the two-input operation. For [positive integers](#positive-integer), no [prime factor](#prime-factor) may divide every entry. Thus $6,10,15$ have [joint coprimality](#joint-coprimality) but fail [pairwise coprimality](#pairwise-coprimality). For two entries, the conditions coincide.

### Least common multiple

↑ **Parent:** [Divisibility](#divisibility)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Least_common_multiple)

For [positive integers](#positive-integer) $a,b$, their least common multiple is the **smallest positive [integer](#integer) that is an [integer multiple](#integer-multiple) of both**. Write it as $\operatorname{lcm}(a,b)$. A positive common [integer multiple](#integer-multiple) always exists, since $ab$ is one, but it can be larger than necessary.

For example, the positive [integer multiples](#integer-multiple) of $12$ begin $12,24,36,48,60,72$, while those of $18$ begin $18,36,54,72$. Their first positive coincidence is $36$, so $\operatorname{lcm}(12,18)=36$. Both also divide zero, but the word positive excludes zero from this minimum.

Suppose two events happen every twelve and eighteen days, and both happen at day $t=0$. Their next meeting is at day $36$, after three twelve-day intervals and two eighteen-day intervals. Through day $72$, their common event times are $0,36,72$.

<a id="image-events-every-12-and-18-days-starting-together-meet-again-every-36-days"></a>
![](least-common-multiple-periods.png)

**[Figure 27](#image-events-every-12-and-18-days-starting-together-meet-again-every-36-days). Events every 12 and 18 days, starting together, meet again every 36 days**. Each row marks the nonnegative [integer multiples](#integer-multiple) of its interval from zero through 72. The highlighted columns $0,36,72$ are shared; 36 is the first positive one and hence the [least common multiple](#least-common-multiple).

The [prime factorization](#fundamental-theorem-of-arithmetic) explains why this coincidence occurs. For the [integers](#integer) $12$ and $18$,

$$
12=2^2\cdot3,\qquad18=2\cdot3^2,\qquad
\operatorname{lcm}(12,18)=2^{\max(2,1)}3^{\max(1,2)}=36.
$$

A common [integer multiple](#integer-multiple) must contain at least the [prime valuations](#prime-valuation) required by each input. Taking the larger [prime valuation](#prime-valuation) at each [prime number](#prime-number) meets both requirements with no extra factors. The [greatest common divisor](#greatest-common-divisor) uses the smaller [prime valuations](#prime-valuation) instead. This is the same coordinate comparison developed under [prime factorization](#fundamental-theorem-of-arithmetic), applied in opposite directions.

<a id="image-for-12-and-18-smaller-prime-valuations-give-greatest-common-divisor-6-and-larger-ones-give-least-common-multiple-36"></a>
![](gcd-lcm-prime-exponents.png)

**[Figure 28](#image-for-12-and-18-smaller-prime-valuations-give-greatest-common-divisor-6-and-larger-ones-give-least-common-multiple-36). For 12 and 18, smaller prime valuations give greatest common divisor 6 and larger ones give least common multiple 36**. Bars show the exponents of the [prime numbers](#prime-number) two and three in $12$, $18$, $6$ and $36$. The table makes the minimum and maximum in each column explicit.

For any [positive integers](#positive-integer) $a,b$, the [prime valuations](#prime-valuation) give

$$
\gcd(a,b)\operatorname{lcm}(a,b)=ab,\qquad
\operatorname{lcm}(a,b)=\frac{ab}{\gcd(a,b)}.
$$

The proof outline is one observation at each [prime number](#prime-number): $\min(r,s)+\max(r,s)=r+s$. Hence the two sides have identical [prime factorizations](#fundamental-theorem-of-arithmetic). Numerically, $6\cdot36=12\cdot18=216$. This also gives a calculation using the [Euclidean algorithm](#euclidean-algorithm) for the [greatest common divisor](#greatest-common-divisor), without first finding the [prime factors](#prime-factor) of both inputs.

Every positive common [integer multiple](#integer-multiple) is an [integer multiple](#integer-multiple) of the [least common multiple](#least-common-multiple), because its [prime valuations](#prime-valuation) must be at least the larger input [prime valuations](#prime-valuation). Including negatives and zero, the common [integer multiples](#integer-multiple) of $12$ and $18$ are exactly $36k$ for [integers](#integer) $k$. For more than two [positive integers](#positive-integer), the same definition and rule of taking the largest [prime valuations](#prime-valuation) apply; one may also combine inputs successively. For example, $\operatorname{lcm}(12,18,20)=\operatorname{lcm}(36,20)=180$.

For nonzero signed [integers](#integer), take [absolute values](real-analysis.md#absolute-value): $\operatorname{lcm}(-12,18)=36$. We extend the definition to zero by the convention $\operatorname{lcm}(a,0)=0$, since zero is then the only common [integer multiple](#integer-multiple); this is an extension, not a positive minimum. In particular $\operatorname{lcm}(0,0)=0$ must be handled separately from the displayed [quotient](arithmetic.md#quotient), which would involve [division](arithmetic.md#division-mathematics) by zero.

The [least common multiple](#least-common-multiple) is useful for combining [fractions](#fraction) with the smallest positive shared [denominator](#denominator). For example,

$$
\frac1{12}+\frac1{18}=\frac3{36}+\frac2{36}=\frac5{36}.
$$

Its scheduling interpretation requires care about starting times. If the events start at [integer](#integer) days $r$ and $s$, a common time must satisfy the [integer congruences](#integer-congruence) $t\equiv r\pmod{12}$ and $t\equiv s\pmod{18}$. The [Chinese remainder theorem for noncoprime moduli](mathematics.md#chinese-remainder-theorem-for-noncoprime-moduli) says a solution exists exactly when $6\mid(r-s)$. If it exists, solutions form one [congruence class](#congruence-class) modulo $36$, but the first meeting need not be day $36$. With starts $r=0,s=6$, the first meeting is day $24$ and subsequent meetings are $60,96,\ldots$; with $r=0,s=1$, they never meet. The beauty of the [least common multiple](#least-common-multiple) is the exact shared spacing, while the [integer congruences](#integer-congruence) determine whether and where the spacing begins.

Book VII, Proposition 34 of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements) constructs the [least common multiple](#least-common-multiple) of two numbers, and Proposition 36 extends the construction to three by first combining two of them. In modern notation this is $\operatorname{lcm}(a,b,c)=\operatorname{lcm}(\operatorname{lcm}(a,b),c)$. These are specific ancient treatments of the construction, rather than a claim about its first discovery. [Euclid, Elements VII.34, T. L. Heath translation: two numbers](https://geometor.github.io/euclid/heath/VII/34/index.html) [Euclid, Elements VII.36, T. L. Heath translation: three numbers](https://geometor.github.io/euclid/heath/VII/36/index.html)

## Modular arithmetic

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_arithmetic)

Modular arithmetic performs [addition](arithmetic.md#addition) and [multiplication](arithmetic.md#multiplication) on [integers](#integer) while remembering only their [remainders](#remainder) for a fixed positive [integer modulus](#modulus-in-modular-arithmetic) $m$. The relation $a\equiv b\pmod m$ means that $m$ divides $a-b$: the two [integers](#integer) lie in the same [congruence class](#congruence-class). For example, $-3$, $2$ and $7$ represent one class modulo $5$. Choosing the [least nonnegative residue](#least-nonnegative-residue) gives exactly $m$ representatives, $0,1,\ldots,m-1$, even though each [congruence class](#congruence-class) contains infinitely many [integers](#integer).

A clock supplies a familiar example. Represent the twelve positions by $0,1,\ldots,11$, with $0$ at the position usually labelled twelve. Starting at ten and moving seven positions gives

$$
10+7=17\equiv5\pmod{12}.
$$

The [integer congruence](#integer-congruence) records the final position; it discards the number of complete revolutions. Adding another twelve changes the elapsed count while preserving the position. The picture also shows a single [congruence class](#congruence-class) modulo five spread along the [number line](arithmetic.md#number-line).

<a id="image-clock-addition-wraps-modulo-twelve-while-integers-separated-by-five-represent-one-congruence-class"></a>
![](modular-arithmetic-clock-and-classes.png)

**[Figure 29](#image-clock-addition-wraps-modulo-twelve-while-integers-separated-by-five-represent-one-congruence-class). Clock addition wraps modulo twelve, while integers separated by five represent one congruence class**.

The useful surprise is that discarding this information still preserves the arithmetic. If $a\equiv a'$ and $b\equiv b'$ modulo $m$, then $a+b\equiv a'+b'$ and $ab\equiv a'b'$ modulo $m$. Thus a large calculation can reduce its intermediate [integers](#integer) after every step. For instance,

$$
10+7\equiv5\pmod{12},\qquad 10\cdot7\equiv10\pmod{12},\qquad 10^2\equiv4\pmod{12}.
$$

Replacing $10$ by $-2$ gives the same answers with smaller intermediate values. The [congruence classes](#congruence-class) with these operations form the [quotient ring](commutative-algebra.md#quotient-ring) $\mathbb Z/m\mathbb Z$; their [addition](arithmetic.md#addition) alone forms a [cyclic group](group.md#cyclic-group). This passage from [integers](#integer) to a finite arithmetic system is the setting for [modular exponentiation](#modular-exponentiation), [primality testing](computer-science.md#primality-testing) and the [RSA cryptosystem](algebra.md#rsa-cryptosystem). [Ankur Moitra, MIT 18.200, Lecture 15, modular arithmetic and its applications](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

[Multiplicative cancellation](commutative-algebra.md#multiplicative-cancellation-in-an-integral-domain) needs extra care. Modulo six, $2\cdot1\equiv2\cdot4$, but $1\not\equiv4$: multiplication by two has merged distinct [congruence classes](#congruence-class). Cancelling a factor while retaining the [integer modulus](#modulus-in-modular-arithmetic) is justified when that factor has a [modular multiplicative inverse](#modular-multiplicative-inverse), equivalently when it is [coprime](#coprime-integers) to the [integer modulus](#modulus-in-modular-arithmetic). A [linear congruence](#linear-congruence) can consequently have no solutions, one solution class, or several solution classes. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) supplies a complementary operation: splitting a calculation across [coprime](#coprime-integers) [integer moduli](#modulus-in-modular-arithmetic) and reconstructing its class modulo their product.

Small remainders can also certify impossibility. A [perfect square](#square-number) has residue zero or one modulo four, as checking the four [congruence classes](#congruence-class) shows. Therefore an [integer](#integer) equation $x^2=4k+2$ has no solution. The converse direction needs care: a permitted residue does not guarantee an [integer](#integer) solution, since $5\equiv1\pmod4$ but five is not a [perfect square](#square-number). Such local tests provide necessary conditions for [Diophantine equations](#diophantine-equation) without replacing the full problem.

In _Disquisitiones arithmeticae_ (1801), [Carl Friedrich Gauss](mathematics.md#carl-friedrich-gauss) defines [integer congruence](#integer-congruence) in article 1 and adopts the symbol $\equiv$ in article 2. Article 12 derives [divisibility](#divisibility) tests from powers of ten and explains checking arithmetic by its remainders. These passages show a systematic treatment of the same idea; they are not a claim that remainders were first used in 1801. [Gauss, Disquisitiones arithmeticae, section I, articles 1–2 and 12; text from the 1870 collected edition](https://la.wikisource.org/wiki/Disquisitiones_arithmeticae/Sectio_prima)

### Modulus in modular arithmetic

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)

The positive [integer](#integer) $m$ in $a\equiv b\pmod m$ is the modulus. It specifies which differences are ignored: exactly the [integer](#integer) multiples of $m$. It is distinct from the [modulus of a complex number](complex-analysis.md#complex-modulus), which measures magnitude.

### Least nonnegative residue

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)

The least nonnegative residue of an [integer](#integer) $a$ modulo a positive [integer modulus](#modulus-in-modular-arithmetic) $m$ is the unique representative $r$ of its [congruence class](#congruence-class) in $\{0,\ldots,m-1\}$. [Euclidean division](#euclidean-division) gives $a=qm+r$. For example, $-3=(-1)\cdot5+2$, so $-3\bmod5=2$; the [integer congruence](#integer-congruence) $-3\equiv2\pmod5$ does not assert equality of those two [integers](#integer).

### Integer congruence

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)

For a positive modulus $m$, integers $a,b$ are congruent when their difference is divisible by $m$. This is an [equivalence relation](set-theory.md#equivalence-relation): zero is divisible by $m$, changing sign preserves [divisibility](#divisibility), and adding two divisible differences proves transitivity. Addition and multiplication respect it, because $(a+c)-(b+d)=(a-b)+(c-d)$ and $ac-bd=c(a-b)+b(c-d)$. Its [equivalence classes](set-theory.md#equivalence-class) are the residue classes used in [modular arithmetic](#modular-arithmetic).

<h3 id="wilson-s-theorem">Wilson's theorem</h3>

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Wilson's_theorem)

For an [integer](#integer) $n>1$, [Wilson's theorem](#wilson-s-theorem) characterizes [prime numbers](#prime-number) by a [factorial](combinatorics.md#factorial):

$$
n\text{ is prime}\quad\Longleftrightarrow\quad(n-1)!\equiv-1\pmod n.
$$

The right side is an [integer congruence](#integer-congruence), so the least nonnegative [remainder](#remainder) is $n-1$. For example, $4!=24\equiv4\pmod5$ certifies that five is a [prime number](#prime-number), whereas $5!=120\equiv0\pmod6$ rules out six. [Wilson's Theorem and Fermat's Theorem by Bruce Ikenaga](mathematics-bibliography.md#wilson-s-theorem-and-fermat-s-theorem-by-bruce-ikenaga)

<a id="image-factorial-residues-distinguish-primes-from-composites-with-inverse-pairs-explaining-the-prime-case"></a>
![](wilson-factorial-residue-primality.png)

**[Figure 30](#image-factorial-residues-distinguish-primes-from-composites-with-inverse-pairs-explaining-the-prime-case). Factorial residues distinguish primes from composites, with inverse pairs explaining the prime case**.

For an odd [prime number](#prime-number) $p$, each nonzero [congruence class](#congruence-class) has a unique [modular multiplicative inverse](#modular-multiplicative-inverse). Pair each class with its inverse: each distinct pair contributes one. A class is its own inverse exactly when $a^2\equiv1\pmod p$; since $p\mid(a-1)(a+1)$, [Euclid's lemma](#euclid-s-lemma) leaves only $a\equiv\pm1$. Their product is $-1$. The [prime number](#prime-number) two needs a separate check: $1!\equiv-1\pmod2$. Conversely, a proper [divisor](#divisor) $1<d<n$ divides both $n$ and $(n-1)!$, so the displayed [integer congruence](#integer-congruence) would force $d\mid1$, a contradiction. [Wilson's Theorem and Fermat's Theorem by Bruce Ikenaga](mathematics-bibliography.md#wilson-s-theorem-and-fermat-s-theorem-by-bruce-ikenaga)

The [composite numbers](#composite-number) have an even sharper pattern: $(n-1)!\equiv0\pmod n$ for every [composite number](#composite-number) $n>4$, but $3!=6\equiv2\pmod4$. To check the zero claim, write $n=ab$ with $1<a\leq b<n$. If $a<b$, both occur as different factors in the [factorial](combinatorics.md#factorial). If $a=b\geq3$, the different factors $a$ and $2a$ both occur since $2a<a^2=n$, and their product is divisible by $n$. The only excluded case is $a=b=2$. Thus four is an exception to the zero pattern, but still fails [Wilson's theorem](#wilson-s-theorem): its required [remainder](#remainder) would be three.

This is an exact [primality testing](computer-science.md#primality-testing) criterion, but direct evaluation is expensive: even reducing modulo $n$ after every multiplication still takes a number of multiplications proportional to $n$, which grows exponentially with the number of [binary digits](#binary-digit) of $n$. The problem is not merely storing a huge [factorial](combinatorics.md#factorial). The more useful role of [Wilson's theorem](#wilson-s-theorem) is simplifying [factorial](combinatorics.md#factorial) expressions in [modular arithmetic](#modular-arithmetic). For instance, if $p>2$ is a [prime number](#prime-number), then $(p-1)(p-2)!\equiv-1\pmod p$ gives $(p-2)!\equiv1\pmod p$ by a [modular multiplicative inverse](#modular-multiplicative-inverse).

#### Wilson factorial congruence modulo a triangular number

↑ **Parent:** [Wilson's theorem](#wilson-s-theorem)

For an odd [prime number](#prime-number) $p$, put $m=(p-1)/2$. Both $(p-1)!$ and $p-1$ are divisible by $m$. By [Wilson's theorem](#wilson-s-theorem), they are also congruent modulo $p$, because each is $-1$ modulo $p$. The [coprime integers](#coprime-integers) $m,p$ therefore both divide their difference, giving the displayed [integer congruence](#integer-congruence). This combines the prime-modulus factorial identity with an elementary divisibility constraint.

#### Odd-residue squared product modulo a prime

↑ **Parent:** [Wilson's theorem](#wilson-s-theorem)

For an odd prime $p$, the even residues are the negatives of the odd residues. If $O=1\cdot3\cdots(p-2)$, then $(p-1)!\equiv(-1)^{(p-1)/2}O^2$. Apply [Wilson theorem](#wilson-s-theorem) to obtain the displayed congruence. The empty product for $p=3$ is one.

#### Complementary factorial congruence

↑ **Parent:** [Wilson's theorem](#wilson-s-theorem)

For a [prime number](#prime-number) $p$ and nonnegative [integers](#integer) $h+k=p-1$, [Wilson theorem](#wilson-s-theorem) gives $(-1)^k h!k!\equiv-1\pmod p$ by replacing the last $k$ factors of $(p-1)!$ with $-1,-2,\ldots,-k$. For odd $p$, $h,k$ have the same parity; for $p=2$, both signs have the same [residue class](#residue-class). Thus $h!k!+(-1)^h\equiv0\pmod p$, including the endpoint cases $0!=1$.

### Congruence class

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)

The [congruence class](#congruence-class) of $a$ modulo a positive integer $N$ is $\{a+Nk:k\in\mathbb Z\}$. Two integers have the same class exactly when their difference is divisible by $N$. Addition and multiplication of representatives descend to well-defined operations on $\mathbb Z/N\mathbb Z$, because replacing a representative by a multiple-of-$N$ translate changes the result by a multiple of $N$.

### Modular congruence

↑ **Parent:** [Modular arithmetic](#modular-arithmetic)

For [integers](#integer) $a,b$ and a positive [integer modulus](#modulus-in-modular-arithmetic) $n$, modular congruence means

$$
a\equiv b\pmod n\iff n\mid(a-b).
$$

Thus $a-b=kn$ for some [integer](#integer) $k$: the two [integers](#integer) differ by complete cycles of length $n$. For example, $14\equiv2\pmod{12}$ because $14-2=12$, and $-1\equiv11\pmod{12}$ because $-1-11=-12$. A [modular congruence](#modular-congruence) need not be an equality of [integers](#integer).

On a twelve-position clock labelled $0,1,\ldots,11$, adding five to nine follows $9\to10\to11\to0\to1\to2$. Hence $9+5=14\equiv2\pmod{12}$: the final position remembers the [remainder](#remainder) while forgetting a complete revolution.

<a id="image-adding-five-to-nine-takes-five-clockwise-steps-and-ends-at-two-modulo-twelve"></a>
![](modular-clock-addition.png)

**[Figure 31](#image-adding-five-to-nine-takes-five-clockwise-steps-and-ends-at-two-modulo-twelve). Adding five to nine takes five clockwise steps and ends at two modulo twelve**.

The same idea tracks any count repeating every $n$ steps. It also lets us compute sums and products with small [residue classes](#residue-class), reducing intermediate results without changing the final class. The justification comes from [addition](arithmetic.md#addition) and [multiplication](arithmetic.md#multiplication) being well-defined on [residue classes](#residue-class).

In _Disquisitiones arithmeticae_ (1801), [Carl Friedrich Gauss](mathematics.md#carl-friedrich-gauss) defines [modular congruence](#modular-congruence) by [divisibility](#divisibility) in article 1; article 2 describes the [integers](#integer) $a+kn$ and adopts $\equiv$. These passages document his presentation and notation, without claiming that repeating remainders began in 1801. [Gauss, Disquisitiones arithmeticae, section I, articles 1–2; original text in the 1870 collected edition](https://la.wikisource.org/wiki/Disquisitiones_arithmeticae/Sectio_prima)

#### Prime-power contraction under pth powers

↑ **Parent:** [Modular congruence](#modular-congruence)

For a prime $p$ and $k\geq1$, write $a=b+p^kh$. The [binomial theorem](combinatorics.md#binomial-theorem) shows $a^p-b^p$ is divisible by $p^{k+1}$: the linear term contains the extra factor $p$ and every higher term contains at least $p^{2k}$. Iteration gives the displayed [modular congruence](#modular-congruence) for every $r\geq0$, including $p=2$. Applied to [Fermat's little theorem](#fermat-little-theorem), it yields $a^{p^n}\equiv a^{p^{n-1}}\pmod{p^n}$.

#### Reduced residue system

↑ **Parent:** [Modular congruence](#modular-congruence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reduced_residue_system)

For a positive modulus $n$, a reduced residue system contains exactly one representative of each [residue class](#residue-class) coprime to $n$. Its size is the [Euler totient function](#euler-totient-function) $\varphi(n)$. Multiplication by any [unit modulo n](#unit-modulo-n) permutes these classes, which proves the [Fermat-Euler theorem](#euler-s-theorem) after multiplying and cancelling their unit product.

#### Linear congruence

↑ **Parent:** [Modular congruence](#modular-congruence)

A linear congruence asks for the [integers](#integer) $x$ satisfying $ax\equiv b\pmod n$, where $a,b$ are [integers](#integer) and $n>1$. Let $d=\gcd(a,n)$ be their [greatest common divisor](#greatest-common-divisor). There are solutions exactly when $d$ divides $b$. When solutions exist, there are **exactly $d$ solution classes modulo $n$**, obtained from one solution $x_0$ by

$$
x\equiv x_0+j\frac nd\pmod n,\qquad j=0,\ldots,d-1.
$$

The [divisibility](#divisibility) condition follows immediately from $ax-b=kn$: every common [divisor](#divisor) of $a,n$ must divide $b$. Conversely, [Bézout's identity](algebra.md#bezout-s-identity) constructs a solution when $d\mid b$. Differences between any two solutions obey $n\mid a(x-x_0)$, equivalently $n/d\mid x-x_0$, since $a/d$ and $n/d$ are [coprime](#coprime-integers). This explains both the spacing and the number of solution classes.

For a complete example, solve $6x\equiv9\pmod{15}$. Here $d=3$ divides nine. Dividing the corresponding [divisibility](#divisibility) statement by three changes the [integer modulus](#modulus-in-modular-arithmetic) too:

$$
6x\equiv9\pmod{15}\iff2x\equiv3\pmod5.
$$

Because $2\cdot3\equiv1\pmod5$, multiplying by the [modular inverse](#modular-multiplicative-inverse) three gives $x\equiv9\equiv4\pmod5$. Lifting this class back to modulus fifteen yields **$x\equiv4,9,14\pmod{15}$**. Direct substitution gives $24$, $54$ and $84$, each with [remainder](#remainder) nine after [division with remainder](#euclidean-division) by fifteen. By contrast, $6x\equiv10\pmod{15}$ has no solutions, because three does not divide ten.

<a id="image-multiplication-by-six-modulo-fifteen-hits-residue-nine-three-times-and-never-hits-residue-ten"></a>
![](linear-congruence-solution-classes.png)

**[Figure 32](#image-multiplication-by-six-modulo-fifteen-hits-residue-nine-three-times-and-never-hits-residue-ten). Multiplication by six modulo fifteen hits residue nine three times and never hits residue ten**.

This is why ordinary-looking [division](arithmetic.md#division-mathematics) cannot be performed blindly in [modular arithmetic](#modular-arithmetic). Reducing the equation and its [integer modulus](#modulus-in-modular-arithmetic) together keeps all solutions; retaining modulus fifteen after dividing by three would lose valid classes. When $d=1$, the [modular inverse](#modular-multiplicative-inverse) of $a$ exists and gives a unique class $x\equiv a^{-1}b\pmod n$. The [Euclidean algorithm](#euclidean-algorithm) computes the [Bézout coefficients](algebra.md#bezout-coefficient) needed for this construction. [Moitra, MIT 18.200, Lecture 15, modular inverses and the extended Euclidean algorithm](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

#### Residue class

↑ **Parent:** [Modular congruence](#modular-congruence)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Residue_class)

For a positive [integer modulus](#modulus-in-modular-arithmetic) $m$, the residue class of an [integer](#integer) $a$ is the [equivalence class](set-theory.md#equivalence-class)

$$
[a]_m=\{a+km:k\in\mathbb Z\}=\{b\in\mathbb Z:b\equiv a\pmod m\}.
$$

It contains all [integers](#integer) in the same position of the repeating cycle. For example,

$$
[-1]_{12}=[11]_{12}=\{\ldots,-13,-1,11,23,35,\ldots\}.
$$

The [residue class](#residue-class) is this whole infinite collection; its canonical representative is the [least nonnegative residue](#least-nonnegative-residue). [Euclidean division](#euclidean-division) gives exactly one such representative in $0,1,\ldots,m-1$, so there are exactly $m$ [residue classes](#residue-class). When $m=1$, there is just one, $[0]_1=\mathbb Z$.

Define [addition](arithmetic.md#addition) and [multiplication](arithmetic.md#multiplication) of [residue classes](#residue-class) by

$$
[a]_m+[b]_m=[a+b]_m,\qquad [a]_m[b]_m=[ab]_m.
$$

These definitions must give the same answer whichever [integers](#integer) represent the classes. If $a'\equiv a$ and $b'\equiv b$ modulo $m$, then

$$
(a'+b')-(a+b)=(a'-a)+(b'-b),\qquad a'b'-ab=b'(a'-a)+a(b'-b).
$$

Both differences are divisible by $m$, proving that the operations are well-defined. For example, $[9]_{12}+[5]_{12}=[2]_{12}$ and $[9]_{12}[5]_{12}=[9]_{12}$, since $45=3\cdot12+9$. Replacing nine by $-3$ gives the same answers with smaller intermediate [integers](#integer).

With these operations the [residue classes](#residue-class) form the finite [commutative ring](commutative-algebra.md#commutative-ring) $\mathbb Z/m\mathbb Z$, a [quotient ring](commutative-algebra.md#quotient-ring). It need not be a [field](algebra.md#field): $[6]_{12}[2]_{12}=[0]_{12}$ although neither factor is the zero class. These [zero divisors](mathematics.md#zero-divisor) explain why [division](arithmetic.md#division-mathematics) requires a [unit modulo n](#unit-modulo-n). Reducing after each [multiplication](arithmetic.md#multiplication) is especially useful in [modular exponentiation](#modular-exponentiation), where the unreduced powers can become enormous.

#### Unit modulo n

↑ **Parent:** [Modular congruence](#modular-congruence)

For a positive [integer modulus](#modulus-in-modular-arithmetic) $n$, a [residue class](#residue-class) $[a]_n$ is a [unit](algebra.md#unit-in-a-ring) when it has a [modular multiplicative inverse](#modular-multiplicative-inverse): some [integer](#integer) $u$ satisfies $au\equiv1\pmod n$. Modulo twelve, the [units](algebra.md#unit-in-a-ring) are exactly

$$
[1]_{12},\quad[5]_{12},\quad[7]_{12},\quad[11]_{12}.
$$

In particular, five is its own [modular inverse](#modular-multiplicative-inverse), since $5\cdot5=25\equiv1\pmod{12}$. Multiplying all twelve [residue classes](#residue-class) by five gives a [permutation](combinatorics.md#permutation); multiplying the outputs by five recovers the inputs. By contrast, multiplying by six gives only zero and six, with six inputs for each output. It cannot be reversed.

<a id="image-multiplication-by-five-permutes-all-twelve-residue-classes-whereas-multiplication-by-six-merges-distinct-inputs"></a>
![](modular-multiplication-units-and-zero-divisors.png)

**[Figure 33](#image-multiplication-by-five-permutes-all-twelve-residue-classes-whereas-multiplication-by-six-merges-distinct-inputs). Multiplication by five permutes all twelve residue classes, whereas multiplication by six merges distinct inputs**.

In general, the exact criterion is

$$
[a]_n\text{ is a unit}\iff\gcd(a,n)=1.
$$

For the forward direction, $au-kn=1$ implies every common [divisor](#divisor) of $a,n$ divides one. Conversely, if their [greatest common divisor](#greatest-common-divisor) is one, [Bézout's identity](algebra.md#bezout-s-identity) supplies $ua+vn=1$, so $u$ is a [modular inverse](#modular-multiplicative-inverse). The [extended Euclidean algorithm](#extended-euclidean-algorithm) computes these coefficients. The [units](algebra.md#unit-in-a-ring) form the [unit group](algebra.md#unit-group) $(\mathbb Z/n\mathbb Z)^\times$ under [multiplication](arithmetic.md#multiplication). [Ankur Moitra, MIT 18.200, Lecture 15 (2024), pp. 3–4: inverses, coprimality and the unit group](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

[Multiplicative cancellation](commutative-algebra.md#multiplicative-cancellation-in-an-integral-domain) while keeping the same [integer modulus](#modulus-in-modular-arithmetic) is valid for a [unit modulo n](#unit-modulo-n): from $ca\equiv cb\pmod n$, multiply by a [modular inverse](#modular-multiplicative-inverse) of $c$ to get $a\equiv b\pmod n$. A nonunit cannot be cancelled as a general rule. For example, $6\cdot0\equiv6\cdot2\pmod{12}$, yet $0\not\equiv2\pmod{12}$. Thus [division](arithmetic.md#division-mathematics) by six cannot undo this [multiplication](arithmetic.md#multiplication); solving a [linear congruence](#linear-congruence) instead keeps track of all possible classes.

This distinction marks the boundary between [commutative rings](commutative-algebra.md#commutative-ring) and [fields](algebra.md#field). Modulo a [prime number](#prime-number) $p>1$, every nonzero [residue class](#residue-class) is a [unit](algebra.md#unit-in-a-ring), so $\mathbb Z/p\mathbb Z$ is a [finite field](algebra.md#finite-field). Modulo twelve it is a [commutative ring](commutative-algebra.md#commutative-ring) with [zero divisors](mathematics.md#zero-divisor), and is not a [field](algebra.md#field). For $n=1$, the sole class satisfies $[0]_1=[1]_1$ and is a [unit](algebra.md#unit-in-a-ring); this one-element [zero ring](commutative-algebra.md#zero-ring) is not a [field](algebra.md#field). [Moitra, MIT 18.200, Lecture 15, pp. 8–9: the prime-modulus field criterion](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf)

## Prime number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_number)

A [prime number](#prime-number) is a [positive integer](#positive-integer) $p>1$ whose only positive [divisors](#divisor) are $1$ and $p$. The first ten [prime numbers](#prime-number) are $2,3,5,7,11,13,17,19,23,29$. In contrast, $12=3\cdot4$ is a [composite number](#composite-number) because it has a positive [divisor](#divisor) strictly between one and itself. The [integer](#integer) one is neither a [prime number](#prime-number) nor a [composite number](#composite-number): the lower bound $p>1$ is part of the definition. Equivalently, the [divisor function](#divisor-function) satisfies $\tau(p)=2$ for a [prime number](#prime-number), whereas $\tau(1)=1$ and $\tau(n)\geq3$ for every [composite number](#composite-number) $n$.

[Prime numbers](#prime-number) are the building blocks of [positive integers](#positive-integer) under [multiplication](arithmetic.md#multiplication). The [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic) says that every [integer](#integer) greater than one is a [product](arithmetic.md#product-of-numbers) of [prime numbers](#prime-number), with a unique collection of factors when their order is ignored. For example, $12=2\cdot2\cdot3$ and $18=2\cdot3\cdot3$. Their common factors reveal the [greatest common divisor](#greatest-common-divisor) $6$, and the combined maximum powers reveal the [least common multiple](#least-common-multiple) $36$. A complicated [divisibility](#divisibility) question becomes a comparison of prime exponents.

There is also a useful finite test. If a [composite number](#composite-number) $n$ equals $ab$ with $1<a\leq b$, then $a^2\leq n$. Therefore some [prime factor](#prime-factor) is at most $\sqrt n$, and [trial division](#trial-division) only needs to check [prime numbers](#prime-number) up to that [square root](algebra.md#square-root). For $97$, checking $2,3,5,7$ suffices; none divides $97$, so it is a [prime number](#prime-number). For $91$, the same test finds $7$, giving $91=7\cdot13$. To find many [prime numbers](#prime-number) together, the [sieve of Eratosthenes](#sieve-of-eratosthenes) reuses the work by marking multiples.

The [division with remainder](#euclidean-division) calculations for $97$ make the test explicit:

$$
97=2\cdot48+1=3\cdot32+1=5\cdot19+2=7\cdot13+6.
$$

Since $9^2<97<10^2$, these are all the [prime numbers](#prime-number) at most its [square root](algebra.md#square-root), and every [remainder](#remainder) is nonzero. Thus the calculation certifies a [prime number](#prime-number), without testing the [integers](#integer) $8,9,10,\ldots,96$ individually. In contrast, $91=7\cdot13+0$ gives a [prime factor](#prime-factor) and proves that $91$ is a [composite number](#composite-number).

The definition has a long history. Book VII of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements) distinguishes [prime numbers](#prime-number) from [composite numbers](#composite-number) through their possible measures; Book IX, Proposition 20 establishes that no finite list exhausts the [prime numbers](#prime-number). The modern argument under [Euclid's theorem](#euclid-s-theorem) needs only [divisibility](#divisibility), so it proves an infinite conclusion without estimating how frequently [prime numbers](#prime-number) occur. [Euclid, Elements, Book VII, definitions 11–14, David Joyce's edition](https://mathcs.clarku.edu/~djoyce/elements/bookVII/defVII11.html) [Euclid, Elements, Book IX, Proposition 20](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX20.html).

### Primality

↑ **Parent:** [Prime number](#prime-number)

[Primality](#primality) is the property of a [positive integer](#positive-integer) being a [prime number](#prime-number). [Primality testing](computer-science.md#primality-testing) determines this property; [integer factorization](#integer-factorization) asks for factors and is a different computational task.

### Trial division

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Trial_division)

[Trial division](#trial-division) searches for [divisors](#divisor) of an [integer](#integer) by testing candidate divisions. For [primality testing](computer-science.md#primality-testing) of an [integer](#integer) $n>1$, testing the [prime numbers](#prime-number) up to $\sqrt n$ suffices: any [composite number](#composite-number) has a [prime factor](#prime-factor) in that range. After finding a [prime factor](#prime-factor), repeated [division](arithmetic.md#division-mathematics) removes its [prime power](#prime-power), and testing the remaining quotient gives an elementary [integer factorization](#integer-factorization) method. This is useful for small inputs, but the number of candidates can grow rapidly with the input's digit count.

### Sieve of Eratosthenes

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sieve_of_Eratosthenes)

The [sieve of Eratosthenes](#sieve-of-eratosthenes) finds all [prime numbers](#prime-number) at most an [integer](#integer) $N\geq2$. Start with the [integers](#integer) $2,\ldots,N$ marked as candidates. For each surviving candidate $p$ in increasing order, mark the multiples $p^2,p^2+p,\ldots$ up to $N$ as [composite numbers](#composite-number). Stop processing candidates once $p^2>N$: the surviving candidates are exactly the [prime numbers](#prime-number). Starting at $p^2$ saves work because any smaller proper multiple of $p$ already has a smaller [prime factor](#prime-factor). [Jerry Cain, Stanford CS106AJ, Section Handout 6, Problem 4: the sieve of Eratosthenes](https://web.stanford.edu/class/cs106aj/res/handouts/36-Section-6.pdf).

For a complete run with $N=60$, the only [prime numbers](#prime-number) at most $\sqrt{60}$ are $2,3,5,7$, since $7^2\leq60<8^2$. Exclude one before starting; it is not a [prime number](#prime-number). The four marking passes are:
- $p=2$: mark $4,6,8,\ldots,60$, removing 29 candidates.
- $p=3$: mark $9,12,15,\ldots,60$. The nine newly removed candidates are $9,15,21,27,33,39,45,51,57$; the [even integers](#even-number) were already marked.
- $p=5$: mark $25,30,35,40,45,50,55,60$. Only $25,35,55$ are newly removed.
- $p=7$: mark $49,56$. Only $49$ is newly removed.

There are $59-29-9-3-1=17$ surviving [prime numbers](#prime-number):

$$
2,3,5,7,11,13,17,19,23,29,31,37,41,43,47,53,59.
$$

The next surviving candidate is $11$, and $11^2>60$, so no further marking pass is necessary. A [prime number](#prime-number) used for marking remains a candidate: starting at $p^2$ never marks $p$ itself.

<a id="image-four-passes-of-the-sieve-of-eratosthenes-through-60-leave-seventeen-prime-numbers"></a>
![](prime-sieve-steps.png)

**[Figure 34](#image-four-passes-of-the-sieve-of-eratosthenes-through-60-leave-seventeen-prime-numbers). Four passes of the sieve of Eratosthenes through 60 leave seventeen prime numbers**. Blue cells are newly marked [composite numbers](#composite-number); gray cells were removed earlier. White cells are candidates in the first three panels, and green cells are the final [prime numbers](#prime-number). The outlined cell identifies the [prime number](#prime-number) used for that pass. One is excluded throughout.

The saving from starting at $p^2$ is justified by the smaller multiplier: if $p k<p^2$ with $2\leq k<p$, then $k$ has a [prime factor](#prime-factor) $q<p$, so $q$ has already marked $p k$. For $p=7$, the earlier multiples $14,21,28,35,42$ have already been marked using $2,3$ or $5$. The first new possibility is $49$.

For $N=100$, only the [prime numbers](#prime-number) $2,3,5,7$ need marking passes. They remove all the [composite numbers](#composite-number), leaving **25 [prime numbers](#prime-number)**. The diagram colors each [composite number](#composite-number) by its smallest [prime factor](#prime-factor), so it shows which marking pass removes it first. The excluded [integer](#integer) one is shown separately.

<a id="image-the-sieve-of-eratosthenes-leaves-25-prime-numbers-among-the-integers-from-one-to-100"></a>
![](prime-sieve-smallest-factors.png)

**[Figure 35](#image-the-sieve-of-eratosthenes-leaves-25-prime-numbers-among-the-integers-from-one-to-100). The sieve of Eratosthenes leaves 25 prime numbers among the integers from one to 100**. Each colored [composite number](#composite-number) is assigned to its smallest [prime factor](#prime-factor), one of $2,3,5,7$. The green survivors are [prime numbers](#prime-number); one is neither a [prime number](#prime-number) nor a [composite number](#composite-number).

Why does the [algorithm](computer-science.md#algorithm) work? A surviving candidate cannot be a [composite number](#composite-number), since its smaller [prime factor](#prime-factor) would already have removed it. Conversely, marking proper multiples never removes a [prime number](#prime-number). Every [composite number](#composite-number) at most $N$ has a [prime factor](#prime-factor) at most $\sqrt N$, so no later pass is needed. The [sieve of Eratosthenes](#sieve-of-eratosthenes) is useful when an entire bounded list is wanted; [primality testing](computer-science.md#primality-testing) of one large [integer](#integer) is a different computational task.

The historical name is supported by a surviving primary account: Nicomachus, in Book I, chapter 13 of _Introduction to Arithmetic_, names Eratosthenes and describes separating [prime numbers](#prime-number) from [composite numbers](#composite-number) by marking multiples among the [odd integers](#odd-integer) beginning with three. That passage documents the sieve tradition; the bounded [algorithm](computer-science.md#algorithm) above and its $p^2$ starting rule are the formulation explained here, rather than instructions quoted from [Euclid's Elements](geometry-and-topology.md#euclid-s-elements). [Nicomachus, Introduction to Arithmetic I.13.2–8, Martin Luther D'Ooge translation (1926), revised classroom edition by Nathanael Hahn (2025), pp. 24–25](https://stoicheiamath.com/wp-content/uploads/2025/09/Nicomachus-Introduction-to-Arithmetic-Student-Edition.pdf#page=28)

### Infinitely many primes congruent to one modulo six

↑ **Parent:** [Prime number](#prime-number)

Assume that $x^2\equiv-3\pmod p$ with $p>3$ implies $p\equiv1\pmod6$. For a finite list of primes in that residue class, let $P$ be their product. Every prime divisor of $4P^2+3$ is greater than three and satisfies that quadratic [modular congruence](#modular-congruence), hence has residue one modulo six. None is listed because $4P^2+3\equiv3$ modulo a listed prime.

// Target: combinatorics.bigb

### Infinitely many primes congruent to minus one modulo six

↑ **Parent:** [Prime number](#prime-number)

For any finite list of such [prime numbers](#prime-number), let $P$ be their product. The integer $6P-1$ has no listed prime divisor, nor the divisors $2,3$. Its remaining prime factors have residues $1,-1$ modulo six, and at least one has residue $-1$ because their product has that residue. Thus no finite list is exhaustive.

// Target: number-theory.bigb

<h3 id="bertrand-s-postulate">Bertrand's postulate</h3>

↑ **Parent:** [Prime number](#prime-number)

For every integer $n>1$, there is a [prime number](#prime-number) strictly between $n$ and $2n$. This supplies cyclic prime moduli comparable to an integer interval's length in [additive combinatorics](additive-combinatorics.md).

### Twin prime

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Twin_prime)

Two [primes](#prime-number) differing by two form a twin-prime pair, for example $3,5$ or $11,13$. The [twin-prime upper bound using Bombieri–Vinogradov](#twin-prime-upper-bound-using-bombieri-vinogradov) limits their number without proving there are infinitely many.

#### Twin prime conjecture

↑ **Parent:** [Twin prime](#twin-prime)

The conjecture asserts that infinitely many [prime numbers](#prime-number) $p$ have $p+2$ prime. The [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture) predicts their quantitative frequency and is stronger. The [Selberg sieve](analytic-number-theory.md#selberg-sieve) supplies an upper bound of the predicted order but does not prove infinitude.

<h5 id="hardy-littlewood-twin-prime-asymptotic-conjecture">Hardy–Littlewood twin-prime asymptotic conjecture</h5>

↑ **Parent:** [Twin prime conjecture](#twin-prime-conjecture)

The local-density prediction for twin primes is the displayed asymptotic, with the [twin-prime constant](#twin-prime-constant) $C_2$. It is stronger than infinitude alone. The [Selberg sieve](analytic-number-theory.md#selberg-sieve) proves the correct order of magnitude as an upper bound, but the [parity problem in sieve theory](analytic-number-theory.md#parity-problem) prevents its elementary majorant from proving this conjectured asymptotic.

// Target: analytic-number-theory.bigb

##### Twin-prime constant

↑ **Parent:** [Twin prime conjecture](#twin-prime-conjecture)

This positive convergent product corrects for the dependence of primality of $n$ and $n+2$ at each odd prime. The associated singular series is $2C_2$: the factor at two is two, and at an odd prime the local correction is $(1-2/p)/(1-1/p)^2$. It appears in the [Hardy–Littlewood twin-prime asymptotic conjecture](#hardy-littlewood-twin-prime-asymptotic-conjecture) and in upper bounds from the [Selberg sieve](analytic-number-theory.md#selberg-sieve).

// Target: analytic-number-theory.bigb

<h4 id="brun-s-theorem">Brun's theorem</h4>

↑ **Parent:** [Twin prime](#twin-prime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Brun's_theorem)

The sum of reciprocals of [twin primes](#twin-prime) converges, whether or not there are infinitely many [twin primes](#twin-prime). The [twin-prime upper bound from a quadratic sieve](analytic-number-theory.md#twin-prime-upper-bound-from-a-quadratic-sieve) and [reciprocal-sum convergence from a counting bound](analytic-number-theory.md#reciprocal-sum-convergence-from-a-counting-bound) prove it. This contrasts with the [Euler proof that the sum of reciprocals of primes diverges](analytic-number-theory.md#euler-proof-that-the-sum-of-reciprocals-of-primes-diverges).

<h4 id="twin-prime-upper-bound-using-bombieri-vinogradov">Twin-prime upper bound using Bombieri–Vinogradov</h4>

↑ **Parent:** [Twin prime](#twin-prime)

Apply the [Selberg upper-bound sieve](analytic-number-theory.md#selberg-upper-bound-sieve) to the numbers $p+2$ with $p\leq x$ [prime](#prime-number). For [odd](calculus.md#odd-function) [squarefree integers](#squarefree-integer) $d$, the local count is $\pi(x;d,-2)$ and the density is $1/\phi(d)$. With sieve level $D=x^{1/3}$, the normalizing sum is $\gg\log x$ by the [truncated Euler-product lower bound](analytic-number-theory.md#truncated-euler-product-lower-bound). The [Selberg least-common-multiple weights](analytic-number-theory.md#selberg-least-common-multiple-weights) have [absolute values](real-analysis.md#absolute-value) at most $3^{\omega(d)}$. The [weighted arithmetic-progression error bound](analytic-number-theory.md#weighted-arithmetic-progression-error-bound) and [Bombieri–Vinogradov theorem](analytic-number-theory.md#bombieri-vinogradov-theorem) make their total error $O(x/\log^3x)$. Consequently the number of [twin prime](#twin-prime) pairs with smaller member at most $x$ is $O(x/\log^2x)$.

<h3 id="euclid-s-theorem">Euclid's theorem</h3>

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid's_theorem)

There are infinitely many [prime numbers](#prime-number). Indeed, for any finite list of [prime numbers](#prime-number) $p_1,\ldots,p_k$, the [integer](#integer) $N=p_1\cdots p_k+1>1$ has a [prime factor](#prime-factor), by the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). None of the listed [prime numbers](#prime-number) divides $N$, since each divides $N-1$ and a common [divisor](#divisor) would divide $1$. Thus no finite list contains all [prime numbers](#prime-number). The constructed $N$ need not itself be a [prime number](#prime-number).

For example, the first six [prime numbers](#prime-number) give

$$
2\cdot3\cdot5\cdot7\cdot11\cdot13+1=30031=59\cdot509.
$$

Both [prime factors](#prime-factor) lie outside the original list, although $30031$ is a [composite number](#composite-number). The construction defeats a proposed complete list; it is not a formula guaranteed to produce a [prime number](#prime-number). Book IX, Proposition 20 of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements) explicitly considers both possibilities, prime and composite. [Euclid, Elements, Book IX, Proposition 20: a prime or composite successor](https://mathcs.clarku.edu/~djoyce/elements/bookIX/propIX20.html).

### Odd prime

↑ **Parent:** [Prime number](#prime-number)

An odd prime is a [prime number](#prime-number) that is an [odd integer](#odd-integer). The only [even number](#even-number) that is a [prime number](#prime-number) is $2$, since every other positive [even number](#even-number) has $2$ as a proper [divisor](#divisor). Thus every [prime number](#prime-number) greater than $2$ is an odd prime. There are infinitely many odd primes, by [Euclid's theorem](#euclid-s-theorem).

### Fermat prime

↑ **Parent:** [Prime number](#prime-number)

A [Fermat prime](#fermat-prime) is a [Fermat number](#fermat-number) that is also a [prime number](#prime-number):

$$
F_k=2^{2^k}+1,\qquad k\geq0.
$$

The defining form alone does not imply [primality](#primality). For example, $65537$ is a [Fermat prime](#fermat-prime), while $4294967297$ is a [Fermat number](#fermat-number) with proper [divisors](#divisor). For $k\geq1$, every [Fermat prime](#fermat-prime) is one modulo four and two modulo three. [Pépin's test](#pepin-s-test) gives an exact [primality testing](computer-science.md#primality-testing) criterion for these candidates, rather than relying on their form.

<h4 id="pepin-s-test">Pépin's test</h4>

↑ **Parent:** [Fermat prime](#fermat-prime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pépin's_test)

For $n\geq1$, [Pépin's test](#pepin-s-test) says that the [Fermat number](#fermat-number) $F_n$ is a [prime number](#prime-number) exactly when the displayed [modular congruence](#modular-congruence) holds. [Modular exponentiation](#modular-exponentiation) evaluates it by [exponentiation by squaring](#exponentiation-by-squaring) without constructing the enormous ordinary power. The index restriction excludes $F_0=3$, where the base itself is divisible by the candidate.[slide 14](mathematics-bibliography.md#primality-testing-then-and-now-by-carl-pomerance)

For a proof outline of sufficiency, any [prime factor](#prime-factor) $p$ of a passing candidate gives $3$ [multiplicative order](#multiplicative-order) exactly $F_n-1$, a [power of two](#power-of-two): its half-power is $-1$, rather than $1$. [Fermat's little theorem](#fermat-little-theorem) forces $F_n-1\mid p-1$, so $p\geq F_n$, and hence $p=F_n$. Conversely, for a prime candidate, $F_n\equiv5\pmod{12}$; [quadratic reciprocity](#quadratic-reciprocity) and [Euler's criterion](#euler-s-criterion) give the required half-power. At $n=1$, the check is $3^2\equiv4=-1\pmod5$.

#### Quadratic nonresidues modulo a Fermat prime

↑ **Parent:** [Fermat prime](#fermat-prime)

For a Fermat prime $p=2^{2^k}+1$, the multiplicative group modulo $p$ has order $2^{2^k}$. Its $\varphi(p-1)=(p-1)/2$ primitive roots are all quadratic nonresidues; since there are also $(p-1)/2$ nonresidues, the two sets coincide.

### Fundamental theorem of arithmetic

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fundamental_theorem_of_arithmetic)

Every [integer](#integer) $n>1$ is a [product](arithmetic.md#product-of-numbers) of [prime numbers](#prime-number), uniquely up to reordering the factors. More precisely, there are unique distinct [prime numbers](#prime-number) $p_1<\cdots<p_r$ and unique positive [integer](#integer) exponents $a_1,\ldots,a_r$ such that

$$
n=p_1^{a_1}\cdots p_r^{a_r}.
$$

In the header's displayed form, $v_p(n)$ is the [prime valuation](#prime-valuation), the exponent of $p$ in this [prime factorization](#fundamental-theorem-of-arithmetic); it is zero when $p$ does not divide $n$. Reordering or regrouping the [prime factors](#prime-factor) does not give a different [prime factorization](#fundamental-theorem-of-arithmetic).

For $360$, repeated [division](arithmetic.md#division-mathematics) gives $360/2=180$, $180/2=90$, $90/2=45$, then $45/3=15$, $15/3=5$, and $5/5=1$. Thus

$$
360=2\cdot2\cdot2\cdot3\cdot3\cdot5=2^3\cdot3^2\cdot5,
\qquad 2^3\cdot3^2\cdot5=8\cdot9\cdot5=360.
$$

Its nonzero [prime valuations](#prime-valuation) are $v_2(360)=3$, $v_3(360)=2$ and $v_5(360)=1$. Recording only the distinct [prime factors](#prime-factor) $2,3,5$ would lose the difference between $30$ and $360$.

This turns [divisibility](#divisibility) into coordinatewise comparison of nonnegative exponents. A positive [divisor](#divisor) of $360$ chooses an exponent from $0,1,2,3$ for $2$, from $0,1,2$ for $3$, and from $0,1$ for $5$, giving $4\cdot3\cdot2=24$ positive [divisors](#divisor). The [greatest common divisor](#greatest-common-divisor) takes the smaller exponent at each [prime number](#prime-number); the [least common multiple](#least-common-multiple) takes the larger. The theorem is a structural description, not an assertion that finding the factors of every large [integer](#integer) is computationally easy.

In general, for [positive integers](#positive-integer) $d,n$, the exact [divisibility](#divisibility) criterion is

$$
d\mid n\quad\Longleftrightarrow\quad v_p(d)\leq v_p(n)\ \text{for every prime }p.
$$

For example, $72=2^3\cdot3^2$ divides $360$, with quotient $5$, whereas $48=2^4\cdot3$ does not: it requires four factors of two, but $360$ supplies only three. Both use only [prime factors](#prime-factor) of $360$, so membership in that list alone does not establish [divisibility](#divisibility). Every positive [divisor](#divisor) of $360$ is uniquely $2^a3^b5^c$ with $0\leq a\leq3$, $0\leq b\leq2$, $0\leq c\leq1$. Sorted, all 24 positive [divisors](#divisor) are

$$
\begin{gathered}
1,2,3,4,5,6,8,9,10,12,15,18,\\
20,24,30,36,40,45,60,72,90,120,180,360.
\end{gathered}
$$

Thus the [divisor function](#divisor-function) gives $\tau(360)=(3+1)(2+1)(1+1)=24$. These include [divisors](#divisor) that are [composite numbers](#composite-number), as well as the [prime factors](#prime-factor) and one.

For another [positive integer](#positive-integer) $m$, the [prime valuations](#prime-valuation) give exact formulas for the [greatest common divisor](#greatest-common-divisor) and [least common multiple](#least-common-multiple):

$$
\begin{aligned}
v_p(\gcd(n,m))&=\min\{v_p(n),v_p(m)\},\\
v_p(\operatorname{lcm}(n,m))&=\max\{v_p(n),v_p(m)\}.
\end{aligned}
$$

With $n=360$ and $m=84=2^2\cdot3\cdot7$, their [prime valuations](#prime-valuation) at $2,3,5,7$ are $(3,2,1,0)$ and $(2,1,0,1)$. The smaller exponents give $(2,1,0,0)$, and the larger give $(3,2,1,1)$, hence

$$
\gcd(360,84)=2^2\cdot3=12,\qquad
\operatorname{lcm}(360,84)=2^3\cdot3^2\cdot5\cdot7=2520.
$$

Indeed, $360/12=30$, $84/12=7$, $2520/360=7$ and $2520/84=30$. The same rules also explain $\gcd(n,m)\operatorname{lcm}(n,m)=nm$: the smaller and larger exponents sum to the two original exponents. Here $12\cdot2520=360\cdot84=30240$.

<a id="image-prime-valuations-compute-the-greatest-common-divisor-least-common-multiple-and-all-24-positive-divisors-of-360"></a>
![](prime-factorization-exponents.png)

**[Figure 36](#image-prime-valuations-compute-the-greatest-common-divisor-least-common-multiple-and-all-24-positive-divisors-of-360). Prime valuations compute the greatest common divisor, least common multiple and all 24 positive divisors of 360**. The upper table compares exponents at the [prime numbers](#prime-number) $2,3,5,7$ for $360$ and $84$, then takes their columnwise minimum and maximum. The lower tables enumerate $2^a3^b5^c$ for $c=0$ and $c=1$; each cell gives one positive [divisor](#divisor).

The useful change of viewpoint is that [multiplication](arithmetic.md#multiplication) becomes [addition](arithmetic.md#addition) of [prime valuations](#prime-valuation), $v_p(nm)=v_p(n)+v_p(m)$, and [divisibility](#divisibility) becomes comparison. Many different-looking calculations therefore share one representation. The [prime valuations](#prime-valuation) are coordinates for [multiplication](arithmetic.md#multiplication), rather than digits in [positional notation](#positional-notation): they do not turn ordinary [addition](arithmetic.md#addition) of [integers](#integer) into coordinatewise [addition](arithmetic.md#addition).

Different intermediate splits lead to the same prime ingredients. Starting with $360=36\cdot10$ gives $36=6\cdot6$ and $10=2\cdot5$; starting with $360=8\cdot45$ gives $8=2\cdot4$ and $45=5\cdot9$. Continuing to split the [composite numbers](#composite-number) produces the same [multiset](set.md#multiset) of [prime factors](#prime-factor): three twos, two threes, and one five. The [factorization tree](#factorization-tree) records choices in the calculation, while the [prime factorization](#fundamental-theorem-of-arithmetic) records the invariant result.

<a id="image-two-factorization-trees-for-360-give-the-same-prime-factorization-2-3-cdot3-2-cdot5"></a>
![](prime-factorization-trees.png)

**[Figure 37](#image-two-factorization-trees-for-360-give-the-same-prime-factorization-2-3-cdot3-2-cdot5). Two factorization trees for $360$ give the same prime factorization $2^3\cdot3^2\cdot5$**.

The proof outline explains the uniqueness. Existence follows by splitting a [composite number](#composite-number) into smaller factors until only [prime numbers](#prime-number) remain. For uniqueness, [Euclid's lemma](#euclid-s-lemma) says that a [prime factor](#prime-factor) of one [product](arithmetic.md#product-of-numbers) must divide one factor of any other prime [product](arithmetic.md#product-of-numbers) equal to it. That factor must be the same [prime number](#prime-number); cancel it and repeat. The crucial [divisibility](#divisibility) step appears in Book VII, Proposition 30 of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements). [Euclid, Elements VII.30: a prime divisor of a product](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII30.html)

The ancient text supplies specific precursors to the modern statement: Book VII, Proposition 31 establishes that every [composite number](#composite-number) has a [prime factor](#prime-factor), and Book IX, Proposition 14 excludes any new [prime factor](#prime-factor) from the [least common multiple](#least-common-multiple) of given [prime numbers](#prime-number). These are the propositions being cited, rather than the complete modern exponent formulation of the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). [Euclid, Elements VII.31: every composite number has a prime divisor](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII31.html) [Euclid, Elements IX.14: prime divisors of a least common multiple of primes](https://mathcs.clarku.edu/~djoyce/java/elements/bookIX/propIX14.html)

Excluding one from the [prime numbers](#prime-number) keeps uniqueness meaningful: otherwise $360=2^3\cdot3^2\cdot5=1\cdot2^3\cdot3^2\cdot5=1\cdot1\cdot2^3\cdot3^2\cdot5$ would give different collections of supposed [prime factors](#prime-factor). For $n=1$, the natural convention is the [empty product](arithmetic.md#empty-product), equal to one, with no [prime factors](#prime-factor) and all [prime valuations](#prime-valuation) zero.

#### Factorization tree

↑ **Parent:** [Fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic)

A [factorization tree](#factorization-tree) is a [rooted tree](combinatorics.md#rooted-tree) whose root is an [integer](#integer) $n>1$. Each nonleaf label is a [composite number](#composite-number) split into two factors greater than one whose [product](arithmetic.md#product-of-numbers) equals that label; the leaves are [prime numbers](#prime-number). Multiplying the leaves recovers $n$. Many [factorization trees](#factorization-tree) can have the same root, but the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic) gives them the same leaf [multiset](set.md#multiset).

### Prime factor

↑ **Parent:** [Prime number](#prime-number)

A [prime factor](#prime-factor) of a nonzero [integer](#integer) $n$ is a [prime number](#prime-number) $p$ satisfying $p\mid n$. For $360=2^3\cdot3^2\cdot5$, the distinct [prime factors](#prime-factor) are $2,3,5$, while counting repeated factors gives six prime entries. A [prime factorization](#fundamental-theorem-of-arithmetic) retains their multiplicities: knowing only the distinct [prime factors](#prime-factor) does not distinguish $12=2^2\cdot3$ from $18=2\cdot3^2$. A negative [integer](#integer) has the same [prime factors](#prime-factor) as its [absolute value](real-analysis.md#absolute-value).

### Prime power

↑ **Parent:** [Prime number](#prime-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_power)

A prime power is a positive integer of the form $p^d$, where $p$ is a [prime number](#prime-number) and $d$ is a nonnegative integer.

## Composite number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Composite_number)

A [composite number](#composite-number) is an [integer](#integer) greater than one that is not a [prime number](#prime-number). Equivalently, it has a factorization $n=ab$ with [integers](#integer) $a,b>1$. Thus $4=2\cdot2$, $9=3\cdot3$, and $12=3\cdot4$ are [composite numbers](#composite-number); one is neither a [composite number](#composite-number) nor a [prime number](#prime-number).

Every [composite number](#composite-number) has a [prime factor](#prime-factor) at most its [square root](algebra.md#square-root). In $91=7\cdot13$, seven is the smaller factor and lies below $\sqrt{91}$; in $49=7^2$, equality occurs. This square-root bound makes [trial division](#trial-division) finite and lets the [sieve of Eratosthenes](#sieve-of-eratosthenes) stop marking with [prime numbers](#prime-number) beyond $\sqrt N$ when listing [prime numbers](#prime-number) up to $N$.

### Semiprime

↑ **Parent:** [Composite number](#composite-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Semiprime)

A [semiprime](#semiprime) is a [composite number](#composite-number) that is a product of exactly two [prime numbers](#prime-number), counted with multiplicity. For example, $6=2\cdot3$ and $9=3^2$ are semiprimes. Distinct factors give $\varphi(pq)=(p-1)(q-1)$ for the [Euler totient function](#euler-totient-function), whereas equal factors give $\varphi(p^2)=p(p-1)$. This distinction matters when constructing a [uniform coprime state for a semiprime](quantum-circuit.md#uniform-coprime-state-for-a-semiprime).

<h2 id="euler-s-theorem">Euler's theorem</h2>

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_theorem)

For an [integer modulus](#modulus-in-modular-arithmetic) $n\geq2$ and an [integer](#integer) $a$ with [greatest common divisor](#greatest-common-divisor) $\gcd(a,n)=1$, Euler's theorem, also called the [Fermat-Euler theorem](#euler-s-theorem), states

$$
a^{\varphi(n)}\equiv1\pmod n.
$$

Here [Euler's totient function](#euler-totient-function) $\varphi(n)$ counts the [units](algebra.md#unit-in-a-ring) in the [unit group](algebra.md#unit-group) $U(n)=(\mathbb Z/n\mathbb Z)^\times$. These [congruence classes](#congruence-class) have [modular multiplicative inverses](#modular-multiplicative-inverse), equivalently their representatives are [coprime](#coprime-integers) to $n$. The guaranteed return to one permits [exponent reduction for units](#exponent-reduction-for-units).[p. 1, Theorem 1.2 and equation (1.1): modulus at least two, invertible classes and totient](mathematics-bibliography.md#euler’s-theorem-by-keith-conrad)

For a [prime number](#prime-number) $p$, $\varphi(p)=p-1$, recovering [Fermat's little theorem](#fermat-little-theorem) in the form $a^{p-1}\equiv1\pmod p$ when $p\nmid a$. Multiplying by $a$ and separately handling $p\mid a$ gives $a^p\equiv a\pmod p$ for every [integer](#integer) $a$. For a [composite number](#composite-number) used as the [integer modulus](#modulus-in-modular-arithmetic), a nonzero [congruence class](#congruence-class) can be a [nonunit](algebra.md#nonunit).

Modulo twelve, the [units](algebra.md#unit-in-a-ring) have representatives $1,5,7,11$, so [Euler's totient function](#euler-totient-function) gives $\varphi(12)=4$. [Multiplication](arithmetic.md#multiplication) by five produces

$$
1\longmapsto5\longmapsto1,\qquad
7\longmapsto11\longmapsto7\pmod{12}.
$$

Thus this [permutation](combinatorics.md#permutation) has two [permutation cycles](finite-group-theory.md#permutation-cycle), each of length two. In particular $5^2\equiv1\pmod{12}$, and the guaranteed return $5^4\equiv1$ follows. **The number of [units](algebra.md#unit-in-a-ring) need not be the length of one [permutation cycle](finite-group-theory.md#permutation-cycle).** Modulo fifteen, [multiplication](arithmetic.md#multiplication) by seven similarly gives the two [permutation cycles](finite-group-theory.md#permutation-cycle) $(1,7,4,13)$ and $(2,14,8,11)$, covering all eight [units](algebra.md#unit-in-a-ring). The powers of seven follow the [permutation cycle](finite-group-theory.md#permutation-cycle) containing one; the other [permutation cycle](finite-group-theory.md#permutation-cycle) shows that these powers do not visit every [unit](algebra.md#unit-in-a-ring).

<a id="image-two-unit-permutations-multiplication-by-five-modulo-twelve-and-by-seven-modulo-fifteen"></a>
![](euler-unit-residue-permutation-cycles.png)

**[Figure 38](#image-two-unit-permutations-multiplication-by-five-modulo-twelve-and-by-seven-modulo-fifteen). Two unit permutations: multiplication by five modulo twelve and by seven modulo fifteen**. Every arrow multiplies by the indicated [unit](algebra.md#unit-in-a-ring) and reduces modulo the indicated [integer modulus](#modulus-in-modular-arithmetic). The [permutation cycles](finite-group-theory.md#permutation-cycle) exhaust each [reduced residue system](#reduced-residue-system). The [permutation cycle](finite-group-theory.md#permutation-cycle) containing one records the powers of the multiplier; its length is the multiplier's [multiplicative order](#multiplicative-order), which can be smaller than [Euler's totient function](#euler-totient-function).

There is a stronger obstruction for a [nonunit](algebra.md#nonunit) than just an occasional failed calculation. If a [positive integer](#positive-integer) $d>1$ divides both $a$ and $n$, then $a^k\equiv0\pmod d$ for every $k\geq1$, so $a^k$ cannot be congruent to one modulo $n$. For example, $\gcd(3,15)=3$ and $3^{\varphi(15)}=3^8\equiv6\pmod{15}$, rather than one. Such a base has no [multiplicative order](#multiplicative-order) modulo that [integer modulus](#modulus-in-modular-arithmetic).[p. 2, explanation following Example 1.8: a positive-exponent return to one forces coprimality](mathematics-bibliography.md#orders-of-units-in-modular-arithmetic-by-keith-conrad)

### Multiplication by a unit permutes reduced residues

↑ **Parent:** [Euler's theorem](#euler-s-theorem)

Choose a [reduced residue system](#reduced-residue-system) $u_1,\ldots,u_{\varphi(n)}$. For a [unit modulo n](#unit-modulo-n) $a$, the [bijection](function.md#bijection) $u\mapsto au$ on the [unit group](algebra.md#unit-group) has inverse $u\mapsto a^{-1}u$. Comparing products before and after this [permutation](combinatorics.md#permutation) gives

$$
P=\prod_{i=1}^{\varphi(n)}u_i
\equiv\prod_{i=1}^{\varphi(n)}(au_i)
=a^{\varphi(n)}P\pmod n.
$$

The product $P$ is a [unit](algebra.md#unit-in-a-ring); its [modular inverse](#modular-multiplicative-inverse) cancels it, proving [Euler's theorem](#euler-s-theorem). Merely being nonzero would not justify cancellation.[pp. 2–3, Section 2: permutation of the units, comparison of products, cancellation](mathematics-bibliography.md#euler’s-theorem-by-keith-conrad)

In the modulo-twelve example, $P=1\cdot5\cdot7\cdot11=385\equiv1\pmod{12}$. The permuted representatives $5,1,11,7$ have the same product, while the unreduced products $(5\cdot1)(5\cdot5)(5\cdot7)(5\cdot11)$ equal $5^4P$. Equating these products modulo twelve exposes the fourth power without calculating it directly. Using all nonzero [congruence classes](#congruence-class) instead would include [nonunits](algebra.md#nonunit), whose product need not permit cancellation.

### Exponent reduction for units

↑ **Parent:** [Euler's theorem](#euler-s-theorem)

For a [unit modulo n](#unit-modulo-n) $a$ and a [nonnegative integer](arithmetic.md#natural-number) $k$, [division with remainder](#euclidean-division) writes $k=q\varphi(n)+r$ with $0\leq r<\varphi(n)$. [Euler's theorem](#euler-s-theorem) then gives

$$
a^k=(a^{\varphi(n)})^q a^r\equiv a^r\pmod n.
$$

This replaces a potentially enormous [exponent](arithmetic.md#exponent) by a small [remainder](#remainder). The [exponent](arithmetic.md#exponent) itself is reduced modulo [Euler's totient function](#euler-totient-function), while the powers are reduced modulo $n$: these are different [integer moduli](#modulus-in-modular-arithmetic).

For a worked modulo-fifteen calculation, seven is [coprime](#coprime-integers) to fifteen and $\varphi(15)=8$. Therefore

$$
2029=253\cdot8+5,\qquad 7^{2029}\equiv7^5\pmod{15}.
$$

Use [exponentiation by squaring](#exponentiation-by-squaring) on the remaining [exponent](arithmetic.md#exponent) $5=(101)_2$, reducing after each [multiplication](arithmetic.md#multiplication):

$$
7^2\equiv49\equiv4,\qquad
7^4\equiv4^2\equiv1,\qquad
7^5\equiv1\cdot7\equiv7\pmod{15}.
$$

Thus **$7^{2029}\bmod15=7$**. [Modular exponentiation](#modular-exponentiation) supplies the computation; [Euler's theorem](#euler-s-theorem) supplies the optional shortening of its [exponent](arithmetic.md#exponent). [Exponentiation by squaring](#exponentiation-by-squaring) also works for [nonunit](algebra.md#nonunit) bases, without using this shortening.

The guaranteed [exponent](arithmetic.md#exponent) $\varphi(n)$ is a common return [exponent](arithmetic.md#exponent) and an upper bound on the shortest period; it need not be that period. The [multiplicative order](#multiplicative-order) $d=\operatorname{ord}_n(a)$ is the least positive return [exponent](arithmetic.md#exponent) for the chosen [unit](algebra.md#unit-in-a-ring). The [Carmichael function](#carmichael-function) $\lambda(n)$ is the least positive return [exponent](arithmetic.md#exponent) that works for every [unit](algebra.md#unit-in-a-ring). Their precise relation is

$$
\operatorname{ord}_n(a)\mid\lambda(n)\mid\varphi(n).
$$

Either smaller return [exponent](arithmetic.md#exponent) can replace $\varphi(n)$ in [exponent reduction for units](#exponent-reduction-for-units). Modulo fifteen, $\operatorname{ord}_{15}(7)=\lambda(15)=4<8=\varphi(15)$, so $2029=507\cdot4+1$ gives $7^{2029}\equiv7$ immediately. For base four the [multiplicative order](#multiplicative-order) is only two, smaller even than $\lambda(15)$. A return at [exponent](arithmetic.md#exponent) eight alone does not prove that the [multiplicative order](#multiplicative-order) is eight.[pp. 1–3, Definition 1.3, the warning on p. 2, Theorem 2.1, Corollary 2.2 and Theorem 2.4](mathematics-bibliography.md#orders-of-units-in-modular-arithmetic-by-keith-conrad)

<a id="image-actual-power-periods-carmichael-function-exponents-and-euler-return-exponents"></a>
![](euler-unit-powers-and-exponent-periods.png)

**[Figure 39](#image-actual-power-periods-carmichael-function-exponents-and-euler-return-exponents). Actual power periods, Carmichael function exponents and Euler return exponents**. Each row lists powers from exponent zero through eight. Highlighted first returns identify [multiplicative orders](#multiplicative-order); the accompanying labels distinguish a chosen base's shortest period, the common exponent for all [units](algebra.md#unit-in-a-ring), and [Euler's totient function](#euler-totient-function). Powers of the [nonunit](algebra.md#nonunit) three modulo fifteen repeat after an initial term but never return to one at a positive exponent. The final calculation compares reduction of $2029$ modulo eight and modulo four.

If the reduced [exponent](arithmetic.md#exponent) is zero, the rule gives $a^k\equiv a^0=1$, and still requires a [unit](algebra.md#unit-in-a-ring). Applying it to the [nonunit](algebra.md#nonunit) three would falsely predict $3^8\equiv3^0=1\pmod{15}$; the actual residue is six. For negative [exponents](arithmetic.md#exponent), first interpret the power using a [modular multiplicative inverse](#modular-multiplicative-inverse), as in [modular exponentiation](#modular-exponentiation).

### Generalized repunit pseudoprime construction

↑ **Parent:** [Euler's theorem](#euler-s-theorem)

For fixed $a>1$ and suitable odd primes $p$, the composite generalized repunit

$$
\frac{a^{2p}-1}{a^2-1}
$$

is congruent to one modulo $2p$ and is a pseudoprime to base $a$.

## Fermat pseudoprime

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_pseudoprime)

An odd composite number $N$ is a Fermat pseudoprime to a coprime base $b$ when

$$
b^{N-1}\equiv1\pmod N.
$$

### Strong pseudoprime

↑ **Parent:** [Fermat pseudoprime](#fermat-pseudoprime)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Strong_pseudoprime)

Write the even number $N-1$ as $2^s m$ with $m$ odd. An odd composite number $N$ is a strong pseudoprime to a coprime base $b$ when

$$
b^m\equiv1\pmod N
$$

or $b^{2^jm}\equiv-1\pmod N$ for some $0\leq j<s$.

#### Strong-pseudoprime bases for a product of two primes with common predecessor divisor ten

↑ **Parent:** [Strong pseudoprime](#strong-pseudoprime)

Let $N=pq$ for distinct odd [prime numbers](#prime-number) $p,q$ with $\gcd(p-1,q-1)=10$. Exactly $100$ unit bases make $N$ a [Fermat pseudoprime](#fermat-pseudoprime), and exactly $50$ of these make it a [strong pseudoprime](#strong-pseudoprime). The Fermat bases form $C_{10}\times C_{10}$ under the [Chinese remainder theorem for unit groups](mathematics.md#chinese-remainder-theorem-for-unit-groups). If $N-1=2^sm$, then $5\mid m$ and $m$ is odd, so the $m$th-power map sends five elements of each $C_{10}$ to $1$ and five to $-1$. The strong condition requires equal signs in both components, giving $5^2+5^2=50$.

## Euler pseudoprime

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_pseudoprime)

An odd composite number $N$ is an Euler pseudoprime to a coprime base $b$ when

$$
b^{(N-1)/2}\equiv\left(\frac bN\right)\pmod N,
$$

where the right side is the Jacobi symbol.

### Euler witness

↑ **Parent:** [Euler pseudoprime](#euler-pseudoprime)

For an odd integer $N$ and a unit $b$ modulo $N$, the base $b$ is an Euler witness when

$$
b^{(N-1)/2}\not\equiv\left(\frac bN\right)\pmod N.
$$

It therefore certifies that $N$ is composite.

#### Euler witnesses occupy at least half the unit bases

↑ **Parent:** [Euler witness](#euler-witness)

If one Euler witness $b_0$ exists modulo $N$, multiplication by $b_0$ injects the set of nonwitnesses into the set of witnesses. Indeed, the product of $b_0$ with a nonwitness cannot be another nonwitness, because cancellation and multiplicativity of the [Jacobi symbol](#jacobi-symbol) would make $b_0$ a nonwitness. Thus at least half of the units modulo $N$ are Euler witnesses.

#### Existence of an Euler witness for every odd composite integer

↑ **Parent:** [Euler witness](#euler-witness)

Every odd composite integer has an [Euler witness](#euler-witness). For a nonsquarefree integer, a base congruent to $1+p$ modulo a repeated prime factor $p^2$ fails the Euler congruence by the [binomial theorem](combinatorics.md#binomial-theorem). For a squarefree integer, use the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) to choose a base that is a [quadratic nonresidue](#quadratic-nonresidue) modulo one prime factor and $1$ modulo another. Its [Jacobi symbol](#jacobi-symbol) is $-1$, while its power is $1$ modulo the second factor.

#### Solovay-Strassen primality test

↑ **Parent:** [Euler witness](#euler-witness)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Solovay–Strassen_primality_test)

The Solovay-Strassen primality test samples unit bases and rejects an odd candidate as composite when it finds an [Euler witness](#euler-witness). Every prime passes every base by [Euler's criterion](#euler-s-criterion), while an odd composite passes a random base with probability at most one half.

## P-adic valuation

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/P-adic_valuation)

For a [prime number](#prime-number) $p$ and a nonzero [integer](#integer) $N$, the [P-adic valuation](#p-adic-valuation) counts the exponent of $p$ in its [prime factorization](#fundamental-theorem-of-arithmetic):

$$
v_p(N)=\max\{a\in\mathbb Z_{\geq0}:p^a\mid N\}.
$$

For $72=2^3\cdot3^2$, it gives $v_2(72)=3$, $v_3(72)=2$, and $v_5(72)=0$. The sign of a nonzero [integer](#integer) does not change these [prime exponents](#p-adic-valuation). Relative to an ordered [factor base](#factor-base), the valuations supply the coordinates of its [exponent vector](#exponent-vector).

The [P-adic valuation](#p-adic-valuation) extends to nonzero [rational numbers](#rational-number) by $v_p(a/b)=v_p(a)-v_p(b)$. For example, $v_5(72/25)=-2$ records a factor in the denominator instead of the numerator. [Multiplication](arithmetic.md#multiplication) adds valuations, $v_p(xy)=v_p(x)+v_p(y)$; this is the arithmetic reason why adding exponent vectors can make a product a square. In particular, a positive [integer](#integer) is a [square of a number](arithmetic.md#square-of-a-number) precisely when all its [prime exponents](#p-adic-valuation) are [even integers](#even-number), the criterion used by a [factor base](#factor-base).

### p-adic integer

↑ **Parent:** [P-adic valuation](#p-adic-valuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/p-adic_integer)

For a [prime number](#prime-number) $p$, the ring of p-adic integers is the [inverse limit](module-theory.md#inverse-limit)

$$
\mathbb Z_p=\varprojlim_n\mathbb Z/p^n\mathbb Z.
$$

Every p-adic integer has a unique convergent expansion $\sum_{j\geq0}b_jp^j$ with $0\leq b_j<p$. It is a complete [discrete valuation ring](commutative-algebra.md#discrete-valuation-ring) with [uniformizer](commutative-algebra.md#uniformizer) $p$ and [residue field](commutative-algebra.md#residue-field) $\mathbb F_p$.

#### Open subgroups of the p-adic integers

↑ **Parent:** [p-adic integer](#p-adic-integer)

The cosets $a+p^n\mathbb Z_p$ form a neighborhood basis in the additive group of [p-adic integers](#p-adic-integer). An open subgroup contains $p^n\mathbb Z_p$ for some $n$, so has finite index. Conversely, if the index is $m$, the finite quotient is annihilated by $m$, giving $m\mathbb Z_p\subset H$. Multiplication by the unit part of $m$ is bijective, so $m\mathbb Z_p=p^{v_p(m)}\mathbb Z_p$ is open. This proof applies to abstract subgroups without assuming beforehand that they are closed.

#### 7-adic integer

↑ **Parent:** [p-adic integer](#p-adic-integer)

A 7-adic integer is an element of the [p-adic integers](#p-adic-integer) for $p=7$, equivalently a compatible sequence of residues modulo $7^r$.

#### 2-adic integer

↑ **Parent:** [p-adic integer](#p-adic-integer)

A 2-adic integer is an element of the [p-adic integers](#p-adic-integer) for $p=2$, equivalently a compatible sequence of residues modulo $2^r$. Its reduction modulo two determines its [parity](quantum-mechanics.md#parity).

#### Topological generator of the additive group of p-adic integers

↑ **Parent:** [p-adic integer](#p-adic-integer)

An element $\alpha\in\mathbb Z_p$ topologically generates the additive group of $\mathbb Z_p$ exactly when $\alpha\not\equiv0\pmod p$, equivalently when $\alpha$ is a [p-adic unit](arithmetic.md#p-adic-unit). In that case its image generates every cyclic quotient $\mathbb Z/p^n\mathbb Z$.

### 2-adic valuation

↑ **Parent:** [P-adic valuation](#p-adic-valuation)

The 2-adic valuation is the [P-adic valuation](#p-adic-valuation) at the [prime number](#prime-number) $p=2$.

<h3 id="legendre-s-formula">Legendre's formula</h3>

↑ **Parent:** [P-adic valuation](#p-adic-valuation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Legendre's_formula)

For a [prime number](#prime-number) $p$ and a positive [integer](#integer) $n$, the [P-adic valuation](#p-adic-valuation) of a [factorial](combinatorics.md#factorial) is

$$
v_p(n!)=\sum_{j\geq1}\left\lfloor\frac{n}{p^j}\right\rfloor.
$$

### Base-p digit sum

↑ **Parent:** [P-adic valuation](#p-adic-valuation)

If

$$
n=\sum_{r\geq0}\alpha_rp^r,
\qquad 0\leq\alpha_r<p,
$$

then the base-$p$ digit sum is $d_p(n)=\sum_r\alpha_r$. The [Legendre formula](#legendre-s-formula) can equivalently be written

$$
v_p(n!)=\frac{n-d_p(n)}{p-1}.
$$

#### Subadditivity of the base-p digit sum

↑ **Parent:** [Base-p digit sum](#base-p-digit-sum)

For nonnegative integers $x$ and $y$,

$$
d_p(x+y)\leq d_p(x)+d_p(y).
$$

In column addition, every carry replaces $p$ units in one digit by one unit in the next digit and therefore decreases the digit sum by $p-1$.

### Valuation of a near-central binomial coefficient

↑ **Parent:** [P-adic valuation](#p-adic-valuation)

If $k\geq1$ and $k+2\leq p\leq2k+1$ is prime, then

$$
v_p\left(\binom{2k+1}{k+1}\right)=1.
$$

Indeed, neither $(k+1)!$ nor $k!$ contains a factor $p$, while $(2k+1)!$ contains $p$ exactly once because $2p>2k+1$.

## Primorial

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primorial)

For real $X\geq1$, the primorial up to $X$ is

$$
P(X)=\prod_{p\leq X}p,
$$

where the product ranges over primes.

### Chebyshev theta function

↑ **Parent:** [Primorial](#primorial)

The Chebyshev theta function is one of the two [Chebyshev functions](#chebyshev-function) and is the [natural logarithm](calculus.md#natural-logarithm) of the [primorial](#primorial):

$$
\vartheta(x)=\sum_{p\leq x}\log p
=\log\prod_{p\leq x}p,
$$

where both the sum and the product range over [prime numbers](#prime-number).

#### Elementary lower bound for the Chebyshev theta function

↑ **Parent:** [Chebyshev theta function](#chebyshev-theta-function)

The [central binomial coefficient](combinatorics.md#central-binomial-coefficient) and [Legendre formula](#legendre-s-formula) imply

$$
\vartheta(x)\geq\frac{x}{12}
$$

for every sufficiently large real number $x$.

### Elementary primorial bound

↑ **Parent:** [Primorial](#primorial)

For every real $X\geq1$,

$$
P(X)\leq4^X.
$$

For integer $n$, strong induction proves this by splitting according to parity. If $n=2k$, every prime in $(k,2k]$ divides $\binom{2k}{k}$, so

$$
P(2k)\leq P(k)\binom{2k}{k}\leq4^k4^k.
$$

If $n=2k+1$, the [valuation of a near-central binomial coefficient](#valuation-of-a-near-central-binomial-coefficient) gives

$$
P(2k+1)\leq P(k+1)\binom{2k+1}{k+1}\leq4^{k+1}4^k.
$$

The binomial estimates follow from the binomial theorem; in the odd case the two equal central coefficients together are at most $2^{2k+1}$. The result for real $X$ follows by replacing $X$ with $\lfloor X\rfloor$.

## Decisive number

↑ **Parent:** [Number theory](number-theory.md)

A positive [integer](#integer) $n$ is decisive when every [integer](#integer) $a$ satisfying $1<a<n$ and $\gcd(a,n)=1$ is a [prime number](#prime-number). There are only finitely many decisive numbers: every prime $p<\sqrt n$ must divide a decisive $n$, so the [Chebyshev theta function](#chebyshev-theta-function) gives $\log n\geq\vartheta(\sqrt n)$, which eventually contradicts the linear lower bound for $\vartheta(\sqrt n)$.

## Prime-counting function

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime-counting_function)

The prime-counting function $\pi(X)$ is the number of primes at most $X$.

### Legendre prime-counting formula

↑ **Parent:** [Prime-counting function](#prime-counting-function)

For $a=\pi(\sqrt x)$, let $p_1,\ldots,p_a$ be the [primes](#prime-number) at most $\sqrt x$. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) counts unsieved positive [integers](#integer) by $\phi(x,a)=\sum_S(-1)^{|S|}\lfloor x/\prod_{i\in S}p_i\rfloor$. These are $1$ and the remaining [primes](#prime-number), since every [composite number](#composite-number) has a [prime factor](#prime-factor) at most its square root. Hence $\pi(x)=\phi(x,a)+a-1$ for $x\geq2$. This is a prime-counting identity, distinct from the [Legendre formula](#legendre-s-formula) for factorial valuations.

### Prime-counting upper bound from a primorial estimate

↑ **Parent:** [Prime-counting function](#prime-counting-function)

If $P(X)\leq A^X$ for every $X\geq1$, where $A>1$, then

$$
\pi(X)\leq(1+2\log A)\frac{X}{\log X}
$$

for $X\geq2$. Every prime in $(\sqrt X,X]$ contributes at least $\sqrt X$ to the [primorial](#primorial), so

$$
(\sqrt X)^{\pi(X)-\pi(\sqrt X)}\leq P(X)\leq A^X.
$$

Taking logarithms, using $\pi(\sqrt X)\leq\sqrt X$, and observing that $\log X\leq\sqrt X$ for $X\geq2$ proves the claim.

## Primitive root modulo n

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Primitive_root_modulo_n)

A unit $g$ modulo $N$ is a primitive root when its multiplicative order is $\varphi(N)$.

### Lifting a primitive root to odd prime powers

↑ **Parent:** [Primitive root modulo n](#primitive-root-modulo-n)

Let $p$ be an odd prime and let $b$ be primitive modulo $p$. Then $b$ is primitive modulo every $p^m$ if and only if it is primitive modulo $p^2$. In that case

$$
\operatorname{ord}_{p^m}(b)=p^{m-1}(p-1).
$$

### Primitive-root modulus classification

↑ **Parent:** [Primitive root modulo n](#primitive-root-modulo-n)

An integer $n$ has a primitive root exactly when

$$
n\in\{1,2,4,p^a,2p^a\},
$$

where $p$ is an odd prime and $a\geq1$. When primitive roots exist, their number is $\varphi(\varphi(n))$.

## Quadratic residue

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_residue)

For an odd prime $p$, a nonzero class $a$ is a quadratic residue when $a\equiv x^2\pmod p$. These residues form an index-two subgroup of $(\mathbb Z/p\mathbb Z)^\times$.

### Square root of minus one modulo a prime

↑ **Parent:** [Quadratic residue](#quadratic-residue)

The congruence is soluble exactly for $p=2$ or $p\equiv1\pmod4$. For odd $p$, [Fermat's little theorem](#fermat-little-theorem) applied to a prospective root [forces](classical-mechanics.md#force) $(p-1)/2$ even. Conversely, when $p\equiv1\pmod4$, pair opposite factors in $(p-1)!$ and use the [Wilson theorem](#wilson-s-theorem) to obtain $(((p-1)/2)!)^2\equiv-1\pmod p$.

### Quadratic nonresidue

↑ **Parent:** [Quadratic residue](#quadratic-residue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_nonresidue)

A nonzero class modulo an odd prime is a quadratic nonresidue when it is not a square.

#### Least quadratic nonresidue

↑ **Parent:** [Quadratic nonresidue](#quadratic-nonresidue)

For an [odd prime](#odd-prime) $p$, the least quadratic nonresidue $n(p)$ is the smallest [positive integer](#positive-integer) whose nonzero [residue class](#residue-class) is a [quadratic nonresidue](#quadratic-nonresidue) modulo $p$.

##### Large-sieve logarithmic exceptional-prime bound for least quadratic nonresidues

↑ **Parent:** [Least quadratic nonresidue](#least-quadratic-nonresidue)

On a dyadic interval $Q<p\leq2Q$, every such exceptional prime makes all $Q^{0.01}$-smooth integers quadratic residues. By [positive density of power-smooth integers](#positive-density-of-power-smooth-integers), there are $\gg Q^2$ of these integers up to $Q^2$. Apply the [variance form of the large sieve](analytic-number-theory.md#variance-form-of-the-large-sieve) or its forbidden-residue consequence with interval length $Q^2$ and prime cutoff $2Q$. Each exceptional prime excludes $(p-1)/2$ residue classes and contributes at least a fixed positive amount to the sieve denominator. Hence each dyadic interval contains $O(1)$ exceptional primes. Summing the intervals gives the logarithmic bound.

// Target: analytic-number-theory.bigb

##### Bounded exceptional primes for least quadratic nonresidues

↑ **Parent:** [Least quadratic nonresidue](#least-quadratic-nonresidue)

If, for every $\eta>0$, the [smooth numbers](#smooth-number) up to $T$ with all [prime factors](#prime-factor) at most $T^\eta$ have density at least $\kappa(\eta)>0$, then for fixed $\varepsilon>0$ there are only $O_\varepsilon(1)$ [primes](#prime-number) $p\leq N$ with $n(p)>N^\varepsilon$. Apply the [variance form of the large sieve](analytic-number-theory.md#variance-form-of-the-large-sieve) to the [indicator function](measure-theory.md#indicator-function) of the $N^\varepsilon$-smooth numbers up to $N^2$. For every exceptional [prime](#prime-number), all these numbers are nonzero [quadratic residues](#quadratic-residue), so half its nonzero [residue classes](#residue-class) are empty. Their variance contribution is at least one third of the square of the total count. The large sieve bounds the sum of contributions by a constant times $N^2$ times that count. The density assumption with $\eta=\varepsilon/2$ finishes the argument.

### Quadratic Gauss sum

↑ **Parent:** [Quadratic residue](#quadratic-residue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_Gauss_sum)

For $\omega=e^{2\pi i/p}$ and the [Legendre symbol](#legendre-symbol) $\chi$, the quadratic Gauss sum is

$$
G(\chi)=\sum_{a=1}^{p-1}\chi(a)\omega^a.
$$

It equals $\sqrt p$ for $p\equiv1\pmod4$ and $i\sqrt p$ for $p\equiv3\pmod4$ with the standard choice of square root.

#### Quadratic periods modulo eleven

↑ **Parent:** [Quadratic Gauss sum](#quadratic-gauss-sum)

If $Q$ and $N$ are the nonzero square and nonsquare classes modulo eleven and $\omega=e^{2\pi i/11}$, then

$$
\sum_{q\in Q}\omega^q=\frac{-1+i\sqrt{11}}2,
\qquad
\sum_{n\in N}\omega^n=\frac{-1-i\sqrt{11}}2.
$$

Their sum is $-1$, and their difference is the [Quadratic Gauss sum](#quadratic-gauss-sum) $i\sqrt{11}$.

### Legendre symbol

↑ **Parent:** [Quadratic residue](#quadratic-residue)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Legendre_symbol)

For an odd prime $p$,

$$
\left(\frac ap\right)=
\begin{cases}
0,&p\mid a,\\
1,&a\not\equiv0\pmod p\text{ is a square},\\
-1,&a\text{ is a nonsquare}.
\end{cases}
$$

#### Multiplicativity of the Legendre symbol

↑ **Parent:** [Legendre symbol](#legendre-symbol)

For an odd prime $p$,

$$
\left(\frac{ab}{p}\right)=
\left(\frac ap\right)\left(\frac bp\right).
$$

In particular, if $p\nmid a$, then $(a^{-1}/p)=(a/p)$.

#### Complete Legendre-symbol sum

↑ **Parent:** [Legendre symbol](#legendre-symbol)

For every odd prime $p$,

$$
\sum_{x\in\mathbb F_p}\left(\frac xp\right)=0.
$$

Multiplication by a quadratic nonresidue permutes $\mathbb F_p$ and negates every term.

#### Quadratic Legendre-symbol correlation

↑ **Parent:** [Legendre symbol](#legendre-symbol)

For every odd prime $p$,

$$
\sum_{x\in\mathbb F_p}\left(\frac{x(x+1)}p\right)=-1.
$$

Equivalently, count the $p-1$ solutions of $t^2=y^2-1$ by factoring $(y-t)(y+t)=1$.

##### Number of consecutive nonzero quadratic residues modulo an odd prime

↑ **Parent:** [Quadratic Legendre-symbol correlation](#quadratic-legendre-symbol-correlation)

The number of $z\in\{1,\ldots,p-2\}$ for which both $z$ and $z+1$ are quadratic residues modulo $p$ is

$$
\frac{p-4-(-1)^{(p-1)/2}}4.
$$

<h4 id="euler-s-criterion">Euler's criterion</h4>

↑ **Parent:** [Legendre symbol](#legendre-symbol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler's_criterion)

For an odd prime $p$ and $p\nmid a$,

$$
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.
$$

##### Primes congruent to five modulo eight from odd squares plus four

↑ **Parent:** [Euler's criterion](#euler-s-criterion)

Every odd prime factor of an odd square plus four is one modulo four. The integer is five modulo eight, so at least one prime factor is five modulo eight. Choosing the odd square divisible by any proposed finite list excludes the list and proves infinitude.

<h4 id="gauss-s-lemma-number-theory">Gauss's lemma (number theory)</h4>

↑ **Parent:** [Legendre symbol](#legendre-symbol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gauss's_lemma_(number_theory))

For an odd prime $p$ and $p\nmid a$, let $m$ be the number of least positive residues among

$$
a,2a,\ldots,\frac{p-1}{2}a
$$

that exceed $p/2$. Then

$$
\left(\frac ap\right)=(-1)^m.
$$

#### Euler criterion

↑ **Parent:** [Legendre symbol](#legendre-symbol)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_criterion)

For an odd prime $p$,

$$
a^{(p-1)/2}\equiv\left(\frac ap\right)\pmod p.
$$

For $p\nmid a$, write $a=g^m$ using a [primitive root](#primitive-root-modulo-n) $g$; then the left side is $(-1)^m$, which is one exactly when $m$ is even and $a$ is a square.

##### First supplementary law for quadratic reciprocity

↑ **Parent:** [Euler criterion](#euler-criterion)

Euler's criterion at $a=-1$ gives

$$
\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2}.
$$

##### Second supplementary law for quadratic reciprocity

↑ **Parent:** [Euler criterion](#euler-criterion)

For every odd prime,

$$
\left(\frac2p\right)=(-1)^{(p^2-1)/8}.
$$

###### Euclid proof for infinitely many primes congruent to seven modulo eight

↑ **Parent:** [Second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity)

If $q_1,\ldots,q_r$ listed all primes congruent to seven modulo eight, then for $n=8q_1\cdots q_r$ the odd number $(n^2-2)/2$ is seven modulo eight. Every prime factor is one or seven modulo eight, at least one is seven, and none is among the $q_i$, a contradiction.

###### Elementary logarithmic lower bound for primes in the quadratic-residue classes of two

↑ **Parent:** [Second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity)

Let $\pi_k(x)$ count primes at most $x$ congruent to $k$ modulo eight. Bounding the prime-power divisibility of

$$
\prod_{\sqrt x/2\leq n\leq\sqrt x}(n^2-2)
$$

above and its size below gives, for all sufficiently large $x$,

$$
\pi_1(x)+\pi_7(x)+1\geq\frac{\log x}{6\log3}.
$$

##### Prime-power binomial congruence for a matrix

↑ **Parent:** [Euler criterion](#euler-criterion)

For an integer matrix $A$ and prime $p$, the commuting-matrix binomial theorem and divisibility of $\binom pj$ for $0<j<p$ give

$$
(I+A)^p\equiv I+A^p\pmod p.
$$

#### Weighted complete Legendre-symbol sum

↑ **Parent:** [Legendre symbol](#legendre-symbol)

For $T=\sum_{a=1}^{p-1}a(\frac ap)$, one has $T=0$ when $p\equiv1\pmod4$, and $T\equiv0\pmod p$ for every $p>3$.

#### Lower-half quadratic-residue sum for primes congruent to seven modulo eight

↑ **Parent:** [Legendre symbol](#legendre-symbol)

If $p\equiv7\pmod8$, the sum of the least positive quadratic residues below $p/2$ is

$$
\frac{p^2-1}{16}.
$$

The proof uses $(\frac2p)=1$ to compare the sum of all residues with its image under doubling.

#### Discriminant criterion for a quadratic congruence modulo an odd prime

↑ **Parent:** [Legendre symbol](#legendre-symbol)

For $p\nmid a$, the congruence $aX^2+bX+c=0\pmod p$ has a solution exactly when its discriminant $b^2-4ac$ is zero or a quadratic residue modulo $p$.

## Primitive-root lifting criterion

↑ **Parent:** [Number theory](number-theory.md)

If $g$ is primitive modulo an odd prime $p$ and $g^{p-1}\not\equiv1\pmod{p^2}$, then $g$ is primitive modulo every $p^k$.

## Jacobi symbol

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jacobi_symbol)

For odd $n=\prod p_i^{e_i}$, $(a/n)=\prod(a/p_i)^{e_i}$. A value $1$ need not mean that $a$ is a square modulo composite $n$.

### Jacobi reciprocity law

↑ **Parent:** [Jacobi symbol](#jacobi-symbol)

For coprime positive odd integers $a,b$, the [Jacobi symbol](#jacobi-symbol) satisfies $(a/b)(b/a)=(-1)^{(a-1)(b-1)/4}$. It follows by factoring $a$ and $b$ into primes and multiplying the [quadratic reciprocity](#quadratic-reciprocity) for each prime pair; the parity of the sums of prime half-differences agrees with $(a-1)/2$ and $(b-1)/2$. A [Jacobi symbol](#jacobi-symbol) equal to one does not imply that its numerator is a [quadratic residue](#quadratic-residue) for a composite denominator.

#### Infinitely many prime quadratic nonresidues of a nonsquare integer

↑ **Parent:** [Jacobi reciprocity law](#jacobi-reciprocity-law)

For an odd positive nonsquare integer $a$, there are infinitely many [primes](#prime-number) $p$ with [Legendre symbol](#legendre-symbol) $(a/p)=-1$. Choose a residue $n$ modulo $a$ with [Jacobi symbol](#jacobi-symbol) $(n/a)=-1$ by making it a [quadratic nonresidue](#quadratic-nonresidue) at one prime occurring to odd multiplicity and a square at every other prime. The [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) also imposes $n\equiv1\pmod4$ and $n\equiv1$ at any finite list of previously found primes. Then [Jacobi reciprocity](#jacobi-reciprocity-law) gives $(a/n)=-1$, so a prime factor of $n$ has $(a/p)=-1$ and is outside that list.

### Multiplicativity of the Jacobi symbol

↑ **Parent:** [Jacobi symbol](#jacobi-symbol)

For odd positive $n$, the [Jacobi symbol](#jacobi-symbol) is multiplicative in its numerator:

$$
\left(\frac{ab}{n}\right)=\left(\frac an\right)\left(\frac bn\right).
$$

It is also multiplicative in an odd denominator: $(a/mn)=(a/m)(a/n)$.

## Quadratic reciprocity

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Quadratic_reciprocity)

Quadratic reciprocity compares two questions: is the [prime number](#prime-number) $p$ a [quadratic residue](#quadratic-residue) modulo $q$, and is $q$ a [quadratic residue](#quadratic-residue) modulo $p$? Let $p,q$ be **distinct [odd primes](#odd-prime)**. In terms of the [Legendre symbol](#legendre-symbol),

$$
\left(\frac pq\right)\left(\frac qp\right)
=(-1)^{\frac{p-1}{2}\frac{q-1}{2}}.
$$

**The two [Legendre symbols](#legendre-symbol) have opposite signs exactly when both [primes](#prime-number) are $3$ modulo $4$; otherwise they are equal.** Their values are nonzero because the [primes](#prime-number) are distinct. Equal signs can mean two [quadratic residues](#quadratic-residue) or two [quadratic nonresidues](#quadratic-nonresidue): reciprocity compares the answers rather than declaring either answer positive.[T. M. Apostol, Chapter 27, §27.9, equation 27.9.3: distinct odd prime hypotheses and reciprocity law](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

For a direct computation, the nonzero [quadratic residues](#quadratic-residue) modulo $3,5,7$ are respectively $\{1\}$, $\{1,4\}$, and $\{1,2,4\}$. Squaring just $1,\ldots,(p-1)/2$ suffices because $x$ and $p-x$ have the same square modulo an [odd prime](#odd-prime) $p$.

$$
\begin{aligned}
\left(\frac37\right)&=-1,&\qquad \left(\frac73\right)&=\left(\frac13\right)=1,\\
\left(\frac57\right)&=-1,&\qquad \left(\frac75\right)&=\left(\frac25\right)=-1.
\end{aligned}
$$

The pair $3,7$ has a sign flip, whereas $5,7$ has two negative signs. These small [quadratic residue](#quadratic-residue) tables make the distinction tangible.

<a id="image-small-prime-square-residue-tables-distinguish-opposite-and-equal-legendre-symbol-signs"></a>
![](quadratic-reciprocity-small-prime-residues.png)

**[Figure 40](#image-small-prime-square-residue-tables-distinguish-opposite-and-equal-legendre-symbol-signs). Small prime square-residue tables distinguish opposite and equal Legendre symbol signs**. Each row uses half the nonzero inputs; the missing entries are unnecessary. The comparisons $3,7$ and $5,7$ are exact finite examples of [quadratic reciprocity](#quadratic-reciprocity), not evidence by themselves for every [prime](#prime-number) pair.

The [first supplementary law for quadratic reciprocity](#first-supplementary-law-for-quadratic-reciprocity) handles numerator $-1$, and the [second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity) handles numerator $2$:

$$
\left(\frac{-1}{p}\right)=(-1)^{(p-1)/2},\qquad
\left(\frac2p\right)=(-1)^{(p^2-1)/8}.
$$

For an [odd prime](#odd-prime) $p$, $-1$ is a [quadratic residue](#quadratic-residue) exactly when $p\equiv1\pmod4$, while $2$ is a [quadratic residue](#quadratic-residue) exactly when $p\equiv1,7\pmod8$. The remaining odd [congruence classes](#congruence-class) modulo $8$, namely $3,5$, make $2$ a [quadratic nonresidue](#quadratic-nonresidue). These laws fill the cases excluded from swapping distinct [odd primes](#odd-prime).[T. M. Apostol, Chapter 27, §27.9, equations 27.9.1–27.9.2: supplementary values](mathematics-bibliography.md#nist-digital-library-of-mathematical-functions)

### Computing Legendre symbols by quadratic reciprocity

↑ **Parent:** [Quadratic reciprocity](#quadratic-reciprocity)

The practical reward of [quadratic reciprocity](#quadratic-reciprocity) is a smaller modulus: swap a pair of distinct [odd primes](#odd-prime), record the required sign, then reduce the numerator by [modular arithmetic](#modular-arithmetic). Use [multiplicativity of the Legendre symbol](#multiplicativity-of-the-legendre-symbol) and the [second supplementary law for quadratic reciprocity](#second-supplementary-law-for-quadratic-reciprocity) to handle a factor of two. For example,

$$
\begin{aligned}
\left(\frac{11}{43}\right)
&=-\left(\frac{43}{11}\right)
=-\left(\frac{10}{11}\right)
=-\left(\frac2{11}\right)\left(\frac5{11}\right)\\
&=\left(\frac5{11}\right)
=\left(\frac{11}{5}\right)
=\left(\frac15\right)=1.
\end{aligned}
$$

Here $11,43$ are both $3$ modulo $4$, so the first swap changes sign; $11\equiv3\pmod8$ gives $(2/11)=-1$; the swap involving five has no sign change. An independent square check is $21^2=441\equiv11\pmod{43}$. The method determines existence of a [square root](algebra.md#square-root) without itself finding that root.

A composite numerator is allowed in a [Legendre symbol](#legendre-symbol); a composite denominator instead calls for a [Jacobi symbol](#jacobi-symbol). Its [Jacobi reciprocity law](#jacobi-reciprocity-law) supports repeated swaps and remainder reductions, in the spirit of the [Euclidean algorithm](#euclidean-algorithm).[Ben Lynn, Quadratic Reciprocity, “The Jacobi Symbol”: product definition and reciprocity for computing symbols without factoring](mathematics-bibliography.md#quadratic-reciprocity-by-ben-lynn)

A final [Jacobi symbol](#jacobi-symbol) of one is not a square-existence certificate for a [composite number](#composite-number) modulus. For example,

$$
\left(\frac2{15}\right)=\left(\frac23\right)\left(\frac25\right)=(-1)(-1)=1,
$$

yet $x^2\equiv2\pmod{15}$ is impossible: reducing it modulo three would require a square congruent to two, and squares modulo three are only zero or one. The product has hidden two local failures. By contrast, for a [prime](#prime-number) denominator, a [Legendre symbol](#legendre-symbol) of one does certify a [quadratic residue](#quadratic-residue).

### Lattice-point count for quadratic reciprocity

↑ **Parent:** [Quadratic reciprocity](#quadratic-reciprocity)

A short proof outline connects [Gauss's lemma](#gauss-s-lemma-number-theory) to counting points with [integer](#integer) coordinates. For distinct [odd primes](#odd-prime) $p,q$, define the two [floor function](calculus.md#floor-function) sums

$$
M=\sum_{i=1}^{(p-1)/2}\left\lfloor\frac{qi}{p}\right\rfloor,\qquad
N=\sum_{j=1}^{(q-1)/2}\left\lfloor\frac{pj}{q}\right\rfloor.
$$

The parity form of [Gauss's lemma](#gauss-s-lemma-number-theory) gives $(q/p)=(-1)^M$ and $(p/q)=(-1)^N$. In the open [rectangle](geometry-and-topology.md#rectangle) $0<x<p/2$, $0<y<q/2$, the [line](geometry-and-topology.md#straight-line) $y=qx/p$ separates $M$ points below it from $N$ points above it. None lies on the [line](geometry-and-topology.md#straight-line), because $py=qx$ and [coprimality](#coprime-integers) would force $p\mid x$. The total is therefore $(p-1)(q-1)/4$. Combining that count with the parity identities gives [quadratic reciprocity](#quadratic-reciprocity).[Ben Lynn, Quadratic Reciprocity, first theorem and proof of the Law of Quadratic Reciprocity: floor-sum parity and the separating-line count](mathematics-bibliography.md#quadratic-reciprocity-by-ben-lynn)

<a id="image-a-line-partitions-the-integer-coordinate-points-behind-the-quadratic-reciprocity-exponent"></a>
![](quadratic-reciprocity-lattice-parity-count.png)

**[Figure 41](#image-a-line-partitions-the-integer-coordinate-points-behind-the-quadratic-reciprocity-exponent). A line partitions the integer coordinate points behind the quadratic reciprocity exponent**. For $p=3,q=7$, the counts are $M=2,N=1$; for $p=5,q=7$, they are $M=N=3$. Dashed edges mark the excluded boundary of the [rectangle](geometry-and-topology.md#rectangle). This illustrates the counting step; the separate parity step from [Gauss's lemma](#gauss-s-lemma-number-theory) is essential to relate the count to [Legendre symbols](#legendre-symbol).

### Quadratic character of minus three

↑ **Parent:** [Quadratic reciprocity](#quadratic-reciprocity)

For an odd prime $p\ne3$, quadratic reciprocity gives

$$
\left(\frac{-3}{p}\right)=\left(\frac p3\right).
$$

Thus $-3$ is a square modulo $p$ exactly when $p\equiv1\pmod3$.

#### Cube roots of minus one modulo an odd prime

↑ **Parent:** [Quadratic character of minus three](#quadratic-character-of-minus-three)

The factorization

$$
X^3+1=(X+1)(X^2-X+1)
$$

shows that $X^3=-1$ always has $X=-1$ as a solution. For $p\ne3$, it has two further solutions exactly when $-3$ is a quadratic residue; for $p=3$, all three factors coalesce at the unique root $-1$.

## Carmichael number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carmichael_number)

A composite $N$ is Carmichael when $a^{N-1}\equiv1\pmod N$ for every $a$ coprime to $N$.

### Korselt criterion

↑ **Parent:** [Carmichael number](#carmichael-number)

A composite integer $N$ is Carmichael exactly when it is square-free and $p-1$ divides $N-1$ for every prime $p$ dividing $N$.

#### Proof of Korselt criterion

↑ **Parent:** [Korselt criterion](#korselt-criterion)

If every integer satisfies $a^n\equiv a\pmod n$, taking $a=p$ shows that $p^2$ cannot divide $n$. Taking a [primitive root](#primitive-root-modulo-n) modulo each prime divisor $p$ shows $p-1\mid n-1$. Conversely, these divisibilities and squarefreeness let [Fermat's little theorem](#fermat-little-theorem) prove the congruence modulo each prime divisor, and coprimality of those divisors combines it modulo $n$.

## Perfect power

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_power)

An integer is a perfect power when it has the form $x^k$ for integers $x$ and $k>1$.

## Smooth number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Smooth_number)

Given a bound $y$, a [positive integer](#positive-integer) is $y$-smooth when all of its [prime factors](#prime-factor) are at most $y$.

### Positive density of power-smooth integers

↑ **Parent:** [Smooth number](#smooth-number)

Fix $\eta=1/k$ with $k\geq2$. Choose $k$ primes in $[H^{\eta-\eta^2},H^\eta]$, repetitions allowed, and an integer cofactor $m$ so that $m p_1\cdots p_k\leq H$. The product is between $H^{1-\eta}$ and $H$, so $m\leq H^\eta$ and all resulting integers are $H^\eta$-smooth. The [Mertens theorem for reciprocal primes](analytic-number-theory.md#mertens-second-theorem) makes the reciprocal prime sum tend to $-\log(1-\eta)>0$. Since $\lfloor H/(p_1\cdots p_k)\rfloor\geq H/(2p_1\cdots p_k)$, there are $\gg_\eta H$ ordered representations. Each integer has only $O_\eta(1)$ prime factors in that interval, counted with multiplicity, so representation multiplicities are bounded by a constant depending on $k$. This proves the density bound. For arbitrary fixed positive $\eta$, choose a smaller reciprocal-integer exponent.

// Target: number-theory.bigb

### B-smooth integer

↑ **Parent:** [Smooth number](#smooth-number)

For a specified finite prime [factor base](#factor-base) $B$, a nonzero integer is $B$-smooth if every prime dividing its absolute value belongs to $B$. Negative residues are handled by including the sign $-1$ in their exponent vectors. This notation refers to a finite prime set, rather than the alternative convention in which a numerical smoothness bound is called $B$.

### S-smooth number

↑ **Parent:** [Smooth number](#smooth-number)

For a finite set $S$ of [primes](#prime-number), an [integer](#integer) is $S$-smooth when every prime dividing it belongs to $S$. Bounding the [largest prime factor](#largest-prime-factor) is equivalent to restricting the integer to be $S$-smooth for a suitable finite $S$.

#### Squarefree-part bound for smooth numbers

↑ **Parent:** [S-smooth number](#s-smooth-number)

If $S$ is a finite set of [prime numbers](#prime-number), every [S-smooth number](#s-smooth-number) has a unique expression $n=ab^2$, where $a$ is [squarefree](#squarefree-integer) and its [prime factors](#prime-factor) lie in $S$. There are at most $2^{|S|}$ choices for $a$ and at most $\lfloor\sqrt x\rfloor$ choices for $b$ when $n\le x$. Consequently $f_S(x)\le2^{|S|}\sqrt x$.

### Largest prime factor

↑ **Parent:** [Smooth number](#smooth-number)

The largest prime factor $P^+(n)$ of an [integer](#integer) $n>1$ is the greatest [prime number](#prime-number) dividing $n$.

## Diophantine equation

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diophantine_equation)

A Diophantine equation is a polynomial equation for which integer solutions are sought. Congruences, factorization, and size bounds often prove that no solution exists.

### Schinzel-Tijdeman exponent theorem

↑ **Parent:** [Diophantine equation](#diophantine-equation)

For a fixed [polynomial](polynomial.md) $f\in\mathbb Q[X]$ with at least two distinct complex roots, [integer](#integer) solutions with $m\ge2$ and $|y|>1$ have an effectively bounded exponent. Factorization over a [splitting field](galois-theory.md#splitting-field) and the fixed differences between distinct roots control common [ideal](commutative-algebra.md#ideal) [divisors](#divisor). Outside a fixed set of primes, each factor's valuation is divisible by $m/\gcd(m,e_i)$, where $e_i$ is its root [multiplicity](polynomial.md#multiplicity-mathematics). The generalized power-equation estimates from [linear forms in logarithms of algebraic numbers](#linear-form-in-logarithms-of-algebraic-numbers), including [unit](algebra.md#unit-in-a-ring) and exceptional-prime factors, give the exponent bound. A single-root [polynomial](polynomial.md) and the values $y=0,\pm1$ cannot be included: $4^m=(2^m)^2$, and $1^m=f(0)$ for $f(X)=X(X-1)+1$, give infinite exponent families.

### Local solubility

↑ **Parent:** [Diophantine equation](#diophantine-equation)

A [Diophantine equation](#diophantine-equation) is soluble at a place of a [number field](algebraic-number-theory.md#number-field) if it has a solution over the corresponding [completion of a valued field](arithmetic.md#completion-of-a-valued-field). It is locally soluble everywhere if this holds at all finite and infinite places. Over the [rational numbers](#rational-number), these are the real field and all [p-adic fields](arithmetic.md#p-adic-field). Local solubility is necessary for a [rational point](algebraic-geometry.md#rational-point), but the [local-to-global gap in isogeny descent](normalization-of-an-algebraic-curve.md#local-to-global-gap-in-isogeny-descent) shows it need not suffice.

### Fermat last theorem

↑ **Parent:** [Diophantine equation](#diophantine-equation)

There are no positive [integer](#integer) solutions to the displayed equation when the exponent is an [integer](#integer) greater than two. Homogeneity means that any hypothetical solution would give infinitely many common multiples; statements bounding solutions by arithmetic height must therefore first distinguish primitive solutions from their multiples.

### abc conjecture

↑ **Parent:** [Diophantine equation](#diophantine-equation)

For every $\epsilon>0$ there is a constant $K_\epsilon$ such that the displayed inequality holds for coprime positive integers $A+B=C$. The radical is the product of the distinct primes dividing the argument. Applying it to a primitive Fermat triple bounds the exponent and the triple simultaneously. For $ax^n-by^n=c\ne0$, division by the gcd, which divides $c$, gives a uniform bound on $\max(x,y)^{n-2(1+\epsilon)}$. Finiteness in the varying exponent requires excluding $x=y=1$ when $a-b=c$.

#### Catalan power bound from abc

↑ **Parent:** [abc conjecture](#abc-conjecture)

Put $M=x^p$ for positive bases $x,y\ge2$. The [coprime](#coprime-integers) triple $(y^q,1,x^p)$ has radical at most $xy<M^{2/3}$. The [abc conjecture](#abc-conjecture) with $\epsilon=1/6$ gives $M\le C_{1/6}M^{7/9}$, proving the bound. Both bases and both exponents are then bounded, since $2^p\le M$ and $2^q\le M-1$. Unlike a homogeneous Fermat equation, no common-scaling ambiguity occurs.

#### Primitive Fermat bound from abc

↑ **Parent:** [abc conjecture](#abc-conjecture)

For a primitive positive solution of $x^n+y^n=z^n$ with $n\ge4$, the three powers are pairwise [coprime](#coprime-integers) and their radical is at most $xyz<z^3$. The [abc conjecture](#abc-conjecture) with $\epsilon=1/6$ gives the displayed inequality, hence $z\le C_{1/6}^2$ uniformly in $n$. The inequality $z^n\le2\max(x,y)^n$ then bounds $n$. Thus there are finitely many primitive triples and exponents. Homogeneity would produce infinitely many unscaled solutions from any one nonzero solution, so a primitive [arithmetic height](algebraic-number-theory.md#height-function) bound alone must not be described as finite many arbitrary multiples.

### Thue theorem

↑ **Parent:** [Diophantine equation](#diophantine-equation)

An irreducible integral binary form of degree at least three has only finitely many integral solutions at a fixed nonzero value. Factor the form in a splitting field. Each linear factor generates an ideal dividing a fixed ideal, so it is one of finitely many chosen factors times a unit. The linear relation among any three distinct factors gives a [unit equation over a number field](#unit-equation-over-a-number-field), hence finitely many ratios and finitely many rational directions. Homogeneity and the fixed nonzero value then bound the scale on each direction. The same argument works for a binary form with at least three distinct projective roots, even without irreducibility.

### Unit equation over a number field

↑ **Parent:** [Diophantine equation](#diophantine-equation)

For fixed nonzero $\alpha,\beta$ in a [number field](algebraic-number-theory.md#number-field), this equation has finitely many unit solutions. By the [Dirichlet unit theorem](algebraic-number-theory.md#dirichlet-s-unit-theorem), a large unit-exponent vector makes one unit exponentially small at some archimedean embedding. The equation makes the other fixed multiple exponentially close to one. Its principal logarithm is a nonzero linear form in fixed algebraic logarithms, with coefficients bounded by the exponent size; a polynomial lower bound contradicts the exponential upper bound. Finite torsion and finitely many embeddings allow uniform constants.

### Infinite descent

↑ **Parent:** [Diophantine equation](#diophantine-equation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Infinite_descent)

An infinite descent rules out a nonempty set of positive integer solutions by constructing from any solution another with a strictly smaller positive integer measure. Choosing a solution of minimal measure gives a contradiction. Common measures are a hypotenuse, a denominator, or the size of a primitive solution.

#### Fourth-power sum cannot be a square

↑ **Parent:** [Infinite descent](#infinite-descent)

Choose a primitive counterexample with minimal $z$ and $y$ even. Its [Pythagorean triple](geometry-and-topology.md#pythagorean-triple) $(x^2,y^2,z)$ has $x^2=m^2-n^2$, $y^2=2mn$. Modulo four forces $m$ odd and $n$ even, so $m=u^2$ and $n=2v^2$. The primitive triangle $(x,2v^2,u^2)$ then has a parametrization with $v^2=rs$ and $u^2=r^2+s^2$. Coprimality makes $r=a^2,s=b^2$, giving $a^4+b^4=u^2$ with $u<z$. This contradicts [infinite descent](#infinite-descent).

## Diophantine approximation

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diophantine_approximation)

Diophantine approximation studies how closely numbers can be approximated by [rational](#rational-number) or [algebraic numbers](algebra.md#algebraic-number) subject to bounds on their arithmetic complexity.

### Transcendence theory

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

Transcendence theory proves that particular numbers are not [algebraic numbers](algebra.md#algebraic-number), or that several numbers satisfy no nonzero polynomial relation with algebraic coefficients. A recurring method constructs an auxiliary expression which is simultaneously too small analytically and too large arithmetically if the proposed values were algebraic.

#### Schneider-Lang theorem

↑ **Parent:** [Transcendence theory](#transcendence-theory)

Let $f_1,\ldots,f_s$ be meromorphic functions with $f_j'\in K[f_1,\ldots,f_s]$ for a fixed [number field](algebraic-number-theory.md#number-field) $K$. Suppose $f_1,f_2$ are algebraically independent over $\mathbb C$ and have finite orders $\rho_1,\rho_2$. The set $S$ of points where every $f_j$ is finite and belongs to $K$ satisfies the displayed bound. The orders are growth orders for meromorphic functions. For $f_1=z$, $f_2=e^z$, the orders are zero and one and the functions are algebraically independent; an algebraic value of $e^\alpha$ at nonzero algebraic $\alpha$ would produce infinitely many such points $n\alpha$.

#### Symmetric Hermite integral obstruction

↑ **Parent:** [Transcendence theory](#transcendence-theory)

Suppose nonzero [algebraic numbers](algebra.md#algebraic-number) $\beta_j$ form a Galois-stable set, with Galois-invariant [integer](#integer) weights $b_j$, and $k\ne0$ is an [integer](#integer). Choose $P\in\mathbb Z[X]$ vanishing at all $\beta_j$ with $P(0)\ne0$, and a positive [integer](#integer) $c$ making all $c\beta_j$ [algebraic integers](algebraic-number-theory.md#algebraic-integer). For a large prime $p$, put $D=(1+\deg P)p-1$ and $f_p(X)=c^DX^{p-1}P(X)^p/(p-1)!$, and let $F_p$ be the sum of its derivatives. The weighted sum $kF_p(0)+\sum b_jF_p(\beta_j)$ is an [integer](#integer), nonzero modulo $p$ when $p\nmid kcP(0)$. If the displayed exponential expression vanished, integrating $(e^{-z}F_p(z))'=-e^{-z}f_p(z)$ along the finitely many segments to $\beta_j$ would bound that nonzero [integer](#integer) by $C^p/(p-1)!\to0$. This contradiction proves the obstruction and supplies direct proofs for $e$ and $\pi$.

<h4 id="gelfond-schneider-theorem">Gelfond–Schneider theorem</h4>

↑ **Parent:** [Transcendence theory](#transcendence-theory)

For algebraic $a\ne0,1$ and algebraic irrational $b$, every value $\exp(b\lambda)$ with $e^\lambda=a$ is transcendental. Consequently any quotient of chosen nonzero logarithms of algebraic numbers is either rational or transcendental.

<h5 id="schneider-lattice-proof-of-the-gelfond-schneider-theorem">Schneider lattice proof of the Gelfond–Schneider theorem</h5>

↑ **Parent:** [Gelfond–Schneider theorem](#gelfond-schneider-theorem)

Assume $a$ and $a^b$ algebraic with algebraic irrational $b$. Apply [Siegel lemma](#siegel-s-lemma) to construct a small-coefficient polynomial $P$ vanishing at the algebraic pairs $(s+tb,a^s(a^b)^t)$ on a large square grid. The function $P(z,e^{\lambda z})$ is a nonzero exponential polynomial. Its many initial zeros make later grid values exponentially tiny, whereas an algebraic norm estimate forbids such tiny nonzero values. Iterating extends the zero grid indefinitely. Its quadratic zero count in disks contradicts the linear zero-count growth of an exponential polynomial.

#### Mahler method

↑ **Parent:** [Transcendence theory](#transcendence-theory)

Mahler's method uses functional equations relating a function at $z$ and at $z^l$ to transport an auxiliary polynomial to points rapidly approaching zero. High vanishing order gives an upper bound which conflicts with an algebraic norm or height lower bound under assumed algebraicity of the values. Functional transcendence ensures that the auxiliary expression is not identically zero.

##### Fredholm lacunary series

↑ **Parent:** [Mahler method](#mahler-method)

This lacunary series is analytic for $|z|<1$ and satisfies $f_l(z^l)=f_l(z)-z$. At roots of unity of $l$-power order, its radial tail diverges, giving a dense set of singularities on the unit circle and excluding algebraicity as a function. The [Mahler method](#mahler-method) proves transcendence of its values at every algebraic $z$ with $0<|z|<1$. At $z=1/2$, reduced truncations have denominators $2^{l^m}$ and error less than twice their $-l$th power; for $l\geq3$, the [Roth theorem](#roth-s-theorem) gives a shorter proof.

###### Roth criterion for rational Fredholm values

↑ **Parent:** [Fredholm lacunary series](#fredholm-lacunary-series)

For $0<p<q$, truncating the [Fredholm series](#fredholm-lacunary-series) at $n$ gives a rational with denominator at most $Q_n=q^{l^n}$ and positive error at most $2Q_n^{-l(1-\log p/\log q)}$ for large $n$. The displayed strict inequality first rules out a rational value by the rational separation bound, and then rules out an algebraic irrational value by [Roth theorem](#roth-s-theorem). Reduced denominators are at most $Q_n$ and tend to infinity because the truncations are distinct. In particular $l\ge3$ and $p<q^\delta$, $\delta<1/3$, imply transcendence.

###### Auxiliary-value height argument for the Fredholm series

↑ **Parent:** [Fredholm lacunary series](#fredholm-lacunary-series)

A nonzero [integer](#integer) [polynomial](polynomial.md) of bidegree at most $N$ can cancel the first $(N+1)^2-1$ Taylor coefficients of the [Fredholm series](#fredholm-lacunary-series). Functional transcendence makes the resulting [analytic function](complex-analysis.md#holomorphic-function) nonzero. If $\alpha$ and $f_l(\alpha)$ were both algebraic, the relation $f_l(\alpha^{l^r})=f_l(\alpha)-\sum_{j<r}\alpha^{l^j}$ would keep the auxiliary values in one fixed [number field](algebraic-number-theory.md#number-field). Their [Absolute logarithmic Weil height](algebraic-number-theory.md#absolute-logarithmic-weil-height) is at most $N l^r h(\alpha)(1+1/(l-1))+O_N(r+1)$, whereas their chosen absolute value is $O_N(|\alpha|^{T_Nl^r})$. The [Liouville height inequality](algebraic-number-theory.md#liouville-height-inequality) forces $T_N=O(N)$, contradicting its quadratic lower bound for sufficiently large $N$.

#### E-function

↑ **Parent:** [Transcendence theory](#transcendence-theory)

In the modern strict sense an E-function satisfies a nonzero linear differential equation over $\overline{\mathbb Q}(z)$, has algebraic coefficients $a_n$ with all conjugates bounded by $C^{n+1}$, and has common positive denominators $d_n\leq C^{n+1}$ making $d_na_0,\ldots,d_na_n$ algebraic integers. Siegel's original arithmetic growth condition permits, for each $\epsilon>0$, bounds of size $O_\epsilon(n^{\epsilon n})$ instead. The strict and original growth formulations should be distinguished rather than asserted equivalent. Exponentials with algebraic exponent satisfy the stronger conditions and a first-order differential equation.

##### Addition closure of Siegel E-functions

↑ **Parent:** [E-function](#e-function)

Work in the [compositum](algebra.md#field-compositum) of the two coefficient fields. Conjugate coefficient bounds add, while multiplying the common denominators clears both coefficient lists. For Siegel's original bounds $O_\epsilon(n^{\epsilon n})$, use $\epsilon/2$ in each denominator estimate. A nonzero [linear differential equation](differential-equation.md#linear-differential-equation) for the sum follows because its derivatives lie in the sum of the two finite-dimensional derivative spaces over the [rational function](isolated-singularity.md#rational-function) [field](algebra.md#field). The stricter exponential arithmetic bounds are preserved as well.

<h5 id="siegel-shidlovsky-theorem">Siegel–Shidlovsky theorem</h5>

↑ **Parent:** [E-function](#e-function)

Let a vector of [E-functions](#e-function) satisfy $f'=A(z)f$ with $A\in\operatorname{Mat}_s(\overline{\mathbb Q}(z))$. At a nonzero algebraic point $\xi$ which is not a pole of $A$, the transcendence degree of the values over $\overline{\mathbb Q}$ equals the transcendence degree of the functions over $\overline{\mathbb Q}(z)$. In particular algebraically independent functions give algebraically independent values. The exponential system $f_j=e^{\gamma_jz}$, for rationally independent algebraic $\gamma_j$, recovers the [Lindemann–Weierstrass theorem](#lindemann-weierstrass-theorem) by evaluating at one.

<h4 id="lindemann-weierstrass-theorem">Lindemann–Weierstrass theorem</h4>

↑ **Parent:** [Transcendence theory](#transcendence-theory)

For distinct [algebraic numbers](algebra.md#algebraic-number) $\alpha_1,\ldots,\alpha_s$, the numbers $e^{\alpha_1},\ldots,e^{\alpha_s}$ are linearly independent over $\overline{\mathbb Q}$. Equivalently, exponentials of numbers linearly independent over $\mathbb Q$ are algebraically independent over $\overline{\mathbb Q}$. The special case of a nonzero algebraic exponent gives a transcendental exponential. In particular $e^{i\pi}=-1$ forces $\pi$ to be transcendental.

##### Hermite auxiliary-polynomial proof for pi

↑ **Parent:** [Lindemann–Weierstrass theorem](#lindemann-weierstrass-theorem)

Under an assumed algebraicity of $i\pi$, form the product $\prod_j(1+e^{\alpha_j})$ over its conjugates; its one known vanishing factor makes the whole product zero and regroup the subset sums as $k+\sum b_je^{\beta_j}=0$, with nonzero exponents and Galois-invariant integral weights. After clearing their denominators, use $f_p(z)=(cz)^{p-1}\prod_j(cz-c\beta_j)^p/(p-1)!$. The sum of its derivatives at each $\beta_j$ is divisible by $p$ in the algebraic integers, whereas at zero its first nonzero derivative is a fixed nonzero residue for all but finitely many primes. Summing with the weights gives a nonzero rational integer. Integrating the derivative of $e^{-z}\sum f_p^{(j)}(z)$ expresses that integer as a quantity bounded by $C^p/(p-1)!$, which tends to zero. This is the contradiction.

### Badly approximable number

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

An irrational real number is badly approximable when $\|q\alpha\|\geq c/q$ for some $c>0$ and every positive integer $q$, where the double bars mean distance to the nearest integer. Equivalently every rational approximation obeys $|\alpha-a/q|\geq c/q^2$. The [Diophantine bound for the square root of two](#diophantine-bound-for-the-square-root-of-two) gives a concrete example and supplies separated rotations for [bilinear cancellation for badly approximable phases](analytic-number-theory.md#bilinear-cancellation-for-badly-approximable-phases).

#### Diophantine bound for the square root of two

↑ **Parent:** [Badly approximable number](#badly-approximable-number)

For the nearest integer $a$ to $q\sqrt2$, the nonzero integer $2q^2-a^2$ has absolute value at least one. Dividing by $q\sqrt2+a\leq4q$ proves the bound. Thus the points $0,\sqrt2,\ldots,W\sqrt2$ modulo one are separated by at least $1/(4W)$. Ordering their distances from zero gives $\sum_{h\leq W}\|h\sqrt2\|^{-1}\ll W\log(2W)$.

### Diophantine frequency vector

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

A vector $\omega\in\mathbb R^n$ satisfying $|k\cdot\omega|\ge\gamma |k|_1^{-\tau}$ for all nonzero integer vectors $k$, with $\gamma>0$. This excludes resonances and controls the [small divisors](#small-divisor) in analytic [cohomological equations on a Diophantine torus](fourier-series.md#cohomological-equation-on-a-diophantine-torus). Different choices of norm change the constant but not the nature of the condition.

#### Small divisor

↑ **Parent:** [Diophantine frequency vector](#diophantine-frequency-vector)

A denominator such as $k\cdot\omega$ which may become small for large integer vectors $k$. Inverting a directional derivative on a [torus](topology.md#torus) divides the nonzero [Fourier coefficients](fourier-series.md#fourier-coefficient) by $i k\cdot\omega$. A [Diophantine condition](#diophantine-frequency-vector) bounds this loss polynomially, so exponential Fourier decay still gives convergence on a smaller complex strip.

### Quantitative quadratic recurrence

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

For a universal constant $C>0$ and $0<\varepsilon\leq1$, every real $\alpha$ admits $1\leq n\leq\varepsilon^{-C}$ with [distance to the nearest integer](#distance-to-the-nearest-integer) of $\alpha n^2$ less than $\varepsilon$. A [Fejér kernel](fourier-series.md#fejer-kernel) detects failure of recurrence as a large [quadratic exponential sum](analytic-number-theory.md#quadratic-exponential-sum). The [Van der Corput inequality for finite scalar sequences](measure-theory.md#van-der-corput-inequality-for-finite-scalar-sequences) then produces a short linear near-return, whose suitable multiple gives the quadratic return. To include $\varepsilon>1$, use the bound $\max\{1,\varepsilon^{-C}\}$.

### Distance to the nearest integer

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

For a [real number](arithmetic.md#real-number) $x$, define $\|x\|_{\mathbb R/\mathbb Z}=\min_{k\in\mathbb Z}|x-k|$. It lies in $[0,1/2]$ and obeys $\|\ell x\|\leq|\ell|\|x\|$ for an [integer](#integer) $\ell$. It is a distance on the circle, rather than a [norm](functional-analysis.md#norm) on the real vector space.

#### Separated reciprocal-distance sum

↑ **Parent:** [Distance to the nearest integer](#distance-to-the-nearest-integer)

If finitely many points on $\mathbb R/\mathbb Z$ are pairwise separated by [distance modulo one](#distance-to-the-nearest-integer) at least $\delta>0$, then the displayed bound holds for $Q\ge2$. An arc of length $2r$ contains at most $1+2r/\delta$ points. First sum over $\|\theta_j\|\le Q^{-1}$, then over the dyadic annuli $2^j/Q<\|\theta_j\|\le2^{j+1}/Q$. Their contributions are $O(Q+\delta^{-1})$ and $O(Q2^{-j}+\delta^{-1})$, respectively. Summing proves the estimate. A point at zero contributes $Q$, using the convention $\min(Q,\infty)=Q$.

<h3 id="dirichlet-s-approximation-theorem">Dirichlet's approximation theorem</h3>

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dirichlet's_approximation_theorem)

For every [irrational number](algebra.md#irrational-number) $\alpha$ and [positive integer](#positive-integer) $N$, there are [integers](#integer) $p,q$ with $1\leq q\leq N$ such that

$$
\left|\alpha-\frac pq\right|\leq\frac1{qN}.
$$

The proof applies the [pigeonhole principle](combinatorics.md#pigeonhole-principle) to the $N+1$ [fractional parts](calculus.md#fractional-part) of $0,\alpha,\ldots,N\alpha$.

### Best rational approximation

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

A reduced fraction $p/q$ is a best rational approximation of the first kind to a [real number](arithmetic.md#real-number) $\alpha$ when no rational number with denominator at most $q$ is closer to $\alpha$.

### Schmidt subspace theorem

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Schmidt_subspace_theorem)

Let $L_1,\ldots,L_n$ be linearly independent [linear forms](linear-algebra.md#linear-functional) in $n$ variables with algebraic coefficients. For every $\varepsilon>0$, the nonzero $\mathbf x\in\mathbb Z^n$ satisfying

$$
\prod_{i=1}^n|L_i(\mathbf x)|
<\|\mathbf x\|^{-\varepsilon}
$$

lie in finitely many proper [linear subspaces](vector-space.md#vector-subspace) of $\mathbb Q^n$. There are variants involving a finite set of places of a [number field](algebraic-number-theory.md#number-field).

<h4 id="roth-s-theorem">Roth's theorem</h4>

↑ **Parent:** [Schmidt subspace theorem](#schmidt-subspace-theorem)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Roth's_theorem)

If $\alpha$ is a real algebraic irrational number and $\varepsilon>0$, then

$$
\left|\alpha-\frac pq\right|<q^{-2-\varepsilon}
$$

has only finitely many reduced rational solutions $p/q$.

#### Ridout theorem

↑ **Parent:** [Schmidt subspace theorem](#schmidt-subspace-theorem)

Let $\alpha$ be an algebraic irrational number, let $S$ be a finite set of [primes](#prime-number), and let $\varepsilon>0$. There are only finitely many reduced fractions $p/q$ whose denominator is [S-smooth number](#s-smooth-number) and which satisfy

$$
\left|\alpha-\frac pq\right|<q^{-1-\varepsilon}.
$$

This is the denominator-restricted consequence of the finite-place [Schmidt subspace theorem](#schmidt-subspace-theorem).

### Linear form in logarithms of algebraic numbers

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

[Baker's theorem](#baker-s-theorem) gives transcendence and quantitative nonvanishing results for such logarithmic forms.

A homogeneous linear form in logarithms of nonzero algebraic numbers has the form

$$
\Lambda=b_1\log\alpha_1+\cdots+b_n\log\alpha_n,
\qquad b_i\in\mathbb Z.
$$

<h4 id="baker-s-theorem">Baker's theorem</h4>

↑ **Parent:** [Linear form in logarithms of algebraic numbers](#linear-form-in-logarithms-of-algebraic-numbers)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Baker's_theorem)

If chosen logarithms of algebraic numbers are linearly independent over $\mathbb Q$, then they, together with one, are linearly independent over $\overline{\mathbb Q}$. More generally a nonzero homogeneous linear combination with algebraic coefficients is transcendental. Quantitative lower bounds for integer coefficients are a separate, effective aspect of logarithmic-form theory.

#### General lower bound for a linear form in logarithms

↑ **Parent:** [Linear form in logarithms of algebraic numbers](#linear-form-in-logarithms-of-algebraic-numbers)

Choose logarithms of nonzero algebraic numbers $\alpha_1,\ldots,\alpha_n$ and algebraic numbers $\beta_0,\ldots,\beta_n$, and put

$$
\Lambda=\beta_0+\sum_{j=1}^n\beta_j\log\alpha_j.
$$

Let $A_j$ bound $10$, the [naive polynomial height](algebraic-number-theory.md#naive-polynomial-height) of the minimal polynomial of $\alpha_j$, and $\exp(|\log\alpha_j|)$. Let $B$ bound all the corresponding heights of the $\beta_j$ and all $\log A_j$. There is an effective constant $C$, depending only on $n$ and the degree of the number field generated by the data, such that

$$
\Lambda\ne0
\quad\Longrightarrow\quad
|\Lambda|>\exp\!\left(-C\prod_{j=1}^n\log A_j\,\log B\right).
$$

#### Baker lower bound for a homogeneous linear form in logarithms

↑ **Parent:** [Linear form in logarithms of algebraic numbers](#linear-form-in-logarithms-of-algebraic-numbers)

This quantitative refinement belongs to the theory of [Baker's theorem](#baker-s-theorem); its dependence on the scaled coefficient bound is more specific than that broad theorem.

Choose logarithms of nonzero algebraic numbers $\alpha_1,\ldots,\alpha_n$, put

$$
\Lambda=\sum_{i=1}^n b_i\log\alpha_i,
\qquad b_i\in\mathbb Z,
$$

and choose $A_i\geq10$ large enough to bound the [naive polynomial height](algebraic-number-theory.md#naive-polynomial-height) of the minimal polynomial of $\alpha_i$ and $\exp(|\log\alpha_i|)$. After relabelling the terms if useful, set

$$
B^*=\max\left(\frac{|b_1|}{\log A_n},\ldots,
\frac{|b_{n-1}|}{\log A_n},|b_n|,10\right).
$$

There is an effectively computable constant $C$, depending only on $n$ and the degree of the number field generated by the $\alpha_i$, such that

$$
\Lambda\ne0
\quad\Longrightarrow\quad
|\Lambda|>\exp\!\left(-C(\log A_1)\cdots(\log A_n)\log B^*\right).
$$

The division by $\log A_n$ is the useful refinement over the [general lower bound for a linear form in logarithms](#general-lower-bound-for-a-linear-form-in-logarithms) when one algebraic number has a large height correlated with a coefficient.

##### Exponent bound for a binomial power equation

↑ **Parent:** [Baker lower bound for a homogeneous linear form in logarithms](#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms)

For fixed positive $a,b$ and fixed nonzero $c$, with $x\ne y$, put $Y=\max(x,y)$ and take $\Lambda=\log(a/b)+n\log(x/y)$, swapping the variables and coefficients if necessary. The equation gives $\log|\Lambda|\leq-n\log Y+O(1)$ when the larger-variable power is sufficiently large. A two-logarithm lower bound gives $\log|\Lambda|\geq-C(a,b)\log Y\log(2n)$. Hence $n\leq C\log(2n)+O(1)$, so $n$ is bounded. The cases $x=y$ and a bounded larger-variable power are elementary. For each remaining exponent, the [Thue theorem](#thue-theorem) for a binomial form supplies finitely many pairs. The constant-power exception $x=y=1$, $a-b=c$, must be removed.

##### Effective norm-form height estimate

↑ **Parent:** [Baker lower bound for a homogeneous linear form in logarithms](#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms)

Let $L$ be a fixed [number field](algebraic-number-theory.md#number-field) and let $V\subset L$ be a fixed rational linear subspace for which the associated [norm form](algebraic-number-theory.md#norm-form) has no unit-family degeneracy. There are effective constants $A,C>0$ such that every $z\in V\cap\mathcal O_L$ with nonzero [field norm](algebraic-number-theory.md#field-norm) $m$ satisfies

$$
H(z)\leq C|m|^A.
$$

To prove this, factor the principal ideal $(z)$, write its generators as a bounded factor times powers of fundamental units, use the linear relations defining $V$, and apply the [Baker lower bound for a homogeneous linear form in logarithms](#baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms) to bound the unit exponents by $O(\log|m|)$. For $L=\mathbb Q(\alpha)K$ with $[\mathbb Q(\alpha):\mathbb Q]=3$, $[K:\mathbb Q]=2$, and $V=\operatorname{span}_{\mathbb Q}\{1,\alpha,\omega\}$ for a basis $1,\omega$ of $K$, the coprime degrees rule out the degeneracy.

<h3 id="siegel-s-lemma">Siegel's lemma</h3>

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Siegel's_lemma)

Let $K$ be a [number field](algebraic-number-theory.md#number-field) of degree $D$, and let $L_1,\ldots,L_M$ be [linear forms](linear-algebra.md#linear-functional) in $N>DM$ variables with coefficients in $K$ and [projective height](algebraic-number-theory.md#projective-height) at most $\mathcal H\geq1$. There is a nonzero $\mathbf x\in\mathbb Z^N$ satisfying every $L_j(\mathbf x)=0$ and

$$
\lVert\mathbf x\rVert_\infty
\leq(N\mathcal H)^{DM/(N-DM)}.
$$

For $K=\mathbb Q$, this follows by applying the [pigeonhole principle](combinatorics.md#pigeonhole-principle) to the images of the integer box $\{0,\ldots,Y\}^N$ under $(L_1,\ldots,L_M)$. Expanding coefficients in a rational basis of $K$ gives the factor $D$ in the general count.

#### Pigeonhole proof of integer Siegel lemma

↑ **Parent:** [Siegel's lemma](#siegel-s-lemma)

For $M<N$ homogeneous equations with integer coefficients of absolute value at most $A\geq1$, map the box $\{0,\ldots,Q\}^N$ to its $M$ equation values. There are $(Q+1)^N$ inputs and at most $(2NAQ+1)^M$ outputs. Taking $Q=\lfloor(2NA)^{M/(N-M)}\rfloor$ makes the first count larger, since $2NAQ+1\leq2NA(Q+1)$. The difference of two inputs with the same output is the required nonzero bounded integer solution. Clearing denominators also treats rational equations; expanding a number-field basis replaces each field equation by finitely many rational equations.

#### Normalized derivative of a polynomial

↑ **Parent:** [Siegel's lemma](#siegel-s-lemma)

The $j$th normalized derivative is

$$
D_jP(X)=\frac1{j!}\frac{d^jP}{dX^j}(X).
$$

If $P(X)=\sum_ra_rX^r$ has integer coefficients, then $D_jP(X)=\sum_{r\geq j}\binom rj a_rX^{r-j}$ also has integer coefficients. For $\deg P\leq n$, its [naive polynomial height](algebraic-number-theory.md#naive-polynomial-height) is at most $2^nH(P)$.

#### Thue-Siegel auxiliary polynomial

↑ **Parent:** [Siegel's lemma](#siegel-s-lemma)

For an algebraic number $\alpha$ of degree $d$ and a small $\kappa>0$, [Siegel lemma](#siegel-s-lemma) constructs integer polynomials $P,Q$ of degree at most $n$ and exponentially bounded coefficients for which $P(X)+\alpha Q(X)$ has a zero at $X=\alpha$ of order close to $2n/d$. A [Wronskian](differential-equation.md#wronskian) then prevents every specialization $P(X)+yQ(X)$ from having a high-order zero at a rational point. This is the auxiliary-polynomial mechanism in the Thue-Siegel method.

##### Rational multiplicity bound for a linear auxiliary polynomial

↑ **Parent:** [Thue-Siegel auxiliary polynomial](#thue-siegel-auxiliary-polynomial)

Let $F(X,Y)=P(X)+YQ(X)$ with $P,Q\in\mathbb Z[X]$ linearly independent, $\deg_XF\leq n$, and $H(F)\leq C^n$. For every $\delta>0$, if a reduced rational $p/q$ has sufficiently large denominator in terms of $C$ and $\delta$, then $F(X,y)$ has multiplicity at most $\delta n+1$ at $p/q$, for every fixed real $y$.

Indeed, the nonzero [Wronskian](differential-equation.md#wronskian)

$$
W=PQ'-P'Q
$$

has degree below $2n$ and height at most $C_0^n$. A zero of multiplicity $r$ of $F(X,y)$ forces a zero of multiplicity at least $r-1$ of $W$. By [Gauss lemma for polynomials](commutative-algebra.md#gauss-lemma-for-polynomials), $(qX-p)^{r-1}$ then divides $W$ in $\mathbb Z[X]$, so $q^{r-1}$ divides the leading coefficient of $W$ and is at most $C_0^n$.

##### Thue-Siegel rational approximation bound

↑ **Parent:** [Thue-Siegel auxiliary polynomial](#thue-siegel-auxiliary-polynomial)

If a real algebraic number $\alpha$ has degree $d\geq3$, then for every $\varepsilon>0$ there are only finitely many reduced fractions $p/q$ such that

$$
\left|\alpha-\frac pq\right|<q^{-d/2-1-\varepsilon}.
$$

The [Thue-Siegel auxiliary polynomial](#thue-siegel-auxiliary-polynomial) proof chooses two such approximations, constructs an auxiliary polynomial nonzero at their pair, and compares its denominator lower bound with the upper bound supplied by its high-order zero at $(\alpha,\alpha)$.

### Pell equation

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Pell_equation)

For a nonsquare positive integer $D$, the Pell equation is

$$
x^2-Dy^2=1.
$$

Periodic [continued fractions](#continued-fraction) of $\sqrt D$ produce infinitely many integer solutions.

#### Unit reduction for quadratic norm equations

↑ **Parent:** [Pell equation](#pell-equation)

In a real quadratic integer ring, multiplying by a positive norm-one fundamental unit preserves a prescribed norm. Choose an exponent so that a positive representative lies in a half-open interval $[A,A\varepsilon)$. Its conjugate is the prescribed norm divided by the representative, so both integer coefficients are bounded on that interval. Enumerating these reduced representatives gives a complete finite list of unit orbits of solutions.

#### Generalized Pell equation

↑ **Parent:** [Pell equation](#pell-equation)

A generalized Pell equation is $x^2-dy^2=N$ for a fixed nonsquare positive integer $d$ and nonzero integer $N$. Multiplication by units of a real [quadratic number field](algebraic-number-theory.md#quadratic-field) preserves the norm up to sign, reducing solutions to finitely many unit orbits when an appropriate bounded reduction interval is used.

### Continued fraction

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continued_fraction)

A simple continued fraction recursively expands a real number by taking integer parts and reciprocals. Its convergents are exceptionally good rational approximations.

#### Continued fraction of the square root of nineteen

↑ **Parent:** [Continued fraction](#continued-fraction)

For a [quadratic irrational](algebra.md#quadratic-irrational-number) $\sqrt D$, write its [complete quotient](#complete-quotient) as $(\sqrt D+m_j)/d_j$. The recurrence $m_{j+1}=d_ja_j-m_j$, $d_{j+1}=(D-m_{j+1}^2)/d_j$, $a_{j+1}=\lfloor(\sqrt D+m_{j+1})/d_{j+1}\rfloor$ computes its [continued fraction](#continued-fraction). For $D=19$, the successive pairs after the initial quotient are $(4,3),(2,5),(3,2),(3,5),(2,3),(4,1)$, and then the cycle repeats. They give the displayed period of length six.

#### Negative continued fraction

↑ **Parent:** [Continued fraction](#continued-fraction)

The finite negative continued fraction is

$$
[a_1,\ldots,a_r]^-=a_1-\frac1{a_2-\frac1{\cdots-1/a_r}}.
$$

For $a_i\ge2$, it describes a negative-framed chain of unknots: the diagonal framings are $-a_i$ and adjacent linking numbers are one. Repeated [slam-dunk moves](knot-theory.md#slam-dunk-move) give rational surgery coefficient $-[a_1,\ldots,a_r]^-$. The corresponding chain matrix is negative definite. To check this, the successive determinants of its negative have recurrence $d_j=a_jd_{j-1}-d_{j-2}$, starting with $d_0=1$, $d_1=a_1$; they are positive and increasing, so Sylvester's criterion applies.

#### Simple continued fraction

↑ **Parent:** [Continued fraction](#continued-fraction)

A continued fraction $[a_0;a_1,a_2,\ldots]$ with integer $a_0$ and positive integer $a_j$ for $j\geq1$. Its partial numerators are all one. The [continued fraction convergents](#continued-fraction-convergent) have the standard two-term numerator and denominator recurrences.

#### Gauss continued-fraction map

↑ **Parent:** [Continued fraction](#continued-fraction)

The map $T(x)=1/x-\lfloor1/x\rfloor$ on $(0,1]$, with $T(0)=0$. Its digit $N(x)=\lfloor1/x\rfloor$ gives the successive partial quotients $N(T^j x)$ of a [continued fraction](#continued-fraction). This is distinct from the geometric [Gauss map](differential-geometry.md#gauss-map) assigning surface normals.

##### Natural extension of the continued-fraction Gauss map

↑ **Parent:** [Gauss continued-fraction map](#gauss-continued-fraction-map)

On each branch with digit $a=\lfloor1/x\rfloor$, the displayed extension of the [Gauss continued-fraction map](#gauss-continued-fraction-map) is invertible almost everywhere: $x=(a+x')^{-1}$ and $y=(y')^{-1}-a$, with $a=\lfloor1/y'\rfloor$. Its invariant joint [probability density function](continuous-probability-distribution.md#probability-density-function) is $[(\log2)(1+xy)^2]^{-1}$. The branch [Jacobian determinant](calculus.md#jacobian-determinant) is $[x^2(a+y)^2]^{-1}$, which cancels the transformation of $1+xy$. Integrating out $y$ gives the [Gauss measure](#gauss-measure) density.

##### Bounded distortion of continued-fraction cylinders

↑ **Parent:** [Gauss continued-fraction map](#gauss-continued-fraction-map)

The inverse branch of the $n$th iterate of the [Gauss continued-fraction map](#gauss-continued-fraction-map) on a fixed digit cylinder has the displayed form, with [continued fraction convergents](#continued-fraction-convergent) $p_j/q_j$. Its derivative has absolute value $(q_n+q_{n-1}y)^{-2}$. Since $q_{n-1}\leq q_n$, the maximum-to-minimum derivative ratio is at most four. The density of the [Gauss measure](#gauss-measure) changes this ratio by at most a further factor two. The cylinders shrink to irrational points, so this uniform distortion bound and the [Lebesgue density theorem](measure-theory.md#lebesgue-s-density-theorem) prove ergodicity of the map.

##### Gauss measure

↑ **Parent:** [Gauss continued-fraction map](#gauss-continued-fraction-map)

The [invariant measure](measure-theory.md#invariant-measure) for the [Gauss continued-fraction map](#gauss-continued-fraction-map) with density $1/[(\log2)(1+x)]$ on $[0,1]$. Inverse branches $x=1/(n+y)$ give transformed density $(\log2)^{-1}\sum_{n\geq1}[(n+y)^{-1}-(n+y+1)^{-1}]$, which telescopes to the same density.

#### Complete quotient

↑ **Parent:** [Continued fraction](#continued-fraction)

For a simple [continued fraction](#continued-fraction), the complete quotients satisfy $\theta_0=x$, $a_n=\lfloor\theta_n\rfloor$ and $\theta_{n+1}=1/(\theta_n-a_n)$ whenever the denominator is nonzero. Thus $\theta_n=[a_n;a_{n+1},\ldots]$.

#### Continued-fraction algorithm

↑ **Parent:** [Continued fraction](#continued-fraction)

Starting from $x_0=x>0$, define

$$
a_n=\lfloor x_n\rfloor,
\qquad
x_{n+1}=\frac1{x_n-a_n}
$$

whenever $x_n$ is not an integer. This produces $x=[a_0;a_1,a_2,\ldots]$.

##### Termination criterion for a simple continued fraction

↑ **Parent:** [Continued-fraction algorithm](#continued-fraction-algorithm)

A simple continued fraction terminates exactly when its value is rational. For a reduced rational $p/q$, each reciprocal step is one step of the Euclidean algorithm and replaces the denominator by a strictly smaller nonnegative remainder.

#### Continued fraction convergent

↑ **Parent:** [Continued fraction](#continued-fraction)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Continued_fraction_convergent)

Truncating a simple continued fraction gives a convergent; sufficiently accurate rational approximations with bounded denominator occur among these convergents.

##### Small norm residues from square-root continued fractions

↑ **Parent:** [Continued fraction convergent](#continued-fraction-convergent)

For nonsquare $N>1$, write the complete quotients after the initial term as $(\sqrt N+m)/d$. They exceed one, while their algebraic conjugates lie between minus one and zero. Thus $d<\sqrt N+m<2\sqrt N$. Comparing coefficients in $\sqrt N=(p_k\alpha_{k+1}+p_{k-1})/(q_k\alpha_{k+1}+q_{k-1})$ gives $p_k^2-Nq_k^2=d_{k+1}(p_kq_{k-1}-q_kp_{k-1})$, and the last determinant has absolute value one. These small residues are useful candidates for [smooth numbers](#smooth-number) in congruence-of-squares factorization.

##### Best approximation of the second kind

↑ **Parent:** [Continued fraction convergent](#continued-fraction-convergent)

A rational $p/q$ is a best approximation of the second kind to $\alpha$ when $|q\alpha-p|$ is no larger than $|b\alpha-a|$ for every competing rational $a/b$ with $0<b\leq q$. Every simple continued-fraction convergent has this property.

##### Continued-fraction matrix

↑ **Parent:** [Continued fraction convergent](#continued-fraction-convergent)

With $M(a)=\left(\begin{smallmatrix}a&1\\1&0\end{smallmatrix}\right)$,

$$
M(a_0)\cdots M(a_n)
=\begin{pmatrix}p_n&p_{n-1}\\q_n&q_{n-1}\end{pmatrix}.
$$

###### Continued-fraction tail formula

↑ **Parent:** [Continued-fraction matrix](#continued-fraction-matrix)

If $p_n/q_n=[a_0,\ldots,a_n]$, then appending a positive tail $x$ gives

$$
[a_0,\ldots,a_n,x]
=\frac{p_nx+p_{n-1}}{q_nx+q_{n-1}}.
$$

###### Reversal identity for a finite continued fraction

↑ **Parent:** [Continued-fraction matrix](#continued-fraction-matrix)

Because each matrix $M(a)=\left(\begin{smallmatrix}a&1\\1&0\end{smallmatrix}\right)$ is symmetric, reversing the partial quotients transposes their product. If the convergents of $[a_0,\ldots,a_n]$ are $p_j/q_j$, then the last two convergents of $[a_n,\ldots,a_0]$ are

$$
\frac{p_n}{p_{n-1}}
\quad\hbox{and}\quad
\frac{q_n}{q_{n-1}}.
$$

#### Positive generalized continued fraction

↑ **Parent:** [Continued fraction](#continued-fraction)

For positive $a_j,b_j$, define $p_0=a_0$, $p_{-1}=1$, $q_0=1$, $q_{-1}=0$ and

$$
p_j=a_jp_{j-1}+b_{j-1}p_{j-2},
\qquad
q_j=a_jq_{j-1}+b_{j-1}q_{j-2}.
$$

Then

$$
\begin{pmatrix}p_n&b_np_{n-1}\\q_n&b_nq_{n-1}\end{pmatrix}
=\prod_{j=0}^n
\begin{pmatrix}a_j&b_j\\1&0\end{pmatrix},
$$

and $p_n/q_n$ is the corresponding finite generalized continued fraction.

##### Convergence of a positive simple continued fraction

↑ **Parent:** [Positive generalized continued fraction](#positive-generalized-continued-fraction)

When $b_j=1$ and $a_j$ are positive integers, adjacent convergents satisfy

$$
p_nq_{n-1}-q_np_{n-1}=(-1)^{n+1}.
$$

Even and odd convergents are monotone from opposite sides, their separation is $1/(q_nq_{n+1})$, and $q_n\to\infty$. They therefore have a common limit $x$, with

$$
\left|\frac{p_n}{q_n}-x\right|
+\left|\frac{p_{n+1}}{q_{n+1}}-x\right|
=\frac1{q_nq_{n+1}}.
$$

###### All-one continued fraction and Fibonacci ratios

↑ **Parent:** [Convergence of a positive simple continued fraction](#convergence-of-a-positive-simple-continued-fraction)

If every $a_j=b_j=1$, then $p_n=F_{n+2}$ and $q_n=F_{n+1}$. Binet's formula

$$
F_n=\frac{\phi^n-\psi^n}{\sqrt5},
\qquad
\phi=\frac{1+\sqrt5}{2},
\quad
\psi=-\phi^{-1},
$$

shows that the convergents tend to $\phi$ and gives sharp scaled errors through $F_{n+1}-\phi F_n=\psi^n$.

#### Lagrange theorem on continued fractions

↑ **Parent:** [Continued fraction](#continued-fraction)

The Lagrange theorem says that a real number has an eventually periodic simple continued fraction exactly when it is a quadratic irrational.

#### Periodic continued fraction of a quadratic irrational

↑ **Parent:** [Continued fraction](#continued-fraction)

The simple continued fraction of a quadratic irrational is eventually periodic. For a nonsquare positive integer $D$, the continued fraction of $\sqrt D$ is periodic after its integer part.

##### Purely periodic continued fraction

↑ **Parent:** [Periodic continued fraction of a quadratic irrational](#periodic-continued-fraction-of-a-quadratic-irrational)

A continued fraction is purely periodic when its repeating block begins at its first partial quotient:

$$
[\overline{a_0,\ldots,a_n}]
=[a_0,\ldots,a_n,a_0,\ldots,a_n,\ldots].
$$

###### Reversed-period identity for a purely periodic continued fraction

↑ **Parent:** [Purely periodic continued fraction](#purely-periodic-continued-fraction)

Let $\theta=[\overline{a_0,\ldots,a_n}]$, and let $\theta'$ be its algebraic conjugate, the other fixed point of the Möbius transformation represented by $M(a_0)\cdots M(a_n)$. Then

$$
-\frac1{\theta'}=[\overline{a_n,\ldots,a_0}].
$$

The identity follows by transposing the continued-fraction matrix and substituting $X=-1/Y$ in its fixed-point equation.

##### Continued fraction of the square root of three

↑ **Parent:** [Periodic continued fraction of a quadratic irrational](#periodic-continued-fraction-of-a-quadratic-irrational)

Successive complete quotients repeat after two steps:

$$
\sqrt3=[1;\overline{1,2}].
$$

##### Continued fraction of the square root of eleven

↑ **Parent:** [Periodic continued fraction of a quadratic irrational](#periodic-continued-fraction-of-a-quadratic-irrational)

Rationalizing successive complete quotients gives

$$
\sqrt{11}=[3;\overline{3,6}].
$$

###### Alternating multiplier recurrence for convergents of the square root of eleven

↑ **Parent:** [Continued fraction of the square root of eleven](#continued-fraction-of-the-square-root-of-eleven)

If $p_n/q_n$ are the convergents of $\sqrt{11}$, then

$$
p_{n+1}+q_{n+1}\sqrt{11}
=\begin{cases}
(3+\sqrt{11})(p_n+q_n\sqrt{11}),&n\text{ odd},\\
\dfrac{3+\sqrt{11}}2(p_n+q_n\sqrt{11}),&n\text{ even}.
\end{cases}
$$

###### Pell-type norm from a periodic continued fraction

↑ **Parent:** [Continued fraction of the square root of eleven](#continued-fraction-of-the-square-root-of-eleven)

For the even convergents of $\sqrt{11}$,

$$
p_{2m}+q_{2m}\sqrt{11}
=(3+\sqrt{11})(10+3\sqrt{11})^m.
$$

Since the second factor has norm one, every such convergent satisfies $p_{2m}^2-11q_{2m}^2=-2$.

### Liouville approximation theorem

↑ **Parent:** [Diophantine approximation](#diophantine-approximation)

If an irrational algebraic number has degree $d$, then $|\alpha-p/q|>C(\alpha)q^{-d}$. Approximations of arbitrarily larger polynomial order therefore prove that a [Liouville number](algebra.md#liouville-number) is transcendental.

#### Unbounded continued-fraction coefficients exclude quadratic irrationality

↑ **Parent:** [Liouville approximation theorem](#liouville-approximation-theorem)

For an irrational $x$ with [continued fraction convergents](#continued-fraction-convergent) $p_n/q_n$, one has $|x-p_n/q_n|\leq1/(q_nq_{n+1})\leq1/(a_{n+1}q_n^2)$. The [Liouville approximation theorem](#liouville-approximation-theorem) for a [quadratic irrational](algebra.md#quadratic-irrational-number) gives a positive lower bound $C/q_n^2$ instead. Thus unbounded partial quotients preclude quadratic irrationality, and in particular imply $x^2$ is irrational.

#### Proof of Liouville approximation theorem

↑ **Parent:** [Liouville approximation theorem](#liouville-approximation-theorem)

For the degree-$d$ minimal polynomial $P\in\mathbb Z[X]$ of $\alpha$, the nonzero integer $q^dP(p/q)$ gives $|P(p/q)|\geq q^{-d}$. On a fixed neighbourhood of $\alpha$, the mean value theorem bounds

$$
|P(p/q)|\leq\max|P'|\,|p/q-\alpha|.
$$

Outside that neighbourhood the desired lower bound is immediate, giving $|\alpha-p/q|>c(\alpha)q^{-d}$ after decreasing the constant.

#### Separation of distinct reduced fractions

↑ **Parent:** [Liouville approximation theorem](#liouville-approximation-theorem)

For distinct reduced fractions $p/q$ and $u/v$,

$$
\left|\frac pq-\frac uv\right|
=\frac{|pv-qu|}{qv}\geq\frac1{qv}.
$$

If $q>v$, this is strictly greater than $q^{-2}$.

#### Transcendental subseries of a positive rational convergent series

↑ **Parent:** [Liouville approximation theorem](#liouville-approximation-theorem)

Every convergent series of positive rational terms has a subseries whose rational partial sums $p_j/q_j$ satisfy

$$
0<\alpha-\frac{p_j}{q_j}<2^{-j}q_j^{-j}.
$$

Choose each new term small enough to enforce all previous tail bounds. Separation of reduced fractions first makes $\alpha$ irrational, and the [Liouville approximation theorem](#liouville-approximation-theorem) then rules out every finite algebraic degree.

## Binary quadratic form

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_quadratic_form)

A binary quadratic form is $ax^2+bxy+cy^2$; integral changes of variables organize forms into equivalence classes.

### Primes represented by x squared plus three y squared

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

Necessity follows by reducing modulo three. For a [prime](#prime-number) $p\equiv1\pmod3$, [quadratic reciprocity](#quadratic-reciprocity) gives $(-3/p)=1$, so the [discriminant criterion for prime representation by a binary quadratic form](#discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form) constructs a primitive positive definite form of [discriminant of a binary quadratic form](#discriminant-of-a-binary-quadratic-form) $-12$ representing $p$. Reduction gives $|b|\leq a\leq c$ and $a\leq2$. The only primitive reduced form is $[1,0,3]$: the alternatives $[2,\pm2,2]$ are not primitive. Integral equivalence preserves represented integers, establishing sufficiency.

### Prime representation via an ideal class

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

Let $I$ be an [integral ideal](commutative-algebra.md#integral-ideal) of an imaginary quadratic [number field](algebraic-number-theory.md#number-field) and $(e_1,e_2)$ an [integral basis](algebraic-number-theory.md#integral-basis) of $I$. Its normalized norm is a positive definite [binary quadratic form](#binary-quadratic-form). An unramified rational prime $p$ is represented by this form exactly when there is an integral [prime ideal](commutative-algebra.md#prime-ideal) $P$ of norm $p$ with $[P]=[I]^{-1}$. Indeed, a representation gives an element $\alpha\in I$ with $N\alpha=pN(I)$, so $P=(\alpha)I^{-1}$ is integral of norm $p$. Conversely, $IP=(\alpha)$ with $\alpha\in I$ produces a representation by expressing $\alpha$ in the basis. [Artin reciprocity](algebraic-number-theory.md#artin-reciprocity-law) then detects this [ideal class](algebraic-number-theory.md#ideal-class) by Frobenius in the [Hilbert class field](algebraic-number-theory.md#hilbert-class-field).

### Discriminant criterion for prime representation by a binary quadratic form

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

For odd prime $p$ and an integral-form discriminant $d$, representation of $p$ by some form of discriminant $d$ is equivalent to solvability of $b^2\equiv d\pmod p$. A primitive representing vector can be completed to a unimodular change giving leading coefficient $p$. Conversely choose $b$ with the required parity and use $[p,b,(b^2-d)/(4p)]$.

### Proper equivalence of binary quadratic forms

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

Integral forms $f$ and $g$ are properly equivalent when

$$
g(x,y)=f(\alpha x+\beta y,\gamma x+\delta y)
$$

for some $\left(\begin{smallmatrix}\alpha&\beta\\\gamma&\delta\end{smallmatrix}\right)\in\operatorname{SL}_2(\mathbb Z)$. Proper equivalence preserves both represented integers and orientation.

### Primitive binary quadratic form

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

An integral binary quadratic form $[a,b,c]$ is primitive when $\gcd(a,b,c)=1$. This property is invariant under proper equivalence because a unimodular change and its integral inverse express either coefficient triple as integer combinations of the other.

### Discriminant of a binary quadratic form

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

The discriminant of $[a,b,c]$ is $D=b^2-4ac$. It is invariant under proper equivalence, and a real form with $a>0$ is positive definite exactly when $D<0$.

### Reduced positive definite binary quadratic form

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

A positive definite integral form $[a,b,c]$ is reduced when $|b|\leq a\leq c$, with $b\geq0$ if $|b|=a$ or $a=c$. Every proper equivalence class has a unique reduced representative under this boundary convention.

#### Reduction algorithm for a positive definite binary quadratic form

↑ **Parent:** [Reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form)

For a positive definite integral form $[a,b,c]$, a unimodular shear can replace $b$ by its representative $b'$ with $|b'|\leq a$. If the resulting $c'=(b'^2-D)/(4a)$ is smaller than $a$, swapping the variables replaces the leading coefficient by the smaller positive integer $c'$. Repeating terminates and produces $|b|\leq a\leq c$; determinant-one sign changes enforce the boundary convention. Thus every positive definite integral binary quadratic form is properly equivalent to a reduced form.

#### Enumeration of reduced binary quadratic forms

↑ **Parent:** [Reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form)

For a reduced form of negative discriminant $D$, the inequalities imply $3a^2\leq|D|$. One can therefore enumerate all classes by checking the finite set

$$
1\leq a\leq\sqrt{|D|/3},\qquad |b|\leq a,
$$

and retaining integral $c=(b^2-D)/(4a)$ with $a\leq c$ and the boundary sign convention.

##### Reduced positive definite binary quadratic forms of discriminant minus thirty-nine

↑ **Parent:** [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)

The [reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form) bounds $|b|\leq a\leq c$ and $b^2-4ac=-39$ imply $1\leq a\leq\sqrt{13}$. Enumerating $a=1,2,3$ and using the nonnegative boundary sign convention gives the four triples $(a,b,c)=(1,1,10),(2,1,5),(2,-1,5),(3,3,4)$. Thus the number of reduced forms is four.

##### Reduced forms of discriminant minus thirty-two

↑ **Parent:** [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)

The reduced-form bound $3a^2\le32$ leaves $a=1,2,3$. Checking $c=(b^2+32)/(4a)$ and the boundary sign convention gives precisely the displayed forms. The middle one is imprimitive and represents the prime two. Odd represented primes are $1$ or $3$ modulo eight by the [discriminant criterion for prime representation by a binary quadratic form](#discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form). The first form represents only $1$ modulo eight among odd integers, and the last only $3$, so a prime is represented by $3x^2+2xy+3y^2$ exactly when it is $3$ modulo eight.

##### Class number one for discriminant minus sixty-seven

↑ **Parent:** [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)

For negative discriminant $-67$, a [reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form) satisfies $1\le a\le\sqrt{67/3}<5$ and $b$ odd with $|b|\le a$. Checking $4a\mid b^2+67$ leaves only $(a,b,c)=(1,1,17)$ under the boundary convention. The [reduction algorithm for a positive definite binary quadratic form](#reduction-algorithm-for-a-positive-definite-binary-quadratic-form) therefore puts every form in this one [proper equivalence of binary quadratic forms](#proper-equivalence-of-binary-quadratic-forms) class. Its unimodular shears give infinitely many distinct forms $x^2+(2n+1)xy+(n^2+n+17)y^2$.

##### Reduced forms of discriminant minus forty-four

↑ **Parent:** [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)

The reduced positive definite triples are $(1,0,11)$, $(2,2,6)$ and $(3,\pm2,4)$. The imprimitive middle form represents only even numbers; the two last forms have identical value sets after reversing one variable.

##### Reduced positive definite binary quadratic forms of discriminant minus thirty-five

↑ **Parent:** [Enumeration of reduced binary quadratic forms](#enumeration-of-reduced-binary-quadratic-forms)

The two reduced positive definite integral forms of discriminant $-35$ are

$$
[1,1,9]\quad\hbox{and}\quad[3,1,3].
$$

For a prime $p>7$, the first represents $p$ exactly when

$$
\left(\frac p5\right)=\left(\frac p7\right)=1,
$$

and the second represents $p$ exactly when both [Legendre symbols](#legendre-symbol) are $-1$.

###### Primitive representation criterion at discriminant minus thirty-five

↑ **Parent:** [Reduced positive definite binary quadratic forms of discriminant minus thirty-five](#reduced-positive-definite-binary-quadratic-forms-of-discriminant-minus-thirty-five)

For odd $n$ prime to 35, proper representation by a positive definite [binary quadratic form](#binary-quadratic-form) of discriminant $-35$ is equivalent to $-35$ being a square modulo every prime divisor of $n$. A primitive representing vector extends to a determinant-one integer matrix, producing a form with leading coefficient $n$ and middle coefficient $b$ satisfying $b^2\equiv-35\pmod{4n}$. Conversely this congruence constructs such a form. Its local roots lift to prime powers and combine by the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem). Every class reduces to one of $x^2+xy+9y^2$ and $3x^2+xy+3y^2$. The condition is local at each prime divisor; a product [Jacobi symbol](#jacobi-symbol) equal to one alone is insufficient.

#### Class number problem

↑ **Parent:** [Reduced positive definite binary quadratic form](#reduced-positive-definite-binary-quadratic-form)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_number_problem)

The class number problem asks for number fields or discriminants having a prescribed class number.

##### Class number of a negative discriminant

↑ **Parent:** [Class number problem](#class-number-problem)

For a negative discriminant $D\equiv0$ or $1\pmod4$, the class number $h(D)$ is the number of proper equivalence classes of primitive positive definite integral binary quadratic forms of discriminant $D$. Equivalently, it is the number of reduced primitive forms of discriminant $D$.

###### Two distinguished classes of discriminant minus eight q

↑ **Parent:** [Class number of a negative discriminant](#class-number-of-a-negative-discriminant)

For an odd [prime number](#prime-number) $q$, the primitive positive definite forms

$$
[1,0,2q]
\qquad\hbox{and}\qquad
[2,0,q]
$$

have discriminant $-8q$ and lie in distinct proper equivalence classes. The first represents one, whereas the second has minimum positive value two.

###### Prime representation when h of minus eight q equals two

↑ **Parent:** [Two distinguished classes of discriminant minus eight q](#two-distinguished-classes-of-discriminant-minus-eight-q)

If $q\equiv3\pmod8$ is prime and $h(-8q)=2$, then for every prime $p>q$,

$$
p=x^2+2qy^2
$$

for some integers $x,y$ exactly when $p\equiv\pm1\pmod8$ and $p$ is a [quadratic residue](#quadratic-residue) modulo $q$.

###### Coprime-factorization lower bound for a quadratic-form class number

↑ **Parent:** [Class number of a negative discriminant](#class-number-of-a-negative-discriminant)

Let $d$ be odd and have $k$ distinct prime divisors. Assigning each complete prime-power factor of $d$ to one of two factors gives $2^k$ ordered coprime factorizations $d=ac$. Interchanging $a$ and $c$ identifies pairs, and each unordered factorization gives a different reduced primitive form $[\min(a,c),0,\max(a,c)]$ of discriminant $-4d$. Hence

$$
h(-4d)\geq2^{k-1}.
$$

### Unimodular reduction of a discriminant-minus-four form to two squares

↑ **Parent:** [Binary quadratic form](#binary-quadratic-form)

The identity

$$
5x^2+16xy+13y^2=(x+2y)^2+(2x+3y)^2
$$

comes from an integer change-of-variable matrix of determinant $-1$. It therefore preserves the set of integers represented and reduces the form to $u^2+v^2$.

<h2 id="euclid-s-lemma">Euclid's lemma</h2>

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclid's_lemma)

If a [prime number](#prime-number) $p$ divides a [product](arithmetic.md#product-of-numbers) $ab$ of [integers](#integer) $a,b$, then $p$ divides $a$ or $b$ (possibly both):

$$
p\mid ab\quad\Longrightarrow\quad p\mid a\text{ or }p\mid b.
$$

For example, $5\mid6\cdot10$ and $5\mid10$. The hypothesis that $p$ is a [prime number](#prime-number) matters: $6\mid2\cdot3$, although six divides neither factor. When $p$ does not divide $a$, the [greatest common divisor](#greatest-common-divisor) of $p$ and $a$ is one; multiply [Bézout's identity](algebra.md#bezout-s-identity) $up+va=1$ by $b$ to see that $p\mid b$. Repeated application makes this the uniqueness step in the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic). [Euclid, Elements, Book VII, Proposition 30](https://mathcs.clarku.edu/~djoyce/elements/bookVII/propVII30.html).

For a completely computed example, $7\mid20\cdot21$ because $20\cdot21=420=7\cdot60$, while $20=7\cdot2+6$ shows that seven does not divide twenty. [Bézout's identity](algebra.md#bezout-s-identity) $3\cdot7-20=1$ becomes, after [multiplication](arithmetic.md#multiplication) by $21$,

$$
21=3\cdot7\cdot21-20\cdot21=7\cdot63-7\cdot60=7\cdot3.
$$

The two terms on the right are divisible by seven, which explicitly recovers the forced [divisibility](#divisibility) of the second factor. Both alternatives can hold: $7\mid14\cdot21$, and seven divides both $14$ and $21$.

In fact the property characterizes [prime numbers](#prime-number) among the [integers](#integer) greater than one. If $c$ is a [composite number](#composite-number), choose $c=ab$ with $1<a,b<c$; then $c\mid ab$, but $c$ divides neither $a$ nor $b$. For several factors, repeated application of [Euclid's lemma](#euclid-s-lemma) says that a [prime number](#prime-number) dividing their [product](arithmetic.md#product-of-numbers) divides at least one factor. In a [product](arithmetic.md#product-of-numbers) of [prime numbers](#prime-number), that factor must equal it, because a [prime number](#prime-number) has no other [prime factor](#prime-factor). This is what prevents a different collection of [prime factors](#prime-factor) from representing the same [positive integer](#positive-integer) in the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic).

Book VII, Proposition 30 of [Euclid's Elements](geometry-and-topology.md#euclid-s-elements) states the result in terms of a [prime number](#prime-number) measuring a [product](arithmetic.md#product-of-numbers); its proof uses [coprimality](#coprime-integers) and [ratios](arithmetic.md#ratio). The calculation using [Bézout's identity](algebra.md#bezout-s-identity) above is a modern way to explain the same [divisibility](#divisibility) statement. [Euclid, Elements VII.30, translated text hosted by David Joyce](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII30.html)

## Prime valuation

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prime_valuation)

For a [prime number](#prime-number) $p$ and a [positive integer](#positive-integer) $n$, the prime valuation is the exponent of $p$ in the [prime factorization](#fundamental-theorem-of-arithmetic) of $n$, equivalently

$$
v_p(n)=\max\{e\in\mathbb Z_{\geq0}:p^e\mid n\}.
$$

Thus $v_2(360)=3$ because $8$ divides $360$ but $16$ does not; $v_3(360)=2$, $v_5(360)=1$ and $v_7(360)=0$. In particular $v_p(1)=0$. [Multiplication](arithmetic.md#multiplication) adds [prime valuations](#prime-valuation), $v_p(ab)=v_p(a)+v_p(b)$, and the [fundamental theorem of arithmetic](#fundamental-theorem-of-arithmetic) makes comparison of [prime valuations](#prime-valuation) an exact test for [divisibility](#divisibility) between [positive integers](#positive-integer). This definition extends to a nonzero [integer](#integer) by taking its [absolute value](real-analysis.md#absolute-value); for zero one commonly sets $v_p(0)=+\infty$.

## Euler totient function

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_totient_function)

[Euler's totient function](#euler-totient-function) is the [arithmetic function](#arithmetic-function)

$$
\varphi(n)=\#\{j\in\{1,\ldots,n\}:\gcd(j,n)=1\},\qquad n>0.
$$

It counts the [congruence classes](#congruence-class) modulo $n$ represented by [integers](#integer) [coprime](#coprime-integers) to $n$. In particular, $\varphi(1)=1$, since $\gcd(1,1)=1$. For $12$, the [coprime integers](#coprime-integers) among $1,\ldots,12$ are $1,5,7,11$, so $\varphi(12)=4$; they form a [reduced residue system](#reduced-residue-system). [Darij Grinberg, MIT 18.781 lecture notes, Definition 2.1.2](https://darijgrinberg.gitlab.io/floor.pdf)

Counting these [congruence classes](#congruence-class) is useful because they are exactly the classes with [modular multiplicative inverses](#modular-multiplicative-inverse). Their number supplies the exponent in [Euler theorem](#euler-theorem). [Möbius inversion](#mobius-inversion-formula) gives the product formula

$$
\varphi(n)=n\prod_{p\mid n}\left(1-\frac1p\right),
$$

where $p$ runs over distinct [prime factors](#prime-factor) of $n$. Thus $\varphi(p^a)=p^{a-1}(p-1)$ for [prime powers](#prime-power) with $a\geq1$, and $\varphi(12)=12(1-1/2)(1-1/3)=4$. The product for $n=1$ is an [empty product](arithmetic.md#empty-product), so it gives the same convention $\varphi(1)=1$.

### Totient divisor-sum identity

↑ **Parent:** [Euler totient function](#euler-totient-function)

The [divisor sum](#divisor-sum) of [Euler's totient function](#euler-totient-function) is the [identity arithmetic function](#identity-arithmetic-function):

$$
\sum_{d\mid n}\varphi(d)=n,\qquad n>0.
$$

Equivalently, $\varphi*\mathbf1=\operatorname{id}$ under [Dirichlet convolution](#dirichlet-convolution), with $\mathbf1$ the [constant-one arithmetic function](#constant-one-arithmetic-function). [Darij Grinberg, MIT 18.781 lecture notes, Propositions 2.4.4 and 2.4.5](https://darijgrinberg.gitlab.io/floor.pdf)

To see why, group the [integers](#integer) $j=1,\ldots,n$ by $h=\gcd(j,n)$. Each $h$ is a positive [integer divisor](#divisor) of $n$. Within its group, $j=ha$ with $1\leq a\leq n/h$ and $\gcd(a,n/h)=1$, by the [scaling identity for greatest common divisors](#scaling-identity-for-greatest-common-divisors). Dividing by $h$ gives a [bijection](function.md#bijection) with the [integers](#integer) counted by $\varphi(n/h)$. The groups form a [partition of a set](set.md#partition-of-a-set), so

$$
n=\sum_{h\mid n}\varphi(n/h)=\sum_{d\mid n}\varphi(d).
$$

For $n=12$, the groups with [greatest common divisor](#greatest-common-divisor) $h=1,2,3,4,6,12$ are respectively $\{1,5,7,11\},\{2,10\},\{3,9\},\{4,8\},\{6\},\{12\}$. Their sizes are $4,2,2,2,1,1$, totaling $12$. [Möbius inversion](#mobius-inversion-formula) reverses this [divisor sum](#divisor-sum) to recover [Euler's totient function](#euler-totient-function) from $g(n)=n$.

### Sum of reduced residues

↑ **Parent:** [Euler totient function](#euler-totient-function)

The map $j\mapsto n-j$ is a [bijection](function.md#bijection) of the [integers](#integer) between one and $n-1$ that are [coprime](#coprime-integers) to $n$. If their sum is $S$, this [bijection](function.md#bijection) gives $S=n\varphi(n)-S$, so $S=n\varphi(n)/2$. This works even at $n=2$, where the single residue is fixed. The same identity follows from the [weighted inclusion-exclusion principle](combinatorics.md#weighted-inclusion-exclusion-principle) by excluding multiples of the [prime factors](#prime-factor) of $n$.

### Integers whose totient divides them

↑ **Parent:** [Euler totient function](#euler-totient-function)

If $n>1$ is odd, its [Euler totient function](#euler-totient-function) is even and cannot divide $n$. Otherwise write $n=2^c\prod_{j=1}^r p_j^{a_j}$ with odd primes $p_j$ and $c\ge1$. Comparing powers of two in $\varphi(n)\mid n$ gives $\sum_j v_2(p_j-1)\le1$. Thus there is at most one odd prime $p$, with $v_2(p-1)=1$. Since $p-1$ divides $\varphi(n)$, it divides $n$, and is [coprime](#coprime-integers) to $p$; with only the prime factors $2,p$ available it must be a power of two. Hence $p-1=2$ and $p=3$. Conversely, for $c\ge1$ the prime-power totient formula verifies divisibility for $2^c3^d$, and $n=1$ is immediate.

### Totient divisibility along divisors

↑ **Parent:** [Euler totient function](#euler-totient-function)

Write $n=\prod p^{a_p}$ and $d=\prod p^{b_p}$, with $0\le b_p\le a_p$. The prime-power formula for the [Euler totient function](#euler-totient-function) gives an integer contribution to $\varphi(n)/\varphi(d)$ from each prime: it is $p^{a_p-b_p}$ when $b_p>0$, and $p^{a_p-1}(p-1)$ when $b_p=0<a_p$. Multiplying proves the [divisibility](#divisibility) assertion, including $d=1$ with $\varphi(1)=1$.

<h3 id="rosser-schoenfeld-totient-bound">Rosser–Schoenfeld totient bound</h3>

↑ **Parent:** [Euler totient function](#euler-totient-function)

For $n\ge3$, this explicit lower bound on the [Euler totient function](#euler-totient-function) implies $\varphi(n)/n=\Omega(1/\log\log n)$ as $n\to\infty$. Here $\gamma_E$ is the [Euler--Mascheroni constant](complex-analysis.md#euler-s-constant). The prime-product formula also gives $\varphi(r)/r\ge\varphi(N)/N$ whenever $r\mid N$, making the bound useful for certified [quantum period finding](quantum-theory.md#quantum-period-finding). The relevant statement is a lower bound: the claimed universal upper estimate $\varphi(n)=O(n/\log\log n)$ would fail at primes. Equations (3.41)–(3.42) of Theorem 15 provide the primary bound: [https://denisevellachemla.eu/Rosser-Schoenfeld-1962.pdf](https://denisevellachemla.eu/Rosser-Schoenfeld-1962.pdf) .

### Elementary totient-ratio lower bound

↑ **Parent:** [Euler totient function](#euler-totient-function)

List the $k$ distinct prime divisors of $r$ in increasing order. The $j$th is at least $j+1$, and $k\leq\log_2r$. The [Euler totient function](#euler-totient-function) product formula gives $\varphi(r)/r\geq\prod_{j=1}^k j/(j+1)=1/(k+1)$. This elementary bound is sufficient to show inverse-polynomial success probability for coprime phase labels in [quantum order finding](quantum-theory.md#quantum-order-finding).

### Euler theorem

↑ **Parent:** [Euler totient function](#euler-totient-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euler_theorem)

If a is coprime to n, then a raised to the power phi(n) is congruent to one modulo n.

Multiplication by a unit $a$ permutes the reduced residue classes modulo $n$. Multiplying all classes before and after this permutation and cancelling their unit product proves $a^{\phi(n)}\equiv1\pmod n$.

### Multiplicativity of the Euler totient function

↑ **Parent:** [Euler totient function](#euler-totient-function)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplicativity_of_the_Euler_totient_function)

For coprime positive integers m and n, the Chinese remainder theorem gives phi(mn)=phi(m)phi(n).

### Finite fibres of the Euler totient function

↑ **Parent:** [Euler totient function](#euler-totient-function)

For each positive integer $k$, only finitely many $n$ satisfy $\varphi(n)=k$. Indeed, every prime $p\mid n$ has $p-1\mid k$, and the exponent of $p$ in $n$ is bounded because $p^{a-1}\mid k$.

<h2 id="jordan-s-totient-function">Jordan's totient function</h2>

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Jordan's_totient_function)

The Jordan totient function counts ordered $k$-tuples modulo $n$ that together with $n$ have [greatest common divisor](#greatest-common-divisor) one. The [inclusion-exclusion principle](combinatorics.md#inclusion-exclusion-principle) gives

$$
J_k(n)=n^k\prod_{p\mid n}(1-p^{-k}).
$$

## Fermat little theorem

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat_little_theorem)

For a prime p, every integer a satisfies a^p congruent to a modulo p.

## Squarefree integer

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Squarefree_integer)

A squarefree integer is not divisible by the square of any prime.

## Square factor

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Square_factor)

An integer has a square factor when some prime square divides it.

## Difference of two squares

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Difference_of_two_squares)

The identity $r^2-s^2=(r-s)(r+s)$ converts a square difference into a factorization.

<h3 id="fermat-s-factorization-method">Fermat's factorization method</h3>

↑ **Parent:** [Difference of two squares](#difference-of-two-squares)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fermat's_factorization_method)

Fermat factorization tests successive $r\geq\lceil\sqrt N\rceil$ until $r^2-N=s^2$, then returns $N=(r-s)(r+s)$.

## Rational number

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rational_number)

A rational number is a quotient of two integers with nonzero denominator.

### Fraction

↑ **Parent:** [Rational number](#rational-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Fraction)

A fraction $a/b$ represents the quotient of its [numerator](#numerator) $a$ by its nonzero [denominator](#denominator) $b$. For [integers](#integer) $a,b$ this is a [rational number](#rational-number). Different fractions can represent the same number: $252/198=14/11$. Dividing both entries by their [greatest common divisor](#greatest-common-divisor) gives a [reduced fraction](#reduced-fraction), with the sign convention that the [denominator](#denominator) is positive.

#### Numerator

↑ **Parent:** [Fraction](#fraction)

The numerator is the upper entry $a$ in a [fraction](#fraction) $a/b$.

#### Denominator

↑ **Parent:** [Fraction](#fraction)

The denominator is the nonzero lower entry $b$ in a [fraction](#fraction) $a/b$.

### Farey sequence

↑ **Parent:** [Rational number](#rational-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Farey_sequence)

The increasing list of reduced [rational numbers](#rational-number) in $[0,1]$ with denominators at most its level $Q$, including zero and one.

#### Farey fraction

↑ **Parent:** [Farey sequence](#farey-sequence)

A member of a [Farey sequence](#farey-sequence). Two distinct level-$Q$ fractions have ordinary distance at least $Q^{-2}$. On the quotient circle identify zero and one before forming a set; the shorter wrapped distance of two remaining distinct fractions obeys the same bound.

### Reduced fraction

↑ **Parent:** [Rational number](#rational-number)

A reduced fraction $a/b$ has [coprime integers](#coprime-integers) $a,b$ and positive denominator $b$. Distinct reduced fractions with denominators at most $Q$ differ by at least $Q^{-2}$, since their difference has a nonzero [integer](#integer) numerator over a denominator at most $Q^2$.

### Density of the rational numbers

↑ **Parent:** [Rational number](#rational-number)

Between any two distinct real numbers lies a [rational number](#rational-number).

### Repeating decimal

↑ **Parent:** [Rational number](#rational-number)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Repeating_decimal)

A real number is rational exactly when its expansion in any integer base is eventually periodic.

#### Decimal preperiod

↑ **Parent:** [Repeating decimal](#repeating-decimal)

The shortest prefix before the repeating tail of a [decimal representation](#decimal-representation). For a [reduced fraction](#reduced-fraction) with [denominator](#denominator) $2^u5^v m$, where $m>1$ is [coprime](#coprime-integers) to ten, its length is $\max(u,v)$; the tail length is given by [decimal period from multiplicative order](#decimal-period-from-multiplicative-order).

### Eventually periodic positional expansion of a rational number

↑ **Parent:** [Rational number](#rational-number)

A positional expansion in an integer base represents a rational number exactly when its digit sequence is eventually periodic. Long division proves the forward implication because only finitely many remainders occur; summing a periodic tail as a [geometric series](real-analysis.md#geometric-series) proves the converse.

## Modular multiplicative inverse

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Modular_multiplicative_inverse)

For [integers](#integer) $a$ and $n>1$, a modular multiplicative inverse is a [congruence class](#congruence-class) $b$ satisfying $ab\equiv1\pmod n$. It exists exactly when $\gcd(a,n)=1$. Necessity follows because every common [divisor](#divisor) of $a,n$ would divide $ab-kn=1$. Conversely, [Bézout's identity](algebra.md#bezout-s-identity) gives $ua+vn=1$ for [coprime integers](#coprime-integers), making $u$ an inverse. This is the basic bridge from [greatest common divisor](#greatest-common-divisor) calculations to reversible [modular arithmetic](#modular-arithmetic).

For example, $5\cdot7-2\cdot17=1$, so $5^{-1}\equiv7\pmod{17}$. The [modular congruence](#modular-congruence) $5x\equiv3\pmod{17}$ therefore has the unique solution class $x\equiv21\equiv4\pmod{17}$. Multiplication by $5$ sends all seventeen residue classes to different classes; multiplying by $7$ reverses it. The inverse criterion and its algorithmic construction are presented in [Ankur Moitra, MIT 18.200, 2024, modular inverses and Euclid's algorithm](https://ocw.mit.edu/courses/18-200-principles-of-discrete-applied-mathematics-spring-2024/mit18_200_s24_lec15.pdf).

By contrast, $5$ has no [modular inverse](#modular-multiplicative-inverse) modulo $15$. Its products have only residues $0,5,10$. Consequently $5x\equiv3\pmod{15}$ has no solution, while $5x\equiv10\pmod{15}$ has five solution classes, $x\equiv2,5,8,11,14$. Dividing by a noninvertible residue would discard this distinction. In a [prime field](algebra.md#prime-field) $\mathbb F_p$, every nonzero residue is invertible; a general integer modulus instead gives a [quotient ring](commutative-algebra.md#quotient-ring) that can have [zero divisors](mathematics.md#zero-divisor).

<a id="image-multiplication-by-five-is-reversible-modulo-seventeen-but-collapses-classes-modulo-fifteen"></a>
![](modular-inverse-permutations.png)

**[Figure 42](#image-multiplication-by-five-is-reversible-modulo-seventeen-but-collapses-classes-modulo-fifteen). Multiplication by five is reversible modulo seventeen but collapses classes modulo fifteen**.

## Carmichael function

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Carmichael_function)

For an [integer](#integer) $n>1$, the [Carmichael function](#carmichael-function) $\lambda(n)$ is the [exponent of a finite group](group-theory.md#exponent-of-a-finite-group) for the [unit group](algebra.md#unit-group) $U(n)=(\mathbb Z/n\mathbb Z)^\times$: the least [positive integer](#positive-integer) $m$ for which

$$
a^m\equiv1\pmod n\qquad\text{for every }a\text{ with }\gcd(a,n)=1.
$$

Here the [greatest common divisor](#greatest-common-divisor) condition selects the [units](algebra.md#unit-in-a-ring). [Euler's totient function](#euler-totient-function) $\varphi(n)$ counts them; the [Carmichael function](#carmichael-function) gives their least common return exponent.[pp. 7–8, definition](mathematics-bibliography.md#notes-on-primitive-lambda-roots-by-peter-j-cameron-and-others)

Modulo eight, the [units](algebra.md#unit-in-a-ring) are $1,3,5,7$, and their squares are all congruent to one. Their [multiplicative orders](#multiplicative-order) are $1,2,2,2$, so $\lambda(8)=2$ although $\varphi(8)=4$. Modulo fifteen, the [units](algebra.md#unit-in-a-ring) $1,2,4,7,8,11,13,14$ have [multiplicative orders](#multiplicative-order) $1,4,2,4,4,2,4,2$. For example, the powers of two return through $1,2,4,8,1$. Thus $\lambda(15)=4$ although $\varphi(15)=8$; the [multiplicative order](#multiplicative-order) of four is only two.

<a id="image-individual-unit-orders-divide-the-least-common-return-exponent-modulo-eight-and-fifteen"></a>
![](carmichael-unit-orders-common-exponent.png)

**[Figure 43](#image-individual-unit-orders-divide-the-least-common-return-exponent-modulo-eight-and-fifteen). Individual unit orders divide the least common return exponent modulo eight and fifteen**.

The three quantities are related by

$$
\lambda(n)=\mathop{\operatorname{lcm}}_{\substack{1\leq a<n\\\gcd(a,n)=1}}\operatorname{ord}_n(a),\qquad
\operatorname{ord}_n(a)\mid\lambda(n)\mid\varphi(n).
$$

A common return exponent must be a multiple of every [multiplicative order](#multiplicative-order), hence of their [least common multiple](#least-common-multiple). Conversely, that [least common multiple](#least-common-multiple) makes every [unit](algebra.md#unit-in-a-ring) return to one. [Lagrange's theorem](group-theory.md#lagrange-s-theorem) makes each [multiplicative order](#multiplicative-order) divide the [group order](group.md#order-of-a-finite-group) $\varphi(n)$, proving the final [divisibility](#divisibility). The [Carmichael function](#carmichael-function) applies to all [units](algebra.md#unit-in-a-ring) at once, while the [multiplicative order](#multiplicative-order) concerns a chosen [unit](algebra.md#unit-in-a-ring).

For the [prime factorization](#fundamental-theorem-of-arithmetic) $n=\prod_{i=1}^r p_i^{e_i}$ with distinct [prime numbers](#prime-number) $p_i$ and $e_i\geq1$, the formulas are

$$
\lambda(n)=\operatorname{lcm}\bigl(\lambda(p_1^{e_1}),\ldots,\lambda(p_r^{e_r})\bigr),\qquad
\lambda(p^e)=p^{e-1}(p-1)\quad(p\text{ an odd prime}),
$$



$$
\lambda(2^e)=
\begin{cases}
1,&e=1,\\
2,&e=2,\\
2^{e-2},&e\geq3.
\end{cases}
$$

These are [least common multiples](#least-common-multiple), rather than products: $\lambda(15)=\operatorname{lcm}(2,4)=4$. The convention $\lambda(1)=1$ handles the trivial case separately.[p. 8, Proposition 5.1(a–c)](mathematics-bibliography.md#notes-on-primitive-lambda-roots-by-peter-j-cameron-and-others)

The [Chinese remainder theorem for unit groups](mathematics.md#chinese-remainder-theorem-for-unit-groups) explains the [least common multiple](#least-common-multiple): a power returns to one in every [prime power](#prime-power) component exactly when it is a multiple of each component's [exponent of a finite group](group-theory.md#exponent-of-a-finite-group). For an odd [prime power](#prime-power), the [unit group](algebra.md#unit-group) is a [cyclic group](group.md#cyclic-group) of [group order](group.md#order-of-a-finite-group) $p^{e-1}(p-1)$. For $e\geq3$, the [unit group](algebra.md#unit-group) modulo $2^e$ is a [direct product of groups](group-theory.md#direct-product-of-groups) $C_2\times C_{2^{e-2}}$, generated by the classes of $-1$ and five, so its [exponent of a finite group](group-theory.md#exponent-of-a-finite-group) is $2^{e-2}$.[Section 7.5, pp. 203–205, Theorem 7.28 and its proof](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

This gives a uniform reduction for [modular exponentiation](#modular-exponentiation): for a [unit](algebra.md#unit-in-a-ring) $a$ and a nonnegative [integer](#integer) $k$, reduce $k$ modulo $\lambda(n)$. For example, $2^{1001}\equiv2\pmod{15}$ because $1001\equiv1\pmod4$. The [unit](algebra.md#unit-in-a-ring) hypothesis matters: $3^2\equiv1\pmod8$, but $2^2\not\equiv1\pmod8$. Computing the formula assumes the [prime factorization](#fundamental-theorem-of-arithmetic) is available. The same common-exponent viewpoint explains [Carmichael numbers](#carmichael-number): a [composite number](#composite-number) $n$ passes the [Fermat primality test](computer-science.md#fermat-primality-test) for every [unit](algebra.md#unit-in-a-ring) base exactly when $\lambda(n)\mid n-1$. For example, $\lambda(561)=\operatorname{lcm}(2,10,16)=80\mid560$.

## Multiplicative order

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Multiplicative_order)

For [coprime integers](#coprime-integers) $a,n$ with $n>1$, the [multiplicative order](#multiplicative-order) is the least [positive integer](#positive-integer) $d$ such that

$$
d=\operatorname{ord}_n(a),\qquad a^d\equiv1\pmod n.
$$

It counts the distinct powers in the [cyclic subgroup](group.md#cyclic-subgroup) generated by the [congruence class](#congruence-class) of $a$. Thus it is an [order of a group element](group-theory.md#order-of-a-group-element) in the [unit group](algebra.md#unit-group) $(\mathbb Z/n\mathbb Z)^\times$.[pp. 153 and 156–157, Theorem 6.29](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

For example, the [modular exponentiation](#modular-exponentiation) $2^k\bmod7$, starting at $k=0$, produces $1,2,4,1,2,4,\ldots$. The first return to one takes three steps, so $\operatorname{ord}_7(2)=3$. Starting at the [congruence class](#congruence-class) three and repeatedly multiplying by two instead gives $3,6,5,3,\ldots$: these are the other three [units](algebra.md#unit-in-a-ring) modulo seven, outside the [cyclic subgroup](group.md#cyclic-subgroup) generated by two.

<a id="image-multiplication-by-two-modulo-seven-has-two-cycles-its-powers-follow-the-cycle-through-one"></a>
![](modular-power-orbits-modulo-seven.png)

**[Figure 44](#image-multiplication-by-two-modulo-seven-has-two-cycles-its-powers-follow-the-cycle-through-one). Multiplication by two modulo seven has two cycles; its powers follow the cycle through one**.

[Euler's theorem](#euler-s-theorem) guarantees a return to one at exponent $\varphi(n)$, where $\varphi$ is [Euler's totient function](#euler-totient-function). Thus the [multiplicative order](#multiplicative-order) exists for every [unit](algebra.md#unit-in-a-ring).[p. 1, Theorem 1.2; pp. 2–3, permutation of the units and cancellation](mathematics-bibliography.md#euler’s-theorem-by-keith-conrad) In fact,

$$
\operatorname{ord}_n(a)\mid\varphi(n).
$$

By [Lagrange's theorem](group-theory.md#lagrange-s-theorem), the size of the [cyclic subgroup](group.md#cyclic-subgroup) divides the size of the [unit group](algebra.md#unit-group), which is [Euler's totient function](#euler-totient-function). For two modulo seven, this is $3\mid6$; the [multiplicative order](#multiplicative-order) need not equal [Euler's totient function](#euler-totient-function). If $a\equiv1\pmod n$, its [multiplicative order](#multiplicative-order) is one.

The [coprime integers](#coprime-integers) hypothesis is necessary: if $a^d=1+kn$, any common [divisor](#divisor) of $a$ and $n$ divides one. For instance, powers of two modulo eight give $1,2,4,0,0,\ldots$, with no positive-exponent return to one. This [sequence](real-analysis.md#sequence) eventually settles, but two has no [multiplicative order](#multiplicative-order) modulo eight.

### Decimal period from multiplicative order

↑ **Parent:** [Multiplicative order](#multiplicative-order)

For a [reduced fraction](#reduced-fraction) $p/q$ with $0<p<q$, $q>1$, and $q,10$ [coprime integers](#coprime-integers), its [decimal representation](#decimal-representation) repeats immediately after the decimal point. The shortest repeating block has length

$$
L=\operatorname{ord}_q(10),\qquad L\mid\varphi(q).
$$

Here $\operatorname{ord}$ denotes [multiplicative order](#multiplicative-order), and $\varphi$ denotes [Euler's totient function](#euler-totient-function). Changing the [numerator](#numerator) preserves the [decimal period](#decimal-period-from-multiplicative-order) as long as the [fraction](#fraction) remains reduced.[pp. 7–8, Theorem 4.5 and Remark 4.9](mathematics-bibliography.md#orders-of-units-in-modular-arithmetic-by-keith-conrad)

For example, [long division](#long-division) of $1/7$ gives the [remainders](#remainder) $1,3,2,6,4,5,1$, with emitted digits $1,4,2,8,5,7$. Consequently

$$
\frac17=0.\overline{142857},\qquad \operatorname{ord}_7(10)=6.
$$

Each [remainder](#remainder) determines both the next digit and the next [remainder](#remainder); returning to one restarts the same six steps.

<a id="image-long-division-remainders-explain-the-six-digit-repeat-of-one-seventh-and-the-two-digit-prefix-of-one-twenty-eighth"></a>
![](long-division-remainder-cycles.png)

**[Figure 45](#image-long-division-remainders-explain-the-six-digit-repeat-of-one-seventh-and-the-two-digit-prefix-of-one-twenty-eighth). Long-division remainders explain the six-digit repeat of one seventh and the two-digit prefix of one twenty-eighth**.

More generally, initialize [long division](#long-division) with $r_0=p$. At each step, [division with remainder](#euclidean-division) gives

$$
10r_{j-1}=qd_j+r_j,\qquad 0\leq d_j\leq9,\qquad 0\leq r_j<q,
$$

so $r_j\equiv p10^j\pmod q$. Since $p,q$ are [coprime integers](#coprime-integers), the [modular inverse](#modular-multiplicative-inverse) of $p$ shows that $r_L=r_0$ exactly when $10^L\equiv1\pmod q$. To see why the digit block cannot repeat sooner than the [remainders](#remainder), a purely [repeating decimal](#repeating-decimal) with a block of $L$ digits represents $D/(10^L-1)$ for an [integer](#integer) $D$. A [reduced fraction](#reduced-fraction) $p/q$ with that value forces $q\mid10^L-1$. Hence the shortest digit repeat and the [multiplicative order](#multiplicative-order) coincide.

Knowing the [decimal period](#decimal-period-from-multiplicative-order) predicts how many digits must be computed and stored: one block determines the whole [repeating decimal](#repeating-decimal). It also constructs the block directly. With $L=\operatorname{ord}_q(10)$, the [integer](#integer)

$$
D=\frac{p(10^L-1)}q
$$

is the block, padded on the left with zeros to $L$ digits. For $1/11$, $L=2$ and $D=9$, so the block is $09$ and $1/11=0.\overline{09}$. Reduction matters: $7/21=1/3=0.\overline3$ has [decimal period](#decimal-period-from-multiplicative-order) one, whereas $\operatorname{ord}_{21}(10)=6$.

If the reduced [denominator](#denominator) contains [prime factors](#prime-factor) two or five, ten has no [multiplicative order](#multiplicative-order) modulo that whole [denominator](#denominator). Write

$$
q=2^u5^v m,\qquad \gcd(m,10)=1,\qquad k_0=\max(u,v).
$$

The [decimal preperiod](#decimal-preperiod) has exactly $k_0$ digits. If $m>1$, the remaining [repeating decimal](#repeating-decimal) has [decimal period](#decimal-period-from-multiplicative-order) $\operatorname{ord}_m(10)$. For instance, $28=2^2\cdot7$ gives $1/28=0.03\overline{571428}$: two prefix digits, then six repeating digits. If $m=1$, the [decimal representation](#decimal-representation) is a [terminating decimal](#terminating-decimal) with exactly $k_0$ fractional places. We use the representation ending in zeros, rather than its alternative ending in nines; for example $1/40=0.025$ terminates after three places.

A short derivation explains both cases. After $k$ digits, multiplying the [reduced fraction](#reduced-fraction) by $10^k$ and discarding its [integer](#integer) part leaves a [reduced fraction](#reduced-fraction) whose [denominator](#denominator) is $q/\gcd(q,10^k)$. This [denominator](#denominator) first becomes [coprime](#coprime-integers) to ten at $k=k_0$. It then equals $m$, giving an immediate repeat when $m>1$, or an [integer](#integer) when $m=1$. The same [long division](#long-division) argument works for [positional notation](#positional-notation) in any base $b\geq2$: for a reduced [denominator](#denominator) $q>1$ [coprime](#coprime-integers) to $b$, the shortest repeating block has length $\operatorname{ord}_q(b)$.

### Cyclic decimal divisibility

↑ **Parent:** [Multiplicative order](#multiplicative-order)

For an $L$-digit decimal integer $n$, moving its leading digit to the end gives a cyclic rotation $c_1(n)$ satisfying

$$
c_1(n)\equiv10n\pmod{10^L-1}.
$$

Thus, when a modulus $d$ divides $10^L-1$, every rotation has the same divisibility by $d$ as $n$, up to multiplication by a power of ten.

### Periodic modular exponentiation

↑ **Parent:** [Multiplicative order](#multiplicative-order)

For a unit $a$ modulo $N$, the function $x\mapsto a^x\bmod N$ is periodic on the integers.

#### Order as the exact period of modular exponentiation

↑ **Parent:** [Periodic modular exponentiation](#periodic-modular-exponentiation)

Let $a,n$ be [coprime integers](#coprime-integers) with $n>1$, and let $d=\operatorname{ord}_n(a)$ be their [multiplicative order](#multiplicative-order). For [integers](#integer) $x,y$,

$$
a^x\equiv a^y\pmod n\quad\Longleftrightarrow\quad d\mid(x-y).
$$

Negative exponents mean powers of the [modular inverse](#modular-multiplicative-inverse) of $a$. Thus [periodic modular exponentiation](#periodic-modular-exponentiation) has smallest positive [period](mathematics.md#period-of-a-function) $d$, and $1,a,\ldots,a^{d-1}$ are distinct [congruence classes](#congruence-class).[pp. 156–157, Theorem 6.29; multiplicative notation on p. 153](mathematics-bibliography.md#a-computational-introduction-to-number-theory-and-algebra-by-victor-shoup)

This lets a huge [modular exponentiation](#modular-exponentiation) reuse a short list: reduce its exponent modulo the [multiplicative order](#multiplicative-order), then look up the corresponding power. For example, $1000\equiv1\pmod3$ gives $2^{1000}\equiv2\pmod7$, while $1001\equiv2\pmod3$ gives $2^{1001}\equiv4\pmod7$. When the [multiplicative order](#multiplicative-order) is unknown, [Euler's theorem](#euler-s-theorem) permits reduction modulo [Euler's totient function](#euler-totient-function), though that [period](mathematics.md#period-of-a-function) may be longer. [Repeated squaring](#exponentiation-by-squaring) remains useful when computing either the unreduced or the reduced power.

For a proof outline, multiply $a^x\equiv a^y$ by the [modular inverse](#modular-multiplicative-inverse) of $a^y$, leaving $a^{x-y}\equiv1$. Apply [Euclidean division](#euclidean-division) to write $x-y=td+r$ with $0\leq r<d$. Then $a^{x-y}\equiv a^r$; minimality of the [multiplicative order](#multiplicative-order) forces $r=0$. The reverse implication follows from $a^d\equiv1$. The [coprime integers](#coprime-integers) hypothesis enables cancellation: modulo eight, $2^3\equiv2^4\equiv0$, but this repetition supplies no [multiplicative order](#multiplicative-order) for two.

### Order verification from divisors

↑ **Parent:** [Multiplicative order](#multiplicative-order)

To verify a candidate order $r$, check $a^r\equiv1$ and rule out $a^{r/q}\equiv1$ for every prime divisor $q$ of $r$.

## Euclidean algorithm

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Euclidean_algorithm)

For positive [integers](#integer) $a,b$, the Euclidean algorithm repeatedly performs [division with remainder](#euclidean-division): write $a=qb+r$ with $0\leq r<b$, then replace $(a,b)$ by $(b,r)$ until the second entry is zero. The final nonzero entry is their [greatest common divisor](#greatest-common-divisor). A remainder preserves the set of common [divisors](#divisor): an [integer](#integer) divides $a$ and $b$ exactly when it divides $b$ and $a-qb$. The positive remainders strictly decrease, so the calculation terminates.

The complete calculation for $252$ and $198$ is

$$
\begin{aligned}
252&=1\cdot198+54,\\
198&=3\cdot54+36,\\
54&=1\cdot36+18,\\
36&=2\cdot18+0.
\end{aligned}
$$

Hence **$\gcd(252,198)=18$**. The [fraction](#fraction) $252/198$ reduces to $14/11$ by dividing numerator and denominator by that common factor. The same remainder calculation has a geometric interpretation: remove squares from a $252$-by-$198$ [rectangle](geometry-and-topology.md#rectangle), then repeat on the remaining strip. Each division step records how many equal squares fit and the width of the new strip.

<a id="image-successive-square-removals-record-the-euclidean-algorithm-for-252-and-198"></a>
![](euclidean-algorithm-rectangles.png)

**[Figure 46](#image-successive-square-removals-record-the-euclidean-algorithm-for-252-and-198). Successive square removals record the Euclidean algorithm for 252 and 198**.

The procedure does more than test individual [divisors](#divisor). Each step replaces the whole common-divisor problem by a smaller equivalent one. Euclid's Book VII, Proposition 2 describes the corresponding repeated-subtraction construction; batching those subtractions into [division with remainder](#euclidean-division) gives the present formulation. [Euclid, Elements VII.2, greatest common measure](https://mathcs.clarku.edu/~djoyce/java/elements/bookVII/propVII2.html)

### Extended Euclidean algorithm

↑ **Parent:** [Euclidean algorithm](#euclidean-algorithm)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Extended_Euclidean_algorithm)

The extended Euclidean algorithm also computes [integers](#integer) $x,y$ satisfying $ax+by=\gcd(a,b)$, as in [Bézout's identity](algebra.md#bezout-s-identity). Back-substitution in the calculation under the [Euclidean algorithm](#euclidean-algorithm) gives

$$
18=54-36=54-(198-3\cdot54)=4(252-198)-198=4\cdot252-5\cdot198.
$$

Thus $(x,y)=(4,-5)$ solves $252x+198y=18$. The [linear Diophantine equation](#linear-diophantine-equation) $252x+198y=c$ is solvable exactly when $18$ divides $c$: necessity follows from common [divisibility](#divisibility), and multiplying this identity proves sufficiency. For [coprime integers](#coprime-integers) $a,b$, the coefficient of $a$ is a [modular inverse](#modular-multiplicative-inverse) of $a$ modulo $b$, and the coefficient of $b$ is a [modular inverse](#modular-multiplicative-inverse) of $b$ modulo $a$, when the respective modulus is greater than one.

### Linear Diophantine equation

↑ **Parent:** [Euclidean algorithm](#euclidean-algorithm)

A linear Diophantine equation in two variables has the form $ax+by=c$ with integer coefficients and seeks integer solutions.

#### All solutions of a linear Diophantine equation

↑ **Parent:** [Linear Diophantine equation](#linear-diophantine-equation)

If $a,b$ are nonzero [integers](#integer), $d=\gcd(a,b)$, and $(x_0,y_0)$ is one solution of the [linear Diophantine equation](#linear-diophantine-equation) $ax+by=c$, then all solutions are

$$
x=x_0+\frac bd\,t,\qquad y=y_0-\frac ad\,t,\qquad t\in\mathbb Z.
$$

Subtract two solutions and use the fact that $a/d$ and $b/d$ are [coprime integers](#coprime-integers). The [linear Diophantine equation solvability criterion](#linear-diophantine-equation-solvability-criterion) says that a particular solution exists exactly when $d$ divides $c$; the [extended Euclidean algorithm](#extended-euclidean-algorithm) constructs one. This parametrization separates existence from the complete family of answers.

#### Linear Diophantine equation solvability criterion

↑ **Parent:** [Linear Diophantine equation](#linear-diophantine-equation)

The equation $ax+by=c$ has an integer solution exactly when $\gcd(a,b)$ divides $c$. Bézout's identity proves sufficiency, while every integer linear combination of $a,b$ is divisible by their greatest common divisor.

## Sum of two squares theorem

↑ **Parent:** [Number theory](number-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sum_of_two_squares_theorem)

A positive integer is a sum of two integer squares exactly when every prime factor congruent to $3$ modulo $4$ has even exponent in its prime factorization.

### Congruence lattice proof of the prime sum of two squares

↑ **Parent:** [Sum of two squares theorem](#sum-of-two-squares-theorem)

If $u^2\equiv-1\pmod p$, this lattice has basis $(1,u),(0,p)$ and covolume $p$. The [Minkowski convex body theorem](algebraic-number-theory.md#minkowski-s-theorem) applied to a disk of squared radius strictly between $4p/\pi$ and $2p$ gives a nonzero lattice vector with $0<a^2+b^2<2p$. The congruence makes its squared length divisible by $p$, forcing $a^2+b^2=p$. The strict radius bounds avoid assuming the critical-volume form of Minkowski's theorem.

## Modular function

↑ **Parent:** [Number theory](number-theory.md)

[This section is present in another page, follow this link to view it.](modular-function.md)

## ↑ Ancestors (3)

1. [Area of mathematics](mathematics.md#area-of-mathematics)
2. [Mathematics](mathematics.md)
3. [Codex Wiki](README.md)

## ← Incoming links (4)

- [Big O notation](real-analysis.md#big-o-notation)
- [Fermat number](#fermat-number)
- [Integral domain](commutative-algebra.md#integral-domain)
- [Normal number](#normal-number)
