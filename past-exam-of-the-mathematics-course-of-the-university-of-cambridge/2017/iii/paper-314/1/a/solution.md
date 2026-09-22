<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $D/Dt=\partial_t+\mathbf u\cdot\nabla$ for the [material derivative](../../../../../../material-derivative.md) and $q=\mathbf u\cdot\mathbf B$ for the [cross-helicity](../../../../../../cross-helicity.md) density, so $H_c=\int_V q\,dV$. The [ideal magnetohydrodynamic induction equation](../../../../../../ideal-magnetohydrodynamic-induction-equation.md) of [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md), with $\nabla\cdot\mathbf B=0$, gives

$$
\frac{D\mathbf B}{Dt}=(\mathbf B\cdot\nabla)\mathbf u-\mathbf B\,\nabla\cdot\mathbf u.
$$

The [dot product](../../../../../../dot-product.md) of the [Euler momentum equation](../../../../../../euler-equations-for-an-inviscid-fluid.md) with the [magnetic field](../../../../../../magnetic-field.md) has no [Lorentz force](../../../../../../lorentz-force.md) contribution, because $\mathbf B\cdot[(\nabla\times\mathbf B)\times\mathbf B]=0$. Consequently,

$$
\frac{Dq}{Dt}=\mathbf B\cdot\nabla\left(\frac{u^2}{2}-\Phi\right)-\frac{\mathbf B\cdot\nabla p}{\rho}-q\,\nabla\cdot\mathbf u.
$$

Here $h=e+p/\rho$ is the [specific enthalpy](../../../../../../specific-enthalpy.md), $T$ the [temperature](../../../../../../temperature.md), and $s$ the [specific entropy](../../../../../../specific-entropy.md); $e$ is the [internal energy](../../../../../../internal-energy.md) per unit mass. The [first law of thermodynamics](../../../../../../first-law-of-thermodynamics.md) in this convention is $de=T\,ds-p\,d(1/\rho)$, so $dh=T\,ds+dp/\rho$. Substitution, followed by $\nabla\cdot\mathbf B=0$, yields the [cross-helicity conservation law](../../../../../../cross-helicity-conservation-law.md)

$$
\partial_tq+\nabla\cdot\left[\mathbf u q+\left(h+\Phi-\frac{u^2}{2}\right)\mathbf B\right]=T\mathbf B\cdot\nabla s.
$$

The [vector triple product](../../../../../../vector-triple-product.md) identity $\mathbf u\times(\mathbf u\times\mathbf B)=\mathbf u q-u^2\mathbf B$ puts this in the equivalent form

$$
\boxed{\partial_t(\mathbf u\cdot\mathbf B)+\nabla\cdot\left[\mathbf u\times(\mathbf u\times\mathbf B)+\left(\frac{u^2}{2}+\Phi+h\right)\mathbf B\right]=T\mathbf B\cdot\nabla s.}
$$

For the fixed volume, the [divergence theorem](../../../../../../divergence-theorem.md) gives the exact [cross-helicity](../../../../../../cross-helicity.md) balance

$$
\frac{dH_c}{dt}=\int_V T\mathbf B\cdot\nabla s\,dV-\int_{\partial V}\left[\mathbf u q+\left(h+\Phi-\frac{u^2}{2}\right)\mathbf B\right]\cdot\mathbf n\,dS.
$$

Thus **[cross-helicity](../../../../../../cross-helicity.md) is constant when the net source equals the outward flux**. Simple sufficient hypotheses are $\mathbf B\cdot\nabla s=0$ throughout the volume and $\mathbf u\cdot\mathbf n=\mathbf B\cdot\mathbf n=0$ on its boundary. The first condition includes a [homentropic flow](../../../../../../homentropic-flow.md); the second prevents both relevant boundary fluxes. [Periodic boundary conditions](../../../../../../periodic-boundary-conditions.md), or sufficiently rapid decay at infinity, provide alternatives. These statements concern smooth [ideal magnetohydrodynamics](../../../../../../ideal-magnetohydrodynamics.md): material [specific entropy](../../../../../../specific-entropy.md) conservation alone, $Ds/Dt=0$, does not eliminate spatial [specific entropy](../../../../../../specific-entropy.md) gradients along the [magnetic field lines](../../../../../../magnetic-field-line.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 314](../../../paper-314-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
