<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $\mathcal L(A_\nu,\partial_\mu A_\nu)$ define $\Pi^{\mu\nu}=\partial\mathcal L/\partial(\partial_\mu A_\nu)$. A fixed-coordinate infinitesimal field variation $\delta A_\nu=\alpha\Delta_\nu$ satisfying $\delta\mathcal L=\alpha\partial_\mu K^\mu$ gives the [Noether current](../../../../../noether-current.md)

$$
\boxed{J^\mu=\Pi^{\mu\nu}\Delta_\nu-K^\mu,\qquad
\partial_\mu J^\mu=0\quad\text{on shell}.}
$$

Indeed, the first variation is

$$
\frac{\delta\mathcal L}{\alpha}
=\left(\mathcal L_{A_\nu}-\partial_\mu\Pi^{\mu\nu}\right)\Delta_\nu
+\partial_\mu(\Pi^{\mu\nu}\Delta_\nu);
$$

subtract the divergence of $K$ and use the [Euler-Lagrange field equations](../../../../../euler-lagrange-field-equation.md). The components of the [Lorentz four-vector](../../../../../four-vector.md) are simply the field labels in this formula. For a transformation moving the coordinates, use its induced fixed-coordinate variation; this includes translations and [Lorentz transformations](../../../../../lorentz-transformation.md). The spatial integral of $J^0$ is conserved when the spatial current has vanishing boundary flux.

With signature $(+,-,-,-)$, a [gauge transformation](../../../../../gauge-transformation.md) is $A_\mu\mapsto A_\mu+\partial_\mu\chi$. The [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md)

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu
$$

is unchanged, since mixed derivatives of $\chi$ commute. Thus $\mathcal L=-F_{\mu\nu}F^{\mu\nu}/4$ is gauge invariant. Write $A_\mu=(\Phi,-\mathbf A)$, so $F_{0i}=E_i$ and $F_{ij}=-\epsilon_{ijk}B_k$. Then

$$
F_{\mu\nu}F^{\mu\nu}=2(\mathbf B^2-\mathbf E^2),
\qquad
\mathcal L=\frac12(\mathbf E^2-\mathbf B^2).
$$

The overall minus sign produces a positive electric kinetic term and a positive physical [Hamiltonian](../../../../../hamiltonian.md). Reversing it reverses the sign of the physical [energy](../../../../../energy.md) and gives the wrong positive-energy theory; the issue is the indefinite spacetime metric, not negative magnetic [energy](../../../../../energy.md).

For $\Delta_\nu=\partial_0A_\nu$, direct differentiation gives $\delta\mathcal L=\alpha\partial_0\mathcal L=\alpha\partial_\mu(\delta^\mu_0\mathcal L)$. Since

$$
\Pi^{\mu\nu}=-F^{\mu\nu},
$$

the [canonical energy-momentum tensor](../../../../../canonical-stress-energy-tensor.md) gives the conserved [energy](../../../../../energy.md) current

$$
J^\mu_{\rm can}=-F^{\mu\nu}\partial_0A_\nu-\delta^\mu_0\mathcal L.
$$

Its time component is

$$
J^0_{\rm can}
=\frac12(\mathbf E^2+\mathbf B^2)+\mathbf E\cdot\nabla\Phi,
$$

because $\partial_0 A_i=E_i+\partial_i\Phi$. Thus Noether's conserved canonical [energy](../../../../../energy.md) is $\int J^0_{\rm can}\,d^3x$. In pure, source-free electromagnetism the field equation gives $\nabla\cdot\mathbf E=0$, and

$$
\int\mathbf E\cdot\nabla\Phi\,d^3x
=\int_{\partial V}\Phi\,\mathbf E\cdot d\mathbf S.
$$

For sufficiently decaying fields, or boundary conditions removing this surface term,

$$
\boxed{H=\frac12\int d^3x\,(\mathbf E^2+\mathbf B^2).}
$$

The canonical density is not locally gauge invariant, even though the total [energy](../../../../../energy.md) with these conditions is.

Now use the [gauge-compensated time translation in electromagnetism](../../../../../gauge-compensated-time-translation-in-electromagnetism.md),

$$
\Delta_\nu=\partial_0A_\nu-\partial_\nu A_0=F_{0\nu}.
$$

The extra term is a [gauge transformation](../../../../../gauge-transformation.md) with the field-dependent parameter $\chi=-\alpha A_0$. It changes no field strength; therefore the combined variation still has $\delta F_{\mu\nu}=\alpha\partial_0F_{\mu\nu}$ and the same $K^\mu=\delta^\mu_0\mathcal L$. The new current is

$$
J^\mu_{\rm inv}=-F^{\mu\nu}F_{0\nu}-\delta^\mu_0\mathcal L.
$$

It is expressed entirely in gauge-invariant field strengths. In particular

$$
\boxed{J^0_{\rm inv}=\frac12(\mathbf E^2+\mathbf B^2),\qquad
\mathbf J_{\rm inv}=\mathbf E\times\mathbf B.}
$$

This is the [energy](../../../../../energy.md) column of the [electromagnetic stress-energy tensor](../../../../../electromagnetic-stress-energy-tensor.md)

$$
T^{\mu\nu}=-F^{\mu\rho}F^\nu{}_\rho
+\frac14g^{\mu\nu}F_{\rho\sigma}F^{\rho\sigma}
$$

in the chosen mostly-minus convention. Its conservation is the [energy](../../../../../energy.md) continuity equation.

The currents differ by

$$
J^\mu_{\rm inv}-J^\mu_{\rm can}
=F^{\mu\nu}\partial_\nu A_0
=\partial_\nu(A_0F^{\mu\nu})
$$

on the source-free field equations. The final expression is an antisymmetric superpotential divergence, so it changes the integrated charge only by a boundary term. **The compensating [gauge transformation](../../../../../gauge-transformation.md) improves the local [energy](../../../../../energy.md) density without changing the physical conserved [energy](../../../../../energy.md) under the stated boundary conditions.**

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
