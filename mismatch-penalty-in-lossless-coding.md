# Mismatch penalty in lossless coding

↑ **Parent:** [Cross-entropy](cross-entropy.md)

Suppose a binary [prefix code](prefix-code.md) has integer [codeword lengths](codeword-length.md) $\ell_i=-\log_2 q_i$. Under a source with [probability mass function](probability-mass-function.md) $p_i$, its average [codeword length](codeword-length.md) is exactly [cross-entropy](cross-entropy.md), $\sum_i p_i\ell_i=H(P,Q)$. The [Kraft inequality](kraft-mcmillan-inequality.md) is satisfied because $\sum_i2^{-\ell_i}=\sum_iq_i=1$. This exact interpretation requires suitable [dyadic rational](dyadic-rational.md) [probabilities](probability.md); a general $-\log_2q_i$ is not an integer [codeword length](codeword-length.md). For positive $q_i$, a [prefix code](prefix-code.md) with lengths $\lceil-\log_2q_i\rceil$ exists by the [Kraft inequality](kraft-mcmillan-inequality.md) and has average length between $H(P,Q)$ and $H(P,Q)+1$. The [ceiling function](ceiling-function.md) causes the one-symbol rounding overhead. The cross-entropy term describes mismatch overhead; those are distinct costs.

## ↑ Ancestors (7)

1. [Cross-entropy](cross-entropy.md)
2. [Information entropy](information-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Cross-entropy](cross-entropy.md)
