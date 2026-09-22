<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider a real [Klein-Gordon field](../../../../../../klein-gordon-field.md) on a prescribed [globally hyperbolic spacetime](../../../../../../globally-hyperbolic-spacetime.md), obeying $(\Box-m^2)\phi=0$ with [metric signature](../../../../../../metric-signature.md) $(-,+,+,+)$. A curvature coupling can be included as $m^2\mapsto m^2+\xi R$. A [Cauchy hypersurface](../../../../../../cauchy-surface.md) $\Sigma$ and compactly supported smooth data $(\phi,n^a\nabla_a\phi)$ determine a unique solution; appropriate falloff can replace compact support. The real solution space has conserved [symplectic form](../../../../../../symplectic-form.md)

$$
\Omega(\phi_1,\phi_2)=\int_\Sigma d\Sigma\,(\phi_1n^a\nabla_a\phi_2-\phi_2n^a\nabla_a\phi_1).
$$

Conservation follows by integrating the divergence-free current $\phi_1\nabla^a\phi_2-\phi_2\nabla^a\phi_1$, with no boundary flux. On complex solutions the conserved [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md) is

$$
(u,v)_{KG}=i\int_\Sigma d\Sigma\,(u^*n^a\nabla_av-vn^a\nabla_au^*).
$$

It is indefinite on the full complex solution space.

Choose a complete positive-norm mode subspace, with modes $u_j$ satisfying

$$
(u_i,u_j)_{KG}=\delta_{ij},\quad (u_i^*,u_j^*)_{KG}=-\delta_{ij},\quad (u_i,u_j^*)_{KG}=0.
$$

Equivalently choose a compatible [complex structure on the Klein-Gordon solution space](../../../../../../complex-structure-on-the-klein-gordon-solution-space.md). The mode labels may be continuous, in which case sums and Kronecker symbols become integrals and [Dirac delta functions](../../../../../../dirac-delta-function.md). Construct the one-particle [Hilbert space](../../../../../../hilbert-space-split.md) from these modes and its [bosonic Fock space](../../../../../../bosonic-fock-space.md). Promote the field to the operator-valued distribution

$$
\widehat\phi(x)=\sum_j\left(a_ju_j(x)+a_j^\dagger u_j^*(x)\right),\qquad [a_i,a_j^\dagger]=\delta_{ij},\quad [a_i,a_j]=[a_i^\dagger,a_j^\dagger]=0.
$$

For a foliation with spatial metric determinant $h$, the conjugate momentum density is $\widehat\pi=\sqrt h\,n^a\nabla_a\widehat\phi$. Mode completeness gives the equal-time [canonical commutation relations](../../../../../../canonical-commutation-relation.md)

$$
[\widehat\phi(x),\widehat\pi(y)]=i\delta^3(x-y),\quad [\widehat\phi(x),\widehat\phi(y)]=[\widehat\pi(x),\widehat\pi(y)]=0.
$$

The [Fock vacuum](../../../../../../fock-vacuum.md) obeys $a_j|0\rangle=0$, and $a_j^\dagger a_j$ counts particles in the chosen mode. For local products and a renormalized [stress-energy tensor](../../../../../../stress-energy-tensor.md), physically admissible states are further restricted by the [Hadamard condition](../../../../../../hadamard-condition.md). The field algebra exists without a preferred [Fock vacuum](../../../../../../fock-vacuum.md).

A different admissible mode splitting can mix positive and negative norms:

$$
v_i=\sum_j(\alpha_{ij}u_j+\beta_{ij}u_j^*),\qquad b_i=(v_i,\widehat\phi)_{KG}=\sum_j(\alpha_{ij}^*a_j-\beta_{ij}^*a_j^\dagger).
$$

Orthonormality imposes the [canonical identities for a bosonic Bogoliubov transformation](../../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md)

$$
\alpha\alpha^\dagger-\beta\beta^\dagger=I,\qquad \alpha\beta^T=\beta\alpha^T.
$$

The same field then has

$$
\langle0_a|b_i^\dagger b_i|0_a\rangle=\sum_j|\beta_{ij}|^2.
$$

Without a preferred notion of [positive frequency](../../../../../../positive-frequency-solution.md), a [nonstationary spacetime](../../../../../../nonstationary-spacetime.md) supplies no distinguished mode splitting: **particle number and vacuum depend on the choice of modes, although the field equation and field algebra do not.** With infinitely many modes the [Bogoliubov transformation](../../../../../../bogoliubov-transformation.md) need not be unitarily implementable; finite total mixing requires a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md) $\beta$.

For a stable [strictly stationary spacetime](../../../../../../strictly-stationary-spacetime.md), a chosen future globally timelike [Killing vector field](../../../../../../killing-vector-field.md) $K$ gives a preferred time translation. Choose modes with

$$
i\mathcal L_Ku_j=\omega_ju_j,\qquad \omega_j>0.
$$

When the corresponding conserved [Killing energy](../../../../../../killing-energy.md) is positive and the spectral problem has suitable boundary conditions and no problematic zero modes, this gives the preferred [vacuum state in a stationary spacetime](../../../../../../vacuum-state-in-a-stationary-spacetime.md) and particles relative to $K$. Positive-frequency mode mixing within that same subspace leaves the [Fock vacuum](../../../../../../fock-vacuum.md) unchanged. Rescaling $K$ by a positive constant changes the frequency units but not their sign.

**Stationarity alone, if it only means a Killing field timelike near infinity, is insufficient for a global unique particle interpretation.** In the [Kerr ergoregion](../../../../../../kerr-ergoregion.md), $\partial_t$ is spacelike, so positive frequency relative to $t$ does not automatically select a positive-norm subspace throughout the geometry; [superradiance](../../../../../../superradiance.md) illustrates the difficulty. Additional vacuum and boundary choices remain necessary. The customary stationary answer therefore assumes a suitable timelike stationary flow and a stable positive-energy quantization; it does not assert that every stationary black-hole extension has one globally preferred vacuum.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 311](../../../paper-311-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
