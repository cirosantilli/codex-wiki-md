# Channel capacity

↑ **Parent:** [Information theory](information-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Channel_capacity)

[Channel capacity](channel-capacity.md) is the best reliable information rate available through a specified [communication channel](communication-channel.md). For a [discrete memoryless channel](discrete-memoryless-channel.md) with finite input and output [alphabets](alphabet.md), fixed [transition probabilities](transition-probability.md) $W(y\mid x)$, and no input-cost constraint, it is

$$
C=\max_{P_X}I(X;Y)
$$

in [bits](bit.md) per channel use, when the [mutual information](mutual-information.md) uses base-two [logarithms](logarithm.md). The maximization varies the input [probability distribution](probability-distribution.md), while keeping the [communication channel](communication-channel.md) fixed. A large input [alphabet](alphabet.md) or a large output [information entropy](information-entropy.md) alone does not determine how much information gets through: the receiver needs information about the input, rather than merely unpredictable output.

The operational meaning comes from the [Shannon second coding theorem](noisy-channel-coding-theorem.md). A [block code](block-code.md) represents one of $M$ possible messages by a word of length $n$, giving a rate $\log_2 M/n$ [bits](bit.md) per use. Take the message label from the [uniform distribution on a finite set](discrete-uniform-distribution.md) of those $M$ choices when measuring average decoding-error [probability](probability.md). For every fixed rate $R<C$, there are sequences of such [block codes](block-code.md) whose decoding-error [probability](probability.md) tends to zero as $n$ grows; a rate above $C$ cannot have vanishing decoding-error [probability](probability.md). This is an asymptotic limit, rather than a promise that an arbitrary finite [block code](block-code.md) at a rate below $C$ works well. See [MIT 18.310, Shannon's Noisy Coding Theorem, sections 1–2](https://ocw.mit.edu/courses/18-310-principles-of-discrete-applied-mathematics-fall-2013/12c7d786302979771e10a8fd31e07405_MIT18_310F13_Ch21.pdf).

For a [binary symmetric channel](binary-symmetric-channel.md) with crossover [probability](probability.md) $p=0.1$, the [binary symmetric channel capacity](binary-symmetric-channel-capacity.md) is approximately $0.53100441$ [bits](bit.md) per use. Thus a binary [code rate](code-rate.md) $R=1/2$ lies below the limit, while $R=3/4$ lies above it. At $R=1/2$, two transmitted symbols represent one message [bit](bit.md) on average; the redundancy helps distinguish messages after noise. This does not split individual physical symbols into fractional pieces.

The result is useful because it separates two tasks. Computing [channel capacity](channel-capacity.md) establishes the target imposed by the [transition probabilities](transition-probability.md); constructing an effective [block code](block-code.md) attempts to approach that target with acceptable delay and decoding effort. The surprise is that reliability can improve indefinitely without forcing every positive rate to disappear. In his 1948 paper, Shannon defines noisy [channel capacity](channel-capacity.md) in section 12 and develops its operational significance in section 13, Theorem 11. His original formulation uses information per unit time; the fixed-duration channel-use convention here expresses the same rate question per symbol. [A Mathematical Theory of Communication by Claude Shannon](a-mathematical-theory-of-communication-by-claude-shannon.md).

**Table of contents**

- [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
  - [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
  - [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
    - [Input distribution optimization for a binary symmetric channel](input-distribution-optimization-for-a-binary-symmetric-channel.md)
    - [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)
  - [Ternary symmetric channel capacity](ternary-symmetric-channel-capacity.md)

## ↑ Ancestors (5)

1. [Information theory](information-theory-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Binary erasure channel](binary-erasure-channel.md)
- [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
- [Capacity of a finite-alphabet erasure channel](capacity-of-a-finite-alphabet-erasure-channel.md)
- [Channel capacity](channel-capacity.md)
- [Channel coding](channel-coding.md)
- [Communication channel](communication-channel.md)
- [Cyclic ternary channel capacity](cyclic-ternary-channel-capacity.md)
- [Discrete memoryless channel](discrete-memoryless-channel.md)
- [Flips versus erasures in a binary channel](flips-versus-erasures-in-a-binary-channel.md)
- [Information theory](information-theory-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-35/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-4/4j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/4g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-30/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-1/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/i/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-2/11g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/3g/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-2/3i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/11i/a/solution.md)
