<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We use the following standard off-diagonal Ramsey result from the course: if $F$ is a [forest](../../../../../../forest.md) on $h-1$ vertices and $K_1\vee F$ is obtained by adjoining a [universal vertex](../../../../../../universal-vertex.md), then, for $k$ sufficiently large in terms of $h$,

$$
r(K_1\vee F,K_k)\leq C\frac{hk^2}{\log k}.
$$

Its proof combines the $r(K_3,K_k)=O(k^2/\log k)$ bound with an iterative neighbourhood embedding of the forest.

The graph $H_\ell$ in the question is exactly $K_1\vee P_{\ell-1}$, and a path is a [tree](../../../../../../tree-graph-theory.md), hence a forest. Substitution of $h=\ell$ gives

$$
R(H_\ell,K_k)\leq C\frac{\ell k^2}{\log k},
$$

as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 122](../../../paper-122-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
