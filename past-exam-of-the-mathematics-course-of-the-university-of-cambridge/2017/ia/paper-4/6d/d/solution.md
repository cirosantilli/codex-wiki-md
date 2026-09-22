<h1 id="6d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each positive [integer](../../../../../../integer.md) $n$, consider the threshold [set](../../../../../../set-split.md) $A^{(n)}=\{a\in A:a\ge1/n\}$. If it were infinite, one could choose recursively a [sequence](../../../../../../sequence.md) of distinct elements from it. Every arithmetic average of that [sequence](../../../../../../sequence.md) would be at least $1/n$, contradicting the assumed limit zero. Hence every $A^{(n)}$ is a [finite set](../../../../../../finite-set.md).

Every positive [real number](../../../../../../real-number.md) $a$ exceeds $1/n$ for some $n$, by the [Archimedean property](../../../../../../archimedean-property.md). Therefore

$$
A=\bigcup_{n=1}^{\infty}A^{(n)}.
$$

A [countable union of countable sets](../../../../../../countable-union-of-countable-sets.md) is countable, so $\boxed{A\text{ is countable}}$. In fact, under the stipulated infinitude, $A$ is a [countably infinite set](../../../../../../countably-infinite-set.md). Positivity matters: it ensures that these thresholds cover $A$. This is [countability from vanishing averages of distinct sequences](../../../../../../countability-from-vanishing-averages-of-distinct-sequences.md); ordinary [Cesaro convergence of a sequence](../../../../../../cesaro-convergence-of-a-sequence.md) of one chosen enumeration would not suffice to control the whole [set](../../../../../../set-split.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6D](../../6d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
