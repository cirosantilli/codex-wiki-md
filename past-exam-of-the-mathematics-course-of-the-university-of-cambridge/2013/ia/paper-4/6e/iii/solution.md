<h1 id="6e/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For [bounded weak compositions](../../../../../../bounded-weak-compositions.md), start with the unrestricted [stars and bars](../../../../../../stars-and-bars-combinatorics.md) set $S$ and let $A_i$ be its subset where $n_i\geq a_i$. For an index subset $J\subseteq\{0,\ldots,r\}$, subtract $a_i$ from each coordinate with $i\in J$. This is a [bijection](../../../../../../bijection.md) from $\bigcap_{i\in J}A_i$ to nonnegative tuples summing to

$$
N-\sum_{i\in J}a_i.
$$

Thus

$$
\left|\bigcap_{i\in J}A_i\right|
=\binom{N+r-\sum_{i\in J}a_i}{r},
$$

where a negative remaining sum gives zero, in accordance with the stipulated convention. Apply the avoidance form of the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md):

$$
\boxed{\#\{(n_i):\textstyle\sum_i n_i=N,\ 0\leq n_i<a_i\}
=\sum_{J\subseteq\{0,\ldots,r\}}(-1)^{|J|}
\binom{N+r-\sum_{i\in J}a_i}{r}.}
$$

Expanding by subset size gives the alternating single-index, pair-index and higher-index sums. The empty subset supplies $\binom{N+r}{r}$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
