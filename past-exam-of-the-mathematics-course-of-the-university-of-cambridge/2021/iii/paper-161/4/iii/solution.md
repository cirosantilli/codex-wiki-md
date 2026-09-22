<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $\mathcal C$ be a [clique](../../../../../../clique-graph-theory.md) and choose the given prime $q$ with $p^2<q<2p^2$. For distinct $A,B\in\mathcal C$, the intersection size is a multiple of $p$ strictly below $p^2$. In $\mathbb F_q$, set

$$
E=\{0,p,2p,\ldots,(p-1)p\}.
$$

These are $p$ distinct residues because $q>p^2$, every off-diagonal intersection size lies in $E$, and the diagonal size $p^2$ does not. Part i, now over $\mathbb F_q$, yields

$$
\omega(G)\leq\sum_{i=0}^{p}\binom{p^3}{i}.
$$

The subsets of a $p^3$-element set having size at most $p$ inject into its ordered $p$-tuples: list a nonempty subset increasingly and repeat its final element, while assigning the empty set one decreasing tuple not used in this way. The injection is not surjective, so

$$
\boxed{\sum_{i=0}^{p}\binom{p^3}{i}<(p^3)^p=p^{3p}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 161](../../../paper-161-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
