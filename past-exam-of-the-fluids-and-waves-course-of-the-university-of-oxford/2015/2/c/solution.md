<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [method of images](../../../../method-of-images.md) places an equal [line source](../../../../line-source.md) at $-ia$, outside the physical [upper half-plane](../../../../upper-half-plane-complex-analysis.md). A convenient [complex potential of a two-dimensional potential flow](../../../../complex-potential-of-a-two-dimensional-potential-flow.md) is

$$
\boxed{w(z)=\frac Q{2\pi}\left[\log(z-ia)+\log(z+ia)\right],\qquad
w'(z)=\frac{Qz}{\pi(z^2+a^2)}.}
$$

The two logarithms can be combined locally as $(Q/(2\pi))\log(z^2+a^2)$; their branches of the [complex logarithm](../../../../complex-logarithm.md) affect only the potential convention, not the single-valued [complex velocity](../../../../complex-velocity.md). The [point source](../../../../point-source.md) in this two-dimensional problem has the [line source](../../../../line-source.md) normalization: its outward [volume flux](../../../../volumetric-flow-rate.md) is $Q$ per unit span.

Writing $R_-^2=x^2+(y-a)^2$, $R_+^2=x^2+(y+a)^2$, and using $w'=u-iv$, the [velocity field](../../../../velocity-field.md) is

$$
\boxed{u=\frac Q{2\pi}\left(\frac{x}{R_-^2}+\frac{x}{R_+^2}\right),\qquad
v=\frac Q{2\pi}\left(\frac{y-a}{R_-^2}+\frac{y+a}{R_+^2}\right).}
$$

On the wall $y=0$, the vertical components cancel:

$$
\boxed{v(x,0)=0,\qquad u(x,0)=\frac{Qx}{\pi(x^2+a^2)}.}
$$

This is the required [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md). Tangential slip is permitted. At large distance the [velocity](../../../../velocity.md) decays as $1/r$, and near $z=ia$ its singular part is exactly that of the specified source; the reflected source is regular throughout the fluid. Away from the injection point, this is an [incompressible flow](../../../../incompressible-flow.md) and an [irrotational flow](../../../../irrotational-flow.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
