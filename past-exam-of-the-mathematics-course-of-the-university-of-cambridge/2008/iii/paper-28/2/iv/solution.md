<h1 id="2/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Double $2Q=(12,52)$ using the tangent formula. The slope is

$$
m=\frac{3\cdot12^2+2\cdot12+13}{2\cdot52-13}=\frac{469}{91}=\frac{67}{13},
$$

so

$$
4Q=\left(\frac{264}{169},\frac{32505}{2197}\right).
$$

This finite point is neither $P$ nor $-P$, since its abscissa is nonzero. Therefore $P\pm4Q$ are both finite nonidentity points.

For a direct exact-coordinate proof, the line from $P$ to $4Q$ has slope $985/104$, while the line from $P$ to $-4Q=(264/169,-3944/2197)$ has slope $-493/429$. For a secant through $P=(0,0)$ and $R=(u,v)$, its slope is $m=v/u$, and the group law gives $x(P+R)=m^2-1-u$, $y(P+R)=13-mx(P+R)$. Simplification yields

$$
\boxed{P+4Q=\left(\frac{5577}{64},-\frac{415909}{512}\right),\qquad
P-4Q=\left(-\frac{1352}{1089},\frac{415909}{35937}\right).}
$$

The first abscissa has odd numerator and denominator $64$. The second has denominator $1089=3^2\cdot11^2$ and numerator not divisible by either $3$ or $11$. Thus **neither point has integral coordinates**.

Reduction also explains the obstruction without requiring the full secant arithmetic. At the good prime $2$, $\overline Q=(0,1)=-\overline P$, and $\overline P$ has order three, so $\overline{P+4Q}=O$. At the good prime $11$, the displayed coordinates of $4Q$ reduce to $(0,0)=\overline P$, so $\overline{P-4Q}=O$. A finite point with integral affine coordinates reduces to an affine point, not to the identity at infinity. Membership in the [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md) therefore certifies the same two nonintegrality conclusions, at primes $2$ and $11$ respectively.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
