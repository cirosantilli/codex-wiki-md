# Finite partitions measurable in a partition tail have zero entropy rate

↑ **Parent:** [Tail sigma-algebra of a measurable partition](tail-sigma-algebra-of-a-measurable-partition.md)

Let $\alpha$ be finite and measurable in $\mathcal T(\xi)$ for a finite [measurable partition](measurable-partition.md) $\xi$, and put $h=h_\mu(T,\xi)$. Choose $r$ with $H(\alpha\mid\xi_0^r)<\varepsilon$. For $\gamma=\alpha_0^{n-1}$ and $\beta=\xi_0^{n+r-1}$, conditional subadditivity gives $H(\gamma\mid\beta)<n\varepsilon$. Tail measurability and [block conditional entropy given the infinite future](block-conditional-entropy-given-the-infinite-future.md) give $H(\beta\mid\gamma)\ge(n+r)h$. Thus $H(\gamma)\le H(\beta)-(n+r)h+n\varepsilon$. Divide by $n$, then let $n\to\infty$ and $\varepsilon\downarrow0$, proving $h_\mu(T,\alpha)=0$. The proof also works for noninvertible transformations.

## ↑ Ancestors (9)

1. [Tail sigma-algebra of a measurable partition](tail-sigma-algebra-of-a-measurable-partition.md)
2. [K-mixing](k-mixing.md)
3. [Ergodic theory](ergodic-theory.md)
4. [Measure theory](measure-theory-split.md)
5. [Real analysis](real-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Completely positive entropy](completely-positive-entropy.md)
