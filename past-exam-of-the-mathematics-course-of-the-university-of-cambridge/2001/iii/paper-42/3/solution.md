<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $z=0$ to be the vertical equilibrium plane and expand the vertical gravitational force to leading order in $H/r\ll1$: $\partial_z\Phi\simeq\Omega_z^2z$. The vertical [hydrostatic equilibrium](../../../../../hydrostatic-equilibrium.md) equation for uniform [density](../../../../../density.md) is $\partial_zp_0=-\rho\Omega_z^2z$. With vacuum [pressure](../../../../../pressure.md) at both [free surfaces](../../../../../free-surface.md), it gives

$$
\boxed{p_0(r,z)=\frac12\rho\Omega_z(r)^2[H(r)^2-z^2],\qquad |z|\leq H.}
$$

The associated radial [pressure](../../../../../pressure.md) correction is small at leading thin-disk order; use the prescribed orbital and [radial epicyclic frequency](../../../../../radial-epicyclic-frequency.md) at the local radius. Here $\Omega_z$ is the [vertical epicyclic frequency](../../../../../vertical-epicyclic-frequency.md).

For the [axisymmetric waves of a homogeneous incompressible disk](../../../../../axisymmetric-waves-of-a-homogeneous-incompressible-disk.md), use a local [WKB approximation](../../../../../wkb-approximation.md) proportional to $\exp[i\int k(r)dr-i\omega t]$, with $|kr|\gg1$. Neglect cylindrical curvature and slow radial changes of the background over one [wavelength](../../../../../wavelength.md), but retain the rotation/shear coupling. Let $(u,v,w)$ be the [velocity](../../../../../velocity.md) [perturbations](../../../../../perturbation.md) and $h=p'/\rho$. The leading equations are

$$
\begin{aligned}
-i\omega u-2\Omega v&=-ikh,\\
-i\omega v+\frac{\kappa^2}{2\Omega}u&=0,\\
-i\omega w&=-h_z,\\
iku+w_z&=0.
\end{aligned}
$$

For $\omega\ne0$ and $\omega^2\ne\kappa^2$, these give $u=\omega kh/(\omega^2-\kappa^2)$ and $w=-ih_z/\omega$. The [incompressible flow](../../../../../incompressible-flow.md) constraint then yields

$$
\boxed{p'_{zz}=\frac{\omega^2}{\omega^2-\kappa^2}k^2p'.}
$$

The vertical [Lagrangian fluid displacement](../../../../../lagrangian-fluid-displacement.md) satisfies $w=-i\omega\xi_z$, so $\xi_z=p'_z/(\rho\omega^2)$. A displaced vacuum interface must have zero [Lagrangian pressure perturbation](../../../../../lagrangian-pressure-perturbation.md), not zero [Eulerian fluid perturbation](../../../../../eulerian-fluid-perturbation.md) of [pressure](../../../../../pressure.md) at the old surface. Neglecting the higher-order radial surface-slope contribution,

$$
\Delta p=p'+\xi_z\partial_zp_0=p'-\rho\Omega_z^2z\xi_z=0.
$$

Thus the [free-surface pressure condition of an incompressible disk](../../../../../free-surface-pressure-condition-of-an-incompressible-disk.md) is

$$
\boxed{p'-\frac{\Omega_z^2}{\omega^2}zp'_z=0\quad\text{at }z=\pm H.}
$$

Because the background and [boundary conditions](../../../../../boundary-condition.md) are symmetric about the midplane, choose [pressure](../../../../../pressure.md) modes of [even function](../../../../../even-function.md) or [odd function](../../../../../odd-function.md) symmetry in $z$. For $\omega^2>\kappa^2$, put $q=k\omega/\sqrt{\omega^2-\kappa^2}$ and $Q=qH$. The solutions are $p'\propto\cosh(qz)$ or $\sinh(qz)$; substituting the surface condition gives the two [surface modes of an incompressible disk](../../../../../surface-modes-of-an-incompressible-disk.md):

$$
\boxed{\begin{array}{ll}
\omega^2=\Omega_z^2Q\tanh Q,&\text{even pressure},\\
\omega^2=\Omega_z^2Q\coth Q,&\text{odd pressure},
\end{array}\qquad (kH)^2=Q^2\left(1-\frac{\kappa^2}{\omega^2}\right).}
$$

These are implicit [dispersion relations](../../../../../dispersion-relation.md), or complete parametric equations with parameter $Q$ and the indicated condition $\omega^2>\kappa^2$.

For $0<\omega^2<\kappa^2$, put $s=k\omega/\sqrt{\kappa^2-\omega^2}$ and $S=sH$. The solutions are $p'\propto\cos(sz)$ or $\sin(sz)$, giving the [inertial modes of an incompressible disk](../../../../../inertial-modes-of-an-incompressible-disk.md):

$$
\boxed{\begin{array}{ll}
\omega^2=-\Omega_z^2S\tan S,&\text{even pressure},\\
\omega^2=\Omega_z^2S\cot S,&\text{odd pressure},
\end{array}\qquad (kH)^2=S^2\left(\frac{\kappa^2}{\omega^2}-1\right).}
$$

The restrictions $0<\omega^2<\kappa^2$ select the admissible segments of the [trigonometric functions](../../../../../trigonometric-function.md), producing infinitely many vertical orders. These four parity/frequency formulas exhaust all nonzero-frequency modes: they solve the second-order [pressure](../../../../../pressure.md) equation and both [boundary conditions](../../../../../boundary-condition.md). For finite $k\ne0$, an exactly epicyclic frequency $\omega^2=\kappa^2$ makes the horizontal equations require $p'=0$, then the vertical equation and the [incompressible flow](../../../../../incompressible-flow.md) constraint force all [velocity](../../../../../velocity.md) components to vanish, so it is not a missing finite-wavenumber branch.

For completeness, the [energy identity for free-surface disk waves](../../../../../energy-identity-for-free-surface-disk-waves.md) shows why these modes have real stable frequencies when $\kappa^2\geq0$ and $\Omega_z^2>0$. After elimination of the azimuthal [velocity](../../../../../velocity.md), the radial and vertical displacement equations are $(\omega^2-\kappa^2)\xi_r=ikh$ and $\omega^2\xi_z=h_z$, with $ik\xi_r+\xi_{z,z}=0$. Multiply by conjugate displacements, integrate in $z$ and use the [boundary condition](../../../../../boundary-condition.md) to obtain

$$
\omega^2\int_{-H}^H(|\xi_r|^2+|\xi_z|^2)dz
=\kappa^2\int_{-H}^H|\xi_r|^2dz
+\Omega_z^2H\{|\xi_z(H)|^2+|\xi_z(-H)|^2\}.
$$

The right side is real and nonnegative, excluding additional growing wave branches in this stable case. At zero frequency there can separately be a stationary [geostrophic balance](../../../../../geostrophic-balance.md): vertically constant $h$, $u=w=0$, $v=ikh/(2\Omega)$, and static interface displacements satisfying $h=\Omega_z^2z\xi_z$ at the surfaces. This neighbouring-equilibrium [perturbation](../../../../../perturbation.md) is not a propagating branch omitted by dividing by $\omega$.

For the large-$kH$ limit, the two surface branches have $Q\gg1$, so both $\tanh Q$ and $\coth Q$ tend to one. Eliminating $Q$ gives their common leading surface dispersion,

$$
\boxed{\omega^2\sim\frac12\left[\kappa^2+\sqrt{\kappa^4+4\Omega_z^4(kH)^2}\right]
=\Omega_z^2kH+\frac12\kappa^2+O((kH)^{-1}).}
$$

In particular $\omega\sim\Omega_z\sqrt{kH}$. The effective surface gravity is $g_s=\Omega_z^2H$, and the [pressure](../../../../../pressure.md) decays into the interior on a scale $k^{-1}$. These are [surface gravity waves](../../../../../surface-gravity-wave.md), or surface f-modes, localized near the upper and lower interfaces. Even and odd [pressure](../../../../../pressure.md) are their symmetric and antisymmetric combinations; their splitting is exponentially small as the surfaces decouple. Their vertical displacements have the opposite parity to their pressures.

For each fixed inertial vertical order, large $kH$ means $\omega\ll\kappa$. The [boundary condition](../../../../../boundary-condition.md) then requires $p'_z\simeq0$ at the surfaces, so the limiting vertical [wavenumbers](../../../../../wavenumber.md) are $S=n\pi/2$, $n=1,2,\ldots$. Thus

$$
\boxed{\omega_n\sim\frac{\kappa n\pi}{2kH}\qquad(kH\to\infty\text{ at fixed }n).}
$$

Even $n$ have even [pressure](../../../../../pressure.md), odd $n$ odd [pressure](../../../../../pressure.md). These vertically oscillatory, rotation-restored [inertial waves](../../../../../inertial-wave.md) occupy $0<\omega<\kappa$ and approach zero at fixed order as radial [wavenumber](../../../../../wavenumber.md) increases. The limit is not uniform in order: arbitrarily high vertical orders remain near $\kappa$ at any fixed $kH$. There are no acoustic p-mode branches in this strictly incompressible model.

For $\Omega_z>\kappa>0$, the two surface curves are unique. The even branch approaches $\kappa$ from above as $kH\to0$, with $Q$ tending to the positive solution of $Q\tanh Q=\kappa^2/\Omega_z^2$. The odd branch approaches $\Omega_z$ because $Q\coth Q\to1$ as $Q\to0$. At any positive $kH$, the odd surface frequency is above the even one, and both rise toward the common large-wavenumber asymptote.

The inertial branches all approach $\kappa$ from below as $kH\to0$. For even [pressure](../../../../../pressure.md) there is one admissible branch in each interval $((j+1/2)\pi,(j+1)\pi)$, $j\geq0$, terminating at $S=(j+1)\pi$ as $kH\to\infty$. For odd [pressure](../../../../../pressure.md) there is one in each interval $(j\pi,(j+1/2)\pi)$, again terminating at its upper endpoint; the first interval is admissible because $\kappa^2/\Omega_z^2<1$. Their curves decrease toward zero as shown in the sketch. The small-$kH$ endpoints are formal local-dispersion limits; the [WKB approximation](../../../../../wkb-approximation.md) still requires $kH\gg H/r$ for a finite-thickness disk.

<a id="3/image-surface-and-inertial-branches-of-a-homogeneous-incompressible-disk-with-kappa-2-omega-z-2-1-2"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-42-dispersion.png)

**[Figure 1](#3/image-surface-and-inertial-branches-of-a-homogeneous-incompressible-disk-with-kappa-2-omega-z-2-1-2). Surface and inertial branches of a homogeneous incompressible disk, with $\kappa^2/\Omega_z^2=1/2$**.

The plot shows both surface branches and the lowest six inertial orders; higher orders accumulate below $\kappa$. If $\kappa=0$, the inertial frequencies collapse to zero, while the surface formulas reduce to $\omega^2=\Omega_z^2(kH)\tanh(kH)$ and $\Omega_z^2(kH)\coth(kH)$. A negative $\kappa^2$ instead introduces instability described by the [Rayleigh centrifugal stability criterion](../../../../../rayleigh-centrifugal-stability-criterion.md) and is outside the real-frequency stable sketch.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
