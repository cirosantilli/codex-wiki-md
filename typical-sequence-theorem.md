# Typical sequence theorem

↑ **Parent:** [Typical set](typical-set.md)

For a [memoryless classical information source](memoryless-classical-information-source.md), the [typical set](typical-set.md) consists of positive-probability words with $|-(1/n)\log_2p(u^n)-H(U)|\leq\varepsilon$. The [weak law of large numbers](weak-law-of-large-numbers.md) applied to $-\log_2p(U_j)$ proves its probability tends to one. Every typical word has probability between $2^{-n(H+\varepsilon)}$ and $2^{-n(H-\varepsilon)}$. Summing the lower bound gives the displayed cardinality upper bound; if the set has probability at least $1-\delta$, summing the upper bound gives cardinality at least $(1-\delta)2^{n(H-\varepsilon)}$.

To compress at any rate $R>H(U)$, choose $0<\varepsilon<R-H(U)$, assign one fixed-length binary index to each typical word, and reserve one additional index for all atypical words. At most $\lceil nR\rceil$ bits suffice for all large $n$. Decoding inverts the typical-word indices and makes an arbitrary output for the reserved index. The reconstruction error is at most the probability of the atypical set and tends to zero.

## ↑ Ancestors (7)

1. [Typical set](typical-set.md)
2. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Memoryless classical information source](memoryless-classical-information-source.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-60/1/solution.md)
