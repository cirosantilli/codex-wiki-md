<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $x$ eastward, $y$ northward and $z$ upward. In a [rotating reference frame](../../../../rotating-reference-frame.md), the horizontal [Cauchy momentum equation](../../../../cauchy-momentum-equation.md) is

$$
\frac{D\mathbf u_h}{Dt}+f\widehat{\mathbf z}\times\mathbf u_h=-\frac1\rho\nabla_h p+\mathbf F_h,
\qquad f=2\Omega\sin\phi.
$$

Here $\mathbf F_h$ represents other accelerations, such as [friction](../../../../friction.md), and $f$ is the [Coriolis parameter](../../../../coriolis-parameter.md). When the [Rossby number](../../../../rossby-number.md) $U/(|f|L)$ and the ratio $1/(|f|\tau)$ are small, and [friction](../../../../friction.md) is weak, both advective and local [acceleration](../../../../acceleration.md) can be neglected. The [Coriolis force](../../../../coriolis-force.md) then balances the [pressure gradient force](../../../../pressure-gradient-force.md): this is [geostrophic balance](../../../../geostrophic-balance.md), with $fv=p_x/\rho$ and $fu=-p_y/\rho$. The [geostrophic wind](../../../../geostrophic-wind.md) runs along [atmospheric isobars](../../../../atmospheric-isobar.md), with low [pressure](../../../../pressure-split.md) on its left in the northern hemisphere.

A rapid change of [pressure](../../../../pressure-split.md) need not bring the corresponding [geostrophic wind](../../../../geostrophic-wind.md) into existence at once. An initially weak wind therefore leaves an inward [pressure gradient force](../../../../pressure-gradient-force.md) around the new low. For a smoothed anomaly of horizontal scale $L=5\times10^5\ \mathrm m$, [geostrophic balance](../../../../geostrophic-balance.md) would require

$$
U_g\sim\frac{|p\prime|}{\rho |f|L}
\simeq33\ \mathrm{m\,s^{-1}}
\left(\frac{1.2\ \mathrm{kg\,m^{-3}}}{\rho}\right)
\left(\frac{10^{-4}\ \mathrm{s^{-1}}}{|f|}\right).
$$

For the illustrative midlatitude value $|f|=10^{-4}\ \mathrm{s^{-1}}$, the implied [Rossby number](../../../../rossby-number.md) is already about $0.67$, so curved-flow [acceleration](../../../../acceleration.md) matters. With a small tropical value $|f|=10^{-5}\ \mathrm{s^{-1}}$, the inferred speed is $333\ \mathrm{m\,s^{-1}}$ and the [Rossby number](../../../../rossby-number.md) about $67$: the assumed [geostrophic balance](../../../../geostrophic-balance.md) is untenable. [Geostrophic adjustment](../../../../geostrophic-adjustment.md) redistributes the anomaly and emits [internal gravity waves](../../../../internal-wave.md), leaving a weaker balanced component.

For a target speed $U_*=10\ \mathrm{m\,s^{-1}}$ on the same scale, the required scale estimate is

$$
\boxed{|p\prime_{\rm adj}|\sim\rho |f|LU_*
=6\ \mathrm{hPa}\left(\frac{\rho}{1.2\ \mathrm{kg\,m^{-3}}}\right)
\left(\frac{|f|}{10^{-4}\ \mathrm{s^{-1}}}\right).}
$$

Thus $6\ \mathrm{hPa}$, or $0.30$ of the initial magnitude, is the midlatitude estimate; at the illustrative tropical $|f|=10^{-5}\ \mathrm{s^{-1}}$ it is $0.6\ \mathrm{hPa}$, or $0.030$ of the initial magnitude. **The paper gives no latitude, so there is no unique numerical reduction.** At the equator itself one must use equatorial dynamics rather than divide by $f=0$. Even the tropical $10\ \mathrm{m\,s^{-1}}$ estimate has [Rossby number](../../../../rossby-number.md) $2$, so it describes the scale permitted by the stated balance, rather than a controlled tropical [geostrophic balance](../../../../geostrophic-balance.md).

There are two qualifications to “unstable”. A literal top-hat [pressure](../../../../pressure-split.md) anomaly has a discontinuous edge, where no finite classical [geostrophic wind](../../../../geostrophic-wind.md) can balance its distributional [pressure gradient](../../../../pressure-gradient.md). The $500\ \mathrm{km}$ estimate assumes a smoothed edge; a thinner edge requires stronger winds. More generally a large low is not, by its amplitude alone, proved to have an exponentially growing instability. For a concrete counterexample to the claim that such an amplitude cannot be stationary, set $p\prime(s)=-P\exp(-s^2/a^2)$, with cylindrical radius $s$, constant $\rho$ and $f>0$. The cyclonic [gradient wind](../../../../gradient-wind.md)

$$
v_\theta(s)=\frac{-fs+\sqrt{f^2s^2+4s p_s/\rho}}2
$$

is real and satisfies $v_\theta^2/s+fv_\theta=p_s/\rho$ for every $P>0$, with a regular limit at the centre. This is a stationary [axisymmetric flow](../../../../axisymmetric-flow.md); no claim about its perturbation stability is needed. Here the physically justified conclusion is that a rapidly imposed anomaly without its balancing wind is **unbalanced**.

Small tropical [Coriolis parameter](../../../../coriolis-parameter.md) allows only weak horizontal [pressure gradients](../../../../pressure-gradient.md) to coexist with ordinary large-scale winds. [Hydrostatic balance](../../../../hydrostatic-balance.md) connects the vertical variation of these [pressure gradients](../../../../pressure-gradient.md) to horizontal [temperature gradients](../../../../temperature-gradient.md); equivalently the approximate [thermal wind](../../../../thermal-wind.md) relation gives $f u_z\simeq-(g/T)T_y$. For comparable vertical wind shear, small $|f|$ means smaller $|T_y|$. [Internal gravity waves](../../../../internal-wave.md) can spread heating-induced [buoyancy](../../../../buoyancy.md) anomalies efficiently before rotation arrests the adjustment. This motivates the [weak temperature gradient approximation](../../../../weak-temperature-gradient-approximation.md) for the tropical free troposphere; it does not require the land surface or atmospheric boundary layer to have uniform [temperature](../../../../temperature-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the geophysical fluid dynamics course of the University of Oxford](../../../split.md)
5. [Geophysical fluid dynamics course of the University of Oxford](../../../../geophysical-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
