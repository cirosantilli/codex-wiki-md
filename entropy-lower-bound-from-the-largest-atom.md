# Entropy lower bound from the largest atom

↑ **Parent:** [Information entropy](information-entropy-split.md)

For a finite [probability distribution](probability-distribution-split.md) with largest atom $\Pi$, its base-two [Shannon entropy](information-entropy-split.md) satisfies $H\geq2(1-\Pi)$. If $\Pi\geq1/2$, coarsen the distribution to the indicator of a largest atom: [Shannon entropy](information-entropy-split.md) cannot increase under a deterministic function, so $H\geq h_2(\Pi)$. The [concavity](concavity-of-information-entropy.md) of [binary entropy](binary-entropy.md) places it above the chord from $(1/2,1)$ to $(1,0)$, giving $h_2(\Pi)\geq2(1-\Pi)$. If $\Pi\leq1/2$, every nonzero probability $p$ has $-\log_2p\geq-\log_2\Pi$, so $H\geq-\log_2\Pi$. The function $-\log_2\Pi-2(1-\Pi)$ vanishes at $1/2$ and has negative derivative on $(0,1/2]$, proving the same bound. Equality in the combined bound occurs for a point mass or a distribution uniform on two points.

## ↑ Ancestors (6)

1. [Information entropy](information-entropy-split.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conditional entropy upper bound on minimum decoding error](conditional-entropy-upper-bound-on-minimum-decoding-error.md)
- [Solution](past-exam-of-the-communication-theory-course-of-the-university-of-oxford/2010/2/b/ii/solution.md)
