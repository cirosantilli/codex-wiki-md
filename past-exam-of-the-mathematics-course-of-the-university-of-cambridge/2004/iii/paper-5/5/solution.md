<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose a maximal [Brauer pair](../../../../../brauer-pair.md) $(D,b_D)$ for $B$. Define its [inertial quotient of a block](../../../../../inertial-quotient-of-a-block.md) and [inertial index of a block](../../../../../inertial-index-of-a-block.md) by

$$
E(B)=N_G(D,b_D)/(DC_G(D)),\qquad e=|E(B)|.
$$

Conjugacy of maximal pairs makes the index well-defined. The standard maximal-pair property used here is that $E(B)$ is a $p'$-group. Since $D$ is cyclic, its faithful conjugation action embeds it into $\operatorname{Aut}(D)$, so $e\mid p-1$. Write $d=p^n$ and $m=(d-1)/e$.

We use two precise structural results. Over an algebraically closed field, the basic algebra of a [block with cyclic defect group](../../../../../block-with-cyclic-defect-group.md) is a [Brauer tree algebra](../../../../../brauer-tree-algebra.md) with $e$ edges and exceptional multiplicity $m$. For a Brauer tree algebra with $t$ edges and exceptional multiplicity $m$, all nonprojective [indecomposable modules](../../../../../indecomposable-module.md) form the [stable Auslander–Reiten quiver](../../../../../stable-auslander-reiten-quiver.md)

$$
\mathbb ZA_{tm}/\langle\tau^t\rangle.
$$

These are the cyclic-defect structure theorem and the stable-quiver classification for tree algebras; we are not taking the requested numerical count as an assumption. [Morita equivalence](../../../../../morita-equivalence.md) preserves simple, projective and indecomposable isomorphism classes.

There is one [simple module](../../../../../irreducible-module.md) per edge, so **$l(B)=e$**. The vertices of $\mathbb ZA_s$ can be indexed by $(j,i)$, $j\in\mathbb Z$, $1\leq i\leq s$. The quotient by $\tau^e$ leaves $e$ choices of $j$ for each $i$. With $s=em=d-1$, there are $e(d-1)$ nonprojective [indecomposable modules](../../../../../indecomposable-module.md). There are also $e$ indecomposable [projective modules](../../../../../projective-module.md), one [projective cover](../../../../../projective-cover.md) per simple. Therefore

$$
\boxed{\#\operatorname{ind}(B)=e(d-1)+e=ed=p^ne.}
$$

This counts isomorphism classes, not multiplicities in the regular module. In the one-edge case it agrees with the $d$ Jordan chains for $k[t]/(t^d)$.

For the definition, take a finite connected [tree](../../../../../tree-graph-theory.md) with a cyclic order of the incident edges at every vertex and positive integer multiplicities equal to one except possibly at a distinguished vertex. Its [Brauer tree path presentation](../../../../../brauer-tree-path-presentation.md) has a quiver vertex for each tree edge, and successor arrows around each tree vertex, including loops for valency one. If edge $i$ has endpoints $v,w$, let $C_{i,v}$ and $C_{i,w}$ be the cycles around these endpoints. The relations identify

$$
C_{i,v}^{m_v}=C_{i,w}^{m_w},
$$

kill $C_{i,v}^{m_v}\alpha_{i,v}$, and kill paths switching between successor cycles belonging to different tree vertices. Redundant valency-one loops may be eliminated. This quotient of the [path algebra](../../../../../path-algebra.md) is the basic [Brauer tree algebra](../../../../../brauer-tree-algebra.md); allowing an arbitrary algebra with [Morita equivalence](../../../../../morita-equivalence.md) to it does not change the module assertions. In particular, the cyclic orders and multiplicity, not merely the underlying graph, are part of the data.

For the construction, use right modules with paths multiplied left to right; equivalently use the opposite quiver for left modules, choosing orientation so radical factors follow the specified order. The indecomposable projective $P_1$ with top $S_1$ has simple socle $S_1$ and two uniserial radical branches $U_v,U_w$ meeting in that socle. The relations show that $U_v$ has length $mr$ and factors $S_2,\ldots,S_r,S_1$ repeated $m$ times. The other branch has length $m_w\operatorname{val}(w)$. Thus $W_v=P_1/U_w$ is a [uniserial module](../../../../../uniserial-module.md) of length $mr$, with factors $S_1,S_2,\ldots,S_r$ cyclically repeated. For $J$ the [Jacobson radical](../../../../../jacobson-radical.md),

$$
\boxed{W_v/J^qW_v,\qquad 1\leq q\leq mr}
$$

is the desired [uniserial branch of a Brauer tree algebra](../../../../../uniserial-branch-of-a-brauer-tree-algebra.md). If an endpoint is a nonexceptional leaf, its branch is just the socle; the formula still applies.

For uniqueness, length one gives just $S_1$. If $q>1$ and $r>1$, the next factor $S_2$ chooses the successor arrow at $v$ uniquely, because two distinct edges cannot meet at both endpoints in a tree. Subsequent factors force the same cyclic succession. Any arrow into an edge not incident with $v$ acts as zero, because that simple does not occur. An opposite nonexceptional leaf loop is the full socle path around $v$, of length $mr$, hence zero on modules of length at most $mr$. If an opposite leaf is exceptional, then $v$ has multiplicity one and each incident simple occurs at most once; its nilpotent self-loop is zero on that one-dimensional vertex space as well.

The remaining action is one nilpotent successor chain. Choose a top generator $z_0$ and let $z_j$ be its successive path images for $0\leq j<q$. Uniseriality makes each image nonzero in its respective radical layer; these images form a basis in the basic algebra description. Their labels are $S_{1+(j\bmod r)}$, the successor arrow sends $z_j$ to $z_{j+1}$, and all other actions vanish. Any nonzero scalar choices are absorbed by rescaling this basis. This determines the module solely by its top and length.

If $r=1$ and $q>1$, then $m>1$ and $v$ is the exceptional leaf. The successor is a single loop and its action is the unique nilpotent Jordan chain of length $q$. The other branch either enters a different edge or is a redundant socle loop and contributes nothing. Hence **the prescribed uniserial module is unique up to isomorphism for every positive integer $q\leq mr$**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
