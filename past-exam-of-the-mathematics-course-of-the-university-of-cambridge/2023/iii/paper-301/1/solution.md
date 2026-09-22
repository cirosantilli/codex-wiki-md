<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A continuous symmetry is a family of transformations depending continuously on parameters for which the [action](../../../../../action.md) is unchanged, possibly up to a spacetime boundary term. For an infinitesimal field variation $\delta\phi=\epsilon\Delta\phi$, a [Noether current](../../../../../noether-current.md) $j^\mu$ obeys

$$
\partial_\mu j^\mu=0
$$

when the [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) holds. Its [Noether charge](../../../../../noether-charge.md)

$$
Q=\int_{\mathbb R^3}j^0(t,\mathbf x)\,d^3x
$$

is conserved provided the flux $\int_{S_\infty}j^i n_i\,dS$ vanishes.

[Noether theorem](../../../../../noether-theorem.md) gives the implication from a differentiable global variational symmetry to an on-shell conserved current. A conserved current gives a conserved charge only under suitable boundary and convergence conditions. Conversely, a conserved charge generates a continuous symmetry through [Poisson brackets](../../../../../poisson-bracket.md) classically or a [commutator](../../../../../commutator.md) quantum mechanically when a regular Hamiltonian formulation exists. Currents can be changed by identically conserved improvement terms, and inverse Noether statements require regularity and the exclusion of such trivial currents, so the three notions are related but not literally in one-to-one correspondence.

For spacetime translations, the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md) is

$$
T^\mu{}_{\nu}
=\frac{\partial\mathcal L}{\partial(\partial_\mu\phi)}\partial_\nu\phi
-\delta^\mu{}_{\nu}\mathcal L.
$$

For

$$
\mathcal L=\frac12\partial_\mu\phi\,\partial^\mu\phi-V(\phi),
$$

raising the second index gives the symmetric tensor

$$
T^{\mu\nu}
=\partial^\mu\phi\,\partial^\nu\phi
-\eta^{\mu\nu}\left(\frac12\partial_\rho\phi\,\partial^\rho\phi-V(\phi)\right).
$$

Translation invariance gives four conserved currents $T^{\mu\nu}$, one for each fixed $\nu$, and the four conserved charges are the [four-momentum](../../../../../four-momentum.md)

$$
P^\nu=\int d^3x\,T^{0\nu}.
$$

$P^0$ is the [energy](../../../../../hamiltonian.md) and $\mathbf P$ is the spatial momentum.

The [Lorentz transformation](../../../../../lorentz-transformation.md) variation of a scalar is generated solely by its argument. The corresponding [Lorentz current](../../../../../lorentz-current.md) is

$$
J^{\mu\rho\sigma}=x^\rho T^{\mu\sigma}-x^\sigma T^{\mu\rho}.
$$

Using $\partial_\mu T^{\mu\nu}=0$ and symmetry of $T^{\rho\sigma}$,

$$
\partial_\mu J^{\mu\rho\sigma}
=T^{\rho\sigma}-T^{\sigma\rho}
+x^\rho\partial_\mu T^{\mu\sigma}
-x^\sigma\partial_\mu T^{\mu\rho}=0.
$$

In particular, conservation of the boost charge

$$
K^i=\int d^3x\,(x^iT^{00}-tT^{0i})
$$

implies

$$
\frac d{dt}\int d^3x\,x^iT^{00}=\int d^3x\,T^{0i}=P^i.
$$

The quantity denoted $V^i$ in the question is therefore the conserved momentum component $P^i$, assuming the same vanishing boundary flux.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 301](../../paper-301-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
