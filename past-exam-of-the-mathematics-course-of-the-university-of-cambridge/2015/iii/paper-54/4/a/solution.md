<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Physical-process first law for a rotating black hole](../../../../../../physical-process-first-law-for-a-rotating-black-hole.md), in four-dimensional [general relativity](../../../../../../general-relativity-split.md) with $G=1$, is

$$
\boxed{\frac{\kappa}{8\pi}\delta A=\delta E-\Omega_H\delta J.}
$$

It applies to a small neutral matter influx into an initially stationary, nonextremal [black hole](../../../../../../black-hole.md) that settles to another stationary state. The background [surface gravity](../../../../../../surface-gravity.md) and angular velocity are $\kappa$ and $\Omega_H$, and $\delta E,\delta J$ are the [Killing energy](../../../../../../killing-energy.md) and [angular momentum](../../../../../../angular-momentum.md) delivered through the [event horizon](../../../../../../event-horizon.md). Other conserved charges are held fixed. The perturbation must be small enough that its horizon generators do not develop caustics, and all equalities below are to first order.

Let $t^a$ be the stationary [Killing vector field](../../../../../../killing-vector-field.md) normalized at infinity, and $\psi^a$ the axial [Killing vector field](../../../../../../killing-vector-field.md) with $2\pi$-periodic orbits. The horizon generator is $\xi^a=t^a+\Omega_H\psi^a$. Choose an affine tangent $k^a$ and parameter $\lambda$ with zero at the past stationary limiting section, so [affine horizon-generator scaling](../../../../../../affine-horizon-generator-scaling.md) gives, on the background horizon

$$
\xi^a=\kappa\lambda k^a.
$$

The background [null expansion](../../../../../../null-expansion.md) and [null shear](../../../../../../null-shear.md) vanish, and [null twist](../../../../../../null-twist.md) vanishes for the hypersurface-orthogonal horizon generators. Linearizing the [Null Raychaudhuri equation](../../../../../../null-raychaudhuri-equation.md) and using the [Einstein field equations](../../../../../../einstein-field-equations.md) gives

$$
\frac{d\,\delta\theta}{d\lambda}=-8\pi\delta T_{ab}k^ak^b.
$$

The quadratic [null expansion](../../../../../../null-expansion.md) and [null shear](../../../../../../null-shear.md) terms are second order. With background cross-sectional measure $dA_0$, the first-order area change is $\delta A=\int_{\mathcal H}\delta\theta\,d\lambda\,dA_0$. Multiplying the evolution equation by $\lambda$ and integrating by parts gives the [first-order horizon-area response to matter flux](../../../../../../first-order-horizon-area-response-to-matter-flux.md)

$$
\delta A=8\pi\int_{\mathcal H}\lambda\,\delta T_{ab}k^ak^b\,d\lambda\,dA_0.
$$

The boundary term $[\lambda\delta\theta]$ vanishes: $\lambda=0$ at the past limiting section, and the final stationary boundary condition gives zero expansion in the settled future. Equivalently, assume a sufficiently localized influx with the required late-time decay.

The energy and angular-momentum fluxes have signs

$$
\delta E=\int_{\mathcal H}\delta T_{ab}t^ak^b\,d\lambda\,dA_0,\qquad\delta J=-\int_{\mathcal H}\delta T_{ab}\psi^ak^b\,d\lambda\,dA_0.
$$

These correspond to the particle conventions $E=-p\cdot t$ and $J=p\cdot\psi$. Their combination is

$$
\delta E-\Omega_H\delta J=\int_{\mathcal H}\delta T_{ab}\xi^ak^b\,d\lambda\,dA_0=\kappa\int_{\mathcal H}\lambda\delta T_{ab}k^ak^b\,d\lambda\,dA_0=\frac\kappa{8\pi}\delta A.
$$

This proves the requested [Physical-process first law of black-hole mechanics](../../../../../../physical-process-first-law-of-black-hole-mechanics.md). For charged infall the corresponding law contains an additional horizon-potential term $\Phi_H\delta Q$; the energy-minus-angular-momentum version assumes that work term is absent.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 54](../../../paper-54-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
