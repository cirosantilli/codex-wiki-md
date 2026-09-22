<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Choose an integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) with unit [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md). For $P\in E(\mathbb Q_p)$, choose homogeneous coordinates $[X:Y:Z]$ in $\mathbb Z_p$ with at least one unit by multiplying all three coordinates by a common power of $p$. Define

$$
\operatorname{red}(P)=[\overline X:\overline Y:\overline Z]\in\widetilde E_p(\mathbb F_p).
$$

Two primitive integral representatives differ by a unit, so this is well-defined. Every point of the reduced cubic is a [nonsingular point of an algebraic curve](../../../../../../nonsingular-point-of-an-algebraic-curve.md), and the identity reduces to $[0:1:0]$. This definition includes points whose affine coordinates are nonintegral.

To prove the [good-reduction map respects elliptic addition](../../../../../../good-reduction-map-respects-elliptic-addition.md), use the smooth proper integral model. The [elliptic curve group law](../../../../../../elliptic-curve-group-law-from-riemann-roch.md) is a morphism on this model, constructed by addition of degree-zero [divisor classes](../../../../../../divisor-class.md); it is defined even where an affine chord formula has a vanishing denominator. Passing to the [residue field](../../../../../../residue-field.md) commutes with this morphism. Hence

$$
\operatorname{red}(P+Q)=\operatorname{red}(P)+\operatorname{red}(Q),
$$

so reduction is a [homomorphism of abelian groups](../../../../../../homomorphism-of-abelian-groups.md).

For surjectivity, the simple-root [Hensel lemma](../../../../../../hensel-s-lemma.md) says that if $g\in\mathbb Z_p[t]$, $g(t_0)\equiv0\pmod p$ and $g'(t_0)\not\equiv0\pmod p$, then there is a unique $t\in\mathbb Z_p$ with $t\equiv t_0\pmod p$ and $g(t)=0$. The point at infinity lifts to $O$. At an affine point $(\overline x,\overline y)$ of the reduced equation $F(x,y)=0$, being a [nonsingular point of an algebraic curve](../../../../../../nonsingular-point-of-an-algebraic-curve.md) means at least one [partial derivative](../../../../../../partial-derivative.md) $F_x,F_y$ is nonzero. If $F_y\ne0$, fix any integral lift $x_0$ of $\overline x$ and apply the [Hensel lemma](../../../../../../hensel-s-lemma.md) to $g(t)=F(x_0,t)$ to lift $\overline y$. If $F_x\ne0$, fix $y_0$ and lift $\overline x$ instead. This proves the [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md) and gives

$$
\boxed{E(\mathbb Q_p)\twoheadrightarrow\widetilde E_p(\mathbb F_p)\text{ as abelian groups}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
