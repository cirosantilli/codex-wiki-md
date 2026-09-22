# Classical Roth bound for three-term progressions

↑ **Parent:** [Roth theorem on three-term arithmetic progressions](roth-theorem-on-three-term-arithmetic-progressions.md)

Write $r_3(N)$ for the maximum [cardinality](cardinality.md) of a [subset](subset.md) of $[N]$ containing no nonconstant three-term [arithmetic progression](arithmetic-progression.md). There is an absolute constant $C$ such that every three-term-progression-free [subset](subset.md) $A\subseteq[N]$ satisfies $|A|\leq CN/\log\log N$ for $N\geq3$. A quantitative [Roth density-increment step](roth-density-increment-step.md) gives, for [subset density](density-of-a-finite-subset.md) $\delta$ and $N\geq4\cdot10^6\delta^{-4}$, a [arithmetic progression](arithmetic-progression.md) of length at least $\delta^2\sqrt N/2000$ and increased [subset density](density-of-a-finite-subset.md) at least $\delta+\delta^2/64$. The increment decreases reciprocal [subset density](density-of-a-finite-subset.md) by at least $1/65$, so fewer than $\lceil65/\delta\rceil$ iterations are possible. If $N_j$ is the successive length, then $\log N_{j+1}\geq\frac12\log N_j-\log(2000/\delta^2)$, using the initial [subset density](density-of-a-finite-subset.md) to bound all later ones. Hence $\log N_j\geq2^{-j}\log N-2\log(2000/\delta^2)$. If $\delta\log\log N$ exceeds a sufficiently large absolute constant, all these intervals remain above the [density increment](density-increment.md) threshold, a contradiction. This proves the displayed bound. The result is a classical quantitative version of [Roth theorem on three-term arithmetic progressions](roth-theorem-on-three-term-arithmetic-progressions.md), without asserting an optimal bound.

## ↑ Ancestors (6)

1. [Roth theorem on three-term arithmetic progressions](roth-theorem-on-three-term-arithmetic-progressions.md)
2. [Additive combinatorics](additive-combinatorics-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-88/2/i/solution.md)
