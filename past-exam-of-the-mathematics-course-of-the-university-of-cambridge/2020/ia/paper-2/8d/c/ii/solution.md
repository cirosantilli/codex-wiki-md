<h1 id="8d/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The set $T$ is uncountable. Partition $\mathbb N$ into countably many infinite sets $B_1,B_2,\ldots$, and choose bijections $h_j:B_j\to\mathbb Z$. For every subset $A\subseteq\mathbb N$, define a permutation $f_A$ separately on each block by

$$
h_j(f_A(x))=
\begin{cases}
h_j(x)+1,&j\in A,\\
h_j(x)-1,&j\notin A.
\end{cases}
$$

Every positive iterate translates each integer coordinate by a nonzero amount, so it has no fixed point and $f_A\in T$. Distinct subsets $A$ give distinct permutations, yielding an injection $\mathcal P(\mathbb N)\hookrightarrow T$. Since the [power set](../../../../../../../power-set.md) is uncountable,

$$
\boxed{T\text{ is uncountable}}.
$$

In fact its cardinality is the continuum, because it is a subset of all functions $\mathbb N\to\mathbb N$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [8D](../../../8d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ia](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
