<h1 id="34b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Born rule](../../../../../../born-rule.md) depends only on transition probabilities

$$
|\langle\phi|\psi\rangle|^2
$$

between rays. A physical transformation must preserve these probabilities. By [Wigner theorem](../../../../../../wigner-s-theorem.md), such a ray transformation is induced by a unitary or antiunitary operator. For ordinary continuously connected transformations one chooses the unitary branch, so

$$
\boxed{U(g)^\dagger U(g)=I_{\mathcal H}}.
$$

The states $U(g_1)U(g_2)|\psi\rangle$ and $U(g_1g_2)|\psi\rangle$ represent the same ray. They may therefore differ by a state-independent [quantum phase](../../../../../../quantum-phase.md):

$$
\boxed{
U(g_1)U(g_2)
=e^{i\phi(g_1,g_2)}U(g_1g_2)}.
$$

Thus quantum transformations form a [projective unitary representation](../../../../../../projective-unitary-representation.md).

If $g$ is a symmetry of the [Hamiltonian operator](../../../../../../hamiltonian-quantum-mechanics.md) $H$, it also obeys

$$
\boxed{U(g)^\dagger H U(g)=H},
$$

equivalently $[U(g),H]=0$. For a differentiable one-parameter subgroup, write

$$
U(s)=e^{-isQ/\hbar}
$$

with a self-adjoint generator $Q$. Differentiating the symmetry equation at $s=0$ yields

$$
[Q,H]=0.
$$

For a time-independent $Q$, the [Heisenberg picture](../../../../../../heisenberg-picture.md) equation is

$$
\frac{dQ}{dt}=\frac i\hbar[H,Q]=0.
$$

**Hence the generator is a conserved observable. Conversely, a self-adjoint conserved $Q$ commutes with $H$ and its unitary group generates symmetries. This is the [conserved generator of a continuous quantum symmetry](../../../../../../conserved-generator-of-a-continuous-quantum-symmetry.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [34B](../../34b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
