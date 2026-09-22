# Flips versus erasures in a binary channel

↑ **Parent:** [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)

A [binary erasure channel](binary-erasure-channel.md) marks its failed transmissions with a special output symbol, whereas a [binary symmetric channel](binary-symmetric-channel.md) changes a [bit](bit.md) without announcing whether it changed. At the same nominal failure [probability](probability.md) $p=0.1$, the two [communication channels](communication-channel.md) therefore leave different uncertainty. With a fair input, an unerased output determines the input exactly, while the erasure flag leaves one [bit](bit.md) of [conditional entropy](conditional-entropy.md). Thus $H(X\mid Y)=p$ and $I(X;Y)=1-p=0.9$ for the [binary erasure channel](binary-erasure-channel.md). This is the binary case of [capacity of a finite-alphabet erasure channel](capacity-of-a-finite-alphabet-erasure-channel.md).

For the [binary symmetric channel](binary-symmetric-channel.md) at $p=0.1$, neither possible received symbol rules out either input, and $H(X\mid Y)=h_2(0.1)\approx0.46899559$. Its [channel capacity](channel-capacity.md) is only $1-h_2(0.1)\approx0.53100441$. A receiver benefits from knowing _where_ information was lost, even when the fraction of affected transmissions is the same.

<a id="image-announced-erasures-preserve-more-information-than-hidden-bit-flips-at-the-same-low-failure-probability"></a>
![](binary-channel-errors-versus-erasures.png)

**[Figure 20](#image-announced-erasures-preserve-more-information-than-hidden-bit-flips-at-the-same-low-failure-probability). Announced erasures preserve more information than hidden bit flips at the same low failure probability**. Solid arrows carry [probability](probability.md) $0.9$ and dashed arrows carry [probability](probability.md) $0.1$ in the two illustrated laws of [transition probabilities](transition-probability.md). The erasure flag is distinct from both [bits](bit.md). The lower plot compares [channel capacity](channel-capacity.md) for $0\leq p\leq1/2$, using $1-p$ for the [binary erasure channel](binary-erasure-channel.md) and $1-h_2(p)$ for the [binary symmetric channel](binary-symmetric-channel.md).

This comparison concerns the specified [transition probabilities](transition-probability.md), rather than a general ordering of every error mechanism. In particular, at $p=1$, an erasure flag conveys no input information, while deterministic inversion still conveys a full [bit](bit.md). Reporting only an error percentage loses the distinction between hidden corruption, announced loss, and a predictable reversible transformation.

## ↑ Ancestors (8)

1. [Binary symmetric channel capacity](binary-symmetric-channel-capacity.md)
2. [Weakly symmetric channel capacity](weakly-symmetric-channel-capacity.md)
3. [Channel capacity](channel-capacity.md)
4. [Information theory](information-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Discrete memoryless channel](discrete-memoryless-channel.md)
