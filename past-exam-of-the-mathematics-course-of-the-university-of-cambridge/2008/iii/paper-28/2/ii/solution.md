<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For this [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), the inverse is $(x,y)\mapsto(x,13-y)$. At a point with $2y-13\ne0$, implicit differentiation gives the tangent slope

$$
m=\frac{3x^2+2x+13}{2y-13}.
$$

If the tangent line is $y=mx+b$, substitution into the equation shows that the three intersection abscissae sum to $m^2-1$. Two of them equal the tangency abscissa $x$, so the third is $x_3=m^2-1-2x$. Reflecting the third intersection by the inverse formula gives the [elliptic curve group law from Riemann-Roch](../../../../../../elliptic-curve-group-law-from-riemann-roch.md) doubling formula

$$
x(2R)=m^2-1-2x(R),\qquad
 y(2R)=13-y(R)+m\bigl(x(R)-x(2R)\bigr).
$$

For $P$, the slope is $13/(-13)=-1$, giving $x(2P)=0$ and $y(2P)=13$. For $Q$, the slope is $(12-4+13)/(6-13)=-3$, giving $x(2Q)=9-1+4=12$ and $y(2Q)=13-3+(-3)(-2-12)=52$. Hence

$$
\boxed{2P=(0,13)=-P,\qquad 2Q=(12,52).}
$$

In particular $P$ has order exactly three: it is nonidentity and $2P=-P$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
