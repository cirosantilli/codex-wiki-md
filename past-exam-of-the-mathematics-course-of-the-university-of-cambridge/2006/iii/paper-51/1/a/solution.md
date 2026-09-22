<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [order parameter](../../../../../../order-parameter.md) distinguishes phases by a macroscopic quantity that changes at the transition. For an [Ising model](../../../../../../ising-model.md) ferromagnet it is the [magnetization](../../../../../../magnetization.md) per [Ising spin](../../../../../../ising-spin-variable.md), $M=N^{-1}\sum_n\langle\sigma_n\rangle$. At zero [magnetic field](../../../../../../magnetic-field.md) the [statistical Hamiltonian](../../../../../../statistical-hamiltonian.md) is invariant under [spin inversion symmetry](../../../../../../spin-inversion-symmetry.md). The disordered phase preserves this [symmetry](../../../../../../symmetry-physics.md), whereas a selected ordered phase has $M\ne0$ and a spin-reversed partner with $-M$. At finite volume with symmetric [boundary conditions](../../../../../../boundary-condition.md) the [expected value](../../../../../../expected-value.md) is zero even below the transition; [spontaneous magnetization](../../../../../../spontaneous-magnetization.md) means taking the [thermodynamic limit](../../../../../../thermodynamic-limit.md) before sending a symmetry-breaking field to zero.

[Landau-Ginzburg theory](../../../../../../landau-ginzburg-theory.md) introduces a coarse-grained local [order parameter](../../../../../../order-parameter.md) $\phi(x)$ and a symmetry-constrained [free-energy functional](../../../../../../free-energy-functional.md). For a short-range system with scalar [spin inversion symmetry](../../../../../../spin-inversion-symmetry.md), a useful expansion is

$$
\mathcal F[\phi]=\int d^Dx\left\{\frac\kappa2|\nabla\phi|^2+\frac r2\phi^2+\frac u4\phi^4+\frac v6\phi^6-h\phi\right\},\qquad \kappa>0.
$$

The coefficients vary smoothly with microscopic control parameters at the level of the [Landau approximation](../../../../../../landau-approximation.md); normally $r=A(T-T_c)$ with $A>0$. The [gradient](../../../../../../gradient.md) term penalizes spatial variation. The [magnetic field](../../../../../../magnetic-field.md) is conjugate to the [order parameter](../../../../../../order-parameter.md), and odd powers at $h=0$ are excluded by [spin inversion symmetry](../../../../../../spin-inversion-symmetry.md). With $u>0$, the sextic term may be omitted locally; with $u<0$, a stabilizing positive $v$ is essential. The equilibrium uniform [order parameter](../../../../../../order-parameter.md) minimizes the local potential $V(M)$, giving

$$
h=rM+uM^3+vM^5.
$$

This [equation of state](../../../../../../equation-of-state.md) follows from minimization, rather than being imposed as an independent assumption. Vector or tensor [order parameters](../../../../../../order-parameter.md) and their allowed invariants describe other [symmetry](../../../../../../symmetry-physics.md) classes.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
