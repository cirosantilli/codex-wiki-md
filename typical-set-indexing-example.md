# Typical-set indexing example

↑ **Parent:** [Bernoulli typical-set example](bernoulli-typical-set-example.md)

The [typical sequence theorem](typical-sequence-theorem.md) turns a probability concentration into a coding construction. Assign one [binary number](binary-number.md) index to each [weakly typical sequence](weakly-typical-sequence.md), plus a reserved index for every word outside the set. The [decoder](channel-decoder.md) recovers every typical word exactly; the reserved index has one predetermined output. The [block code](block-code.md) uses

$$
L_n=\left\lceil\log_2(|T_\varepsilon^{(n)}|+1)\right\rceil
$$

[bits](bit.md) and has reconstruction-error [probability](probability.md) at most $1-P(T_\varepsilon^{(n)})$.

For this example and $\varepsilon=0.1$, $n=40$ needs 34 [bits](bit.md) but permits error up to about $0.3611$. At $n=640$, 570 [bits](bit.md) suffice and the error bound is about $0.0002215$. These are existence calculations for an explicitly enumerated collection, rather than claims about an efficient practical [encoder](channel-encoder.md). The reduction comes from protecting the whole high-probability collection, rather than just its single most likely member.

## ↑ Ancestors (7)

1. [Bernoulli typical-set example](bernoulli-typical-set-example.md)
2. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
