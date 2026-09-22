<h1 id="section-b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the thin-annulus approximation stated in the source, so $u_r'+iku_z=0$. Let

$$
A(r)=2\Omega+r\Omega'=\frac1r(r^2\Omega)',\qquad
\kappa_{\rm ep}^2=2\Omega A=\frac1{r^3}(r^4\Omega^2)'.
$$

Here $\kappa_{\rm ep}^2$ is the conventional [Rayleigh discriminant](../../../../../rayleigh-discriminant.md), also the squared local [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) when positive. For $k\ne0$ and $\omega\ne0$, the azimuthal and axial mode equations give

$$
u_\phi=-\frac{iA}{\omega}u_r,\qquad u_z=\frac k\omega\pi.
$$

The thin-gap [incompressible flow](../../../../../incompressible-flow.md) condition then gives $\pi=i\omega u_r'/k^2$. Substitute these into the radial equation:

$$
-i\omega u_r+\frac{2i\Omega A}{\omega}u_r=-\pi',\qquad
\frac{i\omega}{k^2}u_r''=\frac{i(\omega^2-\kappa_{\rm ep}^2)}\omega u_r.
$$

Thus

$$
u_r''=k^2\left(1-\frac{\kappa_{\rm ep}^2}{\omega^2}\right)u_r.
$$

To put this into exactly the form printed in the paper, define

$$
\boxed{\Phi(r)=-\kappa_{\rm ep}^2
=-\frac{2\Omega}{r}(r^2\Omega)'
=-\frac1{r^3}(r^4\Omega^2)'.}
$$

The [narrow-gap centrifugal stability equation](../../../../../narrow-gap-centrifugal-stability-equation.md) is consequently

$$
\boxed{-u_r''+\frac{k^2}{\omega^2}\Phi(r)u_r=-k^2u_r.}
$$

The two rigid cylinders are impermeable, so the [no-penetration boundary condition](../../../../../no-penetration-boundary-condition.md) gives

$$
\boxed{u_r(R_<)=u_r(R_>)=0.}
$$

There is no inviscid no-slip condition on the tangential or axial components.

The sign deserves emphasis: the source's printed plus sign makes its $\Phi$ the negative of the conventional [Rayleigh discriminant](../../../../../rayleigh-discriminant.md). Using the conventional positive discriminant instead requires a minus sign in front of that potential term. These are equivalent conventions; replacing one without adjusting the other would falsely predict instability of [solid-body rotation](../../../../../solid-body-rotation.md). The $k=0$ and marginal $\omega=0$ cases, excluded by these eliminations, must be treated separately or by limits.

## ↑ Ancestors (14)

1. [D](../d.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
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
