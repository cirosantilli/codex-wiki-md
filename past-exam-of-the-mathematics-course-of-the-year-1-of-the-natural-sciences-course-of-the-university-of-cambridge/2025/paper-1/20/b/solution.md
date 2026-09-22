<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Solve the [Lagrange multiplier](../../../../../lagrange-multiplier.md) equations by separating cases according to which coordinates vanish, so that division by a coordinate loses no [stationary points](../../../../../stationary-point.md).

If $x\ne0$ and $y=z=0$, the surface constraint gives

$$
\boxed{(x,y,z)=(\pm a,0,0),\qquad T=a^4.}
$$

If $x\ne0$ and exactly one of $y,z$ is nonzero, the equation for that nonzero coordinate forces $\lambda=0$, while the $x$ equation gives $\lambda=2a^2x^2>0$. Hence there are no [stationary points](../../../../../stationary-point.md) in that case.

If $x=0$ and $y,z\ne0$, the two remaining equations give $\lambda=a^2z^2=b^2y^2$. The surface constraint therefore has equal contributions from $y$ and $z$, giving four [stationary points](../../../../../stationary-point.md):

$$
\boxed{(x,y,z)=\left(0,\varepsilon\frac a{\sqrt2},\eta\frac b{\sqrt2}\right),\qquad T=\frac{a^2b^2}{4},\quad\varepsilon,\eta\in\{-1,1\}.}
$$

If all three coordinates are nonzero, the equations imply

$$
\lambda=2a^2x^2=a^2z^2=b^2y^2,
$$

so $z^2=2x^2$ and $y^2=2a^2x^2/b^2$. Substitution in the surface constraint gives, with $D=4a^2+b^2$,

$$
x^2=\frac{a^2b^2}{D},\qquad y^2=\frac{2a^4}{D},\qquad z^2=\frac{2a^2b^2}{D}.
$$

Thus the remaining eight [stationary points](../../../../../stationary-point.md) and their [temperatures](../../../../../temperature-split.md) are

$$
\boxed{(x,y,z)=\left(\varepsilon_1\frac{ab}{\sqrt D},\varepsilon_2\frac{\sqrt2a^2}{\sqrt D},\varepsilon_3\frac{\sqrt2ab}{\sqrt D}\right),\qquad T=\frac{a^4b^2}{4a^2+b^2},\quad\varepsilon_1,\varepsilon_2,\varepsilon_3\in\{-1,1\}.}
$$

For example, their common [temperature](../../../../../temperature-split.md) follows from $x^4+y^2z^2=a^4b^4/D^2+4a^6b^2/D^2=a^4b^2/D$. The cases with $x=0$ and $yz=0$ are exactly the coldest [points](../../../../../point-geometry.md) already listed. This exhausts all possibilities, giving fourteen other [stationary points](../../../../../stationary-point.md) in addition to those four.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
