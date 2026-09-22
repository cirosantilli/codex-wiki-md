<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

For an [algebraically closed field](../../../../../algebraically-closed-field.md) $k$, the strong [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) says that every [ideal](../../../../../ideal.md) $J\subseteq k[x_1,\ldots,x_n]$ satisfies

$$
\boxed{I(V(J))=\sqrt J.}
$$

Its weak form says that $V(J)=\varnothing$ exactly when $J=(1)$. Now let $S=\mathbb C[x_0,\ldots,x_n]$ and let $I\subseteq S$ be a [homogeneous ideal](../../../../../homogeneous-ideal.md). The affine zero set of $I$ is the [affine cone](../../../../../affine-cone.md) over $V_+(I)$ together with the origin. Hence, when the projective zero set is empty, either

$$
\boxed{I=(1)}
$$

or the affine zero set is exactly the origin. In the latter case the [Hilbert Nullstellensatz](../../../../../hilbert-nullstellensatz.md) gives

$$
\boxed{\sqrt I=(x_0,\ldots,x_n),}
$$

the [irrelevant ideal of projective space](../../../../../irrelevant-ideal-of-projective-space.md). Equivalently, some power $(x_0,\ldots,x_n)^N$ is contained in $I$. These are precisely the alternatives in the [Projective Nullstellensatz](../../../../../projective-nullstellensatz.md).

Let $V\subseteq\mathbb P^3$ be a [smooth quadric surface](../../../../../smooth-quadric-surface.md). After a [projective linear transformation](../../../../../projective-linear-transformation.md), the [Segre embedding](../../../../../segre-embedding.md) identifies

$$
V\cong\mathbb P^1\times\mathbb P^1.
$$

Choose distinct points $p,q\in\mathbb P^1$. The two fibres

$$
C_p=\mathbb P^1\times\{p\},
\qquad
C_q=\mathbb P^1\times\{q\}
$$

are the promised [disjoint curves on a smooth quadric surface](../../../../../disjoint-curves-on-a-smooth-quadric-surface.md): each is a smooth [projective line](../../../../../projective-line.md), and $C_p\cap C_q=\varnothing$. By the [Bézout theorem](../../../../../bezout-s-theorem.md), any two nonempty curves in the [projective plane](../../../../../projective-plane.md) intersect. An [isomorphism of algebraic varieties](../../../../../isomorphism-of-algebraic-varieties.md) preserves intersections and takes [projective curves](../../../../../projective-curve.md) to projective curves, so these disjoint curves prove

$$
\boxed{V\not\cong\mathbb P^2.}
$$

Next let $W$ be a [smooth projective curve](../../../../../smooth-projective-curve.md) and let $f:W\dashrightarrow Y\subseteq\mathbb P^N$ be a [rational map](../../../../../rational-map-of-projective-varieties.md) to a [projective variety](../../../../../projective-variety.md). At a point $P$ outside its initial domain, write

$$
f=[f_0:\cdots:f_N]
$$

using elements of the [function field](../../../../../function-field-of-an-algebraic-variety.md) $\mathbb C(W)$. The [local ring of a smooth algebraic curve](../../../../../local-ring-of-a-smooth-algebraic-curve.md) at $P$ is a [discrete valuation ring](../../../../../discrete-valuation-ring.md). If $m=\min_i v_P(f_i)$, multiplying every coordinate by a function of valuation $-m$ makes all coordinates regular at $P$ and at least one a unit there. They therefore define a [morphism](../../../../../morphism-of-algebraic-varieties.md) near $P$. Repeating this at the finitely many missing points proves the [extension of a rational map from a smooth projective curve](../../../../../extension-of-a-rational-map-from-a-smooth-projective-curve.md).

Smoothness is essential. Let $\nu:\mathbb P^1\to C$ be the [normalization of a nodal curve](../../../../../normalization-of-a-nodal-curve.md) for a rational nodal cubic $C$. The inverse is a rational map $C\dashrightarrow\mathbb P^1$ on the smooth locus. If it extended to a morphism $g:C\to\mathbb P^1$, then $g\circ\nu$ would agree with the identity on a [dense Zariski-open subset](../../../../../zariski-open-set.md) of $\mathbb P^1$ and hence everywhere. But the two distinct points $a,b\in\mathbb P^1$ above the node would satisfy

$$
a=(g\circ\nu)(a)=g(\nu(a))=g(\nu(b))=(g\circ\nu)(b)=b,
$$

a contradiction. This is the [failure of rational-map extension on a singular curve](../../../../../failure-of-rational-map-extension-on-a-singular-curve.md).

Finally take the [Fermat cubic curve](../../../../../fermat-cubic-curve.md)

$$
F=x^3+y^3+z^3
$$

and define the [projective hypersurface](../../../../../projective-hypersurface.md)

$$
Z=\left\{([x:y:z],[s:t])\in\mathbb P^2\times\mathbb P^1:
sF+txyz=0\right\}.
$$

Because $F$ and $xyz$ have no common [irreducible factor](../../../../../irreducible-polynomial.md), the bihomogeneous polynomial $sF+txyz$ is irreducible, so $Z$ is an [algebraic variety](../../../../../algebraic-variety.md). Let

$$
\pi:Z\longrightarrow\mathbb P^1,
\qquad
([x:y:z],[s:t])\longmapsto[s:t]
$$

be the second [coordinate projection](../../../../../coordinate-projection.md). Every homogeneous cubic in three variables has a projective zero over $\mathbb C$, so every fibre is nonempty and $\pi$ is a [surjective](../../../../../surjective-function.md) [morphism](../../../../../morphism-of-algebraic-varieties.md). Over $p=[1:0]$ the fibre is the [Fermat cubic curve](../../../../../fermat-cubic-curve.md), which is smooth and has [genus](../../../../../genus-of-a-smooth-plane-curve.md)

$$
\frac{(3-1)(3-2)}2=1.
$$

Over $q=[0:1]$ the fibre is

$$
V(xyz)=V(x)\cup V(y)\cup V(z),
$$

the union of exactly three distinct [projective lines](../../../../../projective-line.md), hence exactly three [irreducible components](../../../../../irreducible-component.md). This is the [cubic pencil with a triangular member](../../../../../cubic-pencil-with-a-triangular-member.md) required by the question.

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
