<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This is the [Karp–Lipton theorem](../../../../../../karp-lipton-theorem.md). It is enough to place $\Pi_2^{\mathbf P}$ inside $\Sigma_2^{\mathbf P}$. Let $L\in\Pi_2^{\mathbf P}$, so for a polynomial-time predicate $R$ and polynomially bounded strings,

$$
x\in L
\quad\Longleftrightarrow\quad
\forall y\ \exists z\ R(x,y,z).
$$

The NP search problem that receives $(x,y)$ and seeks such a $z$ has, by part (i), a [polynomial-size circuit family](../../../../../../polynomial-size-circuit-family.md) producing a valid witness whenever one exists. For each input length there is therefore a polynomial-size circuit $C$ such that, for every relevant $x,y$, existence of a witness implies $R(x,y,C(x,y))$.

Consequently

$$
x\in L
\quad\Longleftrightarrow\quad
\exists C\ \forall y\ R(x,y,C(x,y)),
$$

where the existentially guessed circuit description has polynomial length and evaluation of $C$ is polynomial time. This is a $\Sigma_2^{\mathbf P}$ description. Hence $\Pi_2^{\mathbf P}\subseteq\Sigma_2^{\mathbf P}$; complementation gives the reverse inclusion, and merging adjacent equal quantifier blocks collapses every higher level. Thus the [polynomial hierarchy](../../../../../../polynomial-hierarchy.md) satisfies

$$
\boxed{\mathbf{PH}=\Sigma_2^{\mathbf P}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
