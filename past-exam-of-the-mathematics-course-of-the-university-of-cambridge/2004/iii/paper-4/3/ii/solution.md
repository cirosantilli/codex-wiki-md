<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Modulo $G_3$, the subgroup $G_2=G^p$ is central because $[G_2,G]\subseteq G_3$, and has exponent dividing $p$ because $G_2^p=G_3$. Thus the [group](../../../../../../group-split.md) $G/G_3$ has [nilpotency class](../../../../../../nilpotency-class.md) at most two. Collection gives

$$
(xy)^p=x^py^p[y,x]^{\binom p2}\equiv x^py^p\pmod {G_3},
$$

since $[y,x]\in G_2$ and $p\mid\binom p2$. Also replacing $x$ by $xu$ with $u\in G_2$ leaves its $p$-th power unchanged modulo $G_3$. Hence the assignment is well-defined and is a [group homomorphism](../../../../../../group-homomorphism.md). Its image contains all the generators $x^pG_3$ of $G_2/G_3$, so it is onto:

$$
\boxed{G/G_2\twoheadrightarrow G_2/G_3,\qquad xG_2\longmapsto x^pG_3.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
