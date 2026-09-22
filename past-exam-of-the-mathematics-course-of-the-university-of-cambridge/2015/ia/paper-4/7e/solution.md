<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For a finite family of subsets $A_1,\ldots,A_N$ of a finite set $\Omega$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\left|\bigcup_{i=1}^N A_i\right|=\sum_{\varnothing\ne J\subseteq\{1,\ldots,N\}}(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

Let $A_{ij}$ be the set of [permutations](../../../../../permutation.md) with the two-cycle $(ij)$ in their [cycle decomposition of a permutation](../../../../../cycle-decomposition-of-a-permutation.md). Two distinct specified pairs sharing a label cannot both occur, so their intersection is empty. An intersection containing $r$ pairwise disjoint specified pairs fixes those $2r$ labels and leaves $(n-2r)!$ choices for the other labels.

The number of ways to choose $r$ disjoint unordered pairs is $n!/[2^r r!(n-2r)!]$: first order the selected labels, then divide by the two orders within each pair, by the $r!$ orders of the pairs, and by the orders of the unused labels. Applying [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) to the complement of the union yields the count of [permutations without two-cycles](../../../../../permutations-without-two-cycles.md):

$$
\boxed{f(n)=\sum_{r=0}^{\lfloor n/2\rfloor}(-1)^r\frac{n!}{2^rr!}.}
$$

The term $r=0$ is $n!$. Fixed points and cycles of length at least three are allowed; the restriction concerns two-cycles, not whether a [permutation](../../../../../permutation.md) can be expressed as a product of [transpositions](../../../../../transposition-permutation.md).

Dividing by $n!$ gives partial sums of the absolutely convergent [exponential series](../../../../../exponential-series.md), so

$$
\boxed{\lim_{n\to\infty}\frac{f(n)}{n!}=\sum_{r=0}^{\infty}\frac{(-1/2)^r}{r!}=e^{-1/2}.}
$$

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
