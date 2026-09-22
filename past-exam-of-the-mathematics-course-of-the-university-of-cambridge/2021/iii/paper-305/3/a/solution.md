<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Goldstone theorem](../../../../../../goldstone-theorem.md) states that every spontaneously broken generator of a continuous internal global symmetry in a Lorentz-invariant quantum field theory produces a massless scalar particle.

For the classical proof, let $V(\phi)$ be the invariant scalar potential and let $v_i$ be a vacuum. Infinitesimal invariance gives

$$
\frac{\partial V}{\partial\phi_i}(T^a)_{ij}\phi_j=0.
$$

Differentiate with respect to $\phi_k$ and evaluate at the stationary point $v$, where $\partial_iV(v)=0$. The scalar mass matrix then obeys

$$
(M^2)_{ki}(T^a)_{ij}v_j=0,
\qquad
(M^2)_{ki}=\frac{\partial^2V}{\partial\phi_k\partial\phi_i}\bigg|_v.
$$

For every broken generator, $(T^a v)_i\neq0$, so $T^av$ is a zero eigenvector of the [Hessian matrix](../../../../../../hessian-matrix.md). It is a massless fluctuation tangent to the [vacuum manifold](../../../../../../vacuum-manifold.md).

For the quantum proof, spontaneous breaking means that some local field has

$$
\langle0|[\phi_i(0),Q_a]|0\rangle=i(T^a)_{ij}\langle0|\phi_j|0\rangle\neq0.
$$

Write $Q_a=\int d^3x\,j_a^0(x)$ and insert a complete set of momentum eigenstates into the current-field correlation function. [Current conservation](../../../../../../conserved-current.md) and Lorentz covariance imply that a scalar intermediate state couples as

$$
\langle0|j_a^\mu(0)|\pi_b(p)\rangle=if_{ab}p^\mu.
$$

The nonzero equal-time commutator requires a pole at $p^2=0$; otherwise the conserved-current spectral integral vanishes at zero momentum. Thus a massless [Goldstone boson](../../../../../../goldstone-boson.md) exists for every independent broken direction.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 305](../../../paper-305-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
