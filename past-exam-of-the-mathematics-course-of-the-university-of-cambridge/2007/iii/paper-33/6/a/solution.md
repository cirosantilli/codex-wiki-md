<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $E_i=\{M(I_i)=0\}$. For any subset $K\subseteq\{1,\ldots,n\}$, simultaneous voidness is voidness of the union. Since the intervals are disjoint, the assumed [void probability functional](../../../../../../void-probability-functional.md) gives

$$
\mathbb P\left(\bigcap_{i\in K}E_i\right)
=e^{-\lambda(\bigcup_{i\in K}I_i)}
=\prod_{i\in K}e^{-\lambda(I_i)}
=\prod_{i\in K}\mathbb P(E_i).
$$

This includes the empty subset. To check all event patterns explicitly, apply the [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) to the complements in a chosen pattern:

$$
\mathbb P\left(\bigcap_{i\in K}E_i\cap\bigcap_{j\notin K}E_j^c\right)
=\prod_{i\in K}\mathbb P(E_i)\prod_{j\notin K}(1-\mathbb P(E_j)).
$$

Thus **the void events are mutually independent**, and their complementary occupied-cell indicators are mutually independent too. This is joint [independence](../../../../../../independent-random-variables.md), not merely pairwise [independence](../../../../../../independent-random-variables.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
