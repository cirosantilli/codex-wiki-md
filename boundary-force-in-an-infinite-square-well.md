# Boundary force in an infinite square well

↑ **Parent:** [Infinite square well](infinite-square-well.md)

For a normalized sufficiently regular solution of the [Schrödinger equation](schrodinger-equation.md) on $[0,L]$ with Dirichlet walls, the instantaneous outward forces on the walls have magnitudes

$$
P_0=\frac{\hbar^2}{2m}|\psi'(0,t)|^2,\qquad P_L=\frac{\hbar^2}{2m}|\psi'(L,t)|^2.
$$

A wall displacement changes the kinetic-energy quadratic form by the boundary term $-P_j\,dL_j$, giving the local force. Equivalently, direct integration by parts in the time derivative of the mean particle momentum gives

$$
\frac{d\langle p\rangle}{dt}=\frac{\hbar^2}{2m}\left(|\psi'(0,t)|^2-|\psi'(L,t)|^2\right)=P_0-P_L.
$$

The force on the particle is the opposite of the net force $-P_0+P_L$ on the walls. For a stationary [energy eigenstate](energy-eigenstate.md) each magnitude equals $2E_n/L$. For the [equal superposition of the first two box states](equal-superposition-of-the-first-two-box-states.md), writing $C=E_1/L$ and $\Omega=3E_1/\hbar$ gives $P_0=C(5+4\cos\Omega t)$ and $P_L=C(5-4\cos\Omega t)$. Both time averages equal $2\langle E\rangle/L$, the classical mean force on one wall at that energy, even though the quantum forces vary continuously in time.

## ↑ Ancestors (5)

1. [Infinite square well](infinite-square-well.md)
2. [Quantum mechanics](quantum-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-b/b8/d/solution.md)
