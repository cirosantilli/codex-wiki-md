<h1 id="a/2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Baire category theorem](../../../../../baire-category-theorem.md) states that a nonempty complete [metric space](../../../../../metric-space.md) cannot be a countable union of closed [nowhere dense sets](../../../../../nowhere-dense-set.md); equivalently, every countable intersection of open dense sets is dense.

Let $E_n=\operatorname{span}\{e_1,\ldots,e_n\}$ in the space of [finitely supported sequences](../../../../../finitely-supported-sequence.md). Each $E_n$ is a closed [linear subspace](../../../../../vector-subspace.md) for every [norm](../../../../../norm.md), since a [finite-dimensional subspace is closed](../../../../../finite-dimensional-subspace-is-closed.md). Hence

$$
F_n=T^{-1}(E_n)
$$

is a closed [linear subspace](../../../../../vector-subspace.md) of the [Banach space](../../../../../banach-space-split.md) $X$. Every [finitely supported sequence](../../../../../finitely-supported-sequence.md) lies in some $E_n$, so $X=\bigcup_{n\geq1}F_n$. By the [Baire category theorem](../../../../../baire-category-theorem.md), some $F_N$ has nonempty [interior](../../../../../interior-topology.md).

A [linear subspace](../../../../../vector-subspace.md) with nonempty [interior](../../../../../interior-topology.md) is the whole space: translate a ball in it to zero and scale any vector into that ball. Thus $F_N=X$, giving $T(X)\subseteq E_N$ and

$$
\boxed{\operatorname{rank}T\leq N<\infty.}
$$

The proof uses no particular choice of [norm](../../../../../norm.md) on the space of [finitely supported sequences](../../../../../finitely-supported-sequence.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../split.md)
6. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
