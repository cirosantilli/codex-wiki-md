<h1 id="g/g2/solution">Solution</h1>

↑ **Parent:** [G2](../g2.md)

For a normal constrained extremal, introduce a constant [Lagrange multiplier](../../../../lagrange-multiplier.md) and use $L=F-\lambda G$. The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\boxed{L_y-\frac d{dx}L_{y'}=0.}
$$

When both integrands have no explicit $x$ dependence, the [Beltrami identity](../../../../beltrami-identity.md) gives $L-y'L_{y'}=\text{constant}$, as follows by differentiating this expression and using the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md).

Parametrize the surface by $(f(z)\cos\theta,f(z)\sin\theta,z)$. The [cross product](../../../../cross-product.md) of its two coordinate tangents has magnitude $f\sqrt{1+(f')^2}$, so integration in $\theta$ gives $A=2\pi\int_a^bf\sqrt{1+(f')^2}\,dz$. Integrating the cross-sectional disk areas gives $V=\pi\int_a^bf^2\,dz$.

Dividing the augmented functional $A-\lambda V$ by $\pi$, use

$$
L=2f\sqrt{1+(f')^2}-\lambda f^2.
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is

$$
\boxed{\frac d{dz}\left(\frac{2ff'}{\sqrt{1+(f')^2}}\right)
-2\sqrt{1+(f')^2}+2\lambda f=0.}
$$

The [Beltrami identity](../../../../beltrami-identity.md) becomes $2f/\sqrt{1+(f')^2}-\lambda f^2=C$. At an endpoint $f\to0$, the absolute value of the first term is at most $2f$, so $C=0$, even if the profile has an infinite endpoint slope. For a nondegenerate regular closed surface take $f>0$ on $(a,b)$. Then $\lambda>0$, and, with $R=2/\lambda$,

$$
f^2(1+(f')^2)=R^2.
$$

Combining this identity with the [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) yields $f''=-R^2/f^3$. Consequently $(f^2)''=2((f')^2+ff'')=-2$. The two zero endpoint values uniquely determine

$$
\boxed{f(z)^2=(z-a)(b-z)
=\left(\frac{b-a}{2}\right)^2-\left(z-\frac{a+b}{2}\right)^2.}
$$

The positive radius profile is therefore a semicircle and generates a [sphere](../../../../sphere.md), centred at height $(a+b)/2$, with radius $R=(b-a)/2$. In particular

$$
\boxed{\lambda=\frac2R=\frac4{b-a}.}
$$

The [graph](../../../../graph-split.md) is smooth in the interior; its vertical slopes at the two poles are compatible with a smooth spherical surface. Its [volume](../../../../volume.md) is $4\pi R^3/3$, the [volume](../../../../volume.md) associated with this stationary candidate.

For minimality, the three-dimensional [isoperimetric inequality](../../../../isoperimetric-inequality.md) says that every closed surface enclosing [volume](../../../../volume.md) $V$ has $A^3\geq36\pi V^2$, with equality for a [sphere](../../../../sphere.md). The displayed extremal attains equality, proving that it minimizes area at its fixed enclosed [volume](../../../../volume.md). The uniqueness above concerns the regular connected positive profile with the two stated endpoint heights.

## ↑ Ancestors (12)

1. [G2](../g2.md)
2. [G](../../g.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options II course of the University of Oxford](../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
