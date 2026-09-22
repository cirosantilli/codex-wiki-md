<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the proposed [plane wave](../../../../plane-wave.md), define the positive squared effective [wavenumber](../../../../wavenumber.md)

$$
\mathcal K^2=k^2+l^2+\frac{f_0^2}{N^2}m^2.
$$

The horizontal [Laplacian](../../../../laplacian.md) contributes $-(k^2+l^2)\psi'$ and the vertical stretching operator contributes $-(f_0^2/N^2)m^2\psi'$. Substitution in the [Linear Rossby-wave equation](../../../../linear-rossby-wave-equation.md) therefore gives

$$
[-i(\omega-Uk)](-\mathcal K^2)+i\beta k=0,
\qquad
\boxed{\omega=Uk-\frac{\beta k}{k^2+l^2+(f_0^2/N^2)m^2}.}
$$

The intrinsic [phase velocity](../../../../phase-velocity.md) is westward for positive $\beta$. A stationary disturbance with $\omega=0$ and $k\ne0$ must have its westward intrinsic [phase velocity](../../../../phase-velocity.md) exactly cancelled by the eastward background current. Solving for the squared vertical [wavenumber](../../../../wavenumber.md) yields

$$
m^2=\frac{N^2}{f_0^2}\left(\frac\beta U-k^2-l^2\right).
$$

For [Earth](../../../../earth.md), with northward $y$, $\beta=2\Omega\cos\phi/a>0$ in both hemispheres away from the poles. Thus an oscillatory vertical structure requires

$$
\boxed{0<U<\frac\beta{k^2+l^2},\qquad N^2>0,\quad f_0\ne0,\quad k\ne0.}
$$

The background flow must be eastward but not too strong for the chosen horizontal scale. Long horizontal [wavelengths](../../../../wavelength.md) have the largest allowed speed. An easterly current, $U<0$, gives $m^2<0$ and an [evanescent wave](../../../../evanescent-wave.md); so does an eastward current exceeding the upper bound. At equality $m=0$ and the vertical [group velocity](../../../../group-velocity.md) vanishes. A zonally uniform disturbance, $k=0$, is a degenerate stationary pattern with no vertical [Rossby wave](../../../../rossby-wave.md) energy propagation, so it cannot be obtained by cancelling $k$ in the preceding calculation.

A real $m$ alone does not select _upward_ propagation. Differentiate the [dispersion relation](../../../../dispersion-relation-split.md) at fixed $k,l$ to obtain the vertical [group velocity](../../../../group-velocity.md):

$$
c_{g,z}=\frac{\partial\omega}{\partial m}
=\frac{2\beta k(f_0^2/N^2)m}
{[k^2+l^2+(f_0^2/N^2)m^2]^2}.
$$

The outgoing [radiation condition](../../../../radiation-condition.md) for a surface source requires

$$
\boxed{c_{g,z}>0\quad\Longleftrightarrow\quad km>0\quad(\beta>0).}
$$

For the convention $k>0$, take $m>0$. The stationary [phase](../../../../phase-waves.md) lines then obey $dx/dz=-m/k<0$: they tilt westward with height while [wave energy](../../../../wave-energy.md) travels upward. The real conjugate component $(-k,-l,-m)$ describes the same physical upward-propagating wave.

The figure suggests a winter extratropical path from the lower [terrestrial atmosphere](../../../../terrestrial-atmosphere.md) into the [stratosphere](../../../../stratosphere.md), where the mean [zonal flow](../../../../zonal-flow.md) is eastward. The summer [stratosphere](../../../../stratosphere.md) has westward flow and blocks such stationary [Rossby waves](../../../../rossby-wave.md) in this idealization. A zero-wind surface is a stationary-wave [critical layer in a shear flow](../../../../critical-layer-in-a-shear-flow.md); it also bounds the winter westerlies aloft near the upper part of the diagram. For a slowly varying real wind profile, local propagation needs $m^2(z)>0$ along the path, sufficient surface forcing, and no intervening absorbing [critical layer in a shear flow](../../../../critical-layer-in-a-shear-flow.md). A layer where the eastward wind becomes too strong is a turning barrier for the given horizontal [wavenumbers](../../../../wavenumber.md). The uniform-current result is a local guide, not a complete prediction through a sheared spherical [terrestrial atmosphere](../../../../terrestrial-atmosphere.md).

For scale, at $60^\circ$ latitude $\beta\simeq1.14\times10^{-11}\ \mathrm{m^{-1}\,s^{-1}}$. A planetary [zonal wavenumber](../../../../zonal-wavenumber.md) $s$ has local $k=s/(a\cos\phi)$. Taking $l=0$ gives the most permissive limit

$$
U_{\max}=\frac{\beta a^2\cos^2\phi}{s^2}
\simeq\frac{116}{s^2}\ \mathrm{m\,s^{-1}}.
$$

The resulting limits are approximately $116$, $29$ and $13\ \mathrm{m\,s^{-1}}$ for $s=1,2,3$. Therefore the long planetary waves are favored; the strong core of the winter vortex can exclude shorter ones even though it is westerly. Nonzero meridional [wavenumber](../../../../wavenumber.md) lowers these limits further. A compressible [log-pressure coordinate](../../../../log-pressure-coordinate.md) model would also contain a density-scale-height correction; it is absent from the equation supplied here and should not be silently inserted.

Interchanging the Northern and Southern Hemispheres changes the sign of $f_0$, but only $f_0^2$ enters the [dispersion relation](../../../../dispersion-relation-split.md) and vertical [group velocity](../../../../group-velocity.md). With the same eastward $x$ and northward $y$, $\beta$ stays positive. Thus the **propagation criterion is the same in both hemispheres**: it selects the winter westerlies, irrespective of which hemisphere is winter. Actual amplitudes can differ because mountains, land-sea contrasts, forcing spectra and mean winds differ between hemispheres; those source differences do not reverse this propagation criterion.

## ↑ Ancestors (12)

1. [C](../c.md)
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
