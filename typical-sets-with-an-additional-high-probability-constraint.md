# Typical sets with an additional high-probability constraint

↑ **Parent:** [Typical set](typical-set.md)

Let $A^{n,\varepsilon}$ be the weak [typical set](typical-set.md) of a [finite alphabet](finite-alphabet.md) [independent and identically distributed](independent-and-identically-distributed-random-variables.md) source with [Shannon entropy](information-entropy-split.md) $H$, and let $B_n$ be any sets with $\Pr(X^n\in B_n)\to1$. The [asymptotic equipartition property](asymptotic-equipartition-property.md) and [union bound](boole-s-inequality.md) give $\Pr(X^n\in A^{n,\varepsilon}\cap B_n)\to1$. Every word in the intersection has [probability mass](probability-mass.md) between $2^{-n(H+\varepsilon)}$ and $2^{-n(H-\varepsilon)}$. Summing these bounds gives

$$
\Pr(X^n\in A^{n,\varepsilon}\cap B_n)\,2^{n(H-\varepsilon)}
\leq|A^{n,\varepsilon}\cap B_n|\leq2^{n(H+\varepsilon)}.
$$

For every fixed $\delta>0$, the first [probability](probability.md) eventually exceeds $2^{-\delta}$, proving the title bound. A [sample mean](sample-mean.md) within a fixed positive tolerance of the [expected value](expected-value-split.md) supplies $B_n$ by the [strong law of large numbers](strong-law-of-large-numbers.md).

## ↑ Ancestors (7)

1. [Typical set](typical-set.md)
2. [Asymptotic equipartition property](asymptotic-equipartition-property.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-information-theory-course-of-the-university-of-oxford/2023/2/c/ii/solution.md)
