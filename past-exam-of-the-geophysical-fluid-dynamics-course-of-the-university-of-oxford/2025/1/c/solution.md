<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the [velocity field](../../../../velocity-field.md) as $u=U+u\prime$, $v=v\prime$. The uniform background has zero [relative vorticity](../../../../relative-vorticity.md), and the perturbation has $\xi\prime=v\prime_x-u\prime_y$. Keeping only terms linear in the perturbations gives

$$
\boxed{(\partial_t+U\partial_x)\xi\prime+\beta v\prime=0.}
$$

The [incompressibility condition](../../../../incompressible-flow.md) permits a [streamfunction](../../../../stream-function.md) $\psi$ with $u\prime=-\psi_y$, $v\prime=\psi_x$, hence $\xi\prime=\nabla_h^2\psi$. Thus the [Linear Rossby-wave equation](../../../../linear-rossby-wave-equation.md) here is

$$
(\partial_t+U\partial_x)\nabla_h^2\psi+\beta\psi_x=0.
$$

Choose a [plane wave](../../../../plane-wave.md) $\psi=\operatorname{Re}\{\widehat\psi e^{i(kx+ly-\omega t)}\}$, with $K^2=k^2+l^2>0$. Substitution gives

$$
i(\omega-Uk)K^2\widehat\psi+i\beta k\widehat\psi=0,
$$

and therefore the [local Rossby-wave dispersion relation in a zonal jet](../../../../local-rossby-wave-dispersion-relation-in-a-zonal-jet.md)

$$
\boxed{\omega=Uk-\frac{\beta k}{k^2+l^2}.}
$$

The $Uk$ term is the background [Doppler shift](../../../../doppler-effect.md); the intrinsic [phase velocity](../../../../phase-velocity.md) is westward. A real physical [wave](../../../../wave-split.md) can always be represented using the conjugate [wavevector](../../../../wavevector.md) if necessary to choose $\omega\geq0$.

The relevant ground-frame zonal [phase velocity](../../../../phase-velocity.md) and [group velocity](../../../../group-velocity.md) are

$$
c_{p,x}=\frac\omega k=U-\frac\beta{K^2},\qquad
c_{g,x}=\frac{\partial\omega}{\partial k}
=U+\frac{\beta(k^2-l^2)}{K^4},\qquad
c_{g,y}=\frac{\partial\omega}{\partial l}=\frac{2\beta kl}{K^4}.
$$

**Time increases downward in the source diagram.** The individual phase contours lean towards increasing longitude as time increases, so their [phase velocity](../../../../phase-velocity.md) is eastward. The envelope moves eastward faster: successive crests grow at the downstream edge and decay upstream. This illustrates [Rossby-wave downstream development](../../../../rossby-wave-downstream-development.md).

For the intended purely zonal [wave packet](../../../../wave-packet.md), $l=0$, and

$$
c_p=U-\frac\beta{k^2}>0,\qquad c_g=U+\frac\beta{k^2}>U.
$$

Consequently, with $U,\beta>0$ and the positive-frequency choice $k>0$,

$$
\boxed{k>\sqrt{\beta/U}.}
$$

There is a small interpretation qualification: if “zonally propagating” specified only the plotted direction while allowing an unknown nonzero meridional [wavenumber](../../../../wavenumber.md), eastward [phase velocity](../../../../phase-velocity.md) alone would imply $k^2+l^2>\beta/U$, not the stronger bound on $k$ alone. In this uniform model a strictly zonal [group velocity](../../../../group-velocity.md) with $\beta k\ne0$ does imply $l=0$, which supplies the intended interpretation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
