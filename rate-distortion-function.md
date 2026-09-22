# Rate-distortion function

↑ **Parent:** [Rate-distortion theory](rate-distortion-theory.md)

Fix a finite source [alphabet](alphabet.md) $\mathcal X$, a [probability mass function](probability-mass-function.md) $p_X$, a finite [reconstruction alphabet](reconstruction-alphabet.md) $\widehat{\mathcal X}$, and a nonnegative [distortion measure](distortion-measure-information-theory.md) $d(x,\hat x)$. The information rate-distortion function is

$$
R(D)=\inf_{p_{\widehat X\mid X}:\,\mathbb E[d(X,\widehat X)]\leq D} I(X;\widehat X).
$$

The source [probability distribution](probability-distribution-split.md) stays fixed; the [conditional distribution](conditional-distribution.md) of the reconstruction is what we optimize. Each feasible [test channel](test-channel-information-theory.md) must keep [expected distortion](expected-distortion.md) at most $D$. The objective is [mutual information](mutual-information.md), measured in [bits](bit.md) when the [logarithms](logarithm.md) have base two. If no [test channel](test-channel-information-theory.md) satisfies the constraint, the [infimum](infimum.md) is $+\infty$.[§23.2, Theorem 23.2, printed p. 243](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others/chapter-23-rate-distortion-theory.md)

Consider [independent and identically distributed](independent-and-identically-distributed-random-variables.md) fair [bits](bit.md) and [Hamming distortion](hamming-distortion.md), which charges one for an incorrect [bit](bit.md). At zero [expected distortion](expected-distortion.md), every [bit](bit.md) must be reconstructed correctly, and $R(0)=1$. If an average fraction $D=1/4$ of incorrect [bits](bit.md) is allowed, the [binary rate-distortion function](binary-rate-distortion-function.md) gives

$$
\boxed{R(1/4)=1-h_2(1/4)\approx0.18872\text{ bits per source symbol}.}
$$

Here $h_2$ is [binary entropy](binary-entropy.md). This is an asymptotic limit for long [block codes](block-code.md), rather than a claim that a single [bit](bit.md) can be stored in $0.18872$ physical [bits](bit.md). The [three-bit lossy Hamming code](three-bit-lossy-hamming-code.md) gives a small, fully explicit version of the same tradeoff, with rate $1/3$ and [expected distortion](expected-distortion.md) $1/4$.

<a id="image-allowing-more-incorrect-fair-bits-lowers-the-asymptotic-information-rate"></a>
![](binary-rate-distortion-information-bound.png)

**[Figure 17](#image-allowing-more-incorrect-fair-bits-lowers-the-asymptotic-information-rate). Allowing more incorrect fair bits lowers the asymptotic information rate**. The curve is the exact [binary rate-distortion function](binary-rate-distortion-function.md). The marked three-symbol code has rate $1/3$ at [expected distortion](expected-distortion.md) $1/4$; its gap above the curve shows that a small explicit [block code](block-code.md) need not attain the asymptotic bound. Rates count [bits](bit.md) per original source symbol.

[Rate-distortion theory](rate-distortion-theory.md) separates the question of what is possible from the design of a practical [encoder](channel-encoder.md) and [decoder](channel-decoder.md). It also forces the fidelity criterion to be explicit. [Hamming distortion](hamming-distortion.md) treats all symbol mismatches alike; [mean squared error](mean-squared-error.md) instead penalizes larger numerical errors more strongly. Those objectives can favor different reconstructions of the same data. An average error criterion does not by itself control the error on every individual input.

[Claude Shannon](claude-shannon.md)'s [Coding Theorems for a Discrete Source With a Fidelity Criterion by Claude Shannon](coding-theorems-for-a-discrete-source-with-a-fidelity-criterion-by-claude-shannon.md) was published in 1959. Its formulation fixes a cost for replacing one source letter by another and studies the communication rate compatible with the allowed average cost. The important shift is to quantify which distinctions may be discarded, rather than requiring exact recovery of every letter.[Coding Theorems for a Discrete Source With a Fidelity Criterion by Claude Shannon](coding-theorems-for-a-discrete-source-with-a-fidelity-criterion-by-claude-shannon.md)

**Table of contents**

- [Distortion measure (information theory)](distortion-measure-information-theory.md)
  - [Reconstruction alphabet](reconstruction-alphabet.md)
  - [Expected distortion](expected-distortion.md)
  - [Separable distortion](separable-distortion.md)
- [Test channel (information theory)](test-channel-information-theory.md)
- [Hamming distortion](hamming-distortion.md)
  - [Three-bit lossy Hamming code](three-bit-lossy-hamming-code.md)
  - [Binary rate-distortion function](binary-rate-distortion-function.md)
- [Fixed-length lossy code](fixed-length-lossy-code.md)
- [Shannon's rate-distortion theorem](shannon-s-rate-distortion-theorem.md)
- [Zero-rate distortion threshold](zero-rate-distortion-threshold.md)

## ↑ Ancestors (6)

1. [Rate-distortion theory](rate-distortion-theory.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-224/3/c/solution.md)
- [Rate-distortion theory](rate-distortion-theory.md)
- [Shannon's rate-distortion theorem](shannon-s-rate-distortion-theorem.md)
