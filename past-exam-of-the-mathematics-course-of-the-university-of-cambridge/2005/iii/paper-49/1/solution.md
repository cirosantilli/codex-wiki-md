<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(1,-1,-1,-1)$ and the free [real scalar field](../../../../../real-scalar-field.md) Lagrangian density $\mathcal L=\tfrac12\partial_\mu\phi\partial^\mu\phi-\tfrac12m^2\phi^2$. Its conjugate [canonical momentum](../../../../../canonical-momentum.md) is $\pi=\dot\phi$. Spatial [translation symmetry](../../../../../translational-symmetry.md) and [Noether's theorem](../../../../../noether-conserved-quantity-for-a-mechanical-point-symmetry.md) give the [canonical stress-energy tensor](../../../../../canonical-stress-energy-tensor.md)

$$
T^{\mu\nu}=\partial^\mu\phi\partial^\nu\phi-\eta^{\mu\nu}\mathcal L,
\qquad
\partial_\mu T^{\mu\nu}=(\Box\phi+m^2\phi)\partial^\nu\phi=0.
$$

Vanishing boundary flux then makes the [four-momentum of a free real scalar field](../../../../../four-momentum-of-a-free-real-scalar-field.md) constant. In particular the contravariant spatial [momentum](../../../../../momentum.md) is

$$
\boxed{\mathbf P=-\int\pi\,\boldsymbol\nabla\phi\,d^3x}.
$$

The minus sign is from $\partial^i=-\partial_i$; it is essential for the following mode calculation.

In the quantized theory, insert the mode expansions into this integral, using a Hermitian symmetric ordering or [normal ordering](../../../../../normal-ordering.md). Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. The spatial integral is $(2\pi)^3\delta^{(3)}(\mathbf p\pm\mathbf k)$, leaving

$$
\mathbf P=\frac12\int_{\mathbf p}\mathbf p\left(a_{\mathbf p}a_{\mathbf p}^\dagger+a_{\mathbf p}^\dagger a_{\mathbf p}
-a_{-\mathbf p}a_{\mathbf p}-a_{-\mathbf p}^\dagger a_{\mathbf p}^\dagger\right).
$$

Each last term integrates to zero: replace $\mathbf p$ by $-\mathbf p$ and commute the two [annihilation operators](../../../../../annihilation-operator.md) or the two [creation operators](../../../../../creation-operator.md). The mixed terms reorder by the [canonical commutation relation](../../../../../canonical-commutation-relation.md). Their vacuum contribution is proportional to the integral of the odd vector $\mathbf p$ and vanishes with an inversion-symmetric regulator; [normal ordering](../../../../../normal-ordering.md) removes it directly. Thus the [normal-ordered free scalar four-momentum](../../../../../normal-ordered-free-scalar-four-momentum.md) has spatial part

$$
\boxed{\mathbf P=\int_{\mathbf p}\mathbf p\,a_{\mathbf p}^\dagger a_{\mathbf p}}.
$$

These manipulations can be made first with box modes and a symmetric [momentum](../../../../../momentum.md) cutoff, then used on finite-particle wave packets.

The [commutator derivation identity](../../../../../commutator-derivation-identity.md) gives

$$
[P_i,a_{\mathbf q}^\dagger]=\int_{\mathbf p}p_i a_{\mathbf p}^\dagger[a_{\mathbf p},a_{\mathbf q}^\dagger]
=q_i a_{\mathbf q}^\dagger,
\qquad [P_i,a_{\mathbf q}]=-q_i a_{\mathbf q}.
$$

For $U(\mathbf y)=e^{-i\mathbf P\cdot\mathbf y}$, the [commutator expansion for exponential conjugation](../../../../../commutator-expansion-for-exponential-conjugation.md) therefore gives the [translation of a scalar creation operator](../../../../../translation-of-a-scalar-creation-operator.md)

$$
\boxed{U(\mathbf y)a_{\mathbf q}^\dagger U(\mathbf y)^\dagger
=e^{-i\mathbf q\cdot\mathbf y}a_{\mathbf q}^\dagger}.
$$

The vacuum has zero [momentum](../../../../../momentum.md), so $U|0\rangle=|0\rangle$. Hence the one-particle [momentum eigenstate](../../../../../momentum-eigenstate.md) obeys $U|\mathbf q\rangle=e^{-i\mathbf q\cdot\mathbf y}|\mathbf q\rangle$: translation preserves its [momentum](../../../../../momentum.md) and multiplies it by the associated phase.

The [annihilation operator](../../../../../annihilation-operator.md) receives the opposite phase. Substituting both phases into the field expansion gives

$$
\boxed{U(\mathbf y)\phi(\mathbf x)U(\mathbf y)^\dagger=\phi(\mathbf x+\mathbf y)}.
$$

This is the specified conjugation convention for the [spatial translation operator](../../../../../spatial-translation-operator.md). On states, the active translation moves a wave packet by $\mathbf y$, giving a position wavefunction $\psi(\mathbf x-\mathbf y)$. Conjugating the field by $U^\dagger$ instead would give the opposite argument shift. Infinitesimally the displayed result is $[P_i,\phi]=i\partial_i\phi$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
