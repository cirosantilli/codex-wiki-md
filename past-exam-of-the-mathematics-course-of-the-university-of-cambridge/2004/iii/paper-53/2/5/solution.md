<h1 id="2/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Each independent run uses one oracle call and gives a uniformly sampled equation $z\cdot s=0$. Collect $n-1$ linearly independent equations and use [Gaussian elimination](../../../../../../gaussian-elimination.md) over $\mathbb F_2$. Their solution space has dimension one and consists of $\{0,s\}$, so the promised nonzero solution identifies $s$ uniquely.

To quantify the [expected query count for Simon sampling](../../../../../../expected-query-count-for-simon-sampling.md), write $d=n-1$. If the existing equations have rank $k<d$, their span contains $2^k$ of the $2^d$ possible samples. A fresh equation raises the rank with probability $1-2^{k-d}$. The mean waiting time is the corresponding [geometric distribution](../../../../../../geometric-distribution.md) mean, giving

$$
\mathbb E T=\sum_{k=0}^{d-1}\frac1{1-2^{k-d}}=d+\sum_{j=1}^{d}\frac1{2^j-1}<n+1.
$$

The last sum is less than $2$: its first term is $1$ and its remaining terms are bounded by $\sum_{j=2}^\infty2^{1-j}=1$. Hence the expected number of quantum queries is **$O(n)$**. For a fixed high-confidence budget, use $m=d+c$ samples. Failure to span means that a nonzero linear functional on the $d$-dimensional sampling space annihilates every sample. Each such functional has probability $2^{-m}$, so the [union bound](../../../../../../boole-s-inequality.md) gives failure probability at most $(2^d-1)2^{-m}<2^{-c}$. Thus $O(n+\log(1/\delta))$ queries suffice for failure probability at most $\delta$. For $n=1$, the nonzero string is known already and no samples are needed.

Classically, a collision between distinct queried arguments immediately yields $s=x+y$. Random queries produce this collision after order $2^{n/2}$ calls, by the [birthday problem](../../../../../../birthday-problem.md). Conversely, choose the nonzero period uniformly and label the fibres randomly. Before a collision, $q$ queries can exclude at most $\binom q2$ periods, their pairwise argument differences; every remaining period has the same no-collision transcript distribution. When $q=o(2^{n/2})$, those exclusions occupy a vanishing fraction of the candidate periods, and neither collision discovery nor guessing a remaining period has a constant success probability. More quantitatively, conditioned on no previous collision, the next query tests at most $q$ of at least $2^n-1-\binom q2$ remaining periods; summing these conditional probabilities proves the same square-root lower bound. Therefore the optimal bounded-error classical query count is **$\Theta(2^{n/2})$**, exponentially larger in $n$ than the quantum count.

This comparison presumes a hidden nonzero period. Under a literal interpretation asking merely for some $s$ satisfying the printed identity, returning $s=0$ requires no queries at all, quantum or classical. Nonzero $s$ is the necessary intended promise, not a consequence of two-to-one behavior alone.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2](../../2.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
