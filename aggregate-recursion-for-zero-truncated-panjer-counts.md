# Aggregate recursion for zero-truncated Panjer counts

↑ **Parent:** [Zero-truncated claim-count distribution](zero-truncated-claim-count-distribution.md)

Let $N\ge1$ have [probability mass function](probability-mass-function.md) $p_n$ satisfying $p_n=(a+b/n)p_{n-1}$ for $n\ge2$. Let independent positive integer claim sizes have [probability mass function](probability-mass-function.md) $f_j$, independently of $N$. The aggregate [probability mass function](probability-mass-function.md) $g_k$ satisfies the displayed recursion, with $g_0=0$. To prove it, write $P,F,G$ for the count, severity and aggregate [probability generating functions](probability-generating-function.md). The count recurrence gives $(1-az)P'(z)=(a+b)P(z)+p_1$. Since $G=P\circ F$, the [chain rule](chain-rule.md) gives $(1-aF)G'=((a+b)G+p_1)F'$. Comparing coefficients of $z^{k-1}$ gives the recursion. The forcing term $p_1f_k$ distinguishes this algorithm from the usual [Panjer recursion](panjer-recursion.md). For a [zero-truncated Poisson distribution](zero-truncated-poisson-distribution.md) with parameter $\lambda$, take $a=0$, $b=\lambda$ and $p_1=\lambda/(e^\lambda-1)$.

## ↑ Ancestors (8)

1. [Zero-truncated claim-count distribution](zero-truncated-claim-count-distribution.md)
2. [Truncated distribution](truncated-distribution.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-43/1/solution.md)
