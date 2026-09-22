# Parity constraint and total correlation

↑ **Parent:** [Total correlation](total-correlation.md)

Let $X,Y$ be [independent](independent-random-variables.md) fair [bits](bit.md) and set $Z=X\mathbin\oplus Y$, their [exclusive or](exclusive-or.md). The four possible triples are $000,011,101,110$, each with [probability](probability.md) $1/4$. Every coordinate is fair, and every pair has all four outcomes with equal [probability](probability.md). Thus each pair's [mutual information](mutual-information.md) is zero, as in [pairwise independence does not imply joint independence](pairwise-independence-does-not-imply-joint-independence.md).

The full [random vector](random-vector.md) has [joint entropy](joint-entropy.md) $\log_2 4=2$ [bits](bit.md), while the marginal [information entropies](information-entropy.md) sum to three [bits](bit.md). Consequently

$$
\boxed{\operatorname{TC}(X,Y,Z)=3-2=1\text{ bit}.}
$$

The product of the marginals predicts [probability](probability.md) $1/8$ for every triple, including the four impossible ones. On each possible triple, the ratio of true to product [probability](probability.md) is $(1/4)/(1/8)=2$; averaging its base-two [logarithm](logarithm.md) gives the same one [bit](bit.md) of [relative entropy](kullback-leibler-divergence.md).

The example gives a concrete use for joint information measures. A [lossless source coding](lossless-source-coding.md) scheme that treats the three coordinates separately needs three [bits](bit.md) here. If the [decoder](channel-decoder.md) knows the [integer parity](parity-mathematics.md) rule, the [encoder](channel-encoder.md) can send just $X,Y$ and let the [decoder](channel-decoder.md) reconstruct $Z$ exactly. Pairwise [independence](independent-random-variables.md) does not reveal that saving. This is a stipulated source law and an explicit two-[bit](bit.md) code, rather than a promise that arbitrary data can be shortened.

**Table of contents**

- [Noisy parity total correlation](noisy-parity-total-correlation.md)

## ↑ Ancestors (6)

1. [Total correlation](total-correlation.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Chain decomposition of total correlation](chain-decomposition-of-total-correlation.md)
