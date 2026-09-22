<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [diagram in a category](../../../../../diagram-category-theory.md) is a functor $D:\mathcal J\to\mathcal C$. A [cone over a diagram](../../../../../cone-over-a-diagram.md) with vertex $A$ is a family

$$
\gamma_j:A\to D(j)
$$

such that $D(u)\gamma_i=\gamma_j$ for every $u:i\to j$. A [categorical limit](../../../../../categorical-limit.md) is a terminal cone: for every cone $(A,\gamma)$ there is a unique map $A\to\lim D$ commuting with all legs.

Suppose $\mathcal C$ has small [products](../../../../../product-category-theory.md) and [equalizers](../../../../../equaliser.md). For a small diagram $D$, form

$$
P=\prod_{j\in\mathcal J}D(j),
\qquad
Q=\prod_{u:i\to j}D(j).
$$

There are two maps $r,s:P\rightrightarrows Q$. In the coordinate indexed by $u:i\to j$, let

$$
r_u=D(u)\pi_i,
\qquad
s_u=\pi_j.
$$

The [equalizer](../../../../../equaliser.md) $E\to P$ imposes exactly the cone equations. Maps $A\to E$ are therefore naturally the same as cones from $A$ to $D$, so $E\cong\lim D$. This is the [construction of small limits from products and equalizers](../../../../../construction-of-small-limits-from-products-and-equalizers.md).

Let $F:\mathcal I\to\mathcal J$ be [initial](../../../../../initial-functor.md), so every $(F\downarrow j)$ is nonempty and [connected](../../../../../connected-category.md). Restriction sends a cone $(A,\gamma_j)$ over $D$ to $(A,\gamma_{Fi})$ over $DF$. Conversely, given a cone $(A,\delta_i)$ over $DF$, choose an object

$$
(i,u:Fi\to j)\in(F\downarrow j)
$$

and define

$$
\gamma_j=D(u)\delta_i.
$$

A morphism in the comma category shows that this expression is unchanged along one edge, and connectedness makes it independent of the chosen object. The cone equations follow by choosing $(i,vu)$ for an arrow $v:j\to j'$. This construction is inverse to restriction and acts identically on vertex maps, proving the [cone restriction along an initial functor](../../../../../cone-restriction-along-an-initial-functor.md) isomorphism.

Terminal objects in the two cone categories therefore correspond. Whenever the $\mathcal I$-shaped limit exists,

$$
\lim_{\mathcal J}D\cong\lim_{\mathcal I}DF
$$

naturally in $D$. Equivalently, the triangle formed by precomposition

$$
F^*:[\mathcal J,\mathcal C]\to[\mathcal I,\mathcal C]
$$

and the two limit functors commutes up to natural isomorphism.

For the converse, suppose this commutation holds for $\mathcal C=\mathbf{Set}^{\mathrm{op}}$. Passing to [opposite categories](../../../../../opposite-category.md) says that restriction along $F^{\mathrm{op}}$ preserves all set-valued colimits. Fix $j\in\mathcal J$ and take the representable functor

$$
H=\mathcal J(-,j):\mathcal J^{\mathrm{op}}\to\mathbf{Set}.
$$

Its colimit is a singleton: the category of its elements has the initial object $(j,1_j)$. The restricted colimit is

$$
\operatorname*{colim}_{i\in\mathcal I^{\mathrm{op}}}\mathcal J(Fi,j),
$$

whose elements are precisely the connected components of $(F\downarrow j)$. By the assumed comparison this set is also a singleton. Thus $(F\downarrow j)$ is nonempty and connected for every $j$, so $F$ is initial.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
