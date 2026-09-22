<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For fields $\Phi_a$ with a first-derivative [Lagrangian density](../../../../../lagrangian-density.md), suppose an infinitesimal global transformation at fixed coordinates is $\delta\Phi_a=\alpha\Delta_a$ and $\delta\mathcal L=\alpha\partial_\mu K^\mu$, with constant infinitesimal $\alpha$. [Noether theorem](../../../../../noether-theorem.md) gives the [on shell](../../../../../on-shell.md) [conserved current](../../../../../conserved-current.md)

$$
\boxed{J^\mu=\sum_a\frac{\partial\mathcal L}{\partial(\partial_\mu\Phi_a)}\Delta_a-K^\mu,\qquad \partial_\mu J^\mu=0.}
$$

This follows by varying the Lagrangian, integrating the terms with $\partial_\mu\Delta_a$ by parts, and setting the Euler-Lagrange expressions to zero. If spatial boundary flux vanishes, $\int d^3x\,J^0$ is a conserved [Noether charge](../../../../../noether-charge.md). Spacetime symmetries are covered by including the induced field variation at fixed coordinates and the corresponding total derivative $K^\mu$.

An example of a theory with a Lorentz [four-vector](../../../../../four-vector.md) is the source-free [Maxwell field](../../../../../electromagnetic-field.md) with [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md) $A_\mu$. Under an Abelian [gauge transformation](../../../../../gauge-transformation.md),

$$
A_\mu\longmapsto A_\mu+\partial_\mu\chi,\qquad
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu.
$$

The change in $F_{\mu\nu}$ is $\partial_\mu\partial_\nu\chi-\partial_\nu\partial_\mu\chi=0$, so the [Maxwell Lagrangian](../../../../../maxwell-lagrangian.md) is [gauge-invariant](../../../../../gauge-invariance.md). For $A_\mu=(\Phi,-\mathbf A)$ define $E_i=F_{0i}$ and $F_{ij}=-\epsilon_{ijk}B_k$. With signature $+---$,

$$
F_{\mu\nu}F^{\mu\nu}=2(\mathbf B^2-\mathbf E^2),\qquad
\mathcal L=\frac12(\mathbf E^2-\mathbf B^2).
$$

The minus sign in $-F^2/4$ gives the positive electric kinetic term and positive physical field energy; reversing it would reverse the [Hamiltonian](../../../../../hamiltonian.md)'s sign for the physical modes. The normalization $1/4$ accounts for antisymmetry and yields the conventional equations. Varying $A_\nu$ gives $\partial_\mu F^{\mu\nu}=0$.

For time translation at fixed coordinates take $\Delta_\nu=\partial_0A_\nu$. Since $\alpha$ is constant, $\delta F_{\mu\nu}=\alpha\partial_0F_{\mu\nu}$, and hence $\delta\mathcal L=\alpha\partial_0\mathcal L$. Thus $K^\mu=\delta^\mu{}_0\mathcal L$. The momentum derivative is

$$
\frac{\partial\mathcal L}{\partial(\partial_\mu A_\nu)}=-F^{\mu\nu}.
$$

[Noether theorem](../../../../../noether-theorem.md) therefore gives the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md)'s time-translation current

$$
J_{\rm can}^\mu=T_{\rm can}^\mu{}_0
=-F^{\mu\nu}\partial_0A_\nu-\delta^\mu{}_0\mathcal L,
\qquad
\boxed{H_{\rm can}=\int d^3x\left[\frac12(\mathbf E^2+\mathbf B^2)+\mathbf E\cdot\nabla A_0\right].}
$$

Here $\dot A_i=E_i+\partial_iA_0$ was used. The [canonical momentum](../../../../../canonical-momentum.md) of $A_0$ vanishes, while that of the lower spatial component $A_i$ is $E_i$: $A_0$ acts as a multiplier for [Gauss law](../../../../../gauss-s-law.md), not a propagating degree of freedom. The density above is not manifestly [gauge-invariant](../../../../../gauge-invariance.md), but its charge agrees with the physical energy on the constraint surface and with appropriate [boundary conditions](../../../../../boundary-condition.md).

The [gauge-covariant time translation](../../../../../gauge-covariant-time-translation.md) instead has $\Delta_\nu=\partial_0A_\nu-\partial_\nu A_0=F_{0\nu}$. It is time translation combined with a [gauge transformation](../../../../../gauge-transformation.md) of parameter $\chi=-\alpha A_0$. Directly,

$$
\delta F_{\mu\nu}=\alpha(\partial_\mu F_{0\nu}-\partial_\nu F_{0\mu})
=\alpha\partial_0F_{\mu\nu},
$$

using the definition of $F$, equivalently its [Bianchi identity](../../../../../bianchi-identity.md). The total derivative in $\delta\mathcal L$ is unchanged. The improved current is

$$
J_{\rm imp}^\mu=-F^{\mu\nu}F_{0\nu}-\delta^\mu{}_0\mathcal L
=\Theta^\mu{}_0,
\qquad
\Theta^\mu{}_{\nu}=-F^{\mu\rho}F_{\nu\rho}+\frac14\delta^\mu{}_{\nu}F_{\rho\sigma}F^{\rho\sigma}.
$$

It is the [gauge-invariant Maxwell stress-energy tensor](../../../../../gauge-invariant-maxwell-stress-energy-tensor.md). In particular,

$$
\boxed{u=J_{\rm imp}^0=\frac12(\mathbf E^2+\mathbf B^2),\qquad
H=\int d^3x\,u.}
$$

The spatial current is the [Poynting vector](../../../../../poynting-vector.md) $\mathbf E\times\mathbf B$, so conservation gives $\partial_tu+\nabla\cdot(\mathbf E\times\mathbf B)=0$. This is the familiar positive local [electromagnetic field](../../../../../electromagnetic-field.md) energy density, expressed entirely in measurable fields.

To compare the currents,

$$
J_{\rm can}^\mu-J_{\rm imp}^\mu=-F^{\mu\nu}\partial_\nu A_0
=-\partial_\nu(A_0F^{\mu\nu})+A_0\partial_\nu F^{\mu\nu}.
$$

The last term vanishes on the source-free [Maxwell equations](../../../../../maxwell-equations.md), leaving a [stress-energy tensor improvement](../../../../../stress-energy-tensor-improvement.md) generated by a [stress-energy superpotential](../../../../../stress-energy-superpotential.md). At the charge level,

$$
H_{\rm can}-H=\int d^3x\,\mathbf E\cdot\nabla A_0
=\oint A_0\mathbf E\cdot d\mathbf S-\int d^3x\,A_0\nabla\cdot\mathbf E=0
$$

when the surface term vanishes and [Gauss law](../../../../../gauss-s-law.md) holds. Thus the symmetries yield the same conserved energy under these conditions while the second supplies a gauge-invariant local density. Boundary terms would have to be retained if those [boundary conditions](../../../../../boundary-condition.md) were not imposed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
