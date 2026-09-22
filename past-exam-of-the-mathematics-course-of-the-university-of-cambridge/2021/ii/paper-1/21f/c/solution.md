<h1 id="21f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose a contraction

$$
h:A\times I\to A,
\qquad
h(a,0)=a,
\qquad
h(a,1)=a_0.
$$

Apply the [homotopy extension property](../../../../../../homotopy-extension-property.md) to the initial map $\operatorname{id}_X:X\to X$ and to $h$, regarded as a homotopy into $X$. It supplies

$$
H:X\times I\to X
$$

such that

$$
H(x,0)=x,
\qquad
H(a,t)=h(a,t).
$$

At $t=1$, the map $H_1$ sends every point of $A$ to $a_0$. It is therefore constant on the equivalence classes of the [quotient topology](../../../../../../quotient-topology.md) $X/A$. By the [universal property of the quotient topology](../../../../../../universal-property-of-the-quotient-topology.md), there is a continuous map

$$
g:X/A\to X
$$

such that

$$
g\circ q=H_1,
$$

where $q:X\to X/A$ is the [quotient map](../../../../../../quotient-map.md). The homotopy $H$ immediately gives

$$
g\circ q=H_1\simeq H_0=\operatorname{id}_X.
$$

For every $t$, the map $q\circ H_t$ is constant on $A$, because $H(a,t)=h(a,t)\in A$. It therefore descends to

$$
\overline H:(X/A)\times I\to X/A,
\qquad
\overline H([x],t)=q(H(x,t)).
$$

This descended map is continuous: the product $q\times\operatorname{id}_I$ is a quotient map because $I$ is compact Hausdorff, and $q\circ H$ is constant on its fibres.  
At the endpoints,

$$
\overline H([x],0)=[x],
\qquad
\overline H([x],1)=q(g([x])).
$$

Thus

$$
q\circ g\simeq\operatorname{id}_{X/A}.
$$

The maps $q$ and $g$ are homotopy inverses, so

$$
\boxed{X\simeq X/A}.
$$

This proves the theorem on [collapsing a contractible cofibration](../../../../../../collapsing-a-contractible-cofibration.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21F](../../21f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
