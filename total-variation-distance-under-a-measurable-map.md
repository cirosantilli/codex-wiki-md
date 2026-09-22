# Total variation distance under a measurable map

↑ **Parent:** [Total variation distance](total-variation-distance.md)

Applying the same [measurable function](measurable-function.md) $f$ to observations from two [probability distributions](probability-distribution.md) cannot increase their [total variation distance](total-variation-distance.md). Every output [event](event.md) $B$ is tested through its [preimage](preimage.md) $f^{-1}(B)$, which was already one of the input [events](event.md). Therefore

$$
d_{\mathrm{TV}}(P\circ f^{-1},Q\circ f^{-1})\leq d_{\mathrm{TV}}(P,Q).
$$

For the four-outcome example, recording only whether the result is $D$ makes the output [probability distributions](probability-distribution.md) identical: each is a [Bernoulli distribution](bernoulli-distribution.md) with parameter $0.3$. The original [total variation distance](total-variation-distance.md) was $0.3$, but this coarse measurement leaves zero discrepancy. Discarding information can make two sources less distinguishable.

The same contraction holds for a common [Markov kernel](markov-kernel.md) $K$: $d_{\mathrm{TV}}(PK,QK)\leq d_{\mathrm{TV}}(P,Q)$. On a [finite set](finite-set.md), expand $PK-QK$, apply the [triangle inequality](triangle-inequality.md) to each output component, and use that each row of $K$ sums to one. A common randomized postprocessing step cannot increase distinguishability either.

## ↑ Ancestors (5)

1. [Total variation distance](total-variation-distance.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)
