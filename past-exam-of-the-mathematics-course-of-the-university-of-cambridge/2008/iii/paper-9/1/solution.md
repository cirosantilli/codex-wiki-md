<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [topological group](../../../../../topological-group-split.md) is a [group](../../../../../group-split.md) with a topology for which multiplication $G\times G\to G$ and inversion $G\to G$ are continuous. A Hausdorff axiom is not built into this definition. For [neighbourhood bases](../../../../../neighbourhood-basis.md) $\mathcal B_x$ at each point, the precise [neighbourhood criterion for a topological group](../../../../../neighbourhood-criterion-for-a-topological-group.md) is

$$
\begin{aligned}&U\in\mathcal B_{xy}\ \Longrightarrow\ \exists V\in\mathcal B_x,\ W\in\mathcal B_y:\ VW\subseteq U,\\&U\in\mathcal B_{x^{-1}}\ \Longrightarrow\ \exists V\in\mathcal B_x:\ V^{-1}\subseteq U.\end{aligned}
$$

Necessity follows from continuity: the inverse image of a neighbourhood of $xy$ contains a product neighbourhood of $(x,y)$, and the inverse image of a neighbourhood of $x^{-1}$ contains a neighbourhood of $x$. Conversely, these inclusions give exactly those neighbourhood conditions for continuity of multiplication and inversion, since the rectangles $V\times W$ form a basis for the [product topology](../../../../../product-topology.md).

An equivalent identity-level formulation is useful. Bases must be obtainable by translation, $\mathcal B_x=x\mathcal B_e$, and for every $U\in\mathcal B_e$ one must have

$$
\boxed{\exists V\in\mathcal B_e:\ V^2\subseteq U;\qquad\exists V\in\mathcal B_e:\ V^{-1}\subseteq U;\qquad\forall g\in G\ \exists V\in\mathcal B_e:\ gVg^{-1}\subseteq U.}
$$

These conditions are necessary because translations are [homeomorphisms](../../../../../homeomorphism.md), multiplication is continuous at $(e,e)$, inversion is continuous at $e$, and each conjugation is a [homeomorphism](../../../../../homeomorphism.md). For sufficiency at $(x,y)$, first choose $D$ with $D^2\subseteq U$, then $V$ with $y^{-1}Vy\subseteq D$ and take $W=D$. This gives $(xV)(yW)\subseteq xyU$. For inversion near $x$, first choose $H$ with $xHx^{-1}\subseteq U$, then $V$ with $V^{-1}\subseteq H$; thus $(xV)^{-1}=x^{-1}(xV^{-1}x^{-1})\subseteq x^{-1}U$. The pointwise criterion is therefore satisfied everywhere. If Hausdorffness is also required, the additional identity-neighbourhood condition is $\bigcap_{U\in\mathcal B_e}U=\{e\}$: it gives separation of distinct points by translating sufficiently small neighbourhoods.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
