<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [group action](../../../../../../group-action.md), the [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) identifies the [orbit of a group action](../../../../../../orbit-of-a-group-action.md) of $x$ with the left [cosets](../../../../../../coset.md) of its [stabilizer subgroup](../../../../../../stabilizer-subgroup.md):

$$
G/G_x\longrightarrow Gx,\qquad gG_x\longmapsto gx.
$$

This is well defined and bijective because $gx=hx$ exactly when $h^{-1}g\in G_x$. In particular, for finite $G$,

$$
\boxed{|Gx|=[G:G_x],\qquad |G|=|Gx||G_x|.}
$$

Under the [conjugation action](../../../../../../conjugation-action.md) $g\cdot x=gxg^{-1}$, a singleton [orbit of a group action](../../../../../../orbit-of-a-group-action.md) means that $gxg^{-1}=x$ for every $g$. This is equivalent to $gx=xg$ for every $g$, so precisely these elements constitute the [centre of a group](../../../../../../center-of-a-group.md)

$$
Z(G)=\{x\in G:xg=gx\text{ for all }g\in G\}.
$$

The identity is central, and if $x,y$ commute with every element then so do $xy$ and $x^{-1}$. Thus $Z(G)$ is a [subgroup](../../../../../../subgroup.md). Each central element is fixed under every conjugation, giving $gZ(G)g^{-1}=Z(G)$: **the centre is a [normal subgroup](../../../../../../normal-subgroup.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
