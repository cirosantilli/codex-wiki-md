<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a zonal background $U(y)$, its [relative vorticity](../../../../relative-vorticity.md) is $\overline\xi=-U_y$. The meridional [absolute vorticity](../../../../absolute-vorticity.md) gradient is therefore

$$
Q_y=\beta-U_{yy},\qquad
\beta=\frac{2\Omega\cos\phi}{a}.
$$

At $30^\circ\mathrm N$,

$$
\boxed{\beta\simeq1.98\times10^{-11}\ \mathrm{m^{-1}\,s^{-1}}.}
$$

A localized [jet stream](../../../../jet-stream.md) of [velocity](../../../../velocity.md) scale $U=134\ \mathrm{m\,s^{-1}}$ and width $L$ has

$$
\boxed{|\overline\xi_y|=|U_{yy}|\sim\frac U{L^2}
=1.34\times10^{-10}\left(\frac{1000\ \mathrm{km}}L\right)^2
\mathrm{m^{-1}\,s^{-1}}.}
$$

For $L=1000$--$2000\ \mathrm{km}$ this is about $1.7$--$6.8$ times the planetary contribution, so wind curvature cannot generally be neglected. The coefficient in this scaling depends on the chosen jet profile and width convention.

Linearizing the [vorticity equation](../../../../vorticity-equation.md) now gives the [Rossby-wave equation for a sheared zonal current](../../../../rossby-wave-equation-for-a-sheared-zonal-current.md)

$$
(\partial_t+U(y)\partial_x)\nabla_h^2\psi+(\beta-U_{yy})\psi_x=0.
$$

For a qualitative estimate at the jet core, freeze the local coefficients. At a smooth maximum $U_{yy}<0$, so $Q_y>\beta$: the restoring [absolute vorticity](../../../../absolute-vorticity.md) gradient is stronger. The [local Rossby-wave dispersion relation in a zonal jet](../../../../local-rossby-wave-dispersion-relation-in-a-zonal-jet.md) gives, for the same local $U$ and zonal [wavenumber](../../../../wavenumber.md) $k$ with $l=0$,

$$
c_p=U-\frac{Q_y}{k^2},\qquad c_g=U+\frac{Q_y}{k^2},
$$

so

$$
\boxed{\Delta c_p=\frac{U_{yy}}{k^2}<0,\qquad
\Delta c_g=-\frac{U_{yy}}{k^2}>0.}
$$

The envelope in the diagram would advance eastward faster, while individual phase contours would advance more slowly eastward, become stationary if $Q_y=Uk^2$, or move westward if $Q_y>Uk^2$. The separation between envelope and phase speeds increases. On a plot with time downward, compare horizontal displacement at fixed time: the envelope moves farther right, while a given phase moves less far right, or left after reversal. If the [frequency](../../../../frequency.md) changes sign for a fixed signed $k$, conjugate the mode to restore the convention $\omega\geq0$; the physical propagation is unchanged.

This conclusion concerns the concave-down jet core. On a flank with $U_{yy}>0$ the correction has the opposite sign; the value at the edge of the [Hadley cell](../../../../hadley-cell.md) alone does not specify the curvature everywhere. Indeed the angular-momentum-conserving profile in 1(a) is a rising inner branch, not a complete smooth jet maximum. A global sheared-current [normal mode](../../../../normal-mode.md) requires its meridional structure and boundary conditions; the local calculation is the qualitative estimate requested.

## ↑ Ancestors (12)

1. [D](../d.md)
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
