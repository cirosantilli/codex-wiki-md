<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the upper-index coordinates $B^\mu,B^{*\mu}$ specified in the paper. Differentiation of the [Lagrangian density](../../../../lagrangian-density.md) gives the [canonical momenta](../../../../canonical-momentum.md)

$$
\boxed{\pi_\mu=-G^{*0}{}_{\mu},\qquad\pi_\mu^*=-G^0{}_{\mu},\qquad\pi_0=\pi_0^*=0.}
$$

In particular, $\pi_i=G^{*0i}$ and $\pi_i^*=G^{0i}$. No time derivative of $B^0$ appears, so the zero momenta are primary [constraints](../../../../constraint-mechanics.md), not invertible equations for $\dot B^0$.

For spatial indices, $G^{0i}=\dot B^i+\partial_iB_0$, so $\dot B^i=\pi_i^*+\partial^iB_0$, with the conjugate relation for $B^{*i}$. Also

$$
\mathcal L=\sum_i|G^{0i}|^2-\frac12G_{ik}^*G^{ik}+M^2|B_0|^2-M^2\sum_i|B^i|^2.
$$

The [Legendre transform](../../../../convex-conjugate.md) for the [complex Proca Hamiltonian](../../../../complex-proca-hamiltonian.md), $\mathcal H_c=\pi_i\dot B^i+\pi_i^*\dot B^{*i}-\mathcal L$ therefore gives

$$
\boxed{H_c=\int d^3x\left[\pi_i^*\pi_i+\pi_i\partial^iB_0+\pi_i^*\partial^iB_0^*+\frac12G_{ik}^*G^{ik}-M^2B_0^*B_0-M^2B_i^*B^i\right].}
$$

Repeated spatial indices in the positive product $\pi_i^*\pi_i$ denote an ordinary three-component sum. A total [Hamiltonian](../../../../hamiltonian.md) additionally includes multipliers for $\pi_0=\pi_0^*=0$.

The Hamiltonian printed in the source cannot follow from the given complex [Lagrangian density](../../../../lagrangian-density.md): its missing conjugations, mass coefficients and spatial mass sign are inconsistent. A concrete check is spatially uniform initial data $B^1=b\in\mathbb R$, $B^0=B^2=B^3=0$, with all [canonical momenta](../../../../canonical-momentum.md) zero. The correct [Hamiltonian density](../../../../hamiltonian-density.md) is $M^2b^2$, while the printed expression gives $-M^2b^2/2$. These data satisfy the initial [constraints](../../../../constraint-mechanics.md) and evolve as a spatially uniform massive oscillator. Thus the discrepancy is not a harmless surface term or a different complex-field normalization.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
