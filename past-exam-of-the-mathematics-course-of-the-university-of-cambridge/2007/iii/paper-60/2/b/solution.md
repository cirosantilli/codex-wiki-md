<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A real [Lie algebra](../../../../../../lie-algebra-split.md) is a real [vector space](../../../../../../vector-space-split.md) with a bilinear antisymmetric bracket satisfying the [Jacobi identity](../../../../../../jacobi-identity.md). For [matrices](../../../../../../matrix.md), the bracket is the [commutator](../../../../../../commutator.md) $[X,Y]=XY-YX$. The [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md) is

$$
\mathfrak g=\operatorname{Lie}_{\mathbb R}\{iH_0,iH_1,\ldots,iH_m\}\subseteq\mathfrak u(N).
$$

It is found by repeatedly adjoining [commutators](../../../../../../commutator.md) and taking real linear spans until no new independent generators appear. Let $G$ be its connected dynamical [Lie group](../../../../../../lie-group.md). Under the standard assumptions of freely timed controls with unrestricted real amplitudes, the following are the relevant Lie criteria.

For [pure-state controllability](../../../../../../pure-state-controllability.md), $G$ must act transitively on normalized state vectors, or on their rays when [global phase](../../../../../../global-phase.md) is disregarded. The standard finite-dimensional classification is, up to a unitary change of basis,

$$
\mathfrak g=\mathfrak u(N),\quad\mathfrak{su}(N),\quad\text{or, for }N=2n,\quad\mathfrak{sp}(n),\quad\mathfrak{sp}(n)\oplus\mathbb R iI.
$$

Here $\mathfrak{sp}(n)$ is the [compact symplectic Lie algebra](../../../../../../compact-symplectic-lie-algebra.md) in its defining complex $2n$-dimensional representation. Equivalently, the infinitesimal action spans the tangent directions to the whole pure-state orbit. The symplectic cases are important because pure-state reachability alone need not give complete mixed-state reachability.

For [density operator controllability](../../../../../../density-operator-controllability.md), the action must be transitive on every [unitary orbit of a density operator](../../../../../../unitary-orbit-of-a-density-operator.md), meaning on every fixed-spectrum class. The criterion is **$\mathfrak g=\mathfrak{su}(N)$ or $\mathfrak u(N)$**. This concerns all [density operators](../../../../../../density-matrix.md), not merely one unusually degenerate spectrum.

For exact [unitary operator controllability](../../../../../../unitary-operator-controllability.md), the criterion is **$\mathfrak g=\mathfrak u(N)$**. If only the physical gate up to [global phase](../../../../../../global-phase.md) matters, it is enough that the image after removing the scalar direction is $\mathfrak{su}(N)$, equivalently that $\mathfrak g+\mathbb R iI=\mathfrak u(N)$. A traceless system can implement all special-unitary gates while lacking independent control of the overall phase.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
