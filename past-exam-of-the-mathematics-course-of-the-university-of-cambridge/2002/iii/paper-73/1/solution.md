<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a globally static region, choose the time coordinate along the future timelike [Killing vector field](../../../../../killing-vector-field.md) $K=\partial_t$. A [positive-frequency solution](../../../../../positive-frequency-solution.md) of the [Klein-Gordon equation](../../../../../klein-gordon-equation.md) has $i\mathcal L_Kp_i=\omega_i p_i$, with $\omega_i>0$. Assume appropriate boundary conditions and a [Cauchy surface](../../../../../cauchy-surface.md) so that the conserved [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) is

$$
(f,g)=i\int_\Sigma d\Sigma^a\bigl(f^*\nabla_ag-g\nabla_af^*\bigr).
$$

For a real scalar, take the negative-frequency modes to be $n_i=p_i^*$. Choose a complete normalized basis with

$$
(p_i,p_j)=\delta_{ij},\qquad(n_i,n_j)=-\delta_{ij},\qquad(p_i,n_j)=0.
$$

The negative norm of the conjugate modes is crucial; this is not a positive-definite inner product on all classical solutions.

Promote the real [Klein-Gordon field](../../../../../klein-gordon-field.md) to the operator

$$
\widehat\phi=\sum_i(p_i a_i+n_i a_i^\dagger),\qquad
[a_i,a_j^\dagger]=\delta_{ij},\quad[a_i,a_j]=0.
$$

These [canonical commutation relations](../../../../../canonical-commutation-relation.md) implement the canonical field and conjugate-momentum commutator. The static [vacuum state in a stationary spacetime](../../../../../vacuum-state-in-a-stationary-spacetime.md) satisfies $a_i|0\rangle=0$, and the [Hamiltonian](../../../../../hamiltonian.md) is a sum of oscillators, $\sum_i\omega_i(a_i^\dagger a_i+1/2)$ before zero-point regularization. Continuous labels replace sums by correctly normalized integrals. For a complex charged scalar there are separate particle and antiparticle oscillators, with the same mode-mixing argument in each sector.

Choose independently normalized past and future bases, and use the matrix indices of the question. Complex conjugation of the future positive-frequency expansion immediately gives

$$
\boxed{n_i^+=\sum_j\bigl(n_j^- A_{ji}^*+p_j^- B_{ji}^*\bigr).}
$$

Conservation of the [Klein-Gordon inner product](../../../../../klein-gordon-inner-product.md) gives $A^\dagger A-B^\dagger B=I$ and $A^\dagger B^*-B^\dagger A^*=0$ in this column-index convention. These ensure preservation of the [canonical commutation relations](../../../../../canonical-commutation-relation.md).

Let $a_j$ annihilate past modes and $b_i$ annihilate future modes. Extracting the future coefficient from the field gives the [Bogoliubov transformation](../../../../../bogoliubov-transformation.md)

$$
b_i=(p_i^+,\widehat\phi)=\sum_j\bigl(A_{ji}^*a_j-B_{ji}^*a_j^\dagger\bigr).
$$

The minus sign follows from $(n_j^-,n_k^-)=-\delta_{jk}$. In the [in-vacuum](../../../../../in-vacuum.md), only $\langle0_{\rm in}|a_j a_k^\dagger|0_{\rm in}\rangle=\delta_{jk}$ contributes to the expectation of the future [number operator](../../../../../number-operator.md). Therefore

$$
\boxed{\langle0_{\rm in}|b_i^\dagger b_i|0_{\rm in}\rangle=\sum_j|B_{ji}|^2=(B^\dagger B)_{ii}.}
$$

This is [particle number from Bogoliubov coefficients](../../../../../particle-number-from-bogoliubov-coefficients.md): the intervening time-dependent geometry makes a past positive-frequency mode contain a future negative-frequency component. In infinite volume, localized [wave packets](../../../../../wave-packet.md) avoid delta-function normalization artifacts; a common Fock-space implementation needs the usual square-summability condition on the creation-mixing coefficients.

For gravitational collapse, the initial vacuum can be defined before the hole forms, while late outgoing modes are defined using the asymptotic stationary time at [future null infinity](../../../../../future-null-infinity.md). The complete future basis also includes modes falling through the [event horizon](../../../../../event-horizon.md); exterior outgoing modes alone are not a complete basis of all propagated data. Tracing an outgoing mode backwards near a nonextremal horizon gives the exponential ray relation $v=v_H-Ce^{-\kappa u}$, where $u$ is late retarded time and $\kappa$ is the [surface gravity](../../../../../surface-gravity.md). An outgoing factor $e^{-i\omega u}$ becomes proportional to $(v_H-v)^{i\omega/\kappa}$ in the early advanced coordinate, and contains both frequency signs when Fourier decomposed there. Their squared Bogoliubov-coefficient ratio is $e^{-2\pi\omega/\kappa}$; the canonical normalization then gives a Bose factor $(e^{2\pi\omega/\kappa}-1)^{-1}$, multiplied by the [greybody factor](../../../../../greybody-factor.md), the transmission probability through the exterior potential. Thus [Hawking radiation](../../../../../hawking-radiation.md) has temperature $T_H=\kappa/(2\pi)$ in units $\hbar=k_B=c=1$, with [greybody factor](../../../../../greybody-factor.md) modifications to the spectrum. This is a free-field calculation on a fixed or slowly evolving background; eventual backreaction is an additional problem, and the nonextremal exponential map must not be blindly used when $\kappa=0$.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 73](../../paper-73-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
