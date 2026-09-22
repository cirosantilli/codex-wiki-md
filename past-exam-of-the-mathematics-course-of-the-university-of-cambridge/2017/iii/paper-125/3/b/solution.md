<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this integral [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), compute

$$
\Delta=16m^4(m^2-1)^2,\qquad c_4=16(m^4-m^2+1).
$$

If an odd [prime](../../../../../../prime-number.md) divides $m$ or $m^2-1$, then $c_4$ is a unit there and $\Delta$ is not. The [j-invariant of an elliptic curve](../../../../../../j-invariant-of-an-elliptic-curve.md) consequently has negative [valuation](../../../../../../valuation.md). Since [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) implies an integral j-invariant, such a [prime](../../../../../../prime-number.md) cannot be a [prime](../../../../../../prime-number.md) of good reduction, regardless of whether the displayed equation is minimal. Conversely, if it divides neither factor, this equation already has unit discriminant.

At five the good possibilities have $m\equiv\pm2$, so $m^2\equiv4$. At seven they have $m^2\equiv2$ or $4$. Direct [elliptic-curve point count over a finite field](../../../../../../elliptic-curve-point-count-over-a-finite-field.md) gives the following nonzero ordinates, together with the three zero-ordinate points and $O$:

$$
\begin{array}{c|c|c|c}
p&m^2\bmod p&\text{points with }y\ne0&\#\widetilde E(\mathbb F_p)\\\hline
5&4&(2,\pm1),(3,\pm2)&8\\
7&2&(3,\pm2),(4,\pm1)&8\\
7&4&(2,\pm1),(5,\pm2)&8
\end{array}
$$

At either [prime](../../../../../../prime-number.md), [torsion-freeness of the formal group over Qp for odd p](../../../../../../torsion-freeness-of-the-formal-group-over-qp-for-odd-p.md) makes reduction injective on all of $E(\mathbb Q)_{\rm tors}$, so its order is at most eight. Using only prime-to-$p$ injectivity here would leave an unjustified possible $p$-primary component.

All three nonzero [2-torsion](../../../../../../2-torsion.md) points $(0,0),(-1,0),(-m^2,0)$ are rational. The [rational point](../../../../../../rational-point.md) $P=(m,m(m+1))$ lies on the curve, since $m(m+1)(m+m^2)=m^2(m+1)^2$. For an equation $y^2=x(x^2+ax+b)$ the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives

$$
x(2P)=\frac{(x(P)^2-b)^2}{4x(P)(x(P)^2+ax(P)+b)}.
$$

Here $a=1+m^2$, $b=m^2$, so $2P=(0,0)$ and $P$ has order four. The point $(-1,0)$ is not in $\langle P\rangle$, whose only nonzero point of order two is $(0,0)$. Therefore $P$ and $(-1,0)$ generate a subgroup of order eight isomorphic to $\mathbb Z/4\mathbb Z\times\mathbb Z/2\mathbb Z$. The upper bound proves the [rational torsion in the family x times x plus one times x plus m squared](../../../../../../rational-torsion-in-the-family-x-times-x-plus-one-times-x-plus-m-squared.md):

$$
\boxed{E(\mathbb Q)_{\rm tors}\cong\mathbb Z/2\mathbb Z\times\mathbb Z/4\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
