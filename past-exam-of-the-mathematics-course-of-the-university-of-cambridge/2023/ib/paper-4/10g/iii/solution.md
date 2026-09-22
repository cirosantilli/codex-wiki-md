<h1 id="10g/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Define

$$
f:[0,1]^2\longrightarrow S^2,
$$



$$
f(x,y)=\bigl(\sin(\pi y)\cos(2\pi x),
\sin(\pi y)\sin(2\pi x),\cos(\pi y)).
$$

This is continuous and takes values on the [unit sphere](../../../../../../unit-sphere.md). It agrees at $(0,y)$ and $(1,y)$, is constant on the bottom edge, and is constant on the top edge. Thus it is constant on every $R$-class, so the [universal property of the quotient topology](../../../../../../universal-property-of-the-quotient-topology.md) gives a continuous map

$$
\overline f:X/R\longrightarrow S^2.
$$

For $0<y<1$, the third coordinate $\cos(\pi y)$ determines $y$, and the first two coordinates determine $x$ modulo one. Consequently the only equal values of $f$ in the open strip arise from $x=0$ and $x=1$. At $y=0$ the whole edge maps to the north pole, and at $y=1$ the whole edge maps to the south pole. These are exactly the identifications defining $R$, so $\overline f$ is injective. The spherical-coordinate formula also shows that it is surjective.

The square is compact, hence its quotient $X/R$ is compact by part (ii), while $S^2$ is Hausdorff as a subspace of $\mathbb R^3$. The [compact-to-Hausdorff continuous bijection theorem](../../../../../../compact-to-hausdorff-continuous-bijection-theorem.md) now makes $\overline f$ a homeomorphism. Geometrically, identifying the vertical sides produces a cylinder and collapsing each boundary circle to a point produces the [suspension of a topological space](../../../../../../suspension-topology.md) $S^1$, which is $S^2$. This proves the [square quotient model of the two-sphere](../../../../../../square-quotient-model-of-the-two-sphere.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
