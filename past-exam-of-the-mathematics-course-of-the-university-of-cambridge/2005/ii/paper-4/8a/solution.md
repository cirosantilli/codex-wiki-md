<h1 id="8a/solution">Solution</h1>

↑ **Parent:** [8A](../8a.md)

At zero an [ordinary point](../../../../../ordinary-point-criterion-for-a-second-order-equation.md) requires $p,q$ to be analytic. A [regular singular point](../../../../../regular-singular-point.md) requires $zp$ and $z^2q$ to extend analytically to zero, with at least one of $p,q$ failing to be analytic if “singular” excludes [ordinary points](../../../../../ordinary-point-criterion-for-a-second-order-equation.md).

Put $\zeta=1/z$ and $v(\zeta)=w(1/\zeta)$. Differentiation gives $w'=-\zeta^2v'$ and $w''=\zeta^4v''+2\zeta^3v'$, so the transformed equation is

$$
v''+\left(\frac2\zeta-\frac{p(1/\zeta)}{\zeta^2}\right)v'
+\frac{q(1/\zeta)}{\zeta^4}v=0.
$$

The point at infinity is ordinary precisely when both transformed coefficients are analytic at $\zeta=0$. Solving these conditions for the original coefficients gives

$$
\boxed{p(z)=2z^{-1}+z^{-2}P(z^{-1}),\qquad q(z)=z^{-4}Q(z^{-1})},
$$

with $P,Q$ analytic near zero; the sign can be absorbed into the arbitrary analytic $P$.

If the only singular point on the sphere is the regular singularity at zero, then $zp(z)$ and $z^2q(z)$ are entire. The condition at infinity makes the first tend to $2$ and the second to $0$. By [Liouville theorem](../../../../../liouville-theorem.md) they are respectively the constants $2$ and $0$. Thus the unique equation is

$$
\boxed{w''+\frac2z w'=0},
$$

with general solution $w=A+B/z$. Zero is genuinely regular singular and infinity is ordinary. If “no other singular points” were restricted to finite points only, the general coefficients would instead be $p=P(z)/z$ and $q=Q(z)/z^2$ with entire $P,Q$; the preceding question about infinity indicates the spherical interpretation.

## ↑ Ancestors (10)

1. [8A](../8a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
