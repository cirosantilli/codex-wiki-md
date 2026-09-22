<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [Möbius transformation](../../../mobius-transformation.md) is $M(z)=(az+b)/(cz+d)$ with $ad-bc\ne0$, extended to the [Riemann sphere](../../../riemann-sphere.md) at its [pole](../../../pole.md) and at infinity. Wherever its finite coordinate is defined,

$$
M'(z)=\frac{ad-bc}{(cz+d)^2}\ne0.
$$

At a [pole](../../../pole.md), the ordinary complex [derivative](../../../derivative.md) is undefined, rather than zero; using the target coordinate $1/M$ gives a nonzero [derivative](../../../derivative.md) there as well. Thus the source's nowhere-zero assertion is interpreted in local sphere coordinates, or on the finite domain with the [pole](../../../pole.md) excluded.

Composition corresponds to multiplication of the invertible [matrices](../../../matrix.md) $\begin{pmatrix}a&b\\c&d\end{pmatrix}$, with scalar multiples giving the same map. The identity [matrix](../../../matrix.md) gives the identity, and the inverse [matrix](../../../matrix.md) gives an inverse Möbius map. This proves the group property on the [Riemann sphere](../../../riemann-sphere.md).

The two boundary circles meet at $\pm i$. Put

$$
\boxed{w=M(z)=\frac{z-i}{z+i},\qquad z=i\frac{1+w}{1-w}.}
$$

For $w=u+iv$, direct substitution gives

$$
|z+1|^2-2=\frac{4(u-v)}{|1-w|^2},\qquad
|z-1|^2-2=\frac{4(u+v)}{|1-w|^2}.
$$

This gives a [lens-to-half-plane map through the intersection points](../../../lens-to-half-plane-map-through-the-intersection-points.md). Both lens inequalities hold exactly when $u<-|v|$, the open sector with continuous argument between $3\pi/4$ and $5\pi/4$. This proves bijectivity, since the inverse is defined throughout that sector and the excluded endpoint $-i$ is not in the lens.

Rotate the sector through $-3\pi/4$ and square it, obtaining a bijection onto the [upper half-plane](../../../upper-half-plane-complex-analysis.md). Therefore a [conformal map](../../../conformal-map.md) is

$$
\boxed{F(z)=i\left(\frac{z-i}{z+i}\right)^2.}
$$

Squaring is injective on this sector because it contains no pair of opposite points. Its [derivative](../../../derivative.md) and the Möbius [derivative](../../../derivative.md) are nonzero in the interior, so the bijection is conformal.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
