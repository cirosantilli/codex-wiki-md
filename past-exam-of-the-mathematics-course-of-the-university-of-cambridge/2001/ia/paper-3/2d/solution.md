<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

A [Möbius transformation](../../../../../mobius-transformation.md) is $M_A(z)=(az+b)/(cz+d)$ with $\Delta=ad-bc\ne0$. On the [Riemann sphere](../../../../../riemann-sphere.md), a zero denominator represents infinity, and $M_A(\infty)=a/c$ when $c\ne0$; when $c=0$, infinity is fixed. The numerator and denominator cannot vanish together because $\Delta\ne0$.

The [matrix](../../../../../matrix.md) $A=\left(\begin{smallmatrix}a&b\\c&d\end{smallmatrix}\right)$ acts on homogeneous coordinates $[z:1]$, so composition satisfies $M_A\circ M_B=M_{AB}$. The product is invertible since $\det(AB)=\det A\det B\ne0$, proving closure. Composition is associative because these are maps of the sphere. The identity is $z\mapsto z$, and

$$
M_A^{-1}(z)=\frac{dz-b}{-cz+a}
$$

is again a [Möbius transformation](../../../../../mobius-transformation.md). Thus the transformations form a [group](../../../../../group-split.md). Nonzero scalar multiples of a [matrix](../../../../../matrix.md) give the same transformation, but the identity and inverse assertions concern the transformations themselves.

Write $T_q(z)=z+q$, $S_k(z)=kz$ with $k\ne0$, and $H(z)=1/z$. If $c=0$, then $a,d\ne0$ and $M_A=T_{b/d}\circ S_{a/d}$. If $c\ne0$, division gives

$$
\frac{az+b}{cz+d}=\frac ac-\frac{\Delta/c^2}{z+d/c}.
$$

Hence the [Möbius translation-scaling-inversion factorization](../../../../../mobius-translation-scaling-inversion-factorization.md) is

$$
\boxed{M_A=T_{a/c}\circ S_{-\Delta/c^2}\circ H\circ T_{d/c}\quad(c\ne0).}
$$

The scaling coefficient is nonzero. At $z=-d/c$ the reciprocal sends the translated zero to infinity; at infinity it sends infinity to zero. Thus the factorization holds on the entire [Riemann sphere](../../../../../riemann-sphere.md), including both exceptional points, and proves the stated generating property.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
