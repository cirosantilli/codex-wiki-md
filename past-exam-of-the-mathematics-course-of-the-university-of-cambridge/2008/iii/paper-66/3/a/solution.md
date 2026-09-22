<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [geometrized units](../../../../../../geometrized-units.md) $G=c=1$. The [Physical-process first law of black-hole mechanics](../../../../../../physical-process-first-law-of-black-hole-mechanics.md) concerns a small perturbation of a rotating [black hole](../../../../../../black-hole.md) in an initially [stationary spacetime](../../../../../../stationary-spacetime.md) by infalling matter, followed by relaxation to another [stationary spacetime](../../../../../../stationary-spacetime.md). For an uncharged [black hole](../../../../../../black-hole.md), or neutral accretion with charge held fixed, its first-order statement is

$$
\boxed{\delta E-\Omega_H\delta J=\frac{\kappa}{8\pi}\delta A.}
$$

Here $\kappa>0$ is the background [surface gravity](../../../../../../surface-gravity.md), $\Omega_H$ is the background [horizon angular velocity](../../../../../../horizon-angular-velocity.md), and $\delta A$ is the change in [event horizon](../../../../../../event-horizon.md) area. The [energy](../../../../../../energy.md) $\delta E$ and [angular momentum](../../../../../../angular-momentum.md) $\delta J$ are the fluxes carried into the [event horizon](../../../../../../event-horizon.md); when these account for the changes of the [black hole](../../../../../../black-hole.md), they equal $\delta M$ and its change of [angular momentum](../../../../../../angular-momentum.md). The result is a linearized law, not an exact identity for a finite violent accretion event. The perturbation must be small enough that focusing does not produce new caustics or invalidate the expansion about the existing generators.

Let $k^a$ be the stationary [Killing vector field](../../../../../../killing-vector-field.md) normalized at infinity, $m^a$ the axial [Killing vector field](../../../../../../killing-vector-field.md) with $2\pi$-periodic orbits, and

$$
\chi^a=k^a+\Omega_Hm^a.
$$

On the background [Killing horizon](../../../../../../killing-horizon.md), $\chi^a$ is its future-directed null generator and satisfies $\chi^b\nabla_b\chi^a=\kappa\chi^a$. Choose a parameter $v$ with $\chi=\partial_v$. The [null expansion](../../../../../../null-expansion.md) in this parameter is $\theta=\partial_v\log dA$. The generator is not affinely parametrized; if $\ell=\partial_\lambda$ is affine, then $\chi=\kappa\lambda\ell$ after an appropriate choice of affine origin, with $\lambda\propto e^{\kappa v}$. Rescaling the [Null Raychaudhuri equation](../../../../../../null-raychaudhuri-equation.md) gives

$$
\frac{d\theta}{dv}=\kappa\theta-\frac12\theta^2-\widehat\sigma_{ab}\widehat\sigma^{ab}-R_{ab}\chi^a\chi^b.
$$

The [null twist](../../../../../../null-twist.md) vanishes because the generators are normal to the [event horizon](../../../../../../event-horizon.md). By the [Einstein field equations](../../../../../../einstein-field-equations.md), $R_{ab}\chi^a\chi^b=8\pi T_{ab}\chi^a\chi^b$. Background [null expansion](../../../../../../null-expansion.md) and [null shear](../../../../../../null-shear.md) vanish on a [Killing horizon](../../../../../../killing-horizon.md) of the background [stationary spacetime](../../../../../../stationary-spacetime.md). Thus $\theta$ and $\widehat\sigma$ are first order, their squares are second order, and the linearized equation is

$$
\frac{d\theta}{dv}-\kappa\theta=-8\pi\delta T_{ab}\chi^a\chi^b.
$$

The final [stationary spacetime](../../../../../../stationary-spacetime.md) supplies the boundary condition $\theta\to0$ in the future. Explicitly,

$$
\theta(v)=8\pi\int_v^\infty e^{\kappa(v-v')}\delta T_{ab}\chi^a\chi^b(v')\,dv'.
$$

This future boundary condition reflects the global definition of the [event horizon](../../../../../../event-horizon.md). For localized infall, $\theta$ also tends to zero in the remote past. Integrating the linearized equation along the generators, and then over a background cross-section with area element $dA_0$, gives

$$
\kappa\delta A=8\pi\int_{\mathcal H}\delta T_{ab}\chi^a\chi^b\,dv\,dA_0,
\qquad
\delta A=\int_{\mathcal H}\theta\,dv\,dA_0.
$$

Using the background area element introduces only second-order corrections.

With orientations chosen so that future infalling positive [energy](../../../../../../energy.md) has positive flux, the conserved [Killing energy](../../../../../../killing-energy.md) and axial [angular momentum](../../../../../../angular-momentum.md) give

$$
\delta E=\int_{\mathcal H}\delta T_{ab}k^a\chi^b\,dv\,dA_0,
\qquad
\delta J=-\int_{\mathcal H}\delta T_{ab}m^a\chi^b\,dv\,dA_0.
$$

Consequently $\delta E-\Omega_H\delta J=\int_{\mathcal H}\delta T_{ab}\chi^a\chi^b\,dv\,dA_0$, proving the displayed [Physical-process first law of black-hole mechanics](../../../../../../physical-process-first-law-of-black-hole-mechanics.md). Restoring $G$ replaces $8\pi$ by $8\pi G$. The [null energy condition](../../../../../../null-energy-condition.md) makes the integral nonnegative and therefore implies area increase in this regime; that condition is needed for the sign conclusion, not for the linearized flux identity itself. Charged infall would require the additional electrostatic work term, and an extremal background needs separate treatment because the proof uses $\kappa>0$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
