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

- [Channel encoder](channel-encoder.md)
- [Channel decoder](channel-decoder.md)
- [Finite-alphabet erasure channel](finite-alphabet-erasure-channel.md)
  - [Capacity of a finite-alphabet erasure channel](capacity-of-a-finite-alphabet-erasure-channel.md)
- [Binary erasure channel](binary-erasure-channel.md)
- [Z-channel](z-channel.md)

## ↑ Ancestors (5)

1. [Coding theory](coding-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Binary symmetric channel](binary-symmetric-channel.md)
- [Channel capacity](channel-capacity.md)
- [Channel coding](channel-coding.md)
- [Communication channel](communication-channel.md)
- [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
- [Discrete memoryless channel](discrete-memoryless-channel.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-2/3k/solution.md)
- [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
