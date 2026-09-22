<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix a classical [globally hyperbolic spacetime](../../../../../../globally-hyperbolic-spacetime.md) with [metric signature](../../../../../../metric-signature.md) $(-+++)$; in this solution take $\hbar=1$. A free real [Klein-Gordon field](../../../../../../klein-gordon-field.md) can be specified by

$$
S[\phi]=-\frac12\int\sqrt{-g}\,d^4x\left(g^{ab}\nabla_a\phi\nabla_b\phi+(\mu^2+\xi\mathcal R)\phi^2\right),\qquad (\Box-\mu^2-\xi\mathcal R)\phi=0,
$$

where $\mu$ is its mass, $\xi$ its curvature coupling and $\mathcal R$ the [scalar curvature](../../../../../../scalar-curvature.md). [Global hyperbolicity](../../../../../../globally-hyperbolic-spacetime.md) ensures a well-posed initial-value problem on a [Cauchy hypersurface](../../../../../../cauchy-surface.md) $\Sigma$ and the existence of retarded and advanced propagators. Thus compactly supported field and normal-derivative data determine a classical solution. This fixes the dynamics, but not a [Fock vacuum](../../../../../../fock-vacuum.md).

For real solutions with suitable support or falloff, the [symplectic form on scalar-field solutions](../../../../../../symplectic-form-on-scalar-field-solutions.md) is

$$
\Omega(\phi_1,\phi_2)=\int_\Sigma d\Sigma\,\left(\phi_1n^a\nabla_a\phi_2-\phi_2n^a\nabla_a\phi_1\right),
$$

with $n$ the future unit normal. The field equation makes the current conserved, so this [symplectic form](../../../../../../symplectic-form.md) is independent of $\Sigma$ when boundary flux vanishes. Quantize the initial data by the [canonical commutation relation](../../../../../../canonical-commutation-relation.md): with $\pi=n^a\nabla_a\phi$ and the delta function defined relative to $d\Sigma$, $[\widehat\phi(x),\widehat\pi(y)]=i\delta_\Sigma(x,y)$ and the two equal-field commutators vanish. Equivalently, construct the field algebra using the causal propagator. A state on that algebra is additional input.

To construct a particle representation, complexify the classical solution space. Its conserved [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md) is

$$
(u,v)_{KG}=i\int_\Sigma d\Sigma\,\left(u^*n^a\nabla_av-vn^a\nabla_au^*\right).
$$

It is indefinite on all complex solutions. Choose a complete positive-norm subspace and an orthonormal mode basis $u_i$ with $(u_i,u_j)=\delta_{ij}$, $(u_i^*,u_j^*)=-\delta_{ij}$ and $(u_i,u_j^*)=0$. Such a choice is encoded by a compatible [complex structure on the Klein-Gordon solution space](../../../../../../complex-structure-on-the-klein-gordon-solution-space.md). Its positive subspace gives the one-particle [Hilbert space](../../../../../../hilbert-space-split.md), and the associated [bosonic Fock space](../../../../../../bosonic-fock-space.md) contains symmetrized many-particle states. The field expansion is

$$
\widehat\phi=\sum_i(a_i u_i+a_i^\dagger u_i^*),\qquad [a_i,a_j^\dagger]=\delta_{ij},\qquad a_i|0\rangle=0.
$$

The [creation operator](../../../../../../creation-operator.md) $a_i^\dagger$ adds a particle in mode $i$, the [annihilation operator](../../../../../../annihilation-operator.md) removes one, and the [number operator](../../../../../../number-operator.md) is $N_i=a_i^\dagger a_i$. For continuous mode labels the sums and Kronecker deltas become integrals and delta functions, or one can work with normalized wave packets.

The ambiguity is precisely that the field equation and [global hyperbolicity](../../../../../../globally-hyperbolic-spacetime.md) do not select that positive subspace. A different normalized basis may mix $u_j$ and $u_j^*$ by a [Bogoliubov transformation](../../../../../../bogoliubov-transformation.md), and then its [annihilation operators](../../../../../../annihilation-operator.md) mix $a_j$ and $a_j^\dagger$. Its [Fock vacuum](../../../../../../fock-vacuum.md) and [number operators](../../../../../../number-operator.md) differ. The [Hadamard condition](../../../../../../hadamard-condition.md) constrains physically acceptable short-distance singularities and allows local renormalization, but it still leaves many states. Hence there is generally no observer-independent particle count on an arbitrary dynamical geometry.

In a stable [strictly stationary spacetime](../../../../../../strictly-stationary-spacetime.md), a globally future timelike [Killing vector field](../../../../../../killing-vector-field.md) $K$ gives a preferred time translation. Fix its normalization and suitable boundary conditions, and choose [positive-frequency solutions](../../../../../../positive-frequency-solution.md) satisfying $i\mathcal L_Ku=\omega u$ with $\omega>0$. The corresponding positive spectral subspace gives the preferred [vacuum state in a stationary spacetime](../../../../../../vacuum-state-in-a-stationary-spacetime.md). Unitary changes of basis within it leave the vacuum and the particle notion unchanged. This construction assumes a well-defined positive stationary generator; stationarity by itself is insufficient if $K$ becomes spacelike, as in a [Kerr ergoregion](../../../../../../kerr-ergoregion.md), or if unstable or zero modes obstruct the ground-state construction. It selects a preferred ground state under the stated assumptions, not a unique state among all thermal and excited states.

If the geometry is suitably stationary in the asymptotic past and future, choose those preferred mode spaces separately, giving the [in-vacuum](../../../../../../in-vacuum.md) and [out-vacuum](../../../../../../out-vacuum.md). Propagate the past modes through the intervening region using the field equation and compare them to the future modes using the conserved [Klein-Gordon inner product](../../../../../../klein-gordon-inner-product.md). Adopt the convention

$$
u_i^{\rm out}=\sum_j\left(\alpha_{ij}u_j^{\rm in}+\beta_{ij}u_j^{{\rm in}*}\right),\qquad \alpha_{ij}=(u_j^{\rm in},u_i^{\rm out})_{KG},\quad \beta_{ij}=-(u_j^{{\rm in}*},u_i^{\rm out})_{KG}.
$$

The [canonical identities for a bosonic Bogoliubov transformation](../../../../../../canonical-identities-for-a-bosonic-bogoliubov-transformation.md) read $\alpha\alpha^\dagger-\beta\beta^\dagger=I$ and $\alpha\beta^T=\beta\alpha^T$. Extracting the future [annihilation operator](../../../../../../annihilation-operator.md) with the same inner product gives

$$
b_i=(u_i^{\rm out},\widehat\phi)_{KG}=\sum_j\left(\alpha_{ij}^*a_j-\beta_{ij}^*a_j^\dagger\right).
$$

In the [in-vacuum](../../../../../../in-vacuum.md), only $\langle a_j a_k^\dagger\rangle=\delta_{jk}$ contributes to $\langle b_i^\dagger b_i\rangle$. Therefore the [particle number from Bogoliubov coefficients](../../../../../../particle-number-from-bogoliubov-coefficients.md) is

$$
\boxed{\langle0_{\rm in}|N_i^{\rm out}|0_{\rm in}\rangle=\sum_j|\beta_{ij}|^2.}
$$

Nonzero $\beta$ is the production of future particles from the past vacuum. Summing over future modes gives the total expected particle number when that sum is finite. For infinitely many modes, a [Hilbert-Schmidt operator](../../../../../../hilbert-schmidt-operator.md) $\beta$ is the condition for unitary implementability between these pure [bosonic Fock space](../../../../../../bosonic-fock-space.md) representations; finite-volume or wave-packet calculations must respect the relevant measures and convergence. **Particle production is determined by the negative-frequency mixing**, rather than by identifying a single instantaneous vacuum throughout the time-dependent region.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
