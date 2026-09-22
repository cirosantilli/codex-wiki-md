# Discrete memoryless channel

↑ **Parent:** [Coding theory](coding-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Discrete_memoryless_channel)

A [discrete memoryless channel](discrete-memoryless-channel.md) models transmission through finite input and output [alphabets](alphabet.md) using fixed [conditional probabilities](conditional-probability.md) $W(y\mid x)$. For each input $x$, these nonnegative numbers sum to one over the output symbols. Discrete refers to the symbols, and memoryless means that the noise of one use does not remember earlier uses.

For a fixed input word $x^n=(x_1,\ldots,x_n)$ sent without feedback, the output law is

$$
W^n(y^n\mid x^n)=\prod_{j=1}^nW(y_j\mid x_j).
$$

This is conditional independence of the outputs given the prescribed input word. It does not require an [encoder](channel-encoder.md) to choose [independent](independent-random-variables.md) input symbols: the [codewords](codeword.md) of a [block code](block-code.md) deliberately impose relationships among them. Those relationships let a [decoder](channel-decoder.md) distinguish possible messages after noise.

The [binary symmetric channel](binary-symmetric-channel.md) and [binary erasure channel](binary-erasure-channel.md) make two different memoryless noise models with a binary input. One hides flipped [bits](bit.md); the other marks missing [bits](bit.md). Their different [channel capacities](channel-capacity.md) show why the whole [transition matrix](stochastic-matrix.md) matters, as the [flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md) demonstrate.

**Table of contents**

- [Three-input two-point additive-noise channel](three-input-two-point-additive-noise-channel.md)
- [Channel encoder](channel-encoder.md)
- [Channel decoder](channel-decoder.md)
  - [Maximal decoding error probability](maximal-decoding-error-probability.md)
- [Finite-alphabet erasure channel](finite-alphabet-erasure-channel.md)
  - [Capacity of a finite-alphabet erasure channel](capacity-of-a-finite-alphabet-erasure-channel.md)
- [Binary erasure channel](binary-erasure-channel.md)
  - [Repeat-until-success coding over an erasure channel](repeat-until-success-coding-over-an-erasure-channel.md)
  - [Erasure-pattern counting bound for maximal decoding error](erasure-pattern-counting-bound-for-maximal-decoding-error.md)
- [Z-channel](z-channel.md)

## ↑ Ancestors (5)

1. [Coding theory](coding-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (27)

- [Binary symmetric channel](binary-symmetric-channel.md)
- [Capacity after independent output erasure](capacity-after-independent-output-erasure.md)
- [Capacity of a disjoint sum of channels](capacity-of-a-disjoint-sum-of-channels.md)
- [Channel capacity](channel-capacity.md)
- [Channel coding](channel-coding.md)
- [Communication channel](communication-channel.md)
- [Concavity of mutual information in the input distribution](concavity-of-mutual-information-in-the-input-distribution.md)
- [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
- [Discrete memoryless channel](discrete-memoryless-channel.md)
- [Equality in capacity data processing](equality-in-capacity-data-processing.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2008/2/c/i/solution.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2008/3/c/solution.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2009/3/a/solution.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2010/3/a/solution.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2011/3/a/ii/solution.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/3/a/solution.md)
- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2021/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/3k/solution.md)
- [Removing a redundant input symbol from a channel](removing-a-redundant-input-symbol-from-a-channel.md)
- [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
