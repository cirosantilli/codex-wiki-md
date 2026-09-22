<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $O=(0:1:0)$ be the point at infinity of the [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md). It is the [identity element](../../../../../../identity-element.md) for the [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md). For an affine [rational point](../../../../../../rational-point.md) $P=(x,y)$, the inverse is

$$
-P=(x,-y-a_1x-a_3).
$$

Indeed, the two affine intersections with the vertical line have these ordinates, since their sum as roots of the quadratic in $y$ is $-a_1x-a_3$. This reflection is valid for a generalized [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) in every [characteristic of a field](../../../../../../characteristic-of-a-field.md).

For distinct $P,Q$, draw their line; for $P=Q$, draw the [tangent line](../../../../../../tangent-line.md). Let $R$ be its third intersection with the [elliptic curve](../../../../../../elliptic-curve.md), counted with [intersection multiplicity](../../../../../../intersection-multiplicity.md). Then **the sum is the reflection of the third intersection**:

$$
\boxed{P+Q=-R.}
$$

A vertical line has third intersection $O$, so $P+(-P)=O$. If a tangent has third intersection $O$, then $2P=O$. Define addition with $O$ by $P+O=P$; these conventions include all exceptional cases of the affine construction.

The construction is defined over the coefficient [field](../../../../../../field.md): after two known intersections, the remaining root is rational over that [field](../../../../../../field.md). It gives a commutative [group operation](../../../../../../group-operation.md). To see why it is associative, use the [elliptic curve group law from Riemann-Roch](../../../../../../elliptic-curve-group-law-from-riemann-roch.md): the map $P\mapsto[P-O]$ identifies the [elliptic curve](../../../../../../elliptic-curve.md) with its degree-zero [divisor class group](../../../../../../divisor-class-group.md). A line has intersection divisor $P+Q+R$ [linearly equivalent](../../../../../../linear-equivalence-of-weil-divisors.md) to $3O$, the divisor of the line at infinity. Thus $[P-O]+[Q-O]+[R-O]=0$. The geometric sum agrees with addition of [divisor classes](../../../../../../divisor-class.md), which is associative.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
