<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

Normalize the second-order equation as $y''+P(z)y'+Q(z)y=0$, with $P,Q$ holomorphic at all finite nonzero points. The [regular singular point criterion for a second-order equation](../../../../../regular-singular-point-criterion-for-a-second-order-equation.md) at zero says that $zP(z)$ and $z^2Q(z)$ extend holomorphically across zero.

To impose the condition at infinity, set $w=1/z$ and $Y(w)=y(1/w)$. Since $y'=-w^2Y'$ and $y''=w^4Y''+2w^3Y'$, the transformed equation is

$$
Y''+\left(\frac2w-\frac{P(1/w)}{w^2}\right)Y'+\frac{Q(1/w)}{w^4}Y=0.
$$

Regular singularity at $w=0$ makes $2-P(1/w)/w$ and $Q(1/w)/w^2$ bounded and holomorphic there. Equivalently $zP(z)$ and $z^2Q(z)$ are bounded at infinity. They are entire functions by the zero-endpoint condition, so [Liouville's theorem](../../../../../liouville-theorem.md) makes both constants. The [Euler-Cauchy classification from two regular singular points](../../../../../euler-cauchy-classification-from-two-regular-singular-points.md) is therefore

$$
\boxed{z^2y''+Azy'+By=0,\qquad A,B\in\mathbb C.}
$$

Conversely these equations have ordinary coefficients everywhere on $\mathbb C^*$ and meet both regular-singularity bounds. If “regular singular” is required to exclude an ordinary point, omit $(A,B)=(0,0)$, which makes zero ordinary, and $(2,0)$, which makes infinity ordinary. Under the common “at worst regular singular” convention these two cases are included. Multiplication by a nonvanishing coefficient does not change the normalized equation or this classification.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
