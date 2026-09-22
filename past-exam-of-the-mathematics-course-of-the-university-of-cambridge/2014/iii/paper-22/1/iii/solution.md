<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $C$ be the projective cubic of a [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), allowing its [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) to vanish, and let $O=[0:1:0]$. Use only the [smooth locus of a variety](../../../../../../smooth-locus-of-a-variety.md) $C_{\mathrm{sm}}(K)$: the singular point, if present, is excluded. For $P,Q$, intersect their chord with $C$, using the tangent if $P=Q$ and counting [intersection multiplicity](../../../../../../intersection-multiplicity.md). If the third intersection is $R$, define $P+Q=-R$, where

$$
-(x,y)=(x,-y-a_1x-a_3)
$$

in general [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) coordinates. The line through $R$ and $O$ gives this reflection. A vertical chord gives $P+(-P)=O$, and the tangent at $O$ meets $C$ three times at $O$, so $O$ is the identity. The construction is symmetric in $P,Q$. It stays in the nonsingular locus: a line through a singular point has intersection multiplicity at least two there, and therefore cannot also contain two smooth intersections counted with multiplicity.

For the nonsingular case, prove [associativity](../../../../../../associative-property.md) by transporting a known [abelian group](../../../../../../abelian-group.md) law. The [Abel-Jacobi map of a genus-one curve](../../../../../../abel-jacobi-map-of-a-genus-one-curve.md)

$$
\iota:C\longrightarrow\operatorname{Pic}^0(C),\qquad P\longmapsto[P-O]
$$

is bijective over an [algebraic closure](../../../../../../algebraic-closure.md). Indeed, the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) in [genus one](../../../../../../genus-one-curve.md) says that every [divisor class](../../../../../../divisor-class.md) of degree one has a unique effective representative consisting of one point: existence follows from $\ell(D)=1$, and uniqueness follows because two distinct representatives would produce a degree-one map to the [projective line](../../../../../../projective-line.md), impossible for a [genus one curve](../../../../../../genus-one-curve.md). Subtracting $O$ gives the claimed bijection.

Any line section represents the same [divisor class](../../../../../../divisor-class.md) as $3O$, including tangencies. Thus $P+Q+R\sim3O$ as [divisors on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md), while the vertical line gives $R+(-R)+O\sim3O$. Hence

$$
\iota(P+Q)=\iota(P)+\iota(Q).
$$

Addition in the [Picard group](../../../../../../picard-group.md) is associative, so

$$
\boxed{(P+Q)+S=P+(Q+S).}
$$

The [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) is defined over $K$, so the [group operation](../../../../../../group-operation.md) restricts to the $K$-[rational points](../../../../../../rational-point.md).

For completeness, a singular [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) produces the [smooth-locus group of a singular Weierstrass cubic](../../../../../../smooth-locus-group-of-a-singular-weierstrass-cubic.md), not an [elliptic curve](../../../../../../elliptic-curve.md). Over an [algebraic closure](../../../../../../algebraic-closure.md), its [normalization of an algebraic curve](../../../../../../normalization-of-an-algebraic-curve-split.md) is the [projective line](../../../../../../projective-line.md); deleting the two preimages of a [nodal crossing](../../../../../../nodal-crossing.md) gives the [multiplicative algebraic group](../../../../../../multiplicative-algebraic-group.md), while deleting the single preimage of a [cusp](../../../../../../cusp-algebraic-geometry.md) gives the [additive group](../../../../../../additive-group.md). For example, on $y^2=x^3$, the coordinate $u=x/y$, with $u(O)=0$, makes the smooth-locus law addition. On $y^2=x^2(x+1)$ in characteristic different from two, put $t=y/x$ and $z=(t+1)/(t-1)$, with $z(O)=1$; the chord relation gives $z(P)z(Q)z(R)=1$, so the group law is multiplication of $z$. A nonsplit node gives the corresponding form of the [multiplicative algebraic group](../../../../../../multiplicative-algebraic-group.md) over $K$. These descriptions also establish the singular-case group laws.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
