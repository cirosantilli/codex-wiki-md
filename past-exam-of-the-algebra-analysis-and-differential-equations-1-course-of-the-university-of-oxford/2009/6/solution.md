<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The two bounding circles meet at zero and one, which the [Möbius transformation](../../../mobius-transformation.md) sends to zero and infinity. They therefore become straight lines through zero. More explicitly write $w=f(z)$, so $z=w/(1+w)$. The two disk inequalities become

$$
\operatorname{Re}(\overline\zeta w)>0,\qquad\operatorname{Re}(\zeta w)>0.
$$

Since $\zeta=1/2+i\sqrt3/2$, these say $\operatorname{Re}w>\sqrt3|\operatorname{Im}w|$. Thus

$$
\boxed{f(R)=\{w\ne0:-\pi/6<\arg w<\pi/6\}.}
$$

The positive real axis belongs to the image because $f(1/2)=1$, fixing which sector is intended. Cubing maps this sector bijectively onto the [right half-plane](../../../right-half-plane.md): its argument interval of width $\pi/3$ becomes $(-\pi/2,\pi/2)$. The [Cayley transform between the half-plane and disk](../../../cayley-transform-between-the-half-plane-and-disk.md) $v\mapsto(v-1)/(v+1)$ then maps that half-plane bijectively onto the [unit disk](../../../unit-disk.md). Hence a holomorphic bijection is

$$
\boxed{h(z)=\frac{\left(\frac z{1-z}\right)^3-1}{\left(\frac z{1-z}\right)^3+1}
=\frac{z^3-(1-z)^3}{z^3+(1-z)^3}.}
$$

Every denominator is nonzero on the corresponding domain, and the sector width ensures the power map is injective. This is the [conformal map of a symmetric circular lens](../../../conformal-map-of-a-symmetric-circular-lens.md).

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2009](../../2009-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
