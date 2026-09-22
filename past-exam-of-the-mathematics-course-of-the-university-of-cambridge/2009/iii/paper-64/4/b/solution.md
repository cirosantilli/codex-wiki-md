<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Self-adjointness gives $\langle\boldsymbol\xi,F\boldsymbol\xi\rangle=\langle F\boldsymbol\xi,\boldsymbol\xi\rangle=\langle\boldsymbol\xi,F\boldsymbol\xi\rangle^*$, so

$$
\boxed{W[\boldsymbol\xi]\in\mathbb R.}
$$

The integrated expression from part (a) also writes it explicitly as

$$
W[\boldsymbol\xi]=\frac12\int\left[\rho\xi_i^*\Phi_{,ij}\xi_j+(\partial_j\xi_i^*)V_{ijkl}(\partial_l\xi_k)\right]dV.
$$

This is the quadratic change in [potential energy](../../../../../../potential-energy.md) associated with the perturbation, including [pressure](../../../../../../pressure.md), magnetic and imposed-gravity restoring effects. Its sign need not be positive term by term.

The perturbation [kinetic energy](../../../../../../kinetic-energy.md) is $T=\tfrac12\langle\dot{\boldsymbol\xi},\dot{\boldsymbol\xi}\rangle$, and the total quadratic perturbation [energy](../../../../../../energy.md) is

$$
\boxed{E=T+W=\tfrac12\langle\dot{\boldsymbol\xi},\dot{\boldsymbol\xi}\rangle-\tfrac12\langle\boldsymbol\xi,F\boldsymbol\xi\rangle.}
$$

Since the equilibrium and $F$ are time independent, differentiating and using the [self-adjoint operator](../../../../../../self-adjoint-operator.md) identity gives

$$
\frac{dE}{dt}=\operatorname{Re}\langle\dot{\boldsymbol\xi},\ddot{\boldsymbol\xi}\rangle-\operatorname{Re}\langle\dot{\boldsymbol\xi},F\boldsymbol\xi\rangle=0.
$$

Thus $\boxed{dE/dt=0}$ along the linearized motion. This conserved kinetic-plus-restoring [energy](../../../../../../energy.md) is the basis of the [magnetohydrodynamic energy principle](../../../../../../magnetohydrodynamic-energy-principle.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
