# Asymptotic equipartition property

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Asymptotic_equipartition_property)

The [asymptotic equipartition property](asymptotic-equipartition-property.md) explains why a long message from a source can usually be described using its [information entropy](information-entropy-split.md) per symbol. Individual messages can have very different [probabilities](probability.md), but the messages carrying almost all the total [probability](probability.md) have similar logarithmic costs per symbol. The [Bernoulli typical-set example](bernoulli-typical-set-example.md) makes the distinction between an individual message and a large collection explicit.

For [independent and identically distributed random variables](independent-and-identically-distributed-random-variables.md) $X_1,X_2,\ldots$ on a [finite alphabet](finite-alphabet.md), let $p$ be their [probability mass function](probability-mass-function.md) and $H=\mathbb E[-\log_2p(X_1)]$. Then

$$
\boxed{-\frac1n\log_2P(X_1,\ldots,X_n)\longrightarrow H\quad\text{almost surely}.}
$$

Here $P(X_1,\ldots,X_n)$ means the [probability mass](probability-mass.md) of the realized word, evaluated under the source law. The product rule for [independent random variables](independent-random-variables.md) turns its [information content](information-content.md) into a sum:

$$
-\frac1n\log_2P(X_1,\ldots,X_n)
=\frac1n\sum_{j=1}^n[-\log_2p(X_j)].
$$

The [strong law of large numbers](strong-law-of-large-numbers.md) gives the limit. Zero-probability symbols do not occur; on the positive-probability support of a [finite alphabet](finite-alphabet.md), these information costs are finite. The corresponding [typical set](typical-set.md) consists of words whose cost per symbol is within a chosen tolerance of $H$.

For a [strictly stationary process](strictly-stationary-process.md) with a [finite alphabet](finite-alphabet.md), the constant-limit extension requires [ergodicity](ergodicity.md). The [Shannon-McMillan-Breiman theorem](shannon-mcmillan-breiman-theorem.md) then replaces the one-symbol [information entropy](information-entropy-split.md) with the [information rate](entropy-rate.md). [Stationarity without ergodicity in an information source](stationarity-without-ergodicity-in-an-information-source.md) shows why stationarity alone is insufficient.[§8, Theorem 8.1 and Corollary 8.2, printed p. 90: stationary ergodic sources and typical sets](6-441-information-theory-spring-2016-lecture-notes-by-yury-polyanskiy-and-others.md)

**Table of contents**

- [Bernoulli typical-set example](bernoulli-typical-set-example.md)
  - [Typical-set concentration for a biased coin](typical-set-concentration-for-a-biased-coin.md)
  - [Typical-set indexing example](typical-set-indexing-example.md)
- [Stationarity without ergodicity in an information source](stationarity-without-ergodicity-in-an-information-source.md)
- [Shannon's typical-message formulation](shannon-s-typical-message-formulation.md)
- [Typical set](typical-set.md)
  - [Typical sequence theorem](typical-sequence-theorem.md)
  - [Weakly typical sequence](weakly-typical-sequence.md)
  - [Typical-set cardinality bounds](typical-set-cardinality-bounds.md)
    - [Minimal high-probability source-set exponent](minimal-high-probability-source-set-exponent.md)
- [Strongly typical sequence](strongly-typical-sequence.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Asymptotic equipartition property](asymptotic-equipartition-property.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-31/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/ii/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/ii/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-224/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-2/3h/d/solution.md)
- [Typical-set cardinality bounds](typical-set-cardinality-bounds.md)
