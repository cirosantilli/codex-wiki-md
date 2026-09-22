# Entropy bound for a random-length binary string

↑ **Parent:** [Information entropy](information-entropy-split.md)

For a random finite binary string $M$ of length $L$, conditioning on $L=\ell$ leaves at most $2^\ell$ possible strings. Thus its [conditional entropy](conditional-entropy.md) is at most $\ell$. Since the length is a function of the string, the [chain rule for information entropy](chain-rule-for-information-entropy.md) gives

$$
H(M)=H(L)+H(M\mid L)\le H(L)+\mathbb EL.
$$

The term $H(L)$ cannot generally be removed. For concatenations of $m$ words from a fixed finite [decipherable code](decipherable-code.md) with maximum length $d$, it is at most $\log_2(md+1)$. [Decipherability](decipherable-code.md) preserves the [Shannon entropy](information-entropy-split.md) of the source block. For an independent source block, dividing the resulting inequality by $m$ and taking $m\to\infty$ proves the [expected codeword length](expected-codeword-length.md) is at least the one-symbol [Shannon entropy](information-entropy-split.md).

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
