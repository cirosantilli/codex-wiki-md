<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [filter on a set](../../../../../filter-set-theory.md) $X$ is a nonempty family $\mathcal F\subseteq\mathcal P(X)$ that excludes the empty set, is upward closed, and is closed under finite intersections. An [ultrafilter](../../../../../ultrafilter.md) is a proper filter that contains exactly one of $A$ and $X\setminus A$ for every subset $A\subseteq X$.

To prove the [ultrafilter lemma](../../../../../ultrafilter-lemma.md), order the proper filters containing $\mathcal F$ by inclusion. The union of any chain is again a proper filter, so [Zorn lemma](../../../../../zorn-s-lemma.md) gives a maximal extension $\mathcal U$. If neither $A$ nor $X\setminus A$ belonged to $\mathcal U$, adjoining either one would generate an improper filter. There would then be $U,V\in\mathcal U$ with $U\cap A=\varnothing$ and $V\cap(X\setminus A)=\varnothing$. But $U\cap V=\varnothing$, contradicting propriety. Hence $\mathcal U$ is an ultrafilter.

The [Stone-Čech compactification of the natural numbers](../../../../../stone-cech-compactification-of-the-natural-numbers.md) $\beta\mathbb N$ is the set of all ultrafilters on $\mathbb N$, with basic sets

$$
\overline A=\{\mathcal U:A\in\mathcal U\},
\qquad A\subseteq\mathbb N.
$$

The identities

$$
\overline A\cap\overline B=\overline{A\cap B},
\qquad
\beta\mathbb N\setminus\overline A=\overline{\mathbb N\setminus A}
$$

show that these sets form a basis of [clopen sets](../../../../../clopen-set.md). Distinct ultrafilters disagree on some $A$; one lies in $\overline A$ and the other in the disjoint set $\overline{\mathbb N\setminus A}$. Thus $\beta\mathbb N$ is a [Hausdorff space](../../../../../hausdorff-space.md).

If a family of basic closed sets $\overline{A_i}$ has the [finite intersection property](../../../../../finite-intersection-property.md), then the sets $A_i$ have the same property. They generate a proper filter, which extends to an ultrafilter lying in every $\overline{A_i}$. The [Alexander subbase theorem](../../../../../alexander-s-subbase-lemma.md) now implies that $\beta\mathbb N$ is a [compact space](../../../../../compact-space.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
