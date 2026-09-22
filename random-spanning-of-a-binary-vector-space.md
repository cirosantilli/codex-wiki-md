# Random spanning of a binary vector space

↑ **Parent:** [Linear independence](linear-independence.md)

Take independent uniform samples from a $d$-dimensional [vector space](vector-space-split.md) over the two-element [field](field.md). At current [matrix rank](matrix-rank.md) $r$, the existing span contains $2^r$ of the $2^d$ possible vectors, so a new sample increases the [matrix rank](matrix-rank.md) with [probability](probability.md) $1-2^{r-d}$. The mean waiting time for that increase is $1/(1-2^{r-d})$ by the [geometric distribution](geometric-distribution.md). Adding the waiting times gives $\mathbb E M=d+\sum_{j=1}^d(2^j-1)^{-1}<d+2$. For $d\geq1$, the bound follows by separating $j=1$ and using $(2^j-1)^{-1}<2^{1-j}$ for $j\geq2$; for $d=0$, no samples are needed.

After $m=d+t$ samples, failure to span implies that some nonzero [linear functional](linear-functional.md) vanishes on all samples. Each fixed nonzero functional does so with [probability](probability.md) $2^{-m}$; the [union bound](boole-s-inequality.md) over the $2^d-1$ possibilities gives failure less than $2^{-t}$. This provides both an expected sample count and a fixed-budget high-success version of [Simon's algorithm](simon-s-algorithm.md).

## ↑ Ancestors (7)

1. [Linear independence](linear-independence.md)
2. [Vector space](vector-space-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-introduction-to-quantum-information-course-of-the-university-of-oxford/2015/1/e/solution.md)
- [Simon's algorithm](simon-s-algorithm.md)
