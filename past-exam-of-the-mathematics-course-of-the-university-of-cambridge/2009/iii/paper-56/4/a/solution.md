<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a real free [Klein-Gordon field](../../../../../../klein-gordon-field.md) on a prescribed four-dimensional [globally hyperbolic spacetime](../../../../../../globally-hyperbolic-spacetime.md), with signature $(-+++)$ and $\hbar=c=1$. A mass $\mu$ and curvature coupling $\xi$ give the quadratic action

$$
S[\phi]=-\frac12\int d^4x\sqrt{-g}\left(g^{ab}\nabla_a\phi\nabla_b\phi+(\mu^2+\xi R)\phi^2\right),
$$

and the field equation $\boxed{(\Box-\mu^2-\xi R)\phi=0}$. Minimal coupling is $\xi=0$; for a massless scalar in four dimensions, conformal coupling is $\xi=1/6$. [Global hyperbolicity](../../../../../../globally-hyperbolic-spacetime.md) supplies a [Cauchy hypersurface](../../../../../../cauchy-surface.md) $\Sigma$ and a well-posed initial-value problem: suitable data $(\phi,n^a\nabla_a\phi)$ on $\Sigma$ determine a unique solution. One assumes appropriate support or decay conditions so no unaccounted flux crosses spatial infinity. The geometry is classical here; quantum backreaction is a further problem.

The real solution space has the conserved [symplectic form on scalar-field solutions](../../../../../../symplectic-form-on-scalar-field-solutions.md)

$$
\Omega(\phi_1,\phi_2)=\int_\Sigma
(\phi_1n^a\nabla_a\phi_2-\phi_2n^a\nabla_a\phi_1)\,d\Sigma.
$$

Its complexification defines the [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md)

$$
(u,v)_{KG}=i\int_\Sigma n^a(u^*\nabla_av-v\nabla_au^*)\,d\Sigma.
$$

The divergence of its current is $i(u^*\Box v-v\Box u^*)=0$ by the field equation, proving independence of the chosen [Cauchy hypersurface](../../../../../../cauchy-surface.md). This Hermitian form is not positive definite on the whole complex solution space: conjugating a solution reverses its norm.

Choose a complete positive-norm mode space and basis $u_i$ satisfying

$$
(u_i,u_j)_{KG}=\delta_{ij},\qquad
(u_i^*,u_j^*)_{KG}=-\delta_{ij},\qquad
(u_i,u_j^*)_{KG}=0.
$$

Here completeness means that every real solution expands in these modes and their conjugates. Equivalently, one chooses a compatible [complex structure on the Klein-Gordon solution space](../../../../../../complex-structure-on-the-klein-gordon-solution-space.md); this is extra data, not fixed by the field equation. Quantization replaces the mode coefficients by [annihilation operators](../../../../../../annihilation-operator.md) and [creation operators](../../../../../../creation-operator.md):

$$
\widehat\phi(x)=\sum_i\bigl(a_i u_i(x)+a_i^\dagger u_i(x)^*\bigr),\qquad
\boxed{[a_i,a_j^\dagger]=\delta_{ij},\quad[a_i,a_j]=0.}
$$

In a foliation with induced metric determinant $h$, the canonical momentum is $\pi=\sqrt h\,n^a\nabla_a\phi$. The normalized complete mode expansion implements the equal-time [canonical commutation relations](../../../../../../canonical-commutation-relation.md) $[\widehat\phi(x),\widehat\pi(y)]=i\delta^3(x-y)$ and vanishing field-field and momentum-momentum commutators on $\Sigma$. Propagation by the field equation gives [microcausality](../../../../../../microcausality.md): field observables commute at spacelike separation. Thus there is a local quantum field theory before one has selected a particle interpretation.

The chosen positive-mode space completes to a one-particle [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal H_1$. Its [bosonic Fock space](../../../../../../bosonic-fock-space.md) is $\bigoplus_{n=0}^\infty\operatorname{Sym}^n\mathcal H_1$. The [Fock vacuum](../../../../../../fock-vacuum.md) obeys $a_i|0\rangle=0$; acting with $a_i^\dagger$ produces multiparticle states, and $N_i=a_i^\dagger a_i$ counts particles in mode $i$. The vacuum two-point function is $W(x,y)=\sum_i u_i(x)u_i(y)^*$. The [Hadamard condition](../../../../../../hadamard-condition.md) restricts physically admissible states by prescribing their local short-distance singularity; it permits renormalization of the [stress-energy tensor](../../../../../../stress-energy-tensor.md) but does not select one unique vacuum.

The particle ambiguity is that there is generally no distinguished choice of positive-mode space. A second complete normalized basis can be

$$
v_i=\sum_j(\alpha_{ij}u_j+\beta_{ij}u_j^*).
$$

The [Bogoliubov transformation](../../../../../../bogoliubov-transformation.md) preserves the mode normalization precisely when

$$
\alpha\alpha^\dagger-\beta\beta^\dagger=I,\qquad
\alpha\beta^T-\beta\alpha^T=0.
$$

Its operators obey $b_i=(v_i,\widehat\phi)_{KG}=\sum_j(\alpha_{ij}^*a_j-\beta_{ij}^*a_j^\dagger)$. Consequently a state with no $a$-particles generally has $b$-particles if $\beta\ne0$. A unitary change of basis within the same positive-mode space has $\beta=0$ and merely relabels modes; a change mixing the positive and negative subspaces changes the vacuum and particle notion. Arbitrary coordinates called “time” do not resolve this choice. This is the [vacuum ambiguity in a nonstationary spacetime](../../../../../../vacuum-ambiguity-in-a-nonstationary-spacetime.md), while the field equation and local commutator remain unchanged.

In the standard stationary setting, a complete future-directed timelike [Killing vector field](../../../../../../killing-vector-field.md) $K$ generates a time-translation symmetry. With a stable positive energy operator and suitable boundary conditions, choose [positive-frequency solutions](../../../../../../positive-frequency-solution.md) by

$$
i\mathcal L_Ku_\omega=\omega u_\omega,\qquad\omega>0.
$$

The [positive stationary Hamiltonian selects a particle splitting](../../../../../../positive-stationary-hamiltonian-selects-a-particle-splitting.md): positive spectral modes define annihilation operators, and the normal-ordered Hamiltonian is $H_K=\sum_i\omega_i a_i^\dagger a_i$. Its ground state is the [vacuum state in a stationary spacetime](../../../../../../vacuum-state-in-a-stationary-spacetime.md). The Killing symmetry transports this splitting unchanged, so no positive-negative mixing is induced by stationary evolution. Degeneracies allow unitary basis changes without changing the vacuum. Stationarity fixes the ground-state particle interpretation relative to this time flow; it does not forbid excited or thermal states.

The qualification is that asymptotic stationarity alone, in the sense used for a Kerr exterior, is insufficient for a global positive-energy construction: $K$ becomes spacelike in an [ergoregion of a stationary spacetime](../../../../../../ergoregion-of-a-stationary-spacetime.md). The usual unambiguous construction applies to a [strictly stationary spacetime](../../../../../../strictly-stationary-spacetime.md) with the stated stability and spectral assumptions, or to appropriate stationary asymptotic regions for scattering. Zero modes or instability need separate treatment. Likewise different observer time flows on different regions need not define the same particles.

For [particle creation by a nonstationary spacetime](../../../../../../particle-creation-by-a-nonstationary-spacetime.md), choose normalized positive-frequency modes $u_j^{\rm in}$ in the stationary early region and $u_i^{\rm out}$ in the stationary late region. Propagate both sets by the [Klein-Gordon equation](../../../../../../klein-gordon-equation.md) through the intermediate time-dependent geometry. Compute their overlaps on any common [Cauchy hypersurface](../../../../../../cauchy-surface.md):

$$
u_i^{\rm out}=\sum_j\left(\alpha_{ij}u_j^{\rm in}+\beta_{ij}u_j^{{\rm in}*}\right),\qquad
\alpha_{ij}=(u_j^{\rm in},u_i^{\rm out})_{KG},\quad
\beta_{ij}=-(u_j^{{\rm in}*},u_i^{\rm out})_{KG}.
$$

The initial [in-vacuum](../../../../../../in-vacuum.md) has $a_j^{\rm in}|0_{\rm in}\rangle=0$. Since $a_i^{\rm out}=\sum_j(\alpha_{ij}^*a_j^{\rm in}-\beta_{ij}^*a_j^{{\rm in}\dagger})$, contracting the in operators yields the [particle number from Bogoliubov coefficients](../../../../../../particle-number-from-bogoliubov-coefficients.md):

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle
=\sum_j|\beta_{ij}|^2,\qquad
\langle N_{\rm out}\rangle=\sum_{i,j}|\beta_{ij}|^2.}
$$

Thus the procedure is to fix asymptotic mode choices, solve the classical wave equation, project using the conserved inner product, and take squared negative-frequency overlaps. Particle energy comes from the time-dependent background, so particle creation does not contradict the linear deterministic field equation. For an initial state diagonal in in-mode occupation numbers $n_j$, with no anomalous correlations, the more general expectation is $\sum_j[|\alpha_{ij}|^2n_j+|\beta_{ij}|^2(n_j+1)]$.

For continuous spectra, sums become integrals and normalized wave packets avoid meaningless squares of delta functions. A finite total count requires the appropriate convergence of the double sum or integral. The [bosonic mode mixing implementability](../../../../../../bosonic-mode-mixing-implementability.md) condition is that $\beta$ be Hilbert-Schmidt; otherwise the two Fock representations need not be unitarily equivalent, even though the local field algebra and finite-mode particle calculations still make sense. This distinction between deterministic field evolution and a chosen representation is essential to [quantum field theory in curved spacetime](../../../../../../quantum-field-theory-in-curved-spacetime.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 56](../../../paper-56-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
