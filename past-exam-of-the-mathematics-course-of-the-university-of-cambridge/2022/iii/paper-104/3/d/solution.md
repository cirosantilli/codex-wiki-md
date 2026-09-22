<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An element $g$ fixing the first level restricts to an automorphism $g_i$ on each rooted subtree, and composition is coordinatewise. Therefore

$$
\phi(g)=(g_0,g_1,g_2)
$$

is a homomorphism. If all three sections are trivial, $g$ fixes every word, so $\phi$ is injective.

Directly from the recursions,

$$
\phi(b)=(a,1,b),qquad
\phi(aba^{-1})=(b,a,1),qquad
\phi(a^{-1}ba)=(1,b,a).
$$

The generators found in the preceding part therefore have every section in $G$, so $\phi(\operatorname{Stab}_G(1))\subseteq G^3$.

Moreover, every coordinate projection of this image contains both $a$ and $b$, and is therefore onto $G$. Since $a$ acts transitively on the first level, induction shows that $G$ acts transitively on every level of the [rooted tree](../../../../../../rooted-tree.md). The $n$th level has $3^n$ vertices, so the orders of these finite orbits are unbounded. Hence $G$ is infinite.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 104](../../../paper-104-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
