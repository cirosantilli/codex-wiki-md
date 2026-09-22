<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume the usual real Hamiltonian controls with freely chosen finite duration, rather than a fixed-time or amplitude-restricted task. Define the [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md)

$$
\mathfrak g=\operatorname{Lie}_{\mathbb R}\{iH_0,iH_1,\ldots,iH_M\}\subseteq\mathfrak u(N),
$$

the real linear span closed under all nested [commutators](../../../../../../commutator.md). Replacing each generator by $-iH_m$ gives the same algebra. The associated connected reachable group acts on propagators, on each [unitary orbit of a density operator](../../../../../../unitary-orbit-of-a-density-operator.md), and on [pure states](../../../../../../pure-state.md). For $N\ge2$, the necessary and sufficient conditions are as follows.

For exact [unitary operator controllability](../../../../../../unitary-operator-controllability.md), $\boxed{\mathfrak g=\mathfrak u(N)}$. For operator control up to [global phase](../../../../../../global-phase.md), the possibilities are $\mathfrak{su}(N)$ or $\mathfrak u(N)$. If every Hamiltonian is traceless, $\det U(T)=\exp[-i\int_0^T\operatorname{Tr}H(t)\,dt]=1$, so the central phase direction is absent and exact access is to $SU(N)$. The full [special unitary Lie algebra](../../../../../../special-unitary-lie-algebra.md) has dimension $N^2-1$ and the [Lie algebra of the unitary group](../../../../../../unitary-lie-algebra.md) has dimension $N^2$.

For [density operator controllability](../../../../../../density-operator-controllability.md) on every spectral orbit,

$$
\boxed{\mathfrak g=\mathfrak{su}(N)\text{ or }\mathfrak u(N)}.
$$

Scalar phases do not affect conjugation. If only a particular density spectrum is being considered, a smaller group can suffice: for distinct eigenvalue multiplicities $n_j$ and centralizer $\mathfrak c_\rho=\{X\in\mathfrak u(N):[X,\rho]=0\}$, the orbit criterion is $\dim\mathfrak g-\dim(\mathfrak g\cap\mathfrak c_\rho)=N^2-\sum_jn_j^2$. A maximally mixed state has a one-point orbit and needs no controls. This restricted-orbit condition is weaker than controllability for every density spectrum.

For [pure-state controllability](../../../../../../pure-state-controllability.md), up to a fixed unitary change of basis,

$$
\boxed{\mathfrak g=\mathfrak{su}(N),\ \mathfrak u(N),\ \mathfrak{sp}(N/2),\ \text{or }\mathfrak{sp}(N/2)\oplus\mathbb R iI},
$$

where the last two alternatives occur only for even $N$. Here $\mathfrak{sp}(n)$ is the standard [compact symplectic Lie algebra](../../../../../../compact-symplectic-lie-algebra.md) acting on $\mathbb C^{2n}$, not the real noncompact symplectic algebra. These are precisely the unitary matrix algebras whose connected groups act transitively on normalized complex vectors, and also give the ray version of controllability. For $N=2$, $\mathfrak{sp}(1)=\mathfrak{su}(2)$. For even $N\ge4$, the symplectic cases show why pure-state control can be weaker than density control: $\dim\mathfrak{sp}(n)=n(2n+1)$ is smaller than the nondegenerate density-orbit dimension $N^2-N$, and its scalar center acts trivially on that orbit. For $N=1$, the physical density and pure-state spaces are single points, while exact operator controllability still requires the phase algebra $\mathfrak u(1)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
