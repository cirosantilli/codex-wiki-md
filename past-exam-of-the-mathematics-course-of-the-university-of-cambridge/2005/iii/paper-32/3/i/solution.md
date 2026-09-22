<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose an integral [Minimal Weierstrass equation](../../../../../../minimal-weierstrass-equation.md) whose discriminant is a $p$-adic unit. Given $P=[X:Y:Z]\in E(\mathbb Q_p)$, scale the coordinates so that $X,Y,Z\in\mathbb Z_p$ and at least one is a unit. Define

$$
\varphi(P)=[\bar X:\bar Y:\bar Z]\in\widetilde E(\mathbb F_p).
$$

Another primitive representative differs by a unit scalar, so the projective reduction is well defined. The reduced cubic is smooth by [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md).

To prove the [group homomorphism](../../../../../../group-homomorphism.md) property, view this smooth projective cubic with its section $O$ as the integral elliptic model $\mathcal E/\mathbb Z_p$. Its addition law is defined over $\mathbb Z_p$, by adding degree-zero [divisor classes](../../../../../../divisor-class.md), and thus is a regular morphism $\mathcal E\times\mathcal E\to\mathcal E$. Properness identifies $E(\mathbb Q_p)$ with the integral sections just described. Reducing the addition morphism is the [group operation](../../../../../../group-operation.md) of the smooth special fiber. Consequently

$$
\boxed{\varphi(P+Q)=\varphi(P)+\varphi(Q),\qquad\varphi(O)=\widetilde O.}
$$

This is the [good-reduction map respects elliptic addition](../../../../../../good-reduction-map-respects-elliptic-addition.md) argument; it covers tangent, vertical and infinity cases where reducing a single affine slope formula would involve division by a nonunit. Smoothness also makes reduction surjective: at each reduced point a partial derivative is a unit, and the [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts that point in a local affine chart.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
