# Coding theory

↑ **Parent:** [Algebra](algebra.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coding_theory)

**Table of contents**

- [Code encoding](#code-encoding)
  - [Systematic encoding](#systematic-encoding)
    - [Systematic polynomial encoding of a cyclic code](#systematic-polynomial-encoding-of-a-cyclic-code)
- [Gilbert–Varshamov bound](#gilbert-varshamov-bound)
  - [Worst-case correction guarantee from the Gilbert–Varshamov bound](#worst-case-correction-guarantee-from-the-gilbert-varshamov-bound)
  - [Asymptotic Gilbert–Varshamov bound](#asymptotic-gilbert-varshamov-bound)
  - [Varshamov bound for linear codes](#varshamov-bound-for-linear-codes)
- [Codeword](#codeword)
  - [Codeword length](#codeword-length)
- [Cipher](#cipher)
  - [Plaintext](#plaintext)
  - [Ciphertext](#ciphertext)
- [Block code](#block-code)
  - [Binary block code](#binary-block-code)
    - [Error-correcting code](#error-correcting-code)
      - [Repetition code](#repetition-code)
    - [Hamming distance](#hamming-distance)
      - [Hamming space](#hamming-space)
      - [Diameter of a set family](#diameter-of-a-set-family)
      - [Normalized Hamming distance](#normalized-hamming-distance)
      - [Hamming cube](#hamming-cube)
        - [Exponential packing of a Hamming cube](#exponential-packing-of-a-hamming-cube)
      - [Hamming distance between unlabelled bipartitions](#hamming-distance-between-unlabelled-bipartitions)
        - [Sign rounding bound for a unit eigenvector](#sign-rounding-bound-for-a-unit-eigenvector)
      - [Minimum distance of a code](#minimum-distance-of-a-code)
        - [Relative minimum distance of a code](#relative-minimum-distance-of-a-code)
        - [Maximum code size at a given distance](#maximum-code-size-at-a-given-distance)
      - [Hamming ball](#hamming-ball)
        - [Hamming ball volume exponent](#hamming-ball-volume-exponent)
        - [Hoeffding lower-tail bound for Hamming balls](#hoeffding-lower-tail-bound-for-hamming-balls)
        - [Entropy bound for a Hamming ball](#entropy-bound-for-a-hamming-ball)
    - [Perfect code](#perfect-code)
      - [Binary Golay code](#binary-golay-code)
        - [Extended binary Golay code](#extended-binary-golay-code)
          - [Three-error syndrome decoding of extended Golay code](#three-error-syndrome-decoding-of-extended-golay-code)
          - [Systematic-matrix proof of extended Golay distance](#systematic-matrix-proof-of-extended-golay-distance)
        - [Golay generator polynomial](#golay-generator-polynomial)
        - [BCH and parity-extension proof of the binary Golay distance](#bch-and-parity-extension-proof-of-the-binary-golay-distance)
        - [Circular autocorrelation of the binary Golay generator](#circular-autocorrelation-of-the-binary-golay-generator)
    - [Singleton bound](#singleton-bound)
    - [Plotkin bound](#plotkin-bound)
    - [Puncturing (coding theory)](#puncturing-coding-theory)
      - [Punctured code](#punctured-code)
- [One-time pad](#one-time-pad)
  - [Two-time pad attack](#two-time-pad-attack)
  - [Perfect secrecy](#perfect-secrecy)
  - [Malleability of an additive one-time pad](#malleability-of-an-additive-one-time-pad)
- [Secret sharing](#secret-sharing)
  - [Threshold secret sharing](#threshold-secret-sharing)
    - [Shamir's secret sharing](#shamir-s-secret-sharing)
      - [Perfect secrecy of Shamir's threshold scheme](#perfect-secrecy-of-shamir-s-threshold-scheme)
- [Discrete memoryless channel](#discrete-memoryless-channel)
  - [Finite-alphabet erasure channel](#finite-alphabet-erasure-channel)
    - [Capacity of a finite-alphabet erasure channel](#capacity-of-a-finite-alphabet-erasure-channel)
  - [Binary erasure channel](#binary-erasure-channel)
  - [Z-channel](#z-channel)
- [Noisy-channel coding theorem](#noisy-channel-coding-theorem)
  - [Reliable transmission rate](#reliable-transmission-rate)
- [Linear-feedback shift register](#linear-feedback-shift-register)
  - [Output sets of different-length linear-feedback registers](#output-sets-of-different-length-linear-feedback-registers)
  - [Feedback polynomial](#feedback-polynomial)
  - [Feedback shift register](#feedback-shift-register)
  - [Berlekamp-Massey algorithm](#berlekamp-massey-algorithm)
    - [Minimum recurrence length after a new discrepancy](#minimum-recurrence-length-after-a-new-discrepancy)
    - [Minimal recurrence for the binary prefix 11001011](#minimal-recurrence-for-the-binary-prefix-11001011)
  - [Period bound for a linear-feedback shift register](#period-bound-for-a-linear-feedback-shift-register)
  - [Feedback-polynomial parity condition for maximal period](#feedback-polynomial-parity-condition-for-maximal-period)
  - [Zero-run lower bound for a linear-feedback shift register](#zero-run-lower-bound-for-a-linear-feedback-shift-register)
    - [Minimal linear-feedback shift register for the prefix 100000001](#minimal-linear-feedback-shift-register-for-the-prefix-100000001)
  - [Trace-generated maximal-period linear-feedback sequence](#trace-generated-maximal-period-linear-feedback-sequence)
- [Linear code](#linear-code)
  - [Monomial equivalence of linear codes](#monomial-equivalence-of-linear-codes)
  - [Maximum distance separable code](#maximum-distance-separable-code)
  - [Reed-Solomon error correction](#reed-solomon-error-correction)
    - [Primitive cyclic Reed-Solomon code](#primitive-cyclic-reed-solomon-code)
      - [Reed-Solomon key equation](#reed-solomon-key-equation)
      - [Duality of primitive cyclic Reed-Solomon codes](#duality-of-primitive-cyclic-reed-solomon-codes)
    - [Generalized Reed-Solomon code](#generalized-reed-solomon-code)
  - [Code rate](#code-rate)
    - [Asymptotic rate-distance function](#asymptotic-rate-distance-function)
  - [Binary linear code](#binary-linear-code)
    - [Total weight of a full-support binary linear code](#total-weight-of-a-full-support-binary-linear-code)
    - [Even-weight subcode of a binary linear code](#even-weight-subcode-of-a-binary-linear-code)
    - [Doubly even code](#doubly-even-code)
      - [Orthogonal generators of doubly even codes](#orthogonal-generators-of-doubly-even-codes)
    - [Self-orthogonal binary subspace](#self-orthogonal-binary-subspace)
      - [Odd-length binary self-orthogonal dual extension](#odd-length-binary-self-orthogonal-dual-extension)
    - [Single parity-check code](#single-parity-check-code)
  - [Tetracode](#tetracode)
  - [Weight enumerator](#weight-enumerator)
    - [MacWilliams identity](#macwilliams-identity)
  - [Parity bit](#parity-bit)
    - [Parity computation by CNOT gates](#parity-computation-by-cnot-gates)
    - [Even-weight binary code](#even-weight-binary-code)
  - [Binary repetition code](#binary-repetition-code)
  - [Zero code](#zero-code)
  - [Whole-space linear code](#whole-space-linear-code)
  - [Hamming weight](#hamming-weight)
  - [Minimum Hamming distance of a linear code](#minimum-hamming-distance-of-a-linear-code)
  - [Griesmer bound](#griesmer-bound)
  - [Generator matrix](#generator-matrix)
  - [Parity-check matrix](#parity-check-matrix)
    - [Root-evaluation parity-check matrix of a cyclic code](#root-evaluation-parity-check-matrix-of-a-cyclic-code)
    - [Parity-check dependencies determine minimum distance](#parity-check-dependencies-determine-minimum-distance)
    - [Polynomial multiplication parity-check matrix](#polynomial-multiplication-parity-check-matrix)
    - [Reciprocal-polynomial parity-check matrix](#reciprocal-polynomial-parity-check-matrix)
    - [Syndrome](#syndrome)
      - [Syndrome classification of code cosets](#syndrome-classification-of-code-cosets)
        - [Coset leader](#coset-leader)
  - [Parity-check extension of a linear code](#parity-check-extension-of-a-linear-code)
  - [Shortened code](#shortened-code)
  - [Dual code](#dual-code)
    - [Self-dual code](#self-dual-code)
      - [Binary self-dual code contains the all-ones word](#binary-self-dual-code-contains-the-all-ones-word)
  - [Reed-Muller code](#reed-muller-code)
    - [Bar product of binary linear codes](#bar-product-of-binary-linear-codes)
      - [Minimum distance of a bar product](#minimum-distance-of-a-bar-product)
      - [Parity-check matrix of a bar product](#parity-check-matrix-of-a-bar-product)
      - [Reed-Muller bar-product recursion](#reed-muller-bar-product-recursion)
    - [Dual of a Reed-Muller code](#dual-of-a-reed-muller-code)
  - [Hamming code](#hamming-code)
    - [Ternary Hamming code](#ternary-hamming-code)
      - [Ternary Hamming code as a cyclic code](#ternary-hamming-code-as-a-cyclic-code)
      - [Ternary Hamming code as a negacyclic code](#ternary-hamming-code-as-a-negacyclic-code)
    - [Hamming code as a cyclic code](#hamming-code-as-a-cyclic-code)
    - [Hamming code weight enumerator](#hamming-code-weight-enumerator)
      - [Low-weight coefficients of a binary Hamming code](#low-weight-coefficients-of-a-binary-hamming-code)
    - [Extended Hamming code](#extended-hamming-code)
    - [Hamming code of length seven](#hamming-code-of-length-seven)
    - [Binary simplex code](#binary-simplex-code)
      - [Constant weight of a binary simplex code](#constant-weight-of-a-binary-simplex-code)
    - [Perfectness of a Hamming code](#perfectness-of-a-hamming-code)
  - [Minimum-distance error-detection and correction guarantee](#minimum-distance-error-detection-and-correction-guarantee)
- [Cyclic code](#cyclic-code)
  - [Negacyclic code](#negacyclic-code)
  - [Zero of a cyclic code](#zero-of-a-cyclic-code)
  - [Repeated-root cyclic code](#repeated-root-cyclic-code)
    - [Repeated-root parity-check matrix](#repeated-root-parity-check-matrix)
    - [Binary cyclic codes of length a power of two](#binary-cyclic-codes-of-length-a-power-of-two)
  - [Check polynomial of a cyclic code](#check-polynomial-of-a-cyclic-code)
  - [Binary cyclic codes of length five](#binary-cyclic-codes-of-length-five)
  - [Generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code)
    - [Root-evaluation syndrome for a cyclic code](#root-evaluation-syndrome-for-a-cyclic-code)
      - [Single-error test from two binary BCH syndromes](#single-error-test-from-two-binary-bch-syndromes)
  - [Dual of a cyclic code](#dual-of-a-cyclic-code)
  - [Binary cyclic codes of length seven](#binary-cyclic-codes-of-length-seven)
  - [BCH code](#bch-code)
    - [Designed distance](#designed-distance)
    - [Binary cyclotomic coset modulo an odd integer](#binary-cyclotomic-coset-modulo-an-odd-integer)
    - [Error locator polynomial](#error-locator-polynomial)
      - [Chien search](#chien-search)
      - [Error evaluator polynomial](#error-evaluator-polynomial)
        - [Forney algorithm](#forney-algorithm)
    - [BCH bound](#bch-bound)
- [Parity extension](#parity-extension)
- [Hamming bound](#hamming-bound)
  - [Asymptotic Hamming bound](#asymptotic-hamming-bound)
- [Rabin cryptosystem](#rabin-cryptosystem)
  - [Repeated-message attack on the Rabin cryptosystem](#repeated-message-attack-on-the-rabin-cryptosystem)
  - [Factorization from distinct square roots modulo a semiprime](#factorization-from-distinct-square-roots-modulo-a-semiprime)
    - [Square-root oracle reduction for Rabin encryption](#square-root-oracle-reduction-for-rabin-encryption)
    - [Chosen-square attack on Rabin authentication](#chosen-square-attack-on-rabin-authentication)
- [Discrete logarithm problem](#discrete-logarithm-problem)
- [Diffie-Hellman key exchange](#diffie-hellman-key-exchange)
  - [Multilateral Diffie-Hellman key exchange](#multilateral-diffie-hellman-key-exchange)
- [Unique decodability](#unique-decodability)
  - [Decipherable code](#decipherable-code)
    - [Suffix code](#suffix-code)
    - [Optimal source code](#optimal-source-code)
    - [Prefix code](#prefix-code)
      - [Prefix code for a rare geometric success](#prefix-code-for-a-rare-geometric-success)
      - [Prefix tree of a code](#prefix-tree-of-a-code)
      - [Kraft–McMillan inequality](#kraft-mcmillan-inequality)
        - [McMillan inequality](#mcmillan-inequality)
        - [Equivalence of decipherable and prefix code lengths](#equivalence-of-decipherable-and-prefix-code-lengths)
        - [Total length lower bound for a decipherable binary code](#total-length-lower-bound-for-a-decipherable-binary-code)
      - [Shannon-Fano coding](#shannon-fano-coding)
      - [Shannon coding](#shannon-coding)
        - [Cumulative Shannon code](#cumulative-shannon-code)
          - [Competitive optimality of the Shannon code](#competitive-optimality-of-the-shannon-code)
      - [Entropy lower bound for prefix codes](#entropy-lower-bound-for-prefix-codes)
        - [Shannon's source coding theorem](#shannon-s-source-coding-theorem)
- [Binary symmetric channel](#binary-symmetric-channel)
  - [Undetected error](#undetected-error)
  - [Completely noisy binary symmetric channel](#completely-noisy-binary-symmetric-channel)
  - [Positive-rate coding bound below one-quarter crossover](#positive-rate-coding-bound-below-one-quarter-crossover)
- [Maximum a posteriori decoding](#maximum-a-posteriori-decoding)
- [Maximum-likelihood decoding](#maximum-likelihood-decoding)
- [Minimum-distance decoding](#minimum-distance-decoding)
  - [Bounded-distance decoding](#bounded-distance-decoding)

## Code encoding

↑ **Parent:** [Coding theory](coding-theory.md)

Code encoding maps messages injectively to [codewords](#codeword). For a dimension-$k$ [linear code](#linear-code) with [generator matrix](#generator-matrix) $G$, the standard encoder maps $m\in\mathbb F_q^k$ to $mG$. The redundancy makes error detection and recovery possible; for a [Reed-Solomon code](#reed-solomon-error-correction), encoding can instead evaluate a message [polynomial](polynomial.md) at the chosen field elements.

### Systematic encoding

↑ **Parent:** [Code encoding](#code-encoding)

A systematic encoder retains the message symbols unchanged in designated coordinates of its [codeword](#codeword) and calculates the remaining check symbols. For a [linear code](#linear-code), choosing an invertible set of $k$ columns of a [generator matrix](#generator-matrix) and changing its row [basis](vector-space.md#basis) gives this form.

#### Systematic polynomial encoding of a cyclic code

↑ **Parent:** [Systematic encoding](#systematic-encoding)

For a length-$n$, dimension-$k$ [cyclic code](#cyclic-code) with [generator polynomial](#generator-polynomial-of-a-cyclic-code) $g$ of degree $n-k$, let the message [polynomial](polynomial.md) satisfy $\deg M<k$. Subtracting the remainder upon [polynomial division](polynomial.md#polynomial-division) by $g$ makes the displayed word divisible by $g$. The remainder has degree less than $n-k$, so the highest $k$ coordinates retain the coefficients of $M$. This gives [systematic encoding](#systematic-encoding) without losing any message information.

<h2 id="gilbert-varshamov-bound">Gilbert–Varshamov bound</h2>

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Gilbert–Varshamov_bound)

For codes over an alphabet of size $q$, the greedy packing argument gives $A_q(n,d)\ge q^n/V_q(n,d-1)$, where $V_q(n,r)=\sum_{j=0}^r\binom nj(q-1)^j$. A maximal distance-$d$ code has radius-$(d-1)$ Hamming balls covering the entire space; counting their union proves the lower bound. The linear refinement is the [Varshamov bound for linear codes](#varshamov-bound-for-linear-codes).

// Target: algebra.bigb

<h3 id="worst-case-correction-guarantee-from-the-gilbert-varshamov-bound">Worst-case correction guarantee from the Gilbert–Varshamov bound</h3>

↑ **Parent:** [Gilbert–Varshamov bound](#gilbert-varshamov-bound)

A binary [code rate](#code-rate) $R$ is guaranteed with correction of every error pattern of [Hamming weight](#hamming-weight) at most $t=\lfloor pN\rfloor$ when $R\leq1-h_2(2p)$ and $p<1/4$. Choose [minimum Hamming distance](#minimum-distance-of-a-code) $2t+1$. The [Gilbert–Varshamov bound](#gilbert-varshamov-bound) and [entropy bound for a Hamming ball](#entropy-bound-for-a-hamming-ball) give at least $2^{N(1-h_2(2p))}$ codewords. To deduce vanishing error probability for a [binary symmetric channel](#binary-symmetric-channel) with crossover probability $p$, use strict inequality in the rate condition and a correction radius $(p+\varepsilon)N$; the [weak law of large numbers](convergence-of-random-variables.md#weak-law-of-large-numbers) then controls the tail. Correcting exactly the mean number of errors does not by itself ensure reliable transmission.

// Target: algebra.bigb

<h3 id="asymptotic-gilbert-varshamov-bound">Asymptotic Gilbert–Varshamov bound</h3>

↑ **Parent:** [Gilbert–Varshamov bound](#gilbert-varshamov-bound)

For $0\le\delta\le1-1/q$, take logarithms of the [Gilbert–Varshamov bound](#gilbert-varshamov-bound) and apply the [Hamming ball volume exponent](#hamming-ball-volume-exponent). The [Varshamov bound for linear codes](#varshamov-bound-for-linear-codes) gives the same achievable lower bound within linear codes for prime-power $q$.

// Target: algebra.bigb

### Varshamov bound for linear codes

↑ **Parent:** [Gilbert–Varshamov bound](#gilbert-varshamov-bound)

For a prime-power alphabet size $q$, a linear $[n,k,\ge d]$ code exists if $V_q(n-1,d-2)<q^{n-k}$. Choose parity-check columns successively, avoiding combinations of at most $d-2$ earlier columns. Fewer than $q^{n-k}$ vectors are forbidden, so such a choice is possible. No set of at most $d-1$ columns is dependent, and the resulting kernel has dimension at least $k$.

// Target: probability-and-statistics.bigb

## Codeword

↑ **Parent:** [Coding theory](coding-theory.md)

A [codeword](#codeword) is a member of the specified set of words used to encode messages. For a [linear code](#linear-code) specified by a [parity-check matrix](#parity-check-matrix) $H$, the [codewords](#codeword) are precisely the vectors satisfying $Hc=0$. The [minimum distance](#minimum-distance-of-a-code) between distinct codewords controls error correction.

### Codeword length

↑ **Parent:** [Codeword](#codeword)

The codeword length is the number of alphabet symbols in a [codeword](#codeword). For a binary word it counts bits; in a [prefix code](#prefix-code), it is the depth of the corresponding leaf in the code tree.

// Target: algebra.bigb

## Cipher

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cipher)

A cipher is a pair of keyed algorithms that maps a [plaintext](#plaintext) to a [ciphertext](#ciphertext) and recovers the plaintext from the ciphertext when supplied with the appropriate key.

### Plaintext

↑ **Parent:** [Cipher](#cipher)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plaintext)

Plaintext is the unencrypted message supplied to a [cipher](#cipher).

### Ciphertext

↑ **Parent:** [Cipher](#cipher)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Ciphertext)

Ciphertext is the encrypted message produced by a [cipher](#cipher).

## Block code

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Block_code)

A [block code](#block-code) assigns source messages to words of a fixed length over an [alphabet](information-theory.md#alphabet). Its codewords form a subset of that fixed-length word space; a [binary block code](#binary-block-code) uses the two-symbol [finite field](algebra.md#finite-field) $\mathbb F_2$.

### Binary block code

↑ **Parent:** [Block code](#block-code)

A binary $[n,m,d]$ code is a set of $m$ distinct words in $\mathbb F_2^n$ whose minimum pairwise [Hamming distance](#hamming-distance) is $d$. Here $n$ is the block length and $m$ is the number of codewords.

#### Error-correcting code

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error-correcting_code)

An error-correcting code is a set of codewords chosen with enough separation to detect or correct transmission errors.

##### Repetition code

↑ **Parent:** [Error-correcting code](#error-correcting-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Repetition_code)

A binary repetition code represents one bit by repeating it a fixed number of times. Majority decoding corrects fewer than half as many bit flips as the block length.

#### Hamming distance

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamming_distance)

The Hamming distance between two equal-length words is the number of coordinates in which they differ.

##### Hamming space

↑ **Parent:** [Hamming distance](#hamming-distance)

The Hamming space of length $n$ over a [finite field](algebra.md#finite-field) $\mathbb F_q$ is the set $\mathbb F_q^n$ equipped with [Hamming distance](#hamming-distance), the number of coordinates at which two words differ. The [Hamming weight](#hamming-weight) of a word is its distance from zero.

##### Diameter of a set family

↑ **Parent:** [Hamming distance](#hamming-distance)

This is the maximum Hamming distance between the characteristic vectors of members of a set family. In a down-set, one can replace a pair by disjoint subsets with the same union, so the maximum distance equals the largest size of a union of two members. A t-intersecting family has diameter at most $n-t$.

##### Normalized Hamming distance

↑ **Parent:** [Hamming distance](#hamming-distance)

On binary words of length $n$, [normalized Hamming distance](#normalized-hamming-distance) is the fraction of differing coordinates. Unlike unscaled [Hamming distance](#hamming-distance), it makes the [Hamming cubes](#hamming-cube) a [Lévy family](probability-theory.md#levy-family-of-graphs) under uniform [probability measures](probability-theory.md#probability-measure).

##### Hamming cube

↑ **Parent:** [Hamming distance](#hamming-distance)

The [Hamming cube](#hamming-cube) is $\{-1,1\}^n$, or equivalently $\{0,1\}^n$, equipped with [Hamming distance](#hamming-distance). Under its uniform [probability measure](probability-theory.md#probability-measure), the distance from a fixed vertex has the [binomial distribution](discrete-probability-distribution.md#binomial-distribution) with parameters $n,1/2$. This converts geometric ball sizes into probability tails.

###### Exponential packing of a Hamming cube

↑ **Parent:** [Hamming cube](#hamming-cube)

An [inclusion-maximal separated set](topological-analysis.md#inclusion-maximal-separated-set) of separation $an$ covers the [Hamming cube](#hamming-cube) by strict-radius $an$ balls. The [Hoeffding lower-tail bound for Hamming balls](#hoeffding-lower-tail-bound-for-hamming-balls) then gives at least $e^{2n(1/2-a)^2}$ selected vertices. At $a=1/8$ this yields $e^{9n/32}$ vertices, all separated by at least $n/8$.

##### Hamming distance between unlabelled bipartitions

↑ **Parent:** [Hamming distance](#hamming-distance)

This [Hamming distance](#hamming-distance) on partitions identifies a group with its complement because exchanging the two group names does not change the partition. Complementation is an [isometry](riemannian-geometry.md#isometry) of the ordinary [Hamming distance](#hamming-distance), so minimizing over this two-element group action gives a quotient metric and preserves the [triangle inequality](topological-analysis.md#triangle-inequality). Negating a zero-one indicator is not complementation; with $\pm1$ membership vectors, it is.

###### Sign rounding bound for a unit eigenvector

↑ **Parent:** [Hamming distance between unlabelled bipartitions](#hamming-distance-between-unlabelled-bipartitions)

Suppose $v_i=\pm1/\sqrt n$ encodes the true partition and $\widehat v$ is a unit estimated [eigenvector](linear-operator-theory.md#eigenvector). Every coordinate of the wrong sign contributes at least $1/n$ to $\min_{\sigma=\pm1}\|\widehat v-\sigma v\|_2^2=2(1-|\widehat v^\top v|)$. Since this is at most $2(1-|\widehat v^\top v|^2)$, which is the squared Frobenius distance between the rank-one [orthogonal projection matrices](linear-algebra.md#orthogonal-projection-matrix), the bound follows. Coordinates estimated as zero may be assigned consistently to either group.

##### Minimum distance of a code

↑ **Parent:** [Hamming distance](#hamming-distance)

The minimum distance of a code $C$ is the least [Hamming distance](#hamming-distance) between distinct codewords. For a [linear code](#linear-code), translation invariance makes this equal to the least [Hamming weight](#hamming-weight) of a nonzero codeword.

###### Relative minimum distance of a code

↑ **Parent:** [Minimum distance of a code](#minimum-distance-of-a-code)

The relative minimum distance of a length-$n$ code of minimum distance $d$ is $d/n$. It expresses the guaranteed separation as a fraction of the block length.

// Target: algebra.bigb

###### Maximum code size at a given distance

↑ **Parent:** [Minimum distance of a code](#minimum-distance-of-a-code)

The quantity $A_q(n,d)$ is the largest cardinality of a length-$n$ code over an alphabet of size $q$ with minimum Hamming distance at least $d$. The code need not be linear.

// Target: algebra.bigb

##### Hamming ball

↑ **Parent:** [Hamming distance](#hamming-distance)

The Hamming ball of radius $r$ about a word $x$ is the set of words whose [Hamming distance](#hamming-distance) from $x$ is at most $r$.

###### Hamming ball volume exponent

↑ **Parent:** [Hamming ball](#hamming-ball)

For $0\le\rho\le1-1/q$, the exponential growth rate of a q-ary Hamming ball is $H_q(\rho)$. [Stirling's formula](real-analysis.md#stirling-formula) gives the exponent of each summand $\binom ni(q-1)^i$, and the sum lies between its largest term and $n+1$ times that term. Above the entropy-maximizing radius fraction, the exponent is one.

// Target: algebra.bigb

###### Hoeffding lower-tail bound for Hamming balls

↑ **Parent:** [Hamming ball](#hamming-ball)

For a uniform vertex of the [Hamming cube](#hamming-cube), distance from a fixed vertex is the sum of $n$ [independent](random-variable.md#independent-random-variables) [Bernoulli random variables](discrete-probability-distribution.md#bernoulli-distribution) with parameter $1/2$. The lower-tail [Hoeffding inequality](probability-inequality.md#hoeffding-inequality) implies that the fraction of vertices at distance at most $an$, $0<a<1/2$, is at most $e^{-2n(1/2-a)^2}$. Strict-radius balls satisfy the same upper bound.

###### Entropy bound for a Hamming ball

↑ **Parent:** [Hamming ball](#hamming-ball)

For $0<\rho\leq1/2$, the number of binary words within [Hamming distance](#hamming-distance) $\rho n$ of a fixed word is at most $e^{nh(\rho)}$, with the [binary entropy function](combinatorics.md#binary-entropy-function) in natural logarithms. In $1=\sum_j\binom nj\rho^j(1-\rho)^{n-j}$, each summand weight for $j\leq\rho n$ is at least $\rho^{\rho n}(1-\rho)^{n(1-\rho)}=e^{-nh(\rho)}$. Also $h''(\rho)=-1/(\rho(1-\rho))\leq-4$, so $\log2-h(1/2-a)\geq2a^2$. These two bounds give the approximate-recovery denominator in the [list-decoding Fano inequality](information-theory.md#list-decoding-fano-inequality).

#### Perfect code

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_code)

A code of minimum distance $d$ is perfect if its [Hamming balls](#hamming-ball) of radius $\lfloor(d-1)/2\rfloor$ partition the ambient word space. Every word then has a unique nearest codeword within the code's error-correction radius.

##### Binary Golay code

↑ **Parent:** [Perfect code](#perfect-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_Golay_code)

The length-$23$ [binary Golay code](#binary-golay-code) is the [cyclic code](#cyclic-code) over $\mathbb F_2$ generated by

$$
g(X)=1+X+X^5+X^6+X^7+X^9+X^{11}.
$$

It has [dimension](vector-space.md#dimension-vector-space) $12$, [minimum Hamming distance](#minimum-distance-of-a-code) $7$, and its radius-$3$ [Hamming balls](#hamming-ball) partition $\mathbb F_2^{23}$. Its [parity extension](#parity-extension) has length $24$, [dimension](vector-space.md#dimension-vector-space) $12$, and [minimum Hamming distance](#minimum-distance-of-a-code) $8$.

// Target: algebra.bigb

###### Extended binary Golay code

↑ **Parent:** [Binary Golay code](#binary-golay-code)

The extended binary Golay code is the [parity extension](#parity-extension) of the length-$23$ [binary Golay code](#binary-golay-code). It is a [self-dual code](#self-dual-code) and a [doubly even code](#doubly-even-code), with [minimum Hamming distance](#minimum-distance-of-a-code) eight. Its radius-three [Hamming balls](#hamming-ball) are disjoint but do not cover its [Hamming space](#hamming-space); it is not a [perfect code](#perfect-code).

###### Three-error syndrome decoding of extended Golay code

↑ **Parent:** [Extended binary Golay code](#extended-binary-golay-code)

For a binary [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$ with $A^2=I$, the [syndrome](#syndrome) of an error $(p,q)$ relative to the column [parity-check matrix](#parity-check-matrix) $(I;A)$ is $s=p+qA$. An error of total [Hamming weight](#hamming-weight) at most three has at most one nonzero bit in one half. Test $s$, each $s+A_i$, $sA$, and each $sA+A_i$ for weights at most three, two, three and two respectively. These identify $(s,0)$, $(s+A_i,e_i)$, $(0,sA)$ and $(e_i,sA+A_i)$. For the [extended binary Golay code](#extended-binary-golay-code), [minimum Hamming distance](#minimum-distance-of-a-code) eight guarantees that at most one such error exists.

###### Systematic-matrix proof of extended Golay distance

↑ **Parent:** [Extended binary Golay code](#extended-binary-golay-code)

Suppose a binary [symmetric matrix](linear-algebra.md#symmetric-matrix) $A$ satisfies $A^2=I$, has one row of [Hamming weight](#hamming-weight) eleven and eleven rows of [Hamming weight](#hamming-weight) seven, and every sum of two distinct rows has [Hamming weight](#hamming-weight) six. Then $(I\mid A)$ generates a [self-dual code](#self-dual-code). Its rows have weights twelve or eight; their mutual orthogonality makes every generated word [doubly even](#doubly-even-code). A weight-four word $(u,uA)$ would have left-half weight one, two, three or four. The first two cases are excluded by the stated row weights; weight three would force $uA$ to be a unit vector and hence $u$ to be a row of $A$; weight four would force $uA=0$. Thus weight four is impossible and the [minimum Hamming distance](#minimum-distance-of-a-code) is eight.

###### Golay generator polynomial

↑ **Parent:** [Binary Golay code](#binary-golay-code)

The [generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code) defining the [binary Golay code](#binary-golay-code) is $1+X+X^5+X^6+X^7+X^9+X^{11}$.

###### BCH and parity-extension proof of the binary Golay distance

↑ **Parent:** [Binary Golay code](#binary-golay-code)

A root $\beta$ of the binary [Golay generator polynomial](#golay-generator-polynomial) has order $23$, and the [Frobenius endomorphism](galois-theory.md#frobenius-endomorphism) shows that $\beta,\beta^2,\beta^3,\beta^4$ are roots: $2^8\equiv3\pmod{23}$. The [BCH bound](#bch-bound) gives [minimum Hamming distance](#minimum-distance-of-a-code) at least five. The [circular autocorrelation of the binary Golay generator](#circular-autocorrelation-of-the-binary-golay-generator) makes its [parity extension](#parity-extension) [doubly even](#doubly-even-code), excluding original weights five and six. The generator itself has [Hamming weight](#hamming-weight) seven, proving that the distance is exactly seven.

// Target: algebra.bigb

###### Circular autocorrelation of the binary Golay generator

↑ **Parent:** [Binary Golay code](#binary-golay-code)

The polynomial identity $(X+1)g(X)g^{\mathrm{rev}}(X)=X^{23}+1$, where $g^{\mathrm{rev}}(X)=X^{11}g(X^{-1})$, implies

$$
g(X)g(X^{-1})\equiv1+X+\cdots+X^{22}\pmod{X^{23}-1}.
$$

Every coefficient is the binary [inner product](linear-algebra.md#inner-product) of the coefficient vector of $g$ with one cyclic shift. Thus every such [inner product](linear-algebra.md#inner-product) is one. Appending a parity bit to the cyclic shifts gives mutually orthogonal weight-eight vectors, so [orthogonal generators of doubly even codes](#orthogonal-generators-of-doubly-even-codes) applies.

// Target: algebra.bigb

#### Singleton bound

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singleton_bound)

For a code of length $n$, size $M$, and minimum distance $d$ over an alphabet of size $q$, puncturing $d-1$ coordinates gives the Singleton bound

$$
M\leq q^{n-d+1}.
$$

#### Plotkin bound

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Plotkin_bound)

The Plotkin bound limits a code whose minimum distance is more than the average distance between unrestricted words. For a binary code with $n<2d$ and even $d$,

$$
M\leq2\left\lfloor\frac d{2d-n}\right\rfloor.
$$

#### Puncturing (coding theory)

↑ **Parent:** [Binary block code](#binary-block-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Puncturing_(coding_theory))

##### Punctured code

↑ **Parent:** [Puncturing (coding theory)](#puncturing-coding-theory)

Puncturing a code at one coordinate deletes that coordinate from every codeword. For a code of minimum distance $d\geq2$, puncturing preserves its number of words and gives minimum distance $d$ or $d-1$.

## One-time pad

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/One-time_pad)

For messages in a [finite additive group](group.md#finite-additive-group), a one-time pad encrypts $X$ as $C=X+K$, where the key $K$ is uniform and [independent](random-variable.md#independent-random-variables) of $X$, as long as the message, and never reused. Then $C$ is uniform and [independent](random-variable.md#independent-random-variables) of $X$, giving [perfect secrecy](#perfect-secrecy).

### Two-time pad attack

↑ **Parent:** [One-time pad](#one-time-pad)

If two plaintexts are encrypted by adding the same one-time-pad key, subtracting the ciphertexts cancels the key and reveals the difference of the plaintexts. Redundancy in natural language or another structured message space can then reveal both messages, so a one-time pad must never reuse key material.

### Perfect secrecy

↑ **Parent:** [One-time pad](#one-time-pad)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Perfect_secrecy)

An encryption scheme has perfect secrecy when the ciphertext and plaintext are [independent random variables](random-variable.md#independent-random-variables), so observing the ciphertext does not change the plaintext's [probability distribution](probability-theory.md#probability-distribution).

### Malleability of an additive one-time pad

↑ **Parent:** [One-time pad](#one-time-pad)

If an interceptor knows that an additive one-time-pad ciphertext $C$ encrypts plaintext $P$ and wants it to decrypt as $P'$, replacing it by

$$
C'=C-P+P'
$$

works without knowing the key, since $C'=P'+K$.

## Secret sharing

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Secret_sharing)

A secret-sharing scheme distributes shares of a secret so that authorized collections can reconstruct it while unauthorized collections reveal no information about it.

### Threshold secret sharing

↑ **Parent:** [Secret sharing](#secret-sharing)

An $(r,s)$ threshold secret-sharing scheme issues $s$ shares: every collection of at least $r$ shares reconstructs the secret, while every collection of fewer than $r$ shares has a distribution independent of the secret.

<h4 id="shamir-s-secret-sharing">Shamir's secret sharing</h4>

↑ **Parent:** [Threshold secret sharing](#threshold-secret-sharing)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shamir's_secret_sharing)

Shamir's secret sharing places a secret $N$ at the constant term of a random polynomial $f\in\mathbb F_p[X]$ of degree at most $r-1$ and issues distinct nonzero evaluation pairs $(x_i,f(x_i))$. Any $r$ shares recover $f$ by [polynomial interpolation](numerical-analysis.md#polynomial-interpolation). Given fewer than $r$ shares, every candidate constant term has the same number of compatible coefficient tuples, which gives perfect secrecy.

<h5 id="perfect-secrecy-of-shamir-s-threshold-scheme">Perfect secrecy of Shamir's threshold scheme</h5>

↑ **Parent:** [Shamir's secret sharing](#shamir-s-secret-sharing)

Conditioned on any $r-1$ shares in [Shamir's secret sharing](#shamir-s-secret-sharing), each candidate secret in $\mathbb F_p$ remains equally likely. Appending $(0,N)$ to those shares determines exactly one degree-at-most-$(r-1)$ polynomial for every candidate $N$, by the nonzero [Vandermonde determinant](galois-theory.md#vandermonde-determinant).

## Discrete memoryless channel

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_memoryless_channel)

A discrete memoryless channel has finite input and output alphabets and transition probabilities $P(y\mid x)$. Conditional on the input symbols, different channel uses have independent outputs governed by the same transition probabilities.

### Finite-alphabet erasure channel

↑ **Parent:** [Discrete memoryless channel](#discrete-memoryless-channel)

A finite-alphabet erasure channel transmits the input symbol unchanged with probability $1-f$ and replaces it by a distinct erasure flag with probability $f$, independently of the symbol. Given the flag, the posterior remains the input distribution; otherwise the input is known. Thus its [mutual information](information-theory.md#mutual-information) is $(1-f)H(X)$.

#### Capacity of a finite-alphabet erasure channel

↑ **Parent:** [Finite-alphabet erasure channel](#finite-alphabet-erasure-channel)

For a [finite-alphabet erasure channel](#finite-alphabet-erasure-channel) with $k$ input symbols, $I(X;Y)=(1-f)H(X)$. Maximizing [Shannon entropy](information-theory.md#information-entropy) at the uniform input gives [channel capacity](information-theory.md#channel-capacity) $C=(1-f)\log_2k$ bits per use, by the [Shannon second coding theorem](#noisy-channel-coding-theorem).

### Binary erasure channel

↑ **Parent:** [Discrete memoryless channel](#discrete-memoryless-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_erasure_channel)

A binary erasure channel transmits each input bit correctly with probability $1-\varepsilon$ and replaces it by an erasure symbol with probability $\varepsilon$. Its [channel capacity](information-theory.md#channel-capacity) is $1-\varepsilon$ bits per use.

### Z-channel

↑ **Parent:** [Discrete memoryless channel](#discrete-memoryless-channel)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Z-channel)

A Z-channel transmits one binary input without error while the other can change into the first. Unlike a [binary symmetric channel](#binary-symmetric-channel), its errors are one-sided.

## Noisy-channel coding theorem

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Noisy-channel_coding_theorem)

For a discrete memoryless channel, operational capacity equals

$$
C=\max_{P_X}I(X;Y).
$$

Rates below $C$ admit codes whose error tends to zero, while rates above $C$ cannot have vanishing error.

### Reliable transmission rate

↑ **Parent:** [Noisy-channel coding theorem](#noisy-channel-coding-theorem)

A rate $R$ is reliably achievable through a channel when there is a sequence of length-$n$ channel codes with $M_n$ messages such that

$$
\liminf_{n\to\infty}\frac{\log_2M_n}{n}\geq R
$$

and their decoding-error probability tends to zero.

## Linear-feedback shift register

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear-feedback_shift_register)

A binary linear-feedback shift register of degree $d$ updates a $d$-bit state by shifting and inserting a fixed linear combination over $\mathbb F_2$. With recurrence

$$
s_{n+d}=a_{d-1}s_{n+d-1}+\cdots+a_0s_n,
$$

its feedback polynomial is $x^d+a_{d-1}x^{d-1}+\cdots+a_0$.

### Output sets of different-length linear-feedback registers

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

Under the convention that a register emits each shifted-out symbol, its first $d$ output symbols are exactly its initial fill. Thus a binary register of length $d$ has $2^d-1$ distinct outputs from nonzero fills. For lengths $r<s$, at least one longer-register output is absent from the shorter register, guaranteeing a pair of unequal nonzero outputs. The two sets need not be disjoint: recurrences $s_{n+1}=s_n$ and $s_{n+2}=s_n$ both generate constant ones. Nor must they intersect: the length-one recurrence and $s_{n+2}=s_{n+1}+s_n$ have no common nonzero output, since constant ones fail the second recurrence.

### Feedback polynomial

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

The feedback polynomial records the coefficients of an [LFSR](#linear-feedback-shift-register) recurrence. With the convention

$$
s_{n+d}=a_{d-1}s_{n+d-1}+\cdots+a_0s_n,
$$

it is $x^d+a_{d-1}x^{d-1}+\cdots+a_0$.

### Feedback shift register

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Feedback_shift_register)

A feedback shift register updates a finite state by shifting its stored symbols and inserting the value of a feedback function of the previous state. The feedback function need not be linear.

### Berlekamp-Massey algorithm

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Berlekamp–Massey_algorithm)

The Berlekamp-Massey algorithm finds the shortest linear recurrence satisfied by a finite sequence over a field. It processes symbols incrementally, updating the connection polynomial whenever the current recurrence has a nonzero discrepancy.

#### Minimum recurrence length after a new discrepancy

↑ **Parent:** [Berlekamp-Massey algorithm](#berlekamp-massey-algorithm)

Suppose a connection polynomial $C$ of degree at most $L$, with recurrence span $L$ gives zero recurrence discrepancies through index $r-1$ but a nonzero discrepancy at $r$. If a polynomial $D$ of span $L'$ successfully explains the prefix through $r$ and $L+L'\leq r$, evaluate the coefficient at $r$ in the convolution $(CD)x$. Applying $D$ first makes it zero. Applying $C$ first leaves its nonzero discrepancy at $r$, because the earlier discrepancies vanish and $D$ has constant coefficient one. This contradiction gives the displayed lower bound. It is the minimality step used by the [Berlekamp-Massey algorithm](#berlekamp-massey-algorithm); the algorithm cancels the new discrepancy with a shifted earlier failed polynomial.

#### Minimal recurrence for the binary prefix 11001011

↑ **Parent:** [Berlekamp-Massey algorithm](#berlekamp-massey-algorithm)

The shortest binary linear recurrence producing the prefix $11001011$ has length three:

$$
x_n=x_{n-2}+x_{n-3}.
$$

Its connection polynomial is $1+D^2+D^3$.

### Period bound for a linear-feedback shift register

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

A degree-$d$ binary register has $2^d$ states. The zero state is fixed, so a nonzero periodic orbit has length at most $2^d-1$.

### Feedback-polynomial parity condition for maximal period

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

A maximal-period feedback polynomial cannot have $1$ as a root. Over $\mathbb F_2$, this says

$$
1+a_{d-1}+\cdots+a_0\ne0,
$$

so an even number of the coefficients $a_i$ equal one and the full monic polynomial has an odd number of nonzero coefficients.

### Zero-run lower bound for a linear-feedback shift register

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

If an output prefix contains $d$ consecutive zeros followed by a one, no register of degree at most $d$ can generate it: the all-zero state would have been reached and would remain zero forever.

#### Minimal linear-feedback shift register for the prefix 100000001

↑ **Parent:** [Zero-run lower bound for a linear-feedback shift register](#zero-run-lower-bound-for-a-linear-feedback-shift-register)

The seven consecutive zeros followed by one force degree at least eight. Degree eight is attained by $s_{n+8}=s_n$, with initial state $10000000$ and feedback polynomial $x^8+1$.

### Trace-generated maximal-period linear-feedback sequence

↑ **Parent:** [Linear-feedback shift register](#linear-feedback-shift-register)

Let $K=\mathbb F_{2^d}$, let $\alpha$ generate $K^\times$, and let $T:K\to\mathbb F_2$ be nonzero linear with [nondegenerate bilinear form](linear-algebra.md#nondegenerate-bilinear-form) $(x,y)\mapsto T(xy)$. If the [minimal polynomial](linear-operator-theory.md#minimal-polynomial) of $\alpha$ is $P(X)=X^d+\sum_{j<d}c_jX^j$, then $x_n=T(\alpha^n)$ satisfies

$$
x_{n+d}=\sum_{j<d}c_jx_{n+j},
$$

so it is produced by an LFSR of length at most $d$. Its period is exactly $2^d-1$: any period $r$ would imply $T((\alpha^r-1)y)=0$ for every $y\in K$, hence $\alpha^r=1$ by nondegeneracy.

## Linear code

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Linear_code)

A binary linear $[n,k,d]$ code is a $k$-dimensional subspace of $\mathbb F_2^n$ with least nonzero weight $d$. A parity-check matrix presents it as a kernel.

### Monomial equivalence of linear codes

↑ **Parent:** [Linear code](#linear-code)

Two [linear codes](#linear-code) are monomially equivalent if a permutation of coordinates followed by multiplication of individual coordinates by nonzero [field](algebra.md#field) elements takes one to the other. This preserves [dimension](vector-space.md#dimension-vector-space) and [Hamming distance](#hamming-distance). Choosing different representatives for projective parity-check columns produces this equivalence.

### Maximum distance separable code

↑ **Parent:** [Linear code](#linear-code)

A nonzero length-$n$, dimension-$k$ [linear code](#linear-code) is maximum distance separable if its [minimum Hamming distance](#minimum-distance-of-a-code) equals $n-k+1$, attaining the [Singleton bound](#singleton-bound). [Reed-Solomon codes](#reed-solomon-error-correction) and [generalized Reed-Solomon codes](#generalized-reed-solomon-code) provide examples because a nonzero polynomial of degree at most $k-1$ has at most $k-1$ distinct [polynomial roots](polynomial.md#root-of-a-polynomial).

### Reed-Solomon error correction

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reed–Solomon_error_correction)

For distinct elements $a_1,\ldots,a_n$ of a [finite field](algebra.md#finite-field), a Reed-Solomon code consists of the evaluation vectors $(f(a_1),\ldots,f(a_n))$ of [polynomials](polynomial.md) with degree less than $k$. It has [dimension](vector-space.md#dimension-vector-space) $k$ and [minimum Hamming distance](#minimum-distance-of-a-code) $n-k+1$, so it is a [maximum distance separable code](#maximum-distance-separable-code). A nonzero polynomial has at most its degree many distinct [polynomial roots](polynomial.md#root-of-a-polynomial). [Primitive cyclic Reed-Solomon codes](#primitive-cyclic-reed-solomon-code) use all nonzero field elements, ordered as powers of a [primitive root of unity](algebra.md#primitive-root-of-unity); arbitrary evaluation sets need not give a [cyclic code](#cyclic-code).

#### Primitive cyclic Reed-Solomon code

↑ **Parent:** [Reed-Solomon error correction](#reed-solomon-error-correction)

Let $n=q-1$ and let $\omega$ be a [primitive root of unity](algebra.md#primitive-root-of-unity) in $\mathbb F_q$. The length-$n$ [cyclic code](#cyclic-code) with consecutive [zeros of a cyclic code](#zero-of-a-cyclic-code) $\omega^b,\ldots,\omega^{b+n-k-1}$ has dimension $k$. It equals the [generalized Reed-Solomon code](#generalized-reed-solomon-code) of vectors $(\omega^{j(1-b)}f(\omega^j))_{j=0}^{n-1}$, $\deg f<k$. The choice $b=1$ is the unweighted [Reed-Solomon code](#reed-solomon-error-correction) on these evaluation points; allowing other offsets makes this family closed under [dual codes](#dual-code).

##### Reed-Solomon key equation

↑ **Parent:** [Primitive cyclic Reed-Solomon code](#primitive-cyclic-reed-solomon-code)

With [syndromes](#syndrome) $S_\ell=\sum_i E_i X_i^{b+\ell}$ and distinct error-location values $X_i$, form $S(z)=\sum_{\ell=0}^{n-k-1}S_\ell z^\ell$ and the [error locator polynomial](#error-locator-polynomial) $\Lambda(z)=\prod_i(1-X_i z)$. There is an [error evaluator polynomial](#error-evaluator-polynomial) $\Omega$ of degree less than the number of errors satisfying the key equation. When the number of errors is at most $\lfloor(n-k)/2\rfloor$, the [Berlekamp-Massey algorithm](#berlekamp-massey-algorithm) or [extended Euclidean algorithm](number-theory.md#extended-euclidean-algorithm) recovers these polynomials, normalized by $\Lambda(0)=1$.

##### Duality of primitive cyclic Reed-Solomon codes

↑ **Parent:** [Primitive cyclic Reed-Solomon code](#primitive-cyclic-reed-solomon-code)

For $n=q-1$ and $a_j=\omega^j$, the two evaluation forms are $a_j^{1-b}f(a_j)$ and $a_j^b h(a_j)$, with $\deg f<k$ and $\deg h<n-k$. Their [dot product](linear-algebra.md#dot-product) is $\sum_j a_j f(a_j)h(a_j)=0$, since every appearing exponent is between one and $n-1$ and the sums of those powers of $a_j$ vanish. Comparing [dimensions](vector-space.md#dimension-vector-space) proves equality with the [dual code](#dual-code). In particular, the dual of the unweighted evaluation code has multipliers $a_j$; it need not be an unweighted evaluation code on the same ordered points.

#### Generalized Reed-Solomon code

↑ **Parent:** [Reed-Solomon error correction](#reed-solomon-error-correction)

A generalized Reed-Solomon code consists of $(v_i f(a_i))_{i=1}^n$, where the evaluation points are distinct, all coordinate multipliers $v_i$ are nonzero, and $\deg f<k$. It remains a [maximum distance separable code](#maximum-distance-separable-code). Its [dual code](#dual-code) is another generalized Reed-Solomon code with dimension $n-k$ and multipliers proportional to $v_i^{-1}\prod_{j\ne i}(a_i-a_j)^{-1}$.

### Code rate

↑ **Parent:** [Linear code](#linear-code)

For a linear code of length $n$ and dimension $k$ over $\mathbb F_q$, the code rate is $R=k/n$. There are $q^k$ possible messages represented by $q^k$ [codewords](#codeword) of length $n$. More generally a block code $C\subseteq\mathbb F_q^n$ has rate $\log_q|C|/n$. This is a dimensionless redundancy measure, distinct from information transmitted per unit physical time.

#### Asymptotic rate-distance function

↑ **Parent:** [Code rate](#code-rate)

The asymptotic rate-distance function is $\alpha_q(\delta)=\limsup_{n\to\infty}n^{-1}\log_q A_q(n,\max\{1,\lceil\delta n\rceil\})$. It is the best asymptotic [code rate](#code-rate) available at the specified [relative minimum distance](#relative-minimum-distance-of-a-code). A limsup is used because the definition does not assume an ordinary limit exists.

// Target: algebra.bigb

### Binary linear code

↑ **Parent:** [Linear code](#linear-code)

A [linear code](#linear-code) over the two-element [finite field](algebra.md#finite-field). Its dimension $r$ gives $2^r$ codewords. Its [weight enumerator](#weight-enumerator) in the convention $W_C(s,t)=\sum_{c\in C}s^{w(c)}t^{n-w(c)}$ is symmetric in $s,t$ exactly when the all-ones word belongs to $C$: adding that word complements every bit and replaces weight $w$ by $n-w$. Conversely symmetry makes the coefficient of $s^n$ equal the coefficient of $t^n$, which is one.

#### Total weight of a full-support binary linear code

↑ **Parent:** [Binary linear code](#binary-linear-code)

A length-$n$, dimension-$k$ [binary linear code](#binary-linear-code) has full support when no coordinate vanishes on every [codeword](#codeword), equivalently when the union of the [supports of a vector](numerical-analysis.md#support-of-a-vector) of all codewords covers every coordinate. Every coordinate is then a nonzero [linear functional](linear-algebra.md#linear-functional) on the message [vector space](vector-space.md) $\mathbb F_2^k$. Translation by a [vector](vector-space.md#vector) on which it is one pairs the zero and one fibers, so exactly $2^{k-1}$ [codewords](#codeword) contribute one in that coordinate. Summing these contributions proves the formula. If there are $r$ nonzero columns in a full-rank [generator matrix](#generator-matrix), the same argument gives $r2^{k-1}$ instead.

#### Even-weight subcode of a binary linear code

↑ **Parent:** [Binary linear code](#binary-linear-code)

For a [binary linear code](#binary-linear-code) $C$, the [linear functional](linear-algebra.md#linear-functional) $\sigma(x)=\sum_jx_j$ records [Hamming weight](#hamming-weight) modulo two. Its [kernel of a linear map](linear-algebra.md#kernel-of-a-linear-map) is the even-weight subcode. If $\sigma|_C$ vanishes, this is all of $C$; otherwise [rank-nullity theorem](linear-algebra.md#rank-nullity-theorem) gives [dimension](vector-space.md#dimension-vector-space) $\dim C-1$. This also proves closure under addition without treating ordinary integer weight as a linear function.

#### Doubly even code

↑ **Parent:** [Binary linear code](#binary-linear-code)

A [binary linear code](#binary-linear-code) is [doubly even](#doubly-even-code) when the [Hamming weight](#hamming-weight) of every codeword is divisible by four.

// Target: algebra.bigb

##### Orthogonal generators of doubly even codes

↑ **Parent:** [Doubly even code](#doubly-even-code)

Suppose the generators of a [binary linear code](#binary-linear-code) have [Hamming weights](#hamming-weight) divisible by four and have pairwise zero binary [inner products](linear-algebra.md#inner-product). Their [linear span](vector-space.md#linear-span) is [doubly even](#doubly-even-code): for any two vectors,

$$
\operatorname{wt}(u+v)=\operatorname{wt}(u)+\operatorname{wt}(v)-2|\operatorname{supp}(u)\cap\operatorname{supp}(v)|.
$$

The binary [inner product](linear-algebra.md#inner-product) says the intersection size is even. Induction on the number of generators in a sum proves divisibility by four.

// Target: algebra.bigb

#### Self-orthogonal binary subspace

↑ **Parent:** [Binary linear code](#binary-linear-code)

A [linear subspace](vector-space.md#vector-subspace) $W\subseteq\mathbb F_2^n$ is self-orthogonal if $u\cdot v=0$ for every $u,v\in W$. The standard [bilinear form](linear-algebra.md#bilinear-form) is [nondegenerate](linear-algebra.md#nondegenerate-bilinear-form), whence $\dim W+\dim W^\perp=n$ and $\dim W\leq\lfloor n/2\rfloor$. The condition with $u=v$ means every vector has even [Hamming weight](#hamming-weight). Such a [binary linear code](#binary-linear-code) gives the [linear algebra](linear-algebra.md) behind the [Eventown theorem](extremal-set-theory.md#eventown-theorem).

##### Odd-length binary self-orthogonal dual extension

↑ **Parent:** [Self-orthogonal binary subspace](#self-orthogonal-binary-subspace)

If a [self-orthogonal binary subspace](#self-orthogonal-binary-subspace) has odd length $n$ and [dimension](vector-space.md#dimension-vector-space) $(n-1)/2$, its [dual code](#dual-code) is obtained by adjoining the all-ones word. Self-orthogonality makes every [codeword](#codeword) even-weight, so $\mathbf1\in C^\perp$ but $\mathbf1\notin C$. Comparing [dimensions](vector-space.md#dimension-vector-space) proves the formula. The [dimension](vector-space.md#dimension-vector-space) hypothesis alone is insufficient: $C=\langle100\rangle$ at length three is a counterexample.

#### Single parity-check code

↑ **Parent:** [Binary linear code](#binary-linear-code)

The code consisting of all even-weight binary words. For $n\geq1$ its dimension is $n-1$, and its [weight enumerator](#weight-enumerator) is $[(t+s)^n+(t-s)^n]/2$, by selecting the even terms of the [binomial theorem](combinatorics.md#binomial-theorem). The length-one code contains only zero.

### Tetracode

↑ **Parent:** [Linear code](#linear-code)

The two-dimensional ternary [linear code](#linear-code) generated by $(0,1,1,1)$ and $(1,1,-1,0)$. Its eight nonzero words have exactly three nonzero entries, with precisely two opposite words for each position of the zero coordinate.

### Weight enumerator

↑ **Parent:** [Linear code](#linear-code)

The homogeneous [weight enumerator](#weight-enumerator) of a length-$n$ [linear code](#linear-code) $C$ is the [polynomial](polynomial.md)

$$
W_C(s,t)=\sum_{x\in C}s^{\operatorname{wt}(x)}t^{n-\operatorname{wt}(x)}.
$$

Its coefficients count words of each [Hamming weight](#hamming-weight). In this convention $W_C(1,1)=|C|$; some references interchange $s,t$.

#### MacWilliams identity

↑ **Parent:** [Weight enumerator](#weight-enumerator)

For a binary [linear code](#linear-code) of dimension $k$ and its [dual code](#dual-code), the [weight enumerator](#weight-enumerator) convention $s^{\operatorname{wt}(x)}t^{n-\operatorname{wt}(x)}$ gives

$$
W_{C^\perp}(s,t)=2^{-k}W_C(t-s,t+s).
$$

To prove it, insert $\mathbf1_{C^\perp}(y)=2^{-k}\sum_{x\in C}(-1)^{x\cdot y}$ into the enumerator sum. Summing independently over each coordinate of $y$ yields a factor $t+s$ if $x_j=0$ and $t-s$ if $x_j=1$.

### Parity bit

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity_bit)

A parity bit records whether the number of one bits in a word is even or odd and can detect every error that flips an odd number of bits.

#### Parity computation by CNOT gates

↑ **Parent:** [Parity bit](#parity-bit)

Apply one [CNOT gate](quantum-theory.md#controlled-not-gate) from each input [qubit](quantum-mechanics.md#qubit) to the same target. Their actions commute because controls remain unchanged and each contribution is added modulo two. This reversible circuit computes the [parity bit](#parity-bit) with exactly one [two-qubit gate](quantum-circuit.md#two-qubit-gate) per input, and its inverse is the same circuit. Unlike measuring the inputs to compute parity classically, the unitary preserves [quantum superposition](quantum-mechanics.md#quantum-superposition) and can be uncomputed after phase application.

#### Even-weight binary code

↑ **Parent:** [Parity bit](#parity-bit)

The length-$n$ even-weight code consists of binary words whose coordinates sum to zero. It has parameters $[n,n-1,2]$.

### Binary repetition code

↑ **Parent:** [Linear code](#linear-code)

The binary repetition code is $\{0^n,1^n\}$ and has parameters $[n,1,n]$.

### Zero code

↑ **Parent:** [Linear code](#linear-code)

The zero code contains only the zero word and has dimension zero.

### Whole-space linear code

↑ **Parent:** [Linear code](#linear-code)

The whole-space binary code is $\mathbb F_2^n$, with parameters $[n,n,1]$.

### Hamming weight

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamming_weight)

The Hamming weight $\operatorname{wt}(x)$ of a word is the number of its nonzero coordinates.

### Minimum Hamming distance of a linear code

↑ **Parent:** [Linear code](#linear-code)

The minimum Hamming distance of a nonzero [linear code](#linear-code) is the smallest [Hamming weight](#hamming-weight) of a nonzero codeword.

### Griesmer bound

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Griesmer_bound)

Every binary linear $[n,k,d]$ code satisfies

$$
n\geq\sum_{j=0}^{k-1}\left\lceil\frac d{2^j}\right\rceil.
$$

Puncturing on the support of a minimum-weight codeword reduces the rank by one and leaves minimum distance at least $\lceil d/2\rceil$, which proves the bound inductively.

### Generator matrix

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Generator_matrix)

A generator matrix for a [linear code](#linear-code) has a basis of the code as its rows, so its row space is the code.

### Parity-check matrix

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Parity-check_matrix)

A parity-check matrix $H$ for a [linear code](#linear-code) $C$ satisfies

$$
C=\ker H=\{c:Hc^T=0\}.
$$

#### Root-evaluation parity-check matrix of a cyclic code

↑ **Parent:** [Parity-check matrix](#parity-check-matrix)

For a [cyclic code](#cyclic-code) whose [generator polynomial](#generator-polynomial-of-a-cyclic-code) has distinct roots $\alpha_1,\ldots,\alpha_r$ in a [splitting field](galois-theory.md#splitting-field) $E$, the rows $(1,\alpha_i,\ldots,\alpha_i^{n-1})$ impose precisely the codeword conditions $c(\alpha_i)=0$. Expanding each value in a [basis](vector-space.md#basis) of $E$ over the original [finite field](algebra.md#finite-field), then discarding dependent equations, gives a [parity-check matrix](#parity-check-matrix) over that field of [rank](linear-algebra.md#rank-one-quadratic-form) $r$. Alternatively choose one root from each [Frobenius conjugate](algebra.md#frobenius-conjugate) orbit and expand its value in the field it generates.

#### Parity-check dependencies determine minimum distance

↑ **Parent:** [Parity-check matrix](#parity-check-matrix)

In the usual column convention, a [codeword](#codeword) $c$ of a [linear code](#linear-code) obeys $Hc^T=0$, so its nonzero coordinates give a [linear dependence](vector-space.md#linear-dependence) among columns of its [parity-check matrix](#parity-check-matrix). Conversely a dependence gives a nonzero codeword supported on those coordinates. Minimizing the support gives the [minimum Hamming distance of a linear code](#minimum-hamming-distance-of-a-linear-code). In the transposed convention $cP=0$, the corresponding objects are the rows of $P$. The size of a dependent set means the number of its coordinate positions, even when some check vectors coincide.

#### Polynomial multiplication parity-check matrix

↑ **Parent:** [Parity-check matrix](#parity-check-matrix)

A binary check polynomial $h=\sum_{j=0}^{N-1}h_jX^j$ modulo $X^N+1$ gives the circulant matrix $B_{ti}=h_{t-i\bmod N}$ representing multiplication by $h$. Its kernel is the cyclic code. Selecting independent rows gives a parity-check matrix of rank equal to the redundancy, even when the supplied polynomial is not the canonical check polynomial.

// Target: algebra.bigb

#### Reciprocal-polynomial parity-check matrix

↑ **Parent:** [Parity-check matrix](#parity-check-matrix)

If a binary length-$N$ cyclic code has generator of degree $r$ and check polynomial $h$ of degree $N-r$, use the coefficient vectors of $h^*,Xh^*,\ldots,X^{r-1}h^*$ as the rows of a parity-check matrix. They have distinct leading positions and are independent. Their scalar products with a word are the coefficients of $X^{N-r},\ldots,X^{N-1}$ in its product with $h$, which vanish for codewords.

// Target: algebra.bigb

#### Syndrome

↑ **Parent:** [Parity-check matrix](#parity-check-matrix)

The syndrome of a received word $y$ with respect to a [parity-check matrix](#parity-check-matrix) $H$ is $s=Hy^T$. It vanishes exactly when $y$ is a codeword and otherwise identifies the coset containing the error pattern.

##### Syndrome classification of code cosets

↑ **Parent:** [Syndrome](#syndrome)

For a rank-$(N-k)$ parity-check matrix of a linear code $C$, two words have equal syndromes exactly when their difference lies in $C$. Thus attainable syndromes label cosets bijectively. For a received word $c+e$, its syndrome is that of the error $e$, so minimum-weight representatives provide [minimum-distance decoding](#minimum-distance-decoding).

// Target: algebra.bigb

###### Coset leader

↑ **Parent:** [Syndrome classification of code cosets](#syndrome-classification-of-code-cosets)

A coset leader is a minimum-Hamming-weight word in a coset of a linear code. It represents a most economical error pattern with the associated syndrome. Several leaders can tie; they need not be unique outside the code's guaranteed correction radius.

### Parity-check extension of a linear code

↑ **Parent:** [Linear code](#linear-code)

The parity-check extension of a binary [linear code](#linear-code) appends to each codeword the sum of its coordinates in $\mathbb F_2$, making every extended word have even [Hamming weight](#hamming-weight).

### Shortened code

↑ **Parent:** [Linear code](#linear-code)

Shortening a code at one coordinate first retains only words with a chosen symbol there and then applies [puncturing](#puncturing-coding-theory) at that coordinate. The minimum distance cannot decrease. In a binary code one coordinate-symbol fibre contains at least half of the words.

### Dual code

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_code)

The dual code $C^\perp$ consists of the words orthogonal to every word of $C$ under the standard dot product. A [parity-check matrix](#parity-check-matrix) for $C$ is a [generator matrix](#generator-matrix) for $C^\perp$.

#### Self-dual code

↑ **Parent:** [Dual code](#dual-code)

A [linear code](#linear-code) is self-dual when it equals its [dual code](#dual-code) under the standard [dot product](linear-algebra.md#dot-product). For a length-$2k$ code with a rank-$k$ [generator matrix](#generator-matrix) $G$, this is equivalent to $GG^T=0$: orthogonality gives inclusion in the [dual code](#dual-code), and equal [dimensions](vector-space.md#dimension-vector-space) give equality. Over $\mathbb F_2$, a [generator matrix](#generator-matrix) $(I\mid A)$ therefore generates a self-dual code exactly when $AA^T=I$.

##### Binary self-dual code contains the all-ones word

↑ **Parent:** [Self-dual code](#self-dual-code)

For a binary [self-dual code](#self-dual-code), every word $c$ satisfies $c\cdot c=0$. In characteristic two this is $\sum_i c_i=0$, so the all-ones word is orthogonal to every [codeword](#codeword) and lies in the [dual code](#dual-code), hence the code itself. The [dual code](#dual-code) [dimension](vector-space.md#dimension-vector-space) identity gives even length and half-length [dimension](vector-space.md#dimension-vector-space).

### Reed-Muller code

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Reed–Muller_code)

The binary Reed-Muller code $\operatorname{RM}(d,r)$ evaluates Boolean polynomials of degree at most $r$ on $\mathbb F_2^d$. It has parameters

$$
\left[2^d,\sum_{j=0}^r\binom dj,2^{d-r}\right].
$$

The dimension counts square-free monomials, and the minimum weight follows inductively from the decomposition $(u,u+v)$.

#### Bar product of binary linear codes

↑ **Parent:** [Reed-Muller code](#reed-muller-code)

For length-$n$ binary linear codes $C_2\subseteq C_1$, their bar product is

$$
C_1|C_2=\{(u,u+v):u\in C_1,\ v\in C_2\}.
$$

It has length $2n$ and dimension $\dim C_1+\dim C_2$.

##### Minimum distance of a bar product

↑ **Parent:** [Bar product of binary linear codes](#bar-product-of-binary-linear-codes)

If $C_2\subseteq C_1$ have minimum distances $d_2,d_1$, respectively, then

$$
d(C_1|C_2)=\min(2d_1,d_2).
$$

Indeed, $\operatorname{wt}(u)+\operatorname{wt}(u+v)\geq\operatorname{wt}(v)$, while the words $(u,u)$ and $(0,v)$ attain the two candidate bounds.

##### Parity-check matrix of a bar product

↑ **Parent:** [Bar product of binary linear codes](#bar-product-of-binary-linear-codes)

If $H_i$ is a [parity-check matrix](#parity-check-matrix) of $C_i$, then a parity-check matrix of $C_1|C_2$ is

$$
\begin{pmatrix}H_1&0\\H_2&H_2\end{pmatrix}.
$$

Its equations say that the first half $u$ lies in $C_1$ and that the sum of the two halves lies in $C_2$.

##### Reed-Muller bar-product recursion

↑ **Parent:** [Bar product of binary linear codes](#bar-product-of-binary-linear-codes)

For $0<r<d$,

$$
\operatorname{RM}(d,r)
=\operatorname{RM}(d-1,r)
\mid\operatorname{RM}(d-1,r-1).
$$

Consequently

$$
\dim\operatorname{RM}(d,r)=\sum_{j=0}^r\binom dj.
$$

#### Dual of a Reed-Muller code

↑ **Parent:** [Reed-Muller code](#reed-muller-code)

Under the standard binary inner product,

$$
\operatorname{RM}(d,r)^\perp
=\operatorname{RM}(d,d-r-1).
$$

The product of representing polynomials has degree at most $d-1$, so its evaluation word has even weight; equality follows by comparing dimensions.

### Hamming code

↑ **Parent:** [Linear code](#linear-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamming_code)

The binary Hamming code of redundancy $r$ has parameters $[2^r-1,2^r-r-1,3]$. Its parity-check matrix has every nonzero vector of $\mathbb F_2^r$ as a column.

#### Ternary Hamming code

↑ **Parent:** [Hamming code](#hamming-code)

For $s\geq2$, use one nonzero representative from each one-dimensional subspace of $\mathbb F_3^s$ as a [parity-check matrix](#parity-check-matrix) column. The [rank](linear-algebra.md#rank-one-quadratic-form) is $s$; no zero or proportional columns imply [minimum Hamming distance](#minimum-distance-of-a-code) at least three. Two independent columns and the representative of their sum give a weight-three relation, proving equality. Every nonzero [syndrome](#syndrome) uniquely identifies one column and one nonzero error value.

##### Ternary Hamming code as a cyclic code

↑ **Parent:** [Ternary Hamming code](#ternary-hamming-code)

For odd $s\geq3$, put $n=(3^s-1)/2$ and choose $\alpha$ of order $n$ in $\mathbb F_{3^s}$. Because $n$ is odd, the powers $\alpha^i$, $0\leq i<n$, represent every projective point once. The [cyclic code](#cyclic-code) defined by $c(\alpha)=0$ is therefore monomially equivalent to a [ternary Hamming code](#ternary-hamming-code), with the displayed [generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code). This statement requires a qualification: at $s=2$, every ternary cyclic length-four, dimension-two code has a weight-two generator, so none has [Hamming distance](#hamming-distance) three.

##### Ternary Hamming code as a negacyclic code

↑ **Parent:** [Ternary Hamming code](#ternary-hamming-code)

Set $n=(3^s-1)/2$ and let $\beta$ be a [primitive element of a finite field](algebra.md#primitive-element-of-a-finite-field) $\mathbb F_{3^s}$. The powers $1,\beta,\ldots,\beta^{n-1}$ represent every projective point once. Their [kernel](linear-algebra.md#kernel-of-a-linear-map) code is a [ternary Hamming code](#ternary-hamming-code). Since $\beta^n=-1$, its [polynomial](polynomial.md) description is a [negacyclic code](#negacyclic-code), generated by the [minimal polynomial of an algebraic element](galois-theory.md#minimal-polynomial-of-an-algebraic-element) $\beta$ over $\mathbb F_3$.

#### Hamming code as a cyclic code

↑ **Parent:** [Hamming code](#hamming-code)

Let $\omega$ generate $\mathbb F_{2^s}^{\times}$, $s\geq2$, and set $n=2^s-1$. The binary [cyclic code](#cyclic-code) defined by $c(\omega)=0$ has a [parity-check matrix](#parity-check-matrix) consisting of every nonzero vector of $\mathbb F_2^s$ once, after choosing a [basis](vector-space.md#basis) and ordering its columns. It is therefore a [Hamming code](#hamming-code). Its [generator polynomial](#generator-polynomial-of-a-cyclic-code) is the [minimal polynomial of an algebraic element](galois-theory.md#minimal-polynomial-of-an-algebraic-element) $m_\omega(x)=\prod_{j=0}^{s-1}(x-\omega^{2^j})$, of degree $s$.

#### Hamming code weight enumerator

↑ **Parent:** [Hamming code](#hamming-code)

Here $N=2^l-1$, $m=2^{l-1}$ and the [weight enumerator](#weight-enumerator) convention is $W_C(s,t)=\sum_{c\in C}s^{\operatorname{wt}(c)}t^{N-\operatorname{wt}(c)}$. The [dual code](#dual-code) is the [binary simplex code](#binary-simplex-code), with enumerator $t^N+(2^l-1)s^m t^{m-1}$. The [MacWilliams identity](#macwilliams-identity) gives the formula. For $l=3$, the ordinary enumerator $W_C(z,1)$ is $1+7z^3+7z^4+z^7$; for $l=1$, the degenerate one-word code has enumerator $t$.

##### Low-weight coefficients of a binary Hamming code

↑ **Parent:** [Hamming code weight enumerator](#hamming-code-weight-enumerator)

For $n=2^\ell-1$, a [codeword](#codeword) in a [Hamming code](#hamming-code) is a subset of the nonzero [vectors](vector-space.md#vector) of $\mathbb F_2^\ell$ whose sum is zero. Ordered weight-three [supports of a vector](numerical-analysis.md#support-of-a-vector) are determined by two distinct nonzero [vectors](vector-space.md#vector), giving $n(n-1)$ choices. For weight four, the third [vector](vector-space.md#vector) must avoid the three nonzero [vectors](vector-space.md#vector) in the [linear span](vector-space.md#linear-span) of the first two, giving $n(n-1)(n-3)$ choices. For weight five, the first three must be linearly independent, and the fourth must avoid all seven nonzero [vectors](vector-space.md#vector) in their [linear span](vector-space.md#linear-span), giving $n(n-1)(n-3)(n-7)$ choices. The final [vector](vector-space.md#vector) is their sum. Dividing by $3!$, $4!$, and $5!$ counts unordered [supports of a vector](numerical-analysis.md#support-of-a-vector) and proves the displayed [weight enumerator](#weight-enumerator) coefficients.

#### Extended Hamming code

↑ **Parent:** [Hamming code](#hamming-code)

Adding an overall [parity bit](#parity-bit) to the [Hamming code of length seven](#hamming-code-of-length-seven) gives an eight-bit [linear code](#linear-code) with [minimum Hamming distance](#minimum-distance-of-a-code) four: every resulting weight is [even](calculus.md#even-function), every original nonzero weight is at least three, and a weight-three word extends to weight four. Thus it detects up to three errors when testing [codeword](#codeword) membership and corrects one error. Joint single-error correction and double-error detection uses the overall parity together with the seven-bit [syndrome](#syndrome).

#### Hamming code of length seven

↑ **Parent:** [Hamming code](#hamming-code)

The [binary linear code](#binary-linear-code) known as the [Hamming code](#hamming-code) of length seven is the [kernel](linear-algebra.md#kernel-of-a-linear-map) of a $3\times7$ [parity-check matrix](#parity-check-matrix) whose columns are all the nonzero vectors of $\mathbb F_2^3$. Its [dimension](vector-space.md#dimension-vector-space) is four. No one-column or two-column sum vanishes, but some three-column sum does, so its [minimum Hamming distance](#minimum-distance-of-a-code) is three. The [syndrome](#syndrome) of a one-bit error is its column, uniquely identifying the erroneous position.

#### Binary simplex code

↑ **Parent:** [Hamming code](#hamming-code)

The binary simplex code is the dual of the binary Hamming code. For redundancy $r$ it has parameters $[2^r-1,r,2^{r-1}]$.

Its relation to the [Hamming code](#hamming-code) is duality, not equality of the code families.

##### Constant weight of a binary simplex code

↑ **Parent:** [Binary simplex code](#binary-simplex-code)

When the columns of $H$ are every nonzero vector in $\mathbb F_2^l$, a nonzero row vector $a$ defines a nonzero [linear functional](linear-algebra.md#linear-functional) $v\mapsto a\cdot v$. Exactly half the $2^l$ input vectors take value $1$: translation by any vector on which the functional is $1$ pairs its zero and one fibres. Removing the zero input removes only a zero value. Thus every nonzero word in the [binary simplex code](#binary-simplex-code) has [Hamming weight](#hamming-weight) $2^{l-1}$.

#### Perfectness of a Hamming code

↑ **Parent:** [Hamming code](#hamming-code)

A Hamming code has $2^{2^r-r-1}$ words, and each radius-one Hamming ball contains $1+(2^r-1)=2^r$ vectors. Its minimum distance is three, so these balls are disjoint, and their total size is $2^{2^r-1}$. They therefore partition the ambient space, making the code perfect.

### Minimum-distance error-detection and correction guarantee

↑ **Parent:** [Linear code](#linear-code)

A code of minimum Hamming distance $d$ detects every pattern of at most $d-1$ errors and uniquely corrects every pattern of at most $\lfloor(d-1)/2\rfloor$ errors. The correction claim follows because Hamming balls of that radius around distinct codewords are disjoint.

## Cyclic code

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cyclic_code)

A length-$n$ cyclic code over $\mathbb F_q$ is an ideal of $\mathbb F_q[X]/(X^n-1)$. It is generated by a monic divisor of $X^n-1$.

### Negacyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

A [linear code](#linear-code) is negacyclic if $(c_0,\ldots,c_{n-1})$ being a [codeword](#codeword) implies that $(-c_{n-1},c_0,\ldots,c_{n-2})$ is a [codeword](#codeword). [Polynomial](polynomial.md) identification makes it an [ideal](commutative-algebra.md#ideal) modulo $X^n+1$. For odd $n$, the substitution $X\mapsto-X$ gives a [monomial equivalence of linear codes](#monomial-equivalence-of-linear-codes) between negacyclic and [cyclic codes](#cyclic-code).

### Zero of a cyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

A zero of a [cyclic code](#cyclic-code) is a [polynomial root](polynomial.md#root-of-a-polynomial) of its [generator polynomial](#generator-polynomial-of-a-cyclic-code), taken in a [splitting field](galois-theory.md#splitting-field). Every [codeword](#codeword), represented as a [polynomial](polynomial.md), vanishes there. For a [repeated-root cyclic code](#repeated-root-cyclic-code), the [multiplicity of a root](polynomial.md#multiplicity-of-a-root) must also be retained: ordinary evaluations alone need not determine the code.

### Repeated-root cyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

A repeated-root cyclic code has length divisible by the characteristic of its field, so the polynomial $X^N-1$ has repeated factors. Its generator can involve powers of those factors. In characteristic two, length $2^t$ gives $X^{2^t}+1=(X+1)^{2^t}$.

// Target: algebra.bigb

#### Repeated-root parity-check matrix

↑ **Parent:** [Repeated-root cyclic code](#repeated-root-cyclic-code)

If the [generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code) has distinct roots $\alpha_i$ with multiplicities $m_i$, a word belongs to the code exactly when $c^{[\ell]}(\alpha_i)=0$ for $0\leq\ell<m_i$, where $c^{[\ell]}$ is its [Hasse derivative](polynomial.md#hasse-derivative). The corresponding rows have entries $\binom j\ell\alpha_i^{j-\ell}$ for $j\geq\ell$ and zero otherwise. Expansion in a [basis](vector-space.md#basis) of the [splitting field](galois-theory.md#splitting-field) gives equations over the original [finite field](algebra.md#finite-field); an independent selection has [rank](linear-algebra.md#rank-one-quadratic-form) $\sum_i m_i$.

#### Binary cyclic codes of length a power of two

↑ **Parent:** [Repeated-root cyclic code](#repeated-root-cyclic-code)

For $N=2^t$, the binary cyclic codes are exactly the nested ideals generated by $(X+1)^j$ for $0\le j\le N$. They have dimensions $N-j$ and canonical check polynomials $(X+1)^{N-j}$. The endpoint ideals are the entire word space and the zero code.

// Target: algebra.bigb

### Check polynomial of a cyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

For a cyclic code with monic generator $g\mid X^N-1$, the canonical check polynomial is $h=(X^N-1)/g$. A word $a$ belongs to the code exactly when $ah$ is zero modulo $X^N-1$, since cancellation in the polynomial ring turns this condition into $g\mid a$. The kernel condition alone allows additional polynomials: it is equivalent to $\gcd(\widetilde h,X^N-1)=h$. Requiring the monic divisor of the modulus singles out the canonical choice.

// Target: algebra.bigb

### Binary cyclic codes of length five

↑ **Parent:** [Cyclic code](#cyclic-code)

Over $\mathbb F_2$, $X^5-1=(X+1)(X^4+X^3+X^2+X+1)$ and the degree-four factor is irreducible: it has no linear root and is not divisible by the sole irreducible quadratic $X^2+X+1$. The four monic divisors give precisely four [cyclic codes](#cyclic-code): the full five-dimensional space, the four-dimensional even-weight code, the one-dimensional repetition code, and the zero code. Their [generator polynomials of a cyclic code](#generator-polynomial-of-a-cyclic-code) are respectively $1$, $X+1$, $X^4+X^3+X^2+X+1$, and $X^5-1$.

### Generator polynomial of a cyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

The unique monic divisor $g(X)$ of $X^n-1$ generating a cyclic code is its generator polynomial. The code has dimension $n-\deg g$.

#### Root-evaluation syndrome for a cyclic code

↑ **Parent:** [Generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code)

Let $\alpha$ be a root of the [generator polynomial of a cyclic code](#generator-polynomial-of-a-cyclic-code) $g(X)$. Every codeword $c(X)$ satisfies $c(\alpha)=0$, so a received word $r=c+e$ satisfies $r(\alpha)=e(\alpha)$. For a single-symbol error $e(X)=aX^j$, the evaluation $r(\alpha)=a\alpha^j$ identifies its value and position when the relevant powers of $\alpha$ are distinct.

##### Single-error test from two binary BCH syndromes

↑ **Parent:** [Root-evaluation syndrome for a cyclic code](#root-evaluation-syndrome-for-a-cyclic-code)

For a binary [cyclic code](#cyclic-code) with [defining zeros of a cyclic code](#zero-of-a-cyclic-code) $\alpha$ and $\alpha^3$, a single error in coordinate $j$ has [polynomial](polynomial.md) $X^j$ and [syndromes](#syndrome) $S_1=\alpha^j$, $S_3=\alpha^{3j}$. If $S_1\ne0$ and $S_3=S_1^3$, recover $j$ from the exponent of $S_1$, flip that coordinate, and verify that the resulting [polynomial](polynomial.md) vanishes at both roots. When the [linear code](#linear-code) has [minimum Hamming distance](#minimum-distance-of-a-code) at least five, this verified correction is the unique [codeword](#codeword) within two errors. The [syndrome](#syndrome) relation alone should not replace checking the corrected word.

### Dual of a cyclic code

↑ **Parent:** [Cyclic code](#cyclic-code)

The dual of a cyclic code is cyclic. If $g(X)h(X)=X^n-1$, then the dual generator is the monic reciprocal polynomial $h^*(X)$.

### Binary cyclic codes of length seven

↑ **Parent:** [Cyclic code](#cyclic-code)

Over $\mathbb F_2$,

$$
X^7-1=(X+1)(X^3+X+1)(X^3+X^2+1).
$$

Its eight monic divisors generate the eight cyclic codes of length seven: the whole-space, even-weight, two Hamming, two simplex, repetition, and zero codes.

### BCH code

↑ **Parent:** [Cyclic code](#cyclic-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/BCH_code)

Given a primitive $n$th root $\alpha$, a BCH code of design distance $\delta$ has a generator polynomial vanishing at $\delta-1$ consecutive powers $\alpha^b,\ldots,\alpha^{b+\delta-2}$.

#### Designed distance

↑ **Parent:** [BCH code](#bch-code)

The [designed distance](#designed-distance) of a [BCH code](#bch-code) is the value $\delta$ specified by requiring $\delta-1$ consecutive [defining zeros of a cyclic code](#zero-of-a-cyclic-code). The [BCH bound](#bch-bound) guarantees [minimum Hamming distance](#minimum-distance-of-a-code) at least $\delta$, but the actual [minimum Hamming distance](#minimum-distance-of-a-code) can be larger. To prove equality, one can exhibit a nonzero [codeword](#codeword) of [Hamming weight](#hamming-weight) exactly $\delta$.

#### Binary cyclotomic coset modulo an odd integer

↑ **Parent:** [BCH code](#bch-code)

For odd $n$, multiplication by two permutes the residues modulo $n$. Its orbit through $i$ is the [binary cyclotomic coset modulo an odd integer](#binary-cyclotomic-coset-modulo-an-odd-integer). If $\alpha$ has order $n$ in a [finite field](algebra.md#finite-field) whose [field characteristic](algebra.md#characteristic-of-a-field) is two, the [Frobenius automorphism](arithmetic.md#frobenius-automorphism) sends $\alpha^i$ to $\alpha^{2i}$. Hence the [minimal polynomial of an algebraic element](galois-theory.md#minimal-polynomial-of-an-algebraic-element) $\alpha^i$ over $\mathbb F_2$ is $\prod_{j\in C_i}(X-\alpha^j)$. Its coefficients are fixed by Frobenius and lie in $\mathbb F_2$, and its degree is the orbit size. Thus a binary [cyclic code](#cyclic-code) containing one [defining zero of a cyclic code](#zero-of-a-cyclic-code) must contain the full orbit as zeros.

#### Error locator polynomial

↑ **Parent:** [BCH code](#bch-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Error_locator_polynomial)

For error locations $i_1,\ldots,i_\nu$ in a cyclic code with primitive root $\alpha$, the error locator polynomial is $\sigma(Z)=\prod_h(1-\alpha^{i_h}Z)$. Its roots encode the error positions.

##### Chien search

↑ **Parent:** [Error locator polynomial](#error-locator-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Chien_search)

A Chien search finds error positions by evaluating an [error locator polynomial](#error-locator-polynomial) at every possible inverse location value $\omega^{-j}$. A zero identifies coordinate $j$. Using the recurrence between successive powers of $\omega$ avoids recomputing all monomials from scratch.

##### Error evaluator polynomial

↑ **Parent:** [Error locator polynomial](#error-locator-polynomial)

For errors $E_i$ at distinct nonzero locations $X_i$, the evaluator associated with syndromes $S_\ell=\sum_i E_iX_i^{b+\ell}$ is $\Omega(z)=\sum_i E_iX_i^b\prod_{h\ne i}(1-X_hz)$. Its degree is smaller than the number of errors. Together with the [error locator polynomial](#error-locator-polynomial) it gives the [Reed-Solomon key equation](#reed-solomon-key-equation) and the [Forney algorithm](#forney-algorithm) for error magnitudes.

###### Forney algorithm

↑ **Parent:** [Error evaluator polynomial](#error-evaluator-polynomial)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Forney_algorithm)

For distinct error locations and the syndrome convention $S_\ell=\sum_i E_iX_i^{b+\ell}$, the displayed formula recovers the error magnitudes from the [error evaluator polynomial](#error-evaluator-polynomial) and [error locator polynomial](#error-locator-polynomial). At $z=X_i^{-1}$, the evaluator is $E_iX_i^b\prod_{h\ne i}(1-X_h/X_i)$, whereas the locator's [formal derivative](galois-theory.md#formal-derivative) is $-X_i\prod_{h\ne i}(1-X_h/X_i)$. Their quotient gives the formula; the denominator is nonzero because the locations are distinct.

// Target: polynomial.bigb

#### BCH bound

↑ **Parent:** [BCH code](#bch-code)

The minimum distance of a BCH code is at least its design distance. A hypothetical word of smaller weight yields a square Vandermonde system from the consecutive-root equations; its support elements are distinct, so the determinant is nonzero and every word coefficient must vanish.

## Parity extension

↑ **Parent:** [Coding theory](coding-theory.md)

Appending a parity bit makes every word even-weight. A binary $[n,m,d]$ code becomes an $[n+1,m,d^+]$ code, where

$$
d^+=
\begin{cases}
d,&d\text{ even},\\
d+1,&d\text{ odd}.
\end{cases}
$$

## Hamming bound

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Hamming_bound)

A binary length-$n$ code of size $M$ and distance at least $2t+1$ satisfies

$$
M\sum_{j=0}^t\binom nj\le2^n.
$$

Equality means the code is perfect.

### Asymptotic Hamming bound

↑ **Parent:** [Hamming bound](#hamming-bound)

The [Hamming bound](#hamming-bound) packs disjoint balls of radius approximately $\delta n/2$. Taking logarithms and using the [Hamming ball volume exponent](#hamming-ball-volume-exponent) gives the bound for $0\le\delta\le1$.

// Target: algebra.bigb

## Rabin cryptosystem

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rabin_cryptosystem)

Rabin encryption sends $m$ to $m^2$ modulo a product of two secret primes. Decryption computes the four square roots by the Chinese remainder theorem.

### Repeated-message attack on the Rabin cryptosystem

↑ **Parent:** [Rabin cryptosystem](#rabin-cryptosystem)

For coprime moduli $N,N'$ and $0<m<\min(N,N')$, the [Chinese remainder theorem](mathematics.md#chinese-remainder-theorem) recovers the integer $m^2$ uniquely in $[0,NN')$ from the two ciphertexts. An ordinary integer square root then recovers the message. If distinct semiprime moduli share a factor, their greatest common divisor instead reveals factors of both moduli. Learning one message in the coprime case does not by itself give a general factoring algorithm or a decryption key for other ciphertexts.

### Factorization from distinct square roots modulo a semiprime

↑ **Parent:** [Rabin cryptosystem](#rabin-cryptosystem)

If $N=pq$ and $x^2\equiv y^2\pmod N$ while $x\not\equiv\pm y\pmod N$, then

$$
N\mid(x-y)(x+y),
$$

and $\gcd(x-y,N)$ is a nontrivial factor of $N$.

#### Square-root oracle reduction for Rabin encryption

↑ **Parent:** [Factorization from distinct square roots modulo a semiprime](#factorization-from-distinct-square-roots-modulo-a-semiprime)

For $N=pq$ with distinct odd primes, choose a uniform unit $x$ and give only $x^2\bmod N$ to an oracle returning any square root $y$. Conditional on this square, $x$ is uniform among four roots and independent of the oracle's choice. With probability one half, $y$ is not $\pm x$, and $\gcd(x-y,N)$ is a nontrivial factor. Thus full inversion of the squaring map yields randomized [integer factorization](number-theory.md#integer-factorization); this reduction does not equate arbitrary partial leakage with full inversion.

#### Chosen-square attack on Rabin authentication

↑ **Parent:** [Factorization from distinct square roots modulo a semiprime](#factorization-from-distinct-square-roots-modulo-a-semiprime)

If a purported authentication service returns a square root of every chosen square modulo a Rabin modulus, a verifier who knows one root obtains a different root with substantial probability and can factor the modulus. Repeating the challenge therefore reveals the private key.

## Discrete logarithm problem

↑ **Parent:** [Coding theory](coding-theory.md)

Given a cyclic group generator $g$ and an element $h$, the discrete logarithm problem asks for an exponent $a$ such that $g^a=h$.

## Diffie-Hellman key exchange

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Diffie–Hellman_key_exchange)

Alice publishes $g^a$ and Bob publishes $g^b$ in a public cyclic group; each can then compute the shared secret $g^{ab}$. Its security relies on the difficulty of recovering the exponents or otherwise solving the computational Diffie--Hellman problem.

### Multilateral Diffie-Hellman key exchange

↑ **Parent:** [Diffie-Hellman key exchange](#diffie-hellman-key-exchange)

In a [cyclic group](group.md#cyclic-group) with generator $g$, $n$ participants with secret exponents $a_j$ can exchange $n$ tokens around a ring. Token $j$ starts at $g^{a_j}$ and is successively exponentiated by its next $n-2$ recipients before being sent to the final recipient, whose exponent is the only one missing. That recipient completes the exponentiation locally. Each token makes $n-1$ transmissions, and everyone obtains $g^{\prod_j a_j}$. Thus $n(n-1)$ transmitted group elements suffice. As with two-party [Diffie-Hellman key exchange](#diffie-hellman-key-exchange), authentication is needed.

## Unique decodability

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Unique_decodability)

Unique decodability means that every encoded message has at most one decomposition into codewords.

### Decipherable code

↑ **Parent:** [Unique decodability](#unique-decodability)

A code is decipherable, or uniquely decodable, when every finite concatenation of codewords has at most one decomposition into source codewords.

#### Suffix code

↑ **Parent:** [Decipherable code](#decipherable-code)

A [decipherable code](#decipherable-code) is suffix-free when no codeword is a proper suffix of another. Reversing all its words gives a [prefix code](#prefix-code). Consequently it is uniquely decipherable: read a concatenation from the right, where the last codeword is determined uniquely, and continue by induction.

#### Optimal source code

↑ **Parent:** [Decipherable code](#decipherable-code)

For a fixed source distribution and code alphabet, an optimal [uniquely decodable code](#decipherable-code) minimizes expected codeword length. [Huffman coding](information-theory.md#huffman-coding) gives an optimal binary [prefix code](#prefix-code), and the equivalence of attainable uniquely-decodable and prefix-code lengths gives the same minimum for both classes.

#### Prefix code

↑ **Parent:** [Decipherable code](#decipherable-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Prefix_code)

In a prefix code no codeword is the prefix of another, so concatenated messages have unique instantaneous decoding.

##### Prefix code for a rare geometric success

↑ **Parent:** [Prefix code](#prefix-code)

For a success index $J$ with [geometric distribution](discrete-probability-distribution.md#geometric-distribution) of parameter $q=2^{-n}$, write $J-1=2^nQ+R$, $0\leq R<2^n$. Encode $Q$ by $Q$ ones followed by zero, then encode $R$ in exactly $n$ [bits](information-theory.md#bit). This [prefix code](#prefix-code) has length $n+Q+1$. Since $\mathbb P(Q\geq k)=(1-q)^{k2^n}$, its expected length is the displayed expression, at most $n+e/(e-1)$. Thus a very rare success can be communicated in approximately the logarithm of its inverse [probability](probability-theory.md#probability), rather than one [bit](information-theory.md#bit) per trial.

// Target: quantum-theory.bigb

##### Prefix tree of a code

↑ **Parent:** [Prefix code](#prefix-code)

The prefix tree of a code has vertices corresponding to prefixes of codewords, with one edge for each next symbol. The root represents the empty word. In a prefix code, complete codewords are leaves, and their depths are their [codeword lengths](#codeword-length).

// Target: computer-science.bigb

<h5 id="kraft-mcmillan-inequality">Kraft–McMillan inequality</h5>

↑ **Parent:** [Prefix code](#prefix-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kraft–McMillan_inequality)

The lengths of every decipherable binary code satisfy

$$
\sum_i2^{-l_i}\leq1.
$$

Conversely, any positive integer lengths satisfying this bound can be realized by a [prefix code](#prefix-code).

###### McMillan inequality

↑ **Parent:** [Kraft–McMillan inequality](#kraft-mcmillan-inequality)

The lengths of a finite [uniquely decodable code](#decipherable-code) satisfy $\sum_a2^{-l(a)}\leq1$, even when the code is not a [prefix code](#prefix-code). Distinct concatenations of $r$ codewords remain distinct; counting the possible binary strings of each total length bounds $(\sum_a2^{-l(a)})^r$ by $r\max_a l(a)$. Taking $r$th roots proves the claim.

###### Equivalence of decipherable and prefix code lengths

↑ **Parent:** [Kraft–McMillan inequality](#kraft-mcmillan-inequality)

Prescribed positive word lengths admit a [decipherable code](#decipherable-code) if and only if they admit a [prefix code](#prefix-code). Counting length-$L$ concatenations of $m$ words proves the [Kraft inequality](#kraft-mcmillan-inequality) for any [decipherable code](#decipherable-code); choosing free vertices of the ordered $D$-ary [tree](combinatorics.md#tree-graph-theory) constructs a [prefix code](#prefix-code) whenever this inequality holds. Each [prefix code](#prefix-code) has [unique decodability](#unique-decodability).

###### Total length lower bound for a decipherable binary code

↑ **Parent:** [Kraft–McMillan inequality](#kraft-mcmillan-inequality)

If a decipherable binary code has $N$ codewords of lengths $l_1,\ldots,l_N$, then

$$
\sum_{i=1}^N l_i\geq N\log_2N.
$$

This follows by applying the entropy lower bound with the uniform source distribution.

##### Shannon-Fano coding

↑ **Parent:** [Prefix code](#prefix-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shannon–Fano_coding)

Shannon-Fano coding comprises two related [prefix code](#prefix-code) constructions. Shannon coding assigns lengths $\lceil-\log_2p_i\rceil$ to symbols of probability $p_i$; Fano coding recursively partitions the ordered symbols into groups of nearly equal total probability and assigns a bit at each partition.

##### Shannon coding

↑ **Parent:** [Prefix code](#prefix-code)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shannon_coding)

###### Cumulative Shannon code

↑ **Parent:** [Shannon coding](#shannon-coding)

Order source probabilities as $p_1\geq\cdots\geq p_N$, put

$$
b_i=\sum_{j<i}p_j,
\qquad
l_i=\lceil-\log_2p_i\rceil,
$$

and take the first $l_i$ binary digits of $b_i$ as the codeword for symbol $i$. Since $b_j-b_i\geq p_i\geq2^{-l_i}$ for $j>i$, two cumulative probabilities cannot lie in the same dyadic interval selected by the earlier codeword. The resulting code is prefix-free.

###### Competitive optimality of the Shannon code

↑ **Parent:** [Cumulative Shannon code](#cumulative-shannon-code)

If the Shannon length is $l_S(x)=\lceil\log_2(1/p_x)\rceil$ and $l_C$ is the length of any binary decipherable code, then

$$
\mathbb P\{l_S(X)\geq l_C(X)+k\}\leq2^{-k+1}.
$$

Thus the probability that the Shannon code loses to another code by $k$ or more bits decreases exponentially in $k$.

##### Entropy lower bound for prefix codes

↑ **Parent:** [Prefix code](#prefix-code)

Every binary prefix code has expected length at least its source entropy; Shannon lengths achieve expected length strictly below $H+1$.

<h6 id="shannon-s-source-coding-theorem">Shannon's source coding theorem</h6>

↑ **Parent:** [Entropy lower bound for prefix codes](#entropy-lower-bound-for-prefix-codes)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Shannon's_source_coding_theorem)

For a discrete memoryless source of entropy $H$, every uniquely decodable binary code has expected length at least $H$. Shannon code lengths satisfy $H\leq\overline\ell<H+1$, and block coding can make the expected length per source symbol arbitrarily close to $H$.

## Binary symmetric channel

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Binary_symmetric_channel)

A binary symmetric channel independently flips each transmitted bit with a fixed crossover probability $p$.  
Its channel matrix is

$$
\begin{pmatrix}1-p&p\\p&1-p\end{pmatrix}.
$$

### Undetected error

↑ **Parent:** [Binary symmetric channel](#binary-symmetric-channel)

An error is undetected by codeword-membership checking when the received word is a different valid codeword. For a linear code this occurs exactly when the nonzero channel-error vector is itself a codeword.

### Completely noisy binary symmetric channel

↑ **Parent:** [Binary symmetric channel](#binary-symmetric-channel)

At crossover probability $p=1/2$, the two rows of the [transition matrix](markov-process.md#stochastic-matrix) of a [binary symmetric channel](#binary-symmetric-channel) coincide. Its output is then [independent](random-variable.md#independent-random-variables) of its input and its [capacity](information-theory.md#binary-symmetric-channel-capacity) is zero.

### Positive-rate coding bound below one-quarter crossover

↑ **Parent:** [Binary symmetric channel](#binary-symmetric-channel)

If $p<1/4$, choose $p<\delta<1/4$. Binary codes of relative minimum distance above $2\delta$ have positive asymptotic rate by a greedy packing bound, and nearest-codeword decoding fails only when more than $\delta n$ channel errors occur. That probability tends to zero.

## Maximum a posteriori decoding

↑ **Parent:** [Coding theory](coding-theory.md)

Maximum a posteriori decoding chooses the codeword maximizing prior probability times channel likelihood and minimizes average decision error.

## Maximum-likelihood decoding

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Maximum-likelihood_decoding)

Maximum-likelihood decoding chooses the codeword under which the received word has greatest conditional probability.

## Minimum-distance decoding

↑ **Parent:** [Coding theory](coding-theory.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Minimum-distance_decoding)

Minimum-distance decoding chooses a codeword closest to the received word; on a binary symmetric channel with $p<1/2$, it is maximum-likelihood decoding under Hamming distance.

### Bounded-distance decoding

↑ **Parent:** [Minimum-distance decoding](#minimum-distance-decoding)

For a code of [minimum Hamming distance](#minimum-distance-of-a-code) $d$ and radius $t$ with $2t<d$, bounded-distance decoding returns the unique [codeword](#codeword) within [Hamming distance](#hamming-distance) $t$ of the received word, or reports failure if none exists. The disjointness of radius-$t$ [Hamming balls](#hamming-ball) gives uniqueness. It guarantees recovery when at most $t$ errors occurred, but a word produced by more errors can be nearer to a different codeword and be miscorrected.

## ↑ Ancestors (4)

1. [Algebra](algebra.md)
2. [Area of mathematics](mathematics.md#area-of-mathematics)
3. [Mathematics](mathematics.md)
4. [Codex Wiki](README.md)
