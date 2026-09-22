<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

The curvature-minus-one [Poincaré disk model](../../../../../poincare-disk-model.md) has [Riemannian metric](../../../../../riemannian-metric.md)

$$
\boxed{ds^2=\frac{4|dw|^2}{(1-|w|^2)^2}},\qquad |w|<1.
$$

The [geodesics](../../../../../geodesic.md) through zero are Euclidean diameters. Indeed, for a path written in polar coordinates, its length is at least $\int2|\dot r|/(1-r^2)\,dt$, and hence at least $2\operatorname{artanh}r$ between zero and a point of modulus $r$. The radial segment attains this lower bound. By uniqueness of a [geodesic](../../../../../geodesic.md) with given initial tangent, these radial paths describe all [geodesics](../../../../../geodesic.md) through the origin. The radial [hyperbolic distance](../../../../../hyperbolic-distance.md) is

$$
\rho=\int_0^r\frac{2\,ds}{1-s^2}=\log\frac{1+r}{1-r},
\qquad \boxed{r=\tanh(\rho/2)}.
$$

Thus a [hyperbolic circle in the Poincare disc](../../../../../hyperbolic-circle-in-the-poincare-disc.md) is the indicated Euclidean circle.

An [isometry](../../../../../isometry.md) from the [Poincaré half-plane model](../../../../../poincare-half-plane-model.md) to the [Poincaré disk model](../../../../../poincare-disk-model.md) is the [Cayley transform between the half-plane and disk](../../../../../cayley-transform-between-the-half-plane-and-disk.md),

$$
w=\frac{z-i}{z+i},\qquad z=i\frac{1+w}{1-w}.
$$

Writing $z=x+iy$, one has $1-|w|^2=4y/|z+i|^2$ and $|dw|^2=4|dz|^2/|z+i|^4$. Substitution into the disk [Riemannian metric](../../../../../riemannian-metric.md) gives $ds^2=|dz|^2/y^2$, the half-plane [metric](../../../../../metric.md), and $i$ maps to zero.

Put $r=\tanh(\rho/2)$. The inverse image of $|w|=r$ obeys

$$
x^2+(y-1)^2=r^2\bigl(x^2+(y+1)^2\bigr).
$$

Since $(1+r^2)/(1-r^2)=\cosh\rho$, completing the square yields

$$
\boxed{x^2+(y-\cosh\rho)^2=\sinh^2\rho}.
$$

This proves that the [hyperbolic circle in the upper half-plane](../../../../../hyperbolic-circle-in-the-upper-half-plane.md) has Euclidean centre $i\cosh\rho$ and radius $\sinh\rho$.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
