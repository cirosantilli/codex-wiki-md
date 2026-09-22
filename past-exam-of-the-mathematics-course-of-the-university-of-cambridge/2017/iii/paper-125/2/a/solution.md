<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [elliptic curve](../../../../../../elliptic-curve.md) has [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) over $K$ if it admits an integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md) with unit [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md). Equivalently, the reduction of its [Minimal Weierstrass equation](../../../../../../minimal-weierstrass-equation.md) is a nonsingular cubic over the [residue field](../../../../../../residue-field.md) $k$. Its smooth integral projective model is a [group scheme](../../../../../../group-scheme.md) with the point $O$ as identity.

Choose [homogeneous coordinates](../../../../../../homogeneous-coordinate.md) in the [valuation ring](../../../../../../valuation-ring.md) $\mathcal O_K$ with at least one coordinate a unit, and reduce them modulo its [maximal ideal](../../../../../../maximal-ideal.md) $\mathfrak m_K$. This defines $\operatorname{red}:E(K)\to\widetilde E(k)$. The [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) extends over the smooth integral model, so reduction is a [group homomorphism](../../../../../../group-homomorphism.md). For any point of $\widetilde E(k)$, choose an affine projective chart containing it. Smoothness means some [partial derivative](../../../../../../partial-derivative.md) of its equation is nonzero in $k$. Lift the other coordinate arbitrarily and apply the [Hensel lemma](../../../../../../hensel-s-lemma.md) to the coordinate with unit derivative. This constructs a point of $E(K)$ above the prescribed point, proving the [surjectivity of good reduction over a local field](../../../../../../surjectivity-of-good-reduction-over-a-local-field.md).

The [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md) consists precisely of points reducing to $O$. The parameter $t=-x/y$ at $O$ gives a bijection between this kernel and $\mathfrak m_K$: the integral formal-coordinate series solve the equation uniquely near $O$. Addition in these coordinates is the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md), not ordinary addition in $\mathfrak m_K$. Thus

$$
\boxed{0\longrightarrow E_1(K)\longrightarrow E(K)\xrightarrow{\operatorname{red}}\widetilde E(k)\longrightarrow0,\qquad E_1(K)\simeq\widehat E(\mathfrak m_K).}
$$

Here the [group operation](../../../../../../group-operation.md) on the last expression is its [formal group law](../../../../../../formal-group-law.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
