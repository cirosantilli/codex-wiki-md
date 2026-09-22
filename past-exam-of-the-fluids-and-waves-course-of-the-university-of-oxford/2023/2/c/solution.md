<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $q=W'=u-iv$, the [Blasius force theorem](../../../../blasius-force-theorem.md) states that the [force](../../../../force-split.md) per unit length exerted by a steady [incompressible flow](../../../../incompressible-flow.md) and [irrotational flow](../../../../irrotational-flow.md) on an impermeable body is

$$
X-iY=\frac{i\rho}{2}\oint_C q(z)^2\,dz,
$$

where $C$ runs counterclockwise around the body and excludes external flow singularities. The sign corresponds to the [force](../../../../force-split.md) on the body.

Let $c=a^2/b$ and $A=ma^2e^{-i\alpha}/b^2$. The [complex velocity](../../../../complex-velocity.md) may be written

$$
q(z)=\frac{A}{(z-c)^2}+H(z),\qquad
H(z)=-\frac{me^{i\alpha}}{(z-b)^2}.
$$

Only the image point $c$ lies inside the circular contour. The term $A^2/(z-c)^4$ has zero [residue](../../../../residue.md); $H^2$ is regular there. In the cross term, the linear term of the [Taylor expansion](../../../../taylor-expansion.md) of $H$ supplies

$$
\operatorname{Res}_{z=c}q^2
=2AH'(c)
=\frac{4m^2a^2}{b^2(c-b)^3}
=-\frac{4m^2a^2b}{(b^2-a^2)^3}.
$$

The orientation factors have canceled. The [residue theorem](../../../../residue-theorem.md) now gives

$$
X-iY=-\pi\rho\operatorname{Res}_{z=c}q^2,
\qquad
\boxed{X=\frac{4\pi\rho m^2a^2b}{(b^2-a^2)^3},\qquad Y=0}.
$$

Since $b>a$, $X>0$: the obstacle is pulled toward the doublet, independently of $\alpha$. This is a [force](../../../../force-split.md) per unit length perpendicular to the plane of flow.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
