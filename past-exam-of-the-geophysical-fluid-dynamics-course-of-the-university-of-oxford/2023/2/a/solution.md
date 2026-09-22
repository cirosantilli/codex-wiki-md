<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use eastward $x$, northward $y$, [pressure coordinate](../../../../pressure-coordinate.md) $p$ increasing downward, and [geopotential](../../../../geopotential.md) $\Phi=gz$. Horizontal derivatives are taken on an [isobaric surface](../../../../isobaric-surface.md). The horizontal [geostrophic balance](../../../../geostrophic-balance.md) and vertical [hydrostatic balance](../../../../hydrostatic-balance.md) are

$$
f u_g=-\Phi_y,\qquad f v_g=\Phi_x,\qquad
\Phi_p=-\frac1\rho=-\frac{RT}{p},
$$

where $R$ is the [specific gas constant](../../../../specific-gas-constant.md) of dry air and the final equality uses the [ideal gas law](../../../../ideal-gas-law.md). At fixed latitude $f$ is independent of $p$. Cross-differentiating gives

$$
f\,\partial_pu_g=-\partial_y\Phi_p=\frac R p\,T_y,
\qquad
f\,\partial_pv_g=\partial_x\Phi_p=-\frac R p\,T_x.
$$

Consequently the pressure-coordinate [thermal wind](../../../../thermal-wind.md) equations are

$$
\boxed{\frac{\partial u_g}{\partial\ln p}=\frac Rf\frac{\partial T}{\partial y},
\qquad
\frac{\partial v_g}{\partial\ln p}=-\frac Rf\frac{\partial T}{\partial x}.}
$$

Equivalently, $f\mathbf e_z\mathbin\times\partial_{\ln p}\mathbf u_g=R\nabla_pT$. Notice the sign: increasing eastward [velocity](../../../../velocity.md) upward means decreasing eastward [velocity](../../../../velocity.md) with $\ln p$, and hence poleward-decreasing [temperature](../../../../temperature-split.md) in the Northern Hemisphere.

For the [stratospheric polar vortex](../../../../stratospheric-polar-vortex.md) estimate, the original diagram must be read on its logarithmic pressure axis. Near $60^\circ$ in the winter hemisphere, adjacent $10\ \mathrm{m\,s^{-1}}$ wind contours suggest an increase of roughly $20\ \mathrm{m\,s^{-1}}$ through a pressure decade surrounding $10\ \mathrm{mb}$: for example, about $10\ \mathrm{m\,s^{-1}}$ near $30\ \mathrm{mb}$ and $30\ \mathrm{m\,s^{-1}}$ near $3\ \mathrm{mb}$. These are coarse graphical readings, not a sounding. Thus

$$
\frac{\partial u_g}{\partial\ln p}\simeq
\frac{30-10}{\ln(3/30)}\ \mathrm{m\,s^{-1}}
\simeq-8.7\ \mathrm{m\,s^{-1}}.
$$

With $|f|=2\Omega\sin60^\circ\simeq1.26\times10^{-4}\ \mathrm{s^{-1}}$ and $R\simeq287\ \mathrm{J\,kg^{-1}\,K^{-1}}$, the poleward [temperature gradient](../../../../temperature-gradient.md) is approximately

$$
\frac{\partial T}{\partial y_{\rm pole}}
\simeq\frac{|f|}{R}\frac{\partial u_g}{\partial\ln p}
\simeq-3.8\times10^{-6}\ \mathrm{K\,m^{-1}}
\simeq-0.42\ \mathrm{K\ per\ degree\ latitude}.
$$

If the vortex edge is taken to span roughly $50^\circ$ to $70^\circ$, its width is $a(20\pi/180)\simeq2.2\times10^6\ \mathrm m$, giving

$$
\boxed{T(70^\circ)-T(50^\circ)\simeq-8.5\ \mathrm K,
\quad\text{a poleward drop of order }10\ \mathrm K.}
$$

The estimate depends on the width assigned to the edge and the graphical [vertical shear](../../../../vertical-shear.md); a range of several to roughly fifteen kelvin is more justified than a precise value. The sign remains a cold winter pole in either hemisphere. The diagram does not by itself prescribe a unique pair of edge latitudes.

At low latitudes, horizontal free-atmospheric [temperature gradients](../../../../temperature-gradient.md) are usually much smaller than at the winter vortex edge. For a comparable finite wind [vertical shear](../../../../vertical-shear.md), the rearranged [thermal-wind balance](../../../../thermal-wind.md), $T_y=(f/R)u_{\ln p}$, is consistent with weaker [temperature gradients](../../../../temperature-gradient.md) as $|f|$ decreases. However, [geostrophic balance](../../../../geostrophic-balance.md) loses validity near the equator because the [Coriolis parameter](../../../../coriolis-parameter.md) vanishes; division by $f$ cannot be used there to derive a prediction. The [weak temperature gradient approximation](../../../../weak-temperature-gradient-approximation.md) is better motivated by rapid horizontal [internal gravity wave](../../../../internal-wave.md) adjustment, together with tropical [convection](../../../../convection-split.md) and the [Hadley cell](../../../../hadley-cell.md). [Thermal-wind balance](../../../../thermal-wind.md) describes the balanced extratropical relation and its tendency approaching the tropics; it is not a complete causal explanation of equatorial thermal uniformity.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
