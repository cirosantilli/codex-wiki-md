<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Work with the smooth projective cubic, including its points at infinity. For two points $P,Q$, draw their chord, using the tangent when they coincide, and let $R$ be its third intersection counted with [intersection multiplicity](../../../../../intersection-multiplicity.md). Draw the line through $R$ and $o$, again using the tangent if necessary, and let $S$ be its third intersection. Define $P+Q=S$. When $o$ is a flex, this is the familiar reflection of the first third-intersection point across the Weierstrass involution. The two-line construction also works when the chosen identity is not a flex.

To prove associativity without assuming it in the geometry, use [divisor class](../../../../../divisor-class.md). A nonsingular plane cubic has genus one. By the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md), every [divisor class](../../../../../divisor-class.md) of degree one contains exactly one effective [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) of degree one: for such a [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) $D$,

$$
\ell(D)-\ell(K_C-D)=\deg D=1,
$$

and $\deg(K_C-D)=-1$, so $\ell(K_C-D)=0$. Thus $\ell(D)=1$, and the nonzero section is unique up to scalar. Over $K$, a degree-one effective [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) defined over $K$ is a $K$-rational point. This also proves uniqueness of that point. In particular the map

$$
\iota:C(K)\longrightarrow\operatorname{Pic}^0(C),\qquad
P\longmapsto[P-o]
$$

is injective and identifies these points with the corresponding [degree-zero Picard group of a curve](../../../../../degree-zero-picard-group-of-a-curve.md): to recover the point from a class, add $[o]$ and take its unique effective representative. This is the [elliptic curve group law from Riemann-Roch](../../../../../elliptic-curve-group-law-from-riemann-roch.md).

Let $H$ denote the [divisor class](../../../../../divisor-class.md) cut out by a line. The two lines in the [chord-and-tangent group law](../../../../../chord-and-tangent-group-law.md) give

$$
P+Q+R\sim H,\qquad R+o+S\sim H.
$$

Their difference gives $P+Q\sim o+S$, hence

$$
\iota(S)=[P-o]+[Q-o].
$$

Addition of [divisor class](../../../../../divisor-class.md) is associative. Therefore both $(P+Q)+R$ and $P+(Q+R)$ map to $[P-o]+[Q-o]+[R-o]$. Injectivity of $\iota$ proves **the [chord-and-tangent group law](../../../../../chord-and-tangent-group-law.md) is associative**. The same argument gives identity $o$, commutativity and inverses, and covers tangencies through the use of [intersection multiplicities](../../../../../intersection-multiplicity.md). All constructions are defined over $K$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
