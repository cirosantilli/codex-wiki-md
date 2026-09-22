<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The coefficient of the growing term is fixed by the far-field [complex potential](../../../../complex-potential-of-a-two-dimensional-potential-flow.md): $A=\beta e^{i\alpha}$. On $z=ae^{i\theta}$, the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) makes the cylinder a [streamline](../../../../streamline.md), so the imaginary part of $Aa^2e^{2i\theta}+Ba^{-2}e^{-2i\theta}$ must be constant. Choosing the two terms to be complex conjugates makes that constant zero, giving

$$
\boxed{A=\beta e^{i\alpha},\qquad B=a^4\overline A=\beta a^4e^{-i\alpha},\qquad
w=\beta\left(e^{i\alpha}z^2+e^{-i\alpha}\frac{a^4}{z^2}\right).}
$$

This is the zero-[circulation](../../../../circulation-physics.md) solution, also obtained by the [Milne-Thomson circle theorem](../../../../milne-thomson-circle-theorem.md). Impermeability and the leading far field alone permit an additional circulation term $-i\Gamma\log z/(2\pi)$; the requested algebraic form implicitly selects $\Gamma=0$. No [no-slip boundary condition](../../../../no-slip-boundary-condition.md) is imposed on an [inviscid flow](../../../../inviscid-flow.md).

The [streamfunction in polar coordinates](../../../../streamfunction-in-polar-coordinates.md) is

$$
\psi=\beta\left(r^2-\frac{a^4}{r^2}\right)\sin(2\theta+\alpha).
$$

It gives $v_r(a,\theta)=0$ and

$$
v_\theta(a,\theta)=-\left.\partial_r\psi\right|_{a}
=-4a\beta\sin(2\theta+\alpha),\qquad
\boxed{|v_\theta|=4a\beta|\sin(2\theta+\alpha)|.}
$$

The liquid still exerts normal [pressure](../../../../pressure-split.md) on each surface element even though tangential viscous [traction](../../../../traction.md) is absent. For this [steady flow](../../../../steady-flow.md) with zero [vorticity](../../../../vorticity-split.md), the [Bernoulli equation](../../../../bernoulli-equation.md) has one constant $C$ throughout the connected fluid region:

$$
p(a,\theta)=C-\frac12\rho|\mathbf v|^2
=C-8\rho a^2\beta^2\sin^2(2\theta+\alpha).
$$

There is no finite uniform far-field [pressure](../../../../pressure-split.md) to substitute for $C$, because this straining [velocity field](../../../../velocity-field.md) grows with radius. Taking $\mathbf n=(\cos\theta,\sin\theta)$ outward from the cylinder, the fluid [force](../../../../force-split.md) per unit axial width is

$$
\mathbf F=-a\int_0^{2\pi}p(a,\theta)\mathbf n\,d\theta=\boxed{\mathbf0}.
$$

Indeed $p(\theta+\pi)=p(\theta)$ while $\mathbf n(\theta+\pi)=-\mathbf n(\theta)$: diametrically opposite elements cancel exactly. Zero resultant [force](../../../../force-split.md) does not mean zero local [pressure](../../../../pressure-split.md) or zero deformation tendency.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the fluids course of the University of Oxford](../../../split.md)
5. [Fluids course of the University of Oxford](../../../../fluids-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
