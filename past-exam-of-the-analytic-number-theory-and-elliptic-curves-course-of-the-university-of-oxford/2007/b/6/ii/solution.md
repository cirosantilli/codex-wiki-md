<h1 id="b/6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a short [Weierstrass equation of an elliptic curve](../../../../../weierstrass-equation-of-an-elliptic-curve.md) with coefficients in the [p-adic integers](../../../../../p-adic-integer.md), a point with nonintegral $x$ has valuations $v_p(x)=-2m$ and $v_p(y)=-3m$ for some [integer](../../../../../integer-split.md) $m\ge1$: the term $x^3$ strictly dominates $Ax+B$ in the equation, so $2v_p(y)=3v_p(x)$. Its formal parameter $T=-x/y$ therefore has valuation $m\ge1$. These points, together with the identity, form the formal neighborhood $E_1(\mathbb Q_p)$ of the identity, with parameter in $p\mathbb Z_p$ and the elliptic [formal group](../../../../../formal-group-law.md) law over the [p-adic integers](../../../../../p-adic-integer.md). For a point with $x\in\mathbb Z_p$, the equation gives $y\in\mathbb Z_p$ too.

The formal neighborhood has no nontrivial torsion. Multiplication by an [integer](../../../../../integer-split.md) coprime to $p$ has [series](../../../../../series-mathematics.md) $[m](T)=mT+O(T^2)$ and preserves $|T|_p$, so any torsion there must have $p$-power order. If $p\ge3$, part (i) gives $|T|_p\ge p^{-1/(p-1)}>p^{-1}$, contradicting $T\in p\mathbb Z_p$.

The printed hypotheses also allow $p=2$. In that case, a nontrivial torsion point in the formal neighborhood would have order a power of two and hence yield a point of order two in that neighborhood. But every nonidentity point of order two on a short [Weierstrass equation of an elliptic curve](../../../../../weierstrass-equation-of-an-elliptic-curve.md) has $y=0$ and $x$ a root of the monic cubic over the [p-adic integers](../../../../../p-adic-integer.md) $X^3+AX+B$. Such a root lies in the [p-adic integers](../../../../../p-adic-integer.md), so it cannot belong to the formal neighborhood, whose nonidentity points have nonintegral coordinates. This excludes the remaining case. This is the [torsion-free formal subgroup for a short Weierstrass equation](../../../../../torsion-free-formal-subgroup-for-a-short-weierstrass-equation.md). Thus every affine torsion point satisfies

$$
\boxed{|x|_p\le1,\qquad|y|_p\le1.}
$$

With [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md), the reduction [homomorphism](../../../../../homomorphism.md) $E(\mathbb Q_p)\to\widetilde E(\mathbb F_p)$ has kernel exactly this torsion-free formal neighborhood. Its restriction to the [torsion subgroup](../../../../../torsion-subgroup.md) is therefore injective, proving the required subgroup isomorphism. The short model over the [p-adic integers](../../../../../p-adic-integer.md) is essential to the prime-two argument; no blanket torsion-injectivity assertion for arbitrary models is needed.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
