<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use signature $(+---)$ and take the covariant spatial components $A_i$ as canonical coordinates. The [canonical quantization of the electromagnetic field](../../../../../canonical-quantization-of-the-electromagnetic-field.md) begins with the canonical momenta

$$
\Pi^\mu=\frac{\partial\mathcal L}{\partial(\partial_0A_\mu)}=-F^{0\mu},\qquad\Pi^0=0,\qquad\Pi^i=F_{0i}=\dot A_i-\partial_iA_0.
$$

Thus the [primary momentum constraint of the electromagnetic potential](../../../../../primary-momentum-constraint-of-the-electromagnetic-potential.md) is $\Pi^0=0$: $A_0$ has no independent velocity. The [Hamiltonian](../../../../../hamiltonian.md) obtained by the [Legendre transform in mechanics](../../../../../legendre-transform-in-mechanics.md), up to a boundary term, is

$$
H=\int d^3x\left[\frac12\Pi^i\Pi^i+\frac14F_{ij}F_{ij}-A_0\partial_i\Pi^i\right].
$$

Preserving the primary constraint requires the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md), $\partial_i\Pi^i=0$. It also follows by varying $A_0$. These are two [first-class constraints](../../../../../first-class-constraint.md); they generate the gauge freedom and remove two [canonical pairs](../../../../../canonical-pair.md) from the four potential components. The reduced phase space has four dimensions per spatial mode, hence **two propagating [photon](../../../../../photon.md) degrees of freedom**.

Impose [Coulomb gauge](../../../../../coulomb-gauge.md), $\partial_iA_i=0$. With no charges, [Gauss's law](../../../../../gauss-s-law.md) then gives $\nabla^2A_0=0$; vanishing boundary conditions set $A_0=0$. This is [radiation gauge](../../../../../radiation-gauge.md). The remaining components are transverse and obey the massless [wave equation](../../../../../wave-equation-split.md). Let $\epsilon_i^{(r)}(\mathbf k)$, $r=1,2$, be orthonormal transverse [polarization vectors](../../../../../polarization-vector.md). Their [photon polarization completeness relation](../../../../../photon-polarization-completeness-relation.md) is

$$
k_i\epsilon_i^{(r)}=0,\qquad\sum_{r=1}^2\epsilon_i^{(r)}\epsilon_j^{(r)*}=P^T_{ij}(\mathbf k):=\delta_{ij}-\frac{k_ik_j}{|\mathbf k|^2}.
$$

The [canonical transverse photon field](../../../../../canonical-transverse-photon-field.md) is the Hermitian operator

$$
A_i^T(x)=\sum_{r=1}^2\int\frac{d^3k}{(2\pi)^3\sqrt{2\omega_{\mathbf k}}}\left[\epsilon_i^{(r)}a_r(\mathbf k)e^{-ik\cdot x}+\epsilon_i^{(r)*}a_r^\dagger(\mathbf k)e^{ik\cdot x}\right],\qquad\omega_{\mathbf k}=|\mathbf k|,
$$

where

$$
[a_r(\mathbf k),a_s^\dagger(\mathbf k')]=(2\pi)^3\delta_{rs}\delta^3(\mathbf k-\mathbf k'),\qquad[a_r,a_s]=[a_r^\dagger,a_s^\dagger]=0.
$$

The field and its [conjugate momentum](../../../../../canonical-momentum.md) have the [transverse equal-time commutator](../../../../../transverse-equal-time-commutator.md)

$$
[A_i^T(t,\mathbf x),\Pi^{Tj}(t,\mathbf y)]=i\delta^T_{ij}(\mathbf x-\mathbf y),\qquad\delta^T_{ij}(\mathbf x)=\int\frac{d^3k}{(2\pi)^3}P^T_{ij}(\mathbf k)e^{i\mathbf k\cdot\mathbf x}.
$$

This is the quantized reduced bracket, or equivalently the [Dirac bracket](../../../../../dirac-bracket.md) after imposing the constraints and gauge conditions. The normal-ordered [Hamiltonian](../../../../../hamiltonian.md) is $\sum_r\int d^3k\,\omega_{\mathbf k}a_r^\dagger a_r/(2\pi)^3$. Its excitations are [photons](../../../../../photon.md); circular combinations of the two transverse polarizations have [helicity](../../../../../helicity.md) $+1$ and $-1$. The scalar and longitudinal potential components do not create additional physical [photons](../../../../../photon.md).

The [Feynman propagator](../../../../../feynman-propagator.md) is the vacuum expectation of a [time-ordered product](../../../../../time-ordered-product.md). The mode expansion directly gives the [radiation-gauge photon propagator](../../../../../radiation-gauge-photon-propagator.md), with $z=x-y$:

$$
\begin{aligned}
D^F_{ij}(z)&=\int\frac{d^3k}{(2\pi)^3}\frac{P^T_{ij}(\mathbf k)}{2\omega_{\mathbf k}}e^{i\mathbf k\cdot\mathbf z}\left[\theta(z^0)e^{-i\omega_{\mathbf k}z^0}+\theta(-z^0)e^{i\omega_{\mathbf k}z^0}\right]\\
&=\int\frac{d^4k}{(2\pi)^4}\frac{iP^T_{ij}(\mathbf k)}{k^2+i0}e^{-ik\cdot z}.
\end{aligned}
$$

The first expression comes from the creation-annihilation commutator; the second is its contour-integral representation. The positive-energy pole lies below the real axis and the negative-energy pole above it. In this reduced free-field description, the temporal operator is zero. A [photon propagator](../../../../../photon-propagator.md) must specify its gauge; the spatial transverse propagator is not the same tensor as the covariant four-potential propagator.

For the commonly used covariant form, add the [gauge fixing](../../../../../gauge-fixing.md) term $-(\partial_\mu A^\mu)^2/(2\xi)$. The resulting Fourier-space kinetic operator is

$$
K^{\mu\nu}(k)=-k^2\eta^{\mu\nu}+(1-\xi^{-1})k^\mu k^\nu.
$$

The [inversion of the gauge-fixed Maxwell kinetic operator](../../../../../inversion-of-the-gauge-fixed-maxwell-kinetic-operator.md) gives $K^{\mu\nu}D^F_{\nu\rho}=i\delta^\mu{}_{\rho}$. In [Feynman gauge](../../../../../feynman-gauge.md), $\xi=1$, the [photon propagator](../../../../../photon-propagator.md) is

$$
\boxed{D^F_{\mu\nu}(x-y)=\int\frac{d^4k}{(2\pi)^4}\frac{-i\eta_{\mu\nu}}{k^2+i0}e^{-ik\cdot(x-y)}.}
$$

Equivalently, $\Box D^F_{\mu\nu}=i\eta_{\mu\nu}\delta^4(x-y)$ with the vacuum pole prescription. For general $\xi$, the momentum-space numerator is $\eta_{\mu\nu}-(1-\xi)k_\mu k_\nu/(k^2+i0)$.

A covariant canonical realization uses four polarization oscillators with $[a_r,a_s^\dagger]=-(2\pi)^3\eta_{rs}\delta^3(\mathbf k-\mathbf k')$. The resulting indefinite [inner product](../../../../../inner-product.md) is auxiliary. In [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md), impose $(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0$ and take the [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md). The scalar-longitudinal combination is thereby removed from the physical state space, leaving the same two transverse [photon](../../../../../photon.md) states. Thus the four-component Feynman-gauge numerator does not imply four physical polarization states.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
