<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here “controllable” means [density operator controllability](../../../../../../density-operator-controllability.md), so all transformations on a fixed spectral orbit are available. Strict [unitary operator controllability](../../../../../../unitary-operator-controllability.md), including an independently specified [global phase](../../../../../../global-phase.md), is a stronger condition. Assume the usual finite-dimensional real controls and freely chosen duration.

The dimension hypothesis actually identifies the algebra, not just its size. For completeness, put the invariant inner product $\langle X,Y\rangle=-\operatorname{Tr}(XY)$ on $\mathfrak u(N)$ and write $\mathfrak g^\perp=\mathbb R Z$. Since $\mathfrak g$ is closed under [commutators](../../../../../../commutator.md), $[X,Z]$ lies in $\mathfrak g^\perp$ for every $X\in\mathfrak g$. The adjoint action is skew-adjoint for this inner product, so $[X,Z]$ is also orthogonal to $Z$ and must vanish. If $Z$ were nonscalar, its orthogonal eigenspaces would give a centralizer of dimension at most $(N-1)^2+1<N^2-1$, too small to contain $\mathfrak g$. Therefore $Z$ is scalar and $\mathfrak g=\mathfrak{su}(N)$. This proves [codimension-one quantum dynamical algebra is special unitary](../../../../../../codimension-one-quantum-dynamical-algebra-is-special-unitary.md).

**a1 is true for density-state controllability; a2 is true; a3 is false.** The algebra $\mathfrak{su}(N)$ generates every determinant-one unitary. For any $V\in U(N)$, choose $\varphi$ with $e^{iN\varphi}=\det V$; then $e^{-i\varphi}V\in SU(N)$, proving that every gate is available up to [global phase](../../../../../../global-phase.md). But all generated [Quantum Hamiltonians](../../../../../../hamiltonian-quantum-mechanics.md) are traceless, and

$$
\frac d{dt}\det U(t)=-i\operatorname{Tr}H(t)\det U(t)=0,
$$

so evolution starting at the identity always has determinant one. Arbitrary determinant, requiring the additional central direction $iI$, cannot be generated. If a1 is instead read as phase-sensitive unitary-operator controllability, it is false for precisely the same reason as a3; the physical distinction is explicit here.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
