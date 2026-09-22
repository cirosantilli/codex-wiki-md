<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the free [Maxwell Lagrangian](../../../../../maxwell-lagrangian.md) $\mathcal L=-F_{\mu\nu}F^{\mu\nu}/4$ in mostly-minus signature. In terms of the spatial [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md), define $\mathbf E=-\dot{\mathbf A}-\boldsymbol\nabla A_0$ and $\mathbf B=\boldsymbol\nabla\times\mathbf A$. Thus $\mathcal L=(\mathbf E^2-\mathbf B^2)/2$. Taking the Cartesian components of $\mathbf A$ as coordinates gives the [canonical momenta](../../../../../canonical-momentum.md)

$$
\boxed{\Pi^0=0,\qquad \Pi_i=\frac{\partial\mathcal L}{\partial\dot A_i}=\dot A_i+\partial_iA_0=-E_i.}
$$

This sign convention treats $A_i$ here as Cartesian spatial-vector labels; it is not a claim that covariant and contravariant four-vector components coincide.

The temporal momentum vanishes because no $\dot A_0$ occurs. This is the [primary momentum constraint of the electromagnetic potential](../../../../../primary-momentum-constraint-of-the-electromagnetic-potential.md), so one cannot treat all four components as independent unconstrained oscillators. The [Legendre transformation](../../../../../convex-conjugate.md) for the spatial components gives $\Pi_i\dot A_i-\mathcal L=(\boldsymbol\Pi^2+\mathbf B^2)/2-\boldsymbol\Pi\cdot\boldsymbol\nabla A_0$. After integration by parts, the [Hamiltonian](../../../../../hamiltonian.md) is

$$
\boxed{H=\int d^3x\left[\frac12(\boldsymbol\Pi^2+\mathbf B^2)+A_0\boldsymbol\nabla\cdot\boldsymbol\Pi\right].}
$$

Surface terms vanish for decaying fields or the corresponding regulated boundary conditions. The total constrained [Hamiltonian](../../../../../hamiltonian.md) also contains an arbitrary multiplier of $\Pi^0$. Preserving $\Pi^0=0$ under time evolution requires

$$
\dot\Pi^0=-\frac{\delta H}{\delta A_0}=-\boldsymbol\nabla\cdot\boldsymbol\Pi=0,
$$

which is the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md). Both constraints are [first-class constraints](../../../../../first-class-constraint.md); they express the [gauge invariance](../../../../../gauge-invariance.md) $\mathbf A\mapsto\mathbf A+\boldsymbol\nabla\alpha$, $A_0\mapsto A_0-\dot\alpha$. The electric and magnetic fields are unchanged, so different gauge potentials need not describe different physical states.

One consistent [canonical quantization of the electromagnetic field](../../../../../canonical-quantization-of-the-electromagnetic-field.md) first reduces this redundancy. Choose [Coulomb gauge](../../../../../coulomb-gauge.md) $\boldsymbol\nabla\cdot\mathbf A=0$. In the absence of charges, the [Gauss law constraint in gauge theory](../../../../../gauss-law-constraint-in-gauge-theory.md) gives $\nabla^2A_0=0$; decay at infinity sets $A_0=0$. Residual spatially constant gauge parameters do not change $\mathbf A$. The remaining variables are the transverse pairs $\mathbf A^T,\boldsymbol\Pi^T=\dot{\mathbf A}^T$. Their [gauge reduction of the Maxwell Hamiltonian](../../../../../gauge-reduction-of-the-maxwell-hamiltonian.md) is

$$
\boxed{H_T=\frac12\int d^3x\left[(\boldsymbol\Pi^T)^2+(\boldsymbol\nabla\times\mathbf A^T)^2\right].}
$$

The two transverse coordinates for each nonzero momentum are the physical [degrees of freedom](../../../../../degree-of-freedom.md). Treating the constraints as operator identities while retaining unconstrained componentwise commutators would be inconsistent: differentiating $[A_i^T,\Pi_j^T]=i\delta_{ij}\delta^3$ would give a nonzero right side even though $\partial_iA_i^T=0$.

The reduced [Dirac bracket](../../../../../dirac-bracket.md), promoted to a [canonical commutation relation](../../../../../canonical-commutation-relation.md), instead gives the [transverse equal-time commutator](../../../../../transverse-equal-time-commutator.md):

$$
\boxed{[A_i^T(t,\mathbf x),\Pi_j^T(t,\mathbf y)]=i\delta^T_{ij}(\mathbf x-\mathbf y),\qquad
[A_i^T,A_j^T]=[\Pi_i^T,\Pi_j^T]=0,}
$$

where

$$
\delta^T_{ij}(\mathbf r)=\int\frac{d^3k}{(2\pi)^3}e^{i\mathbf k\cdot\mathbf r}
\left(\delta_{ij}-\frac{k_i k_j}{|\mathbf k|^2}\right).
$$

Indeed the spatial [transverse projector of a vector field](../../../../../transverse-projector-of-a-vector-field.md) $P^T_{ij}=\delta_{ij}-k_ik_j/|\mathbf k|^2$ is symmetric, has $P^T\mathbf k=0$ and $(P^T)^2=P^T$. Projecting both entries of the unconstrained canonical bracket onto the transverse subspace therefore produces $P^T\delta^3$, equivalently the constrained [Dirac bracket](../../../../../dirac-bracket.md). The spatial zero mode is excluded by the decay condition; in a finite-volume regulator it must be treated separately.

Choose two orthonormal transverse [photon polarization vectors](../../../../../photon-polarization-vector.md) $\boldsymbol\epsilon_r(\mathbf k)$, so that

$$
\mathbf k\cdot\boldsymbol\epsilon_r=0,\qquad
\boldsymbol\epsilon_r^*\cdot\boldsymbol\epsilon_s=\delta_{rs},\qquad
\sum_{r=1}^2\epsilon_i^{(r)}\epsilon_j^{(r)*}=P^T_{ij}.
$$

The [canonical transverse photon field](../../../../../canonical-transverse-photon-field.md) has mode expansion

$$
A_i^T(x)=\sum_{r=1}^2\int\frac{d^3k}{(2\pi)^3\sqrt{2\omega_{\mathbf k}}}
\left[\epsilon_i^{(r)}(\mathbf k)a_r(\mathbf k)e^{-ik\cdot x}
+\epsilon_i^{(r)*}(\mathbf k)a_r^\dagger(\mathbf k)e^{ik\cdot x}\right],
\qquad \omega_{\mathbf k}=|\mathbf k|.
$$

Differentiate in time to obtain $\Pi_i^T$: the annihilation coefficient acquires $-i\omega_{\mathbf k}$ and the creation coefficient $+i\omega_{\mathbf k}$. The oscillator [canonical commutation relations](../../../../../canonical-commutation-relation.md) are

$$
\boxed{[a_r(\mathbf k),a_s^\dagger(\mathbf q)]=(2\pi)^3\delta_{rs}\delta^3(\mathbf k-\mathbf q),\qquad
[a_r,a_s]=[a_r^\dagger,a_s^\dagger]=0.}
$$

Substitution into $[A_i^T,\Pi_j^T]$ gives $i/2$ times the sum of the two Fourier kernels with phases $\pm i\mathbf k\cdot(\mathbf x-\mathbf y)$. The polarization completeness relation and the evenness of $P^T(\mathbf k)$ make that sum exactly $i\delta^T_{ij}$. This derives, rather than presumes, the correspondence between the oscillator and field commutators.

Substitute the mode expansions into $H_T$. Spatial integration sets paired momenta equal or opposite. The $aa$ and $a^\dagger a^\dagger$ terms from the electric and magnetic energies cancel because $\omega_{\mathbf k}^2=|\mathbf k|^2$ and $\mathbf k\cdot\boldsymbol\epsilon_r=0$. The remaining terms are harmonic-oscillator energies. Removing the state-independent zero-point energy by [normal ordering](../../../../../normal-ordering.md) gives

$$
\boxed{:\!H_T\!:=\sum_{r=1}^2\int\frac{d^3k}{(2\pi)^3}\omega_{\mathbf k}
 a_r^\dagger(\mathbf k)a_r(\mathbf k).}
$$

The corresponding [momentum operator](../../../../../momentum-operator.md) is $\mathbf P=\sum_r\int d^3k\,\mathbf k\,a_r^\dagger a_r/(2\pi)^3$. These expressions imply $[H_T,a_r^\dagger(\mathbf k)]=\omega_{\mathbf k}a_r^\dagger(\mathbf k)$ and $[\mathbf P,a_r^\dagger(\mathbf k)]=\mathbf k a_r^\dagger(\mathbf k)$.

Define the [Fock vacuum](../../../../../fock-vacuum.md) by $a_r(\mathbf k)|0\rangle=0$. Applying $a_r^\dagger(\mathbf k)$ creates a **[photon](../../../../../photon.md) of energy $|\mathbf k|$, momentum $\mathbf k$, and one of two transverse polarizations**. Its mass is zero because $k^2=0$. The relativistically normalized state is $|\mathbf k,r\rangle=\sqrt{2\omega_{\mathbf k}}a_r^\dagger(\mathbf k)|0\rangle$, with inner product $2\omega_{\mathbf k}(2\pi)^3\delta_{rs}\delta^3(\mathbf k-\mathbf q)$. Smearing these momentum eigenstates gives normalizable wave packets. Repeated commuting [bosonic creation operators](../../../../../bosonic-creation-operator.md) construct the symmetric multiphoton [bosonic Fock space](../../../../../bosonic-fock-space.md). Circular combinations of the two transverse [photon polarization vectors](../../../../../photon-polarization-vector.md) transform with opposite phases under rotations about $\mathbf k$, giving the two physical [helicities](../../../../../helicity.md) $\boxed{h=\pm1}$.

The same physical states can be obtained while retaining manifest Lorentz covariance through [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md). Add the [Feynman gauge](../../../../../feynman-gauge.md) term $-(\partial_\mu A^\mu)^2/2$ and quantize four auxiliary oscillator polarizations. Their algebra has an indefinite metric, including a negative-norm temporal excitation. Impose $(\partial_\mu A^\mu)^{(+)}|\mathrm{phys}\rangle=0$ and take the [Gupta-Bleuler null-state quotient](../../../../../gupta-bleuler-null-state-quotient.md). Temporal and longitudinal excitations then do not survive as independent physical states. The result agrees with the positive, two-polarization space obtained by [Coulomb gauge](../../../../../coulomb-gauge.md) reduction; covariant gauge fixing is a different implementation of the same physical constraint, not four physical photon states.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
