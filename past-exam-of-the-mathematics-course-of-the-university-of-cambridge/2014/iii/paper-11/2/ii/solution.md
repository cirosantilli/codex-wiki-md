<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Form the family $\mathcal F=\{A\subseteq[n]:\sum_{i\in A}c_i>1/2\}$. The nonnegative weights make it an [up-set](../../../../../../up-set.md). It is an [intersecting family](../../../../../../intersecting-family.md), since two disjoint members would have combined weight exceeding one. The no-tie hypothesis makes it a [self-dual set family](../../../../../../self-dual-set-family.md): exactly one of $A,A^c$ belongs.

Let $a_j=|\mathcal F\cap\binom{[n]}j|/\binom nj$. Self-duality gives $a_{n-j}=1-a_j$. The [Erdős-Ko-Rado theorem](../../../../../../erdos-ko-rado-theorem.md) gives $a_j\le j/n$ for $j<n/2$; at $j=0$ this is immediate. If $n$ is even, $a_{n/2}=1/2$.

The [biased measure of a set family](../../../../../../biased-measure-of-a-set-family.md) is $\mu_p(\mathcal F)=\sum_j\binom nj a_jp^j(1-p)^{n-j}$. By independence of the [Bernoulli random variables](../../../../../../bernoulli-distribution.md), it equals $\mathbb P(Z\ge1/2)$, since equality is excluded. Subtract $p=\sum_j\binom nj(j/n)p^j(1-p)^{n-j}$ and pair complementary levels. The [complementary-layer bound for biased measure](../../../../../../complementary-layer-bound-for-biased-measure.md) gives

$$
\mu_p(\mathcal F)-p=\sum_{j<n/2}\binom nj\left(\frac jn-a_j\right)\left[p^{n-j}(1-p)^j-p^j(1-p)^{n-j}\right]\ge0.
$$

Both factors are nonnegative for $p\ge1/2$. The endpoints $p=1/2,1$ also follow directly, or by continuity. Thus the [weighted Bernoulli majority bound](../../../../../../weighted-bernoulli-majority-bound.md) is

$$
\boxed{\mathbb P(Z\ge1/2)\ge p}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
