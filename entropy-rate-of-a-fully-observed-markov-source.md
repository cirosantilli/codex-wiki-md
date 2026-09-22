# Entropy rate of a fully observed Markov source

↑ **Parent:** [Fully observed Markov source](fully-observed-markov-source.md)

For a [fully observed Markov source](fully-observed-markov-source.md), the [Markov property](markov-property.md) makes the last state sufficient for the next symbol's [conditional distribution](conditional-distribution.md). With [stationary distribution](stationary-distribution.md) $\pi$, the [conditional entropy](conditional-entropy.md) is therefore

$$
h=H(X_2\mid X_1)=-\sum_i\pi_i\sum_jP_{ij}\log_2P_{ij},
$$

using $0\log_2 0=0$. The [chain rule for information entropy](chain-rule-for-information-entropy.md) gives the exact finite-block identity

$$
H(X_1,\ldots,X_n)=H(\pi)+(n-1)h.
$$

Dividing by $n$ proves the displayed [entropy rate](entropy-rate.md). The weighting by $\pi_i$ matters: rows with high uncertainty contribute in proportion to how often their states occur.

For an original asymmetric example, take

$$
P=\begin{pmatrix}7/8&1/8\\3/8&5/8\end{pmatrix},\qquad \pi=(3/4,1/4).
$$

The equality $\pi P=\pi$ verifies the [stationary distribution](stationary-distribution.md). The single-symbol [information entropy](information-entropy.md) is $h_2(1/4)\simeq0.81127812$, whereas

$$
\boxed{h=\frac34h_2(1/8)+\frac14h_2(3/8)\simeq0.64628183\ \text{bits per symbol}.}
$$

This formula describes observed states. If several states emit the same symbol, calculating the output [entropy rate](entropy-rate.md) requires accounting for the hidden-state uncertainty; it is not generally the same row average.

## ↑ Ancestors (7)

1. [Fully observed Markov source](fully-observed-markov-source.md)
2. [Markov information source](markov-information-source.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Fully observed Markov source](fully-observed-markov-source.md)
