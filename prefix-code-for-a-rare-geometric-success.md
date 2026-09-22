# Prefix code for a rare geometric success

↑ **Parent:** [Prefix code](prefix-code.md)

For a success index $J$ with [geometric distribution](geometric-distribution.md) of parameter $q=2^{-n}$, write $J-1=2^nQ+R$, $0\leq R<2^n$. Encode $Q$ by $Q$ ones followed by zero, then encode $R$ in exactly $n$ [bits](bit.md). This [prefix code](prefix-code.md) has length $n+Q+1$. Since $\mathbb P(Q\geq k)=(1-q)^{k2^n}$, its expected length is the displayed expression, at most $n+e/(e-1)$. Thus a very rare success can be communicated in approximately the logarithm of its inverse [probability](probability.md), rather than one [bit](bit.md) per trial.

// Target: quantum-theory.bigb

## ↑ Ancestors (8)

1. [Prefix code](prefix-code.md)
2. [Decipherable code](decipherable-code.md)
3. [Unique decodability](unique-decodability.md)
4. [Coding theory](coding-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Asymptotic remote state preparation by block indexing](asymptotic-remote-state-preparation-by-block-indexing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59/2/solution.md)
