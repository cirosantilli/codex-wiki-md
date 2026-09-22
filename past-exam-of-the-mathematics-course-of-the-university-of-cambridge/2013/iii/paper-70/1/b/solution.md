<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [Ffowcs Williams-Hawkings equation](../../../../../../ffowcs-williams-hawkings-equation.md), the other source types are a surface [acoustic monopole](../../../../../../acoustic-monopole.md) associated with [acoustic thickness noise](../../../../../../acoustic-thickness-noise.md), and a volume [acoustic quadrupole](../../../../../../acoustic-quadrupole.md) involving the [Lighthill stress tensor](../../../../../../lighthill-stress-tensor.md). On an impermeable material surface, fluid and surface [normal velocities](../../../../../../normal-velocity.md) agree. There is no through-surface mass-flux source; the remaining thickness source is $Q=\rho_0v_n$. For a [rigid body](../../../../../../rigid-body-dynamics.md), the leading [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md) to that source has

$$
\int_SQ\,dS=\rho_0\int_Sv_n\,dS=\rho_0\frac{d\mathcal V}{dt}=0.
$$

Thus there is no leading net-volume [acoustic monopole](../../../../../../acoustic-monopole.md). To neglect thickness radiation beyond that leading cancellation, assume negligible volume displacement, as for ideal thin blades, or that its higher multipoles are small compared with the retained [acoustic loading noise](../../../../../../acoustic-loading-noise.md). Rigidity alone does not make a moving finite-volume body's local thickness source identically zero.

The volume [acoustic quadrupole](../../../../../../acoustic-quadrupole.md) may be neglected for low [Mach number](../../../../../../mach-number.md) motion when exterior turbulent or nonlinear stresses do not provide a competing strong source. We also assume small [linear acoustics](../../../../../../linear-acoustics-split.md) perturbations, a uniform reference [sound speed](../../../../../../speed-of-sound.md), and negligible relevant viscous and entropy sources. These are source-strength approximations, particularly important if a loading contribution itself cancels by symmetry. Under them, the retained [acoustic dipole](../../../../../../acoustic-dipole.md) is the [force](../../../../../../force.md) exerted by the object on the fluid, with the sign used in the previous solution.

Let $R=|x|$, $n=x/R$, and $\tau_0=t-R/c_0$. In the [acoustic far field](../../../../../../acoustic-far-field.md), $R$ is large compared with the object and $\omega R/c_0\gg1$. For a source of size $\ell$ with $\omega\ell/c_0\ll1$ and small surface [Mach number](../../../../../../mach-number.md), source-dependent delays and the Doppler factor can be neglected to leading order. The surface integral then contains just the total [force](../../../../../../force.md) $\mathcal F(\tau)=\int_S F\,dS$. Differentiating its [retarded time](../../../../../../retarded-time.md), rather than its $R^{-1}$ spreading factor, gives the radiating term

$$
\boxed{\rho'(x,t)\sim\frac{n\cdot\dot{\mathcal F}(\tau_0)}{4\pi c_0^3R},\qquad
p'(x,t)=c_0^2\rho'\sim\frac{n\cdot\dot{\mathcal F}(\tau_0)}{4\pi c_0R}.}
$$

The sign follows from $\partial_{x_i}\tau_0=-n_i/c_0$. Differentiating $R^{-1}$ or the direction $n$ instead produces the lower-order near field. A constant total [force](../../../../../../force.md) does not radiate at this leading compact order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
