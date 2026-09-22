<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the elastic-rod bending functional for an abstract inextensible [worm-like chain](../../../../worm-like-chain.md),

$$
G_b=\frac{\kappa}{2}\int C(s')^2\,ds',\qquad\kappa=l_pk_BT.
$$

A circular ring of radius $R$ has [curvature](../../../../curvature.md) $1/R$ and length $2\pi R$, hence [energy](../../../../energy-split.md) $\pi\kappa/R$. With $n(R_i)$ rings of each radius, add their energies:

$$
\boxed{G_b=\pi l_pk_BT\sum_i\frac{n(R_i)}{R_i}.}
$$

For a cylindrical annulus of height $h$, choose neighboring rings separated vertically by $s$. Then $n=h/s$, while adjacent radial layers are separated by $\sqrt3s/2$. Replacing the radial sum by its continuum integral gives

$$
L=\frac{2}{\sqrt3s}\int_{R_{\rm in}}^{R_{\rm out}}2\pi R\frac hs\,dR
=\frac{2\pi h}{\sqrt3s^2}(R_{\rm out}^2-R_{\rm in}^2),
$$

and

$$
G_b=\frac{2\pi l_pk_BTh}{\sqrt3s^2}\int_{R_{\rm in}}^{R_{\rm out}}\frac{dR}{R}
=\frac{2\pi l_pk_BTh}{\sqrt3s^2}\ln\frac{R_{\rm out}}{R_{\rm in}}.
$$

Eliminate the inner radius to obtain

$$
\boxed{G_b=\frac{\pi l_pk_BTh}{\sqrt3s^2}
\ln\!\left[\frac{R_{\rm out}^2}{R_{\rm out}^2-\sqrt3Ls^2/(2\pi h)}\right].}
$$

The dimensions are [energy](../../../../energy-split.md), and the expression is positive for $0<L<2\pi hR_{\rm out}^2/(\sqrt3s^2)$. It tends to zero with $L$ and diverges as the inner hole closes in this continuum model. The divergence signals the growing cost of forcing an inextensible chain to zero radius; it is not a physical prediction at arbitrarily small molecular scales. Interstrand, hydration and configurational contributions have been excluded, and disconnected ideal rings represent local [curvature](../../../../curvature.md) without modeling the connections between them.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
