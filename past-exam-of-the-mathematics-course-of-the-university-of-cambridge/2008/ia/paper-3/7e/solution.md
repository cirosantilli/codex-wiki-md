<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

Write a [Möbius transformation](../../../../../mobius-transformation.md) as $M(z)=(az+b)/(cz+d)$ with $ad-bc\ne0$, interpreted on the [Riemann sphere](../../../../../riemann-sphere.md). Let $T_u(z)=z+u$, $D_\lambda(z)=\lambda z$ with $\lambda\ne0$, and $I(z)=1/z$.

If $c=0$, then $a,d\ne0$ and $M(z)=(a/d)z+b/d=T_{b/d}\circ D_{a/d}(z)$. If $c\ne0$, algebraic division gives

$$
M(z)=\frac ac+\frac{bc-ad}{c^2}\frac1{z+d/c}.
$$

Consequently

$$
\boxed{M=T_{a/c}\circ D_{(bc-ad)/c^2}\circ I\circ T_{d/c}.}
$$

The scaling coefficient is nonzero because $ad-bc\ne0$. Thus translations, nonzero complex scalings and reciprocal inversion generate every [Möbius map](../../../../../mobius-transformation.md). The formulas extend over their poles and infinity by the sphere interpretation.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
