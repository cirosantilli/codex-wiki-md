<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Color each integer independently and uniformly with one of $k$ colors. For a translate $S+t$, let $E_t$ be the event that some color is missing. The [union bound](../../../../../../boole-s-inequality.md) gives

$$
\mathbb P(E_t)\le k(1-1/k)^s\le ke^{-s/k}.
$$

Join two events in the [dependency graph of events](../../../../../../dependency-graph-of-events.md) when their translates overlap. Nonneighbors depend on disjoint sets of independent colors, giving the required joint independence. Overlap occurs only if $u-t\in S-S$, so the maximum degree is at most $s(s-1)$.

With natural logarithms, $s\ge6k\log k$ and $k\ge20$ imply

$$
eq(d+1)\le ek s^2e^{-s/k}\le\frac{36e(\log k)^2}{k^3}\le\frac{36e}{k^2}\le\frac{36e}{400}<1.
$$

The middle estimate uses that $s^2e^{-s/k}$ is decreasing for $s\ge2k$, and the next uses $\log k\le\sqrt{k}$. Therefore the [Lovász local lemma](../../../../../../lovasz-local-lemma.md) supplies a coloring avoiding every bad event in any specified finite family of translates.

To obtain one coloring for all translates, use the [compactness extension of the Lovász local lemma](../../../../../../compactness-extension-of-the-lovasz-local-lemma.md). At level $N$, consider colorings of $[-N,N]\cap\mathbb Z$ satisfying every constraint whose translate is contained in that interval. There are finitely many constraints, and the preceding argument makes the level nonempty. Restrictions connect these colorings into a finitely branching [tree](../../../../../../tree-graph-theory.md). The [König infinity lemma](../../../../../../konig-s-lemma.md) gives an infinite branch, hence a coloring of all integers. Every translate eventually lies in a level of this branch, so it contains every color.

Thus **there exists a $k$-coloring of $\mathbb Z$ in which every translate of $S$ contains all $k$ colors**. This is a [polychromatic coloring of integer translates](../../../../../../polychromatic-coloring-of-integer-translates.md); the compactness step establishes existence of one simultaneous coloring.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
