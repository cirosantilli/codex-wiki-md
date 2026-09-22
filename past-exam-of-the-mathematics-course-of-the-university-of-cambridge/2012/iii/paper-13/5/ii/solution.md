<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [elliptic curve](../../../../../../elliptic-curve.md) works over every [algebraically closed field](../../../../../../algebraically-closed-field.md), including one algebraic over a finite field. Give it explicitly in $\mathbb P^2$ by

$$
E:\quad
\begin{cases}
y^2z=x^3-xz^2,&\operatorname{char}k\ne2,\\
y^2z+yz^2=x^3,&\operatorname{char}k=2.
\end{cases}
$$

In the first case the only point at infinity is $O=[0:1:0]$, where the derivative with respect to $z$ is nonzero. In the affine chart $z=1$, a [singular point of an algebraic variety](../../../../../../singular-point-of-an-algebraic-variety.md) would have $y=0$, $x^3-x=0$, and $3x^2-1=0$. The possible roots $x=0,1,-1$ cannot satisfy the last equation in [characteristic](../../../../../../characteristic-of-a-field.md) different from $2$: at $0$ it is $-1$, and at $\pm1$ it is $2$. In the second case the three homogeneous [partial derivatives](../../../../../../partial-derivative.md) are $x^2,z^2,y^2$, up to harmless signs, and cannot vanish simultaneously at a projective point. Thus both cubics are [smooth varieties](../../../../../../smooth-algebraic-variety.md). A reducible plane cubic would have intersecting positive-degree components by [Bézout theorem](../../../../../../bezout-s-theorem.md), and be singular at an intersection; therefore these smooth cubics are [irreducible varieties](../../../../../../irreducible-variety.md). The [genus-degree formula](../../../../../../genus-degree-formula.md) gives $g=(3-1)(3-2)/2=1$. With the marked point $O$ they are [elliptic curves](../../../../../../elliptic-curve.md).

For a [smooth algebraic curve](../../../../../../smooth-algebraic-curve.md), its [divisor class group](../../../../../../divisor-class-group.md) is its [Picard group](../../../../../../picard-group.md). Its degree-zero subgroup is

$$
\operatorname{Pic}^0(E)=\{[D]:\deg D=0\}.
$$

The map $P\mapsto[P-O]$ gives an [isomorphism](../../../../../../isomorphism.md) of [abelian groups](../../../../../../abelian-group.md)

$$
E(k)\cong\operatorname{Pic}^0(E).
$$

To recall why it is a bijection, [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) in [geometric genus](../../../../../../geometric-genus.md) one says every degree-one [divisor class](../../../../../../divisor-class.md) has exactly one independent section: a [canonical divisor](../../../../../../canonical-divisor.md) has degree zero, so the dual degree-$-1$ term has no section. Thus the class contains one effective [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) of degree one, namely a point $P$, and that point is unique. Translating by $-O$ gives the claimed bijection; this is precisely the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) on the [elliptic curve](../../../../../../elliptic-curve.md).

Choose a prime integer $\ell$ different from $\operatorname{char}k$. The [multiplication-by-n morphism](../../../../../../multiplication-by-n-morphism.md) $[\ell]:E\to E$ has derivative $\ell$ times the identity at $O$, so it is nonconstant. A nonconstant [morphism of algebraic varieties](../../../../../../morphism-of-algebraic-varieties.md) between [smooth projective curves](../../../../../../smooth-projective-curve.md) is surjective: its image is closed by [proper morphism](../../../../../../proper-morphism.md) and cannot have [algebraic dimension](../../../../../../dimension-of-an-algebraic-set.md) zero. Since $k$ is an [algebraically closed field](../../../../../../algebraically-closed-field.md), this makes $[\ell]$ surjective on $k$-points. Therefore

$$
E(k)=\ell E(k).
$$

Yet $E(k)$ is infinite. For each $x\in k$, the affine equation has a solution for $y$ in the [algebraically closed field](../../../../../../algebraically-closed-field.md); since $k$ is infinite, this gives infinitely many points.

By the [Fundamental theorem of finitely generated abelian groups](../../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md), a [finitely generated abelian group](../../../../../../finitely-generated-abelian-group.md) $A$ satisfying $A=\ell A$ has no free part and is a finite [torsion group](../../../../../../torsion-group.md) of order prime to $\ell$. The infinite group $E(k)$ cannot have this property while being finitely generated. Thus $\operatorname{Pic}^0(E)$ is not finitely generated. A subgroup of a [finitely generated abelian group](../../../../../../finitely-generated-abelian-group.md) is finitely generated, so

$$
\boxed{\operatorname{Cl}(E)\text{ is not a finitely generated abelian group}.}
$$

This proof uses divisibility and infinitude, rather than uncountability, so it remains valid over countable [algebraically closed fields](../../../../../../algebraically-closed-field.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
