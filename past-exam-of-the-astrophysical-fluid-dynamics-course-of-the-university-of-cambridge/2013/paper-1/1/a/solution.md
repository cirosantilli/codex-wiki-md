<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $x$ measure distance down the incline and $y$ distance perpendicular to it, with the wall at $y=0$ and the [free surface](../../../../../free-surface.md) at $y=h$. A uniform steady [falling film flow](../../../../../falling-film-flow.md) has $\mathbf u=u(y)\mathbf e_x$. Its [convective acceleration](../../../../../convective-acceleration.md) vanishes because $\mathbf u\cdot\nabla=u\partial_x$ and $\partial_xu=0$. A flat surface exposed to constant atmospheric [pressure](../../../../../pressure-split.md) has

$$
p(y)=p_{\rm atm}+\rho g\cos\alpha\,(h-y).
$$

Thus $\partial_xp=0$, and the downslope component of the [Navier-Stokes equations](../../../../../navier-stokes-equation.md) reduces to $0=g\sin\alpha+(\eta/\rho)u''$. The printed pressure-free equation must be understood as this **downslope projection**: its full vector version would incorrectly omit the normal [hydrostatic pressure](../../../../../hydrostatic-pressure.md) gradient that balances $g\cos\alpha$.

The [no-slip boundary condition](../../../../../no-slip-boundary-condition.md) gives $u(0)=0$. Neglecting air [shear stress](../../../../../shear-stress.md) makes the surface shear-free, so $u'(h)=0$. Two integrations give the [uniform gravity-driven Newtonian film](../../../../../uniform-gravity-driven-newtonian-film.md) profile

$$
u'(y)=\frac{\rho g\sin\alpha}{\eta}(h-y),\qquad
u(y)=\frac{\rho g\sin\alpha}{\eta}\left(hy-\frac{y^2}{2}\right).
$$

The [velocity](../../../../../velocity.md) increases up to the [free surface](../../../../../free-surface.md), where

$$
\boxed{u_{\max}=\frac{\rho gh^2\sin\alpha}{2\eta}.}
$$

This assumes a uniform laminar [Newtonian fluid](../../../../../newtonian-fluid.md) film, a stationary wall and negligible surface shear; a varying thickness or externally imposed downslope [pressure gradient](../../../../../pressure-gradient.md) would alter the balance.

<a id="1/a/image-uniform-inclined-film-surface-speed-maximum-and-normal-hydrostatic-pressure"></a>
![](../../../../../past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1-inclined-film.png)

**[Figure 1](#1/a/image-uniform-inclined-film-surface-speed-maximum-and-normal-hydrostatic-pressure). Uniform inclined film: surface speed maximum and normal hydrostatic pressure**.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
