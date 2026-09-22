<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At leading anisotropic order, perpendicular [Alfvénic turbulence](../../../../../../alfvenic-turbulence.md) evolves independently of the compressive fluctuations. The [slow modes](../../../../../../slow-magnetosonic-wave.md) and the [entropy mode](../../../../../../entropy-mode.md) are transported by that [turbulence](../../../../../../turbulence-split.md). The fast magnetosonic [frequency](../../../../../../frequency.md) is of order $k_\perp(v_A^2+c_s^2)^{1/2}$, much larger than the reduced Alfvén [frequency](../../../../../../frequency.md); the low-frequency [reduced magnetohydrodynamics](../../../../../../reduced-magnetohydrodynamics.md) ordering filters out that fast-wave sector.

The passive evolution can be made explicit for a uniform ideal adiabatic [plasma](../../../../../../plasma-physics.md). Let $c_s^2=\gamma p_0/\rho_0$, $\delta=\delta\rho/\rho_0$, $b=\delta B_\parallel/B_0$, and define the normalized [entropy](../../../../../../entropy.md) perturbation

$$
s=\frac{\delta p}{p_0}-\gamma\delta.
$$

Use $D=\partial_t+\mathbf u_\perp\cdot\nabla_\perp$ and $\nabla_\parallel=\partial_z+(\delta\mathbf B_\perp/B_0)\cdot\nabla_\perp$. Perpendicular force balance makes the leading total-pressure perturbation vanish:

$$
\delta p+\rho_0v_A^2b=0.
$$

The ideal [entropy](../../../../../../entropy.md) equation gives $Ds=0$. The leading continuity and parallel-induction equations have the same compressive [divergence](../../../../../../divergence.md) term; subtracting them gives $D(\delta-b)=-\nabla_\parallel u_\parallel$. Parallel momentum gives $Du_\parallel=-\nabla_\parallel\delta p/\rho_0$. Put

$$
r=\delta+\frac{s}{\gamma},\qquad\delta p=\rho_0c_s^2r,\qquad b=-\frac{c_s^2}{v_A^2}r.
$$

The two compressive equations therefore become

$$
Dr=-\frac{v_A^2}{v_A^2+c_s^2}\nabla_\parallel u_\parallel,\qquad Du_\parallel=-c_s^2\nabla_\parallel r.
$$

Let $c_T=v_Ac_s/(v_A^2+c_s^2)^{1/2}$ be the [tube speed](../../../../../../tube-speed.md) and $h=c_s^2r/c_T$. Then

$$
Du_\parallel=-c_T\nabla_\parallel h,\qquad Dh=-c_T\nabla_\parallel u_\parallel.
$$

Thus the [slow and entropy fluctuations in reduced magnetohydrodynamics](../../../../../../slow-and-entropy-fluctuations-in-reduced-magnetohydrodynamics.md) have characteristic amplitudes $f^\pm=u_\parallel\pm h$ obeying

$$
\boxed{Df^\pm=\mp c_T\nabla_\parallel f^\pm,\qquad Ds=0.}
$$

The two slow-wave populations propagate in opposite directions along the bent field lines while being mixed across them by $\mathbf u_\perp$. The [entropy](../../../../../../entropy.md) perturbation is carried by the fluid without a restoring-wave [frequency](../../../../../../frequency.md). A pure [entropy](../../../../../../entropy.md) perturbation has $r=b=u_\parallel=0$ and $\delta=-s/\gamma$, so its [density](../../../../../../density.md) variation is accompanied by a [temperature](../../../../../../temperature.md) change with no leading [pressure](../../../../../../pressure.md) variation.

The coefficients and advecting fields in these three scalar equations come from the Alfvénic cascade; the scalars do not enter the leading perpendicular Alfvén equations. They therefore develop small perpendicular scales through passive mixing. If a scalar $f$ has constant [variance](../../../../../../variance-split.md) flux $\mathcal F_f$ and is mixed on the Goldreich–Sridhar time $\tau_\ell\sim\mathcal E^{-1/3}\ell_\perp^{2/3}$, then

$$
\delta f_\ell^2\sim\mathcal F_f\tau_\ell,\qquad\boxed{E_f(k_\perp)\sim\mathcal F_f\mathcal E^{-1/3}k_\perp^{-5/3}.}
$$

The flux and amplitude need not equal the Alfvénic [energy](../../../../../../energy.md) flux. This passive-spectrum statement uses the same locality and stationary inertial-range assumptions as part (a), and ignores additional damping. If a passive mode is absent initially and is not forced, its homogeneous leading equation keeps it absent; the Alfvénic cascade does not have to generate every compressive mode.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
