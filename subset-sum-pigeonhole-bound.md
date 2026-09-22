# Subset-sum pigeonhole bound

↑ **Parent:** [Dissociated set](dissociated-set.md)

Let $S$ be a finite [set](set-split.md) of positive [integers](integer-split.md) and let $T=\sum_{s\in S}s$. Every [sum of a subset](sum-of-a-subset.md) is an [integer](integer-split.md) in $\{0,\ldots,T\}$. If $2^{|S|}>T+1$, the [pigeonhole principle](pigeonhole-principle.md) forces two distinct [subsets](subset.md) to have equal sums. Thus $S$ cannot be a [dissociated set](dissociated-set.md).

Cancelling their common intersection even produces two disjoint [subsets](subset.md) with the same sum. Positivity means neither remaining subset can be empty. Conversely, equality of two distinct [subset sums](subset-sum-problem.md) gives a nonzero relation with coefficients in $\{-1,0,1\}$, exactly the obstruction to being a [dissociated set](dissociated-set.md).

For an $r$-element [subset](subset.md) of $\{1,\ldots,n\}$, the largest possible $T$ is $r(2n-r+1)/2$. Therefore

$$
2^r>1+\frac{r(2n-r+1)}2
$$

is a sufficient condition forcing a collision for every such [subset](subset.md). This counting bound is sufficient rather than necessary. Powers of two show how a collision-free collection can instead use the [binary representation](binary-number.md) to make all sums different.

## ↑ Ancestors (8)

1. [Dissociated set](dissociated-set.md)
2. [Large spectrum](large-spectrum.md)
3. [Normalized Fourier analysis on a finite abelian group](normalized-fourier-analysis-on-a-finite-abelian-group.md)
4. [Additive combinatorics](additive-combinatorics-split.md)
5. [Combinatorics](combinatorics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2021/discrete-mathematics-continuous-mathematics-and-probability/3/d/solution.md)
