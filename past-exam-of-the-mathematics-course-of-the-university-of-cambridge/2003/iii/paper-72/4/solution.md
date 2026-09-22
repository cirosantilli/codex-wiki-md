<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [Rossby wave](../../../../../rossby-wave.md) is a displacement of a materially conserved [potential vorticity](../../../../../potential-vorticity.md) distribution whose induced balanced velocity propagates that displacement. In a [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) interior, take a locally uniform zonal current $U$ and meridional background PV gradient $B=\overline Q_y$. A small meridional parcel displacement $\eta$ produces $q'=-B\eta$. The linear [potential-vorticity equation](../../../../../potential-vorticity-evolution-equation.md) is

$$
(\partial_t+U\partial_x)q'+Bv'=0.
$$

For a shallow-water vertical mode, [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md) is $q'=(\nabla_H^2-L_D^{-2})\psi'$ and $v'=\psi'_x$. Substitution of $e^{i(kx+ly-\omega t)}$ gives

$$
\boxed{\omega=kU-\frac{Bk}{k^2+l^2+L_D^{-2}}.}
$$

The same structure holds for other vertical modes, with their own deformation lengths, and for barotropic waves with $L_D^{-1}=0$. A topographic or shear-induced PV gradient can replace the planetary one: locally $B=\beta-U''$ in a barotropic zonal current, with the corresponding bottom contribution when present.

The restoring process can be seen directly by choosing $\eta=\eta_0\cos(kx-\omega t)$ in one horizontal dimension with no mean flow. Then $q'=-B\eta$ and $\psi'=B\eta/(k^2+L_D^{-2})$. The resulting $v'=\psi'_x$ is a quarter wavelength out of phase with the displacement and requires $\omega=-Bk/(k^2+L_D^{-2})$. A PV anomaly is therefore not merely carried passively: its nonlocal balanced velocity moves the displaced contours.

For $B>0$, the intrinsic zonal [phase velocity](../../../../../phase-velocity.md) is

$$
\boxed{c_x-U=-\frac B{k^2+l^2+L_D^{-2}}<0.}
$$

Changing the sign of $k$ gives the conjugate representation of the same real pattern, not an eastward intrinsic phase branch. More generally the intrinsic phase-velocity vector has nonpositive zonal component $-Bk^2/[|\mathbf k|^2(k^2+l^2+L_D^{-2})]$. This one-way phase property contrasts with acoustic and [internal gravity waves](../../../../../internal-wave.md), whose frequency equations have two independent propagation branches. The direction reverses when the relevant PV gradient reverses; a sufficiently strong current can make the laboratory phase move eastward. Thus one-way refers to propagation relative to the mean flow and a specified gradient, not an absolute geographic direction in every problem.

Scale dependence is supplied by [potential-vorticity inversion](../../../../../potential-vorticity-inversion.md). At short horizontal scales, a fixed PV anomaly creates $\psi'\sim q'/|\mathbf k|^2$, so the intrinsic phase speed is small, of order $B/|\mathbf k|^2$. At long scales with finite $L_D$, it approaches $-BL_D^2$. The [group velocity](../../../../../group-velocity.md) need not have the phase direction:

$$
\boxed{c_{gx}=U+B\frac{k^2-l^2-L_D^{-2}}{(k^2+l^2+L_D^{-2})^2},\qquad
c_{gy}=\frac{2Bkl}{(k^2+l^2+L_D^{-2})^2}.}
$$

In particular, short nearly zonal waves can carry a packet eastward relative to the current while their crests move westward. A group-velocity statement requires a slowly varying, propagating packet and a smooth dispersion branch; turning regions and critical levels require further analysis.

Interior PV gradients are not the only support. In a stratified [quasi-geostrophic approximation](../../../../../quasi-geostrophic-approximation.md) fluid the inversion operator includes $\partial_z[(f^2/N^2)\psi'_z]$. The boundary [buoyancy](../../../../../buoyancy.md) $b'=f\psi'_z$ also supplies inversion data. A meridional boundary-buoyancy gradient is equivalent, in the inversion problem, to a boundary PV sheet. Consequently [Boundary Rossby waves](../../../../../boundary-rossby-wave.md) can exist even if the interior PV gradient vanishes. Their perturbations decay away from the boundary over a horizontal-wavenumber-dependent Rossby height; opposite boundaries can support oppositely directed intrinsic waves because their effective sheet gradients have opposite signs.

The [Eady model](../../../../../eady-model.md) makes this concrete. For $U=\Lambda z$, constant $N$ and horizontal wave-vector magnitude $k_h$, put $K=Nk_h/|f|$. Zero interior PV gives $\psi'_{zz}-K^2\psi'=0$, and each rigid boundary has the buoyancy condition

$$
(U_b-c)\psi'_z-\Lambda\psi'=0.
$$

A lower isolated boundary has $\psi'\propto e^{-Kz}$, so $c_{\rm lower}=U(0)+\Lambda/K$. An upper isolated boundary has $\psi'\propto e^{K(z-H)}$, so $c_{\rm upper}=U(H)-\Lambda/K$. For positive shear, the lower wave is intrinsically eastward and the upper wave intrinsically westward, entirely consistently with their opposite effective PV gradients.

In the [finite-depth Eady dispersion relation](../../../../../finite-depth-eady-dispersion-relation.md), $\gamma=KH/2$. For $\gamma\gg1$, $\tanh\gamma$ and $\coth\gamma$ both tend to one. The square root therefore tends to $\gamma-1$, giving

$$
\boxed{c\longrightarrow\frac\Lambda K\quad\hbox{or}\quad\Lambda H-\frac\Lambda K.}
$$

These are the two uncoupled [Eady edge waves](../../../../../eady-edge-wave.md), not a pair of opposite branches on a single boundary. Their overlap is exponentially small in $KH$. For smaller separation, the interaction can phase-lock the counterpropagating boundary waves; the square root becomes imaginary for $0<KH<2.399\ldots$, yielding [Eady instability](../../../../../eady-instability.md). The short-wave limit is stable and illustrates why interior-PV-only reasoning misses boundary wave propagation and baroclinic instability.

The governing balance requires a small [Rossby number](../../../../../rossby-number.md), weak fractional height or density perturbations, stable stratification where relevant, and frequencies slow relative to $|f|$. The local gradient must change little across a wavelength; on a planetary beta-plane $\beta\ell/|f|\ll1$ is the associated small parameter. A hydrostatic stratified example also requires a small vertical-to-horizontal aspect ratio and $N$ large compared with its slow frequency. For reference, midlatitude $|f|\sim10^{-4}\,\mathrm{s}^{-1}$ and $\beta\sim2\times10^{-11}\,\mathrm{m}^{-1}\mathrm{s}^{-1}$. Atmospheric deformation lengths of order $10^6\,\mathrm m$ give long-wave speeds of order $\beta L_D^2\sim20\,\mathrm{m\,s}^{-1}$ and synoptic-to-planetary times of days to weeks. An oceanic baroclinic deformation length of order $3\times10^4\,\mathrm m$ instead gives about $0.02\,\mathrm{m\,s}^{-1}$ and much longer basin-crossing times. Structural constants and background advection matter; these are scale estimates, not universal measured speeds.

Finite-amplitude [Rossby waves](../../../../../rossby-wave.md) can overturn or strongly filament PV contours, especially near a critical layer where their phase speed approaches the local current. Smooth inviscid motion still conserves each parcel's PV. Apparent mixing comes from the resulting fine structure under coarse-graining or from weak diffusion; it can flatten a coarse-grained background PV gradient and sharpen neighboring jet-edge gradients. A simplest description of [Rossby-wave PV mixing and zonal momentum](../../../../../rossby-wave-pv-mixing-and-zonal-momentum.md) is a downgradient flux

$$
\overline{v'q'}=-\kappa\overline Q_y,\qquad \kappa\ge0.
$$

For barotropic zonal averages with zero mean meridional transport, $u'=-\psi'_y$, $v'=\psi'_x$ and $q'=\nabla_H^2\psi'$. Zonal integration by parts gives the [Taylor identity for quasi-geostrophic flux](../../../../../taylor-identity-for-quasi-geostrophic-flux.md)

$$
\overline{v'q'}=-\partial_y\overline{u'v'},\qquad
\boxed{\partial_t\overline U=-\partial_y\overline{u'v'}=\overline{v'q'}\simeq-\kappa\overline Q_y.}
$$

Thus mixing down a positive PV gradient produces westward acceleration in the mixing region: wave-generated [Reynolds stress](../../../../../reynolds-stress.md) redistributes zonal momentum. The inversion relation $\overline Q_y=\beta-\overline U''$ then relates PV homogenization to a reshaped current. Total zonal momentum cannot simply disappear in an isolated domain; integrated stress convergence is a boundary flux, so compensating momentum changes or boundary forcing must accompany localized drag.

In small conservative waves with $B>0$, the quadratic [wave activity](../../../../../wave-activity.md) is $\mathcal A=\overline{q'^2}/(2B)$. Multiplying the linear PV equation by $q'/B$ gives $\mathcal A_t=-\overline{v'q'}$ for a zonal average on a locally uniform current. Together with the momentum equation this yields $\partial_t(\overline U+\mathcal A)=0$ during conservative growth or decay. In a commonly used momentum convention the Rossby-wave pseudomomentum is $-\mathcal A$; signs must be stated rather than inferred from the word activity. Breaking and absorption invalidate the reversible small-wave description and deposit the wave's momentum through its flux convergence. A steady undamped conservative wave cannot provide sustained local drag without a flux divergence or boundary exchange, as expressed by the [non-acceleration theorem for quasi-geostrophic waves](../../../../../non-acceleration-theorem-for-quasi-geostrophic-waves.md).

**Rossby propagation is the slow, direction-selective motion produced by PV advection coupled to balanced inversion.** Interior gradients and boundary sheets share that mechanism; inversion determines the scale dependence, while wave packets, boundary-wave interaction and breaking govern how energy and momentum reach other regions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 72](../../paper-72-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
