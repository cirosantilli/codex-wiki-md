<h1 id="linear-alfven-wave-equations">Linear Alfvén wave equations</h1>

↑ **Parent:** [Alfvén wave](alfven-wave.md)

Take a static uniform [fluid](fluid.md) of [mass density](density.md) $\rho>0$, constant gas [pressure](pressure-split.md), and background [magnetic field](magnetic-field-split.md) $\mathbf B_0=B_0\mathbf e_z$ with $B_0>0$. Use SI units, [vacuum permeability](vacuum-permeability.md) $\mu_0$, zero [electrical resistivity](electrical-resistivity.md) and zero [viscosity](dynamic-viscosity-split.md). Write $\mathbf B=\mathbf B_0+\mathbf b_\perp(z,t)$ and $\mathbf u=\mathbf u_\perp(z,t)$, with both disturbances perpendicular to $\mathbf e_z$. Retain only [linear order](linear-order.md) in their [amplitudes](wave-amplitude.md). There is no background [fluid flow](fluid-flow.md), so the linear [material derivative](material-derivative.md) is $\partial_t$.

The [continuity equation](continuity-equation.md) has $\nabla\cdot\mathbf u_\perp=0$, hence $\partial_t\delta\rho=0$; choosing no initial [mass density](density.md) fluctuation gives $\delta\rho=0$. For this shear mode the gas [pressure](pressure-split.md) fluctuation is also zero. In the [ideal magnetohydrodynamic momentum equation](ideal-magnetohydrodynamic-momentum-equation.md), the [Lorentz force density](lorentz-force-density.md) can be written

$$
\frac{(\nabla\times\mathbf B)\times\mathbf B}{\mu_0}
=\frac{(\mathbf B\cdot\nabla)\mathbf B}{\mu_0}
-\nabla\frac{B^2}{2\mu_0}.
$$

Because $\mathbf B_0\cdot\mathbf b_\perp=0$, the perturbed [magnetic pressure](magnetic-pressure.md) starts at quadratic order. The surviving transverse [magnetic tension](magnetic-tension.md) gives the first equation below. Expanding the [ideal magnetohydrodynamic induction equation](ideal-magnetohydrodynamic-induction-equation.md) gives the second:

$$
\rho\,\partial_t\mathbf u_\perp=\frac{B_0}{\mu_0}\partial_z\mathbf b_\perp,
\qquad
\partial_t\mathbf b_\perp=B_0\partial_z\mathbf u_\perp.
$$

Differentiate the first in time and substitute the second. Both [velocity](velocity.md) and [magnetic field](magnetic-field-split.md) disturbances obey the [one-dimensional wave equation](one-dimensional-wave-equation.md):

$$
\partial_t^2\mathbf u_\perp=v_A^2\partial_z^2\mathbf u_\perp,
\qquad v_A=\frac{B_0}{\sqrt{\mu_0\rho}}.
$$

For a [plane wave](plane-wave.md) proportional to $e^{i(k_\parallel z-\omega t)}$, this gives $\omega^2=k_\parallel^2v_A^2$, or $\omega=\pm k_\parallel v_A$. The magnetic and [velocity](velocity.md) [amplitudes](wave-amplitude.md) satisfy $\mathbf b_\perp=-(B_0k_\parallel/\omega)\mathbf u_\perp$: they have opposite signs for propagation along $+\mathbf e_z$ and equal signs for propagation along $-\mathbf e_z$. The general uniform-background shear [polarization of waves](polarization-waves.md), perpendicular to both $\mathbf k$ and $\mathbf B_0$, gives the same [dispersion relation](dispersion-relation-split.md) with $k_\parallel=\mathbf k\cdot\mathbf e_z$. Its [group velocity](group-velocity.md) is $\pm v_A\mathbf e_z$, whereas its [phase velocity](phase-velocity.md) normal to an oblique wavefront has magnitude $v_A|k_\parallel|/|\mathbf k|$.

## ↑ Ancestors (9)

1. [Alfvén wave](alfven-wave.md)
2. [Magnetohydrodynamic wave](magnetohydrodynamic-wave.md)
3. [Ideal magnetohydrodynamics](ideal-magnetohydrodynamics-split.md)
4. [Magnetohydrodynamics](magnetohydrodynamics-split.md)
5. [Astrophysical fluid dynamics](astrophysical-fluid-dynamics-split.md)
6. [Fluid mechanics](fluid-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Alfvén wave energy transport](alfven-wave-energy-transport.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2013/paper-1/2/a/solution.md)
- [Resistive damping of an Alfvén wave](resistive-damping-of-an-alfven-wave.md)
