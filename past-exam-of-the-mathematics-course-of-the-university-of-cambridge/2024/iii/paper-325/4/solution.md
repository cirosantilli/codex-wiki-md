<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For particle positions $\mathbf r_1,\mathbf r_2$, the two-particle [Schrödinger equation](../../../../../schrodinger-equation.md) is

$$
\boxed{
i\hbar\frac{\partial\Psi}{\partial t}
=\left[-\frac{\hbar^2}{2m_1}\nabla_1^2
-\frac{\hbar^2}{2m_2}\nabla_2^2
-\frac{Gm_1m_2}{|\mathbf r_1-\mathbf r_2|}\right]\Psi}.
$$

Write $|a\rangle_i$ for the localized [wave packet](../../../../../wave-packet.md) $\psi_{ai}$ and $d_{ab}=|x_{a1}-x_{b2}|$. Neglecting packet spreading and branch overlap, the initial [product state](../../../../../product-state.md) evolves branchwise as

$$
|\Psi(t)\rangle\simeq\frac12\sum_{a,b=0}^1
\exp\left(\frac{iGm_1m_2t}{\hbar d_{ab}}\right)
|a\rangle_1|b\rangle_2,
$$

up to phases generated independently on the two particles. These branch-dependent phases generally cannot be separated into one phase depending only on $a$ and one depending only on $b$, so the [Newtonian gravitational potential energy](../../../../../newtonian-gravitational-potential-energy.md) creates [gravitationally induced entanglement](../../../../../gravitationally-induced-entanglement.md).

If $d_{10}=|x_{11}-x_{02}|=d$ is much smaller than the other separations, remove their nearly common phase and retain only

$$
\phi=\frac{Gm_1m_2t}{\hbar d}.
$$

The state is approximately

$$
|\Psi(t)\rangle
=\frac12\left(|00\rangle+|01\rangle
+e^{i\phi}|10\rangle+|11\rangle\right).
$$

Its [concurrence](../../../../../concurrence.md) is $|\sin(\phi/2)|$, so it becomes [maximally entangled](../../../../../maximally-entangled-state.md) first at $\phi=\pi$. For $m_1=m_2=m$,

$$
\boxed{t_{\rm ent}
=\frac{\pi\hbar d}{Gm^2}
=\frac{hd}{2Gm^2}}
=\frac{(6.6\times10^{-34})(2\times10^{-4})}
{2(6.7\times10^{-11})(10^{-14})^2}
\simeq9.9\ \mathrm{s}.
$$

Thus the near-maximal entanglement time is about $\boxed{10\ \mathrm{s}}$ within the stated approximation.

A single prescribed [classical gravitational potential](../../../../../newtonian-gravitational-potential.md) gives a Hamiltonian of the form $H_1[\Phi]\otimes I+I\otimes H_2[\Phi]$. Its evolution factorizes as $U_1\otimes U_2$ and preserves every initial [product state](../../../../../product-state.md), so it cannot generate this entanglement. A semiclassical mean field sourced only by expectation values likewise gives each particle a local one-body potential and does not provide a quantum mediator carrying branch correlations.

An [entanglement witness](../../../../../entanglement-witness.md) is a [Hermitian operator](../../../../../hermitian-operator.md) $W$ whose expectation is nonnegative on every [separable state](../../../../../separable-quantum-state.md) but negative on at least one [entangled state](../../../../../entangled-state.md). At $\phi=\pi$, define

$$
|\Psi_*\rangle
=\frac12(|00\rangle+|01\rangle-|10\rangle+|11\rangle),
\qquad
W=\frac12I-|\Psi_*\rangle\langle\Psi_*|.
$$

The largest [Schmidt coefficient](../../../../../schmidt-coefficient.md) of $|\Psi_*\rangle$ is $1/\sqrt2$, so every product state $|u\rangle|v\rangle$ in the four-dimensional branch subspace satisfies $|\langle\Psi_*|u,v\rangle|^2\leq1/2$. By closure under [convex combinations](../../../../../convex-combination.md), $\operatorname{Tr}(W\rho_{\rm sep})\geq0$ for every separable mixture, whereas

$$
\langle\Psi_*|W|\Psi_*\rangle=-\frac12.
$$

A negative measured value therefore certifies entanglement. Under the assumptions that the masses began unentangled and interacted only through gravity, such certification would show that the mediator can transmit quantum coherence; it would be evidence against a purely classical gravitational channel and for the quantum nature of gravity.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
