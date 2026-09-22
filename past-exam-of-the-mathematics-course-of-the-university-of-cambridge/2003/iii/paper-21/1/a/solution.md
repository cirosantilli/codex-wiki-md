<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Mordell-Weil theorem](../../../../../../mordell-weil-group.md) gives $E(\mathbb Q)\cong E(\mathbb Q)_{\rm tors}\oplus\mathbb Z^r$. Move the rational point of order two to $(0,0)$ and clear denominators to obtain an integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md)

$$
E:y^2=x(x^2+ax+b),\qquad b(a^2-4b)\ne0.
$$

The [two-isogeny formula](../../../../../../two-isogeny-formula.md) gives $E':Y^2=X(X^2-2aX+a^2-4b)$ and [dual isogenies](../../../../../../dual-isogeny.md) $\phi:E\to E'$, $\widehat\phi:E'\to E$ with $\widehat\phi\phi=[2]$. Compute the [torsion subgroup](../../../../../../torsion-subgroup.md) using [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) at several good primes, followed by [division polynomials of an elliptic curve](../../../../../../division-polynomials.md) to identify the possible points.

For the free part, use [two-isogeny descent](../../../../../../two-isogeny-descent.md). The [two-torsion square-class homomorphism](../../../../../../two-torsion-square-class-homomorphism.md) is

$$
\alpha(O)=1,\qquad \alpha((0,0))=[b],\qquad \alpha((x,y))=[x]
$$

in $\mathbb Q^*/\mathbb Q^{*2}$, with [kernel](../../../../../../kernel-of-a-linear-map.md) $\widehat\phi E'(\mathbb Q)$; define $\alpha'$ on $E'$ similarly. The [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) restricts the first image to signed square-free divisors of $b$ and the second to those of $a^2-4b$. For each candidate $d$, solve its [two-isogeny descent quartic](../../../../../../quartic-covering-in-a-two-isogeny-descent.md)

$$
N^2=dU^4+aU^2V^2+\frac bd V^4.
$$

Test [local solubility](../../../../../../local-solubility.md) at the real place and the relevant [p-adic fields](../../../../../../p-adic-field.md), discard impossible classes, and search the surviving coverings for [rational points](../../../../../../rational-point.md). A point with $UV\ne0$ gives $x=d(U/V)^2$, $y=dUN/V^3$. Include the identity and rational [2-torsion](../../../../../../2-torsion.md) cases separately. Once both rational images are determined, the [two-isogeny rank formula](../../../../../../square-class-index-formula-for-two-isogeny-descent.md) gives

$$
2^r=\frac{\#\alpha(E(\mathbb Q))\,\#\alpha'(E'(\mathbb Q))}{4}.
$$

The point searches give explicit candidates for a basis. Their [canonical height pairing](../../../../../../canonical-height-pairing.md) can certify independence; [Mordell-Weil saturation](../../../../../../mordell-weil-saturation.md) and effective height bounds then certify that they generate the full free part. Rank alone does not certify generators of the whole [Mordell-Weil group](../../../../../../mordell-weil-group.md). If the rational images are not fully determined, the procedure instead supplies lower and upper bounds on the [rank of an elliptic curve](../../../../../../rank-of-an-elliptic-curve.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
