<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $P_0,P_1$ be any two rank-one [orthogonal projections](../../../../../../orthogonal-projection.md). Choose $0<q<1/N$ and $p=1-(N-1)q$, so $p>q$, and form the mixed [density operators](../../../../../../density-matrix.md)

$$
\rho_j=qI+(p-q)P_j.
$$

They have the same [spectrum](../../../../../../spectrum-functional-analysis.md). If [density operator controllability](../../../../../../density-operator-controllability.md) holds, a reachable $U$ obeys $U\rho_0U^\dagger=\rho_1$, and subtraction of $qI$ gives $UP_0U^\dagger=P_1$. Thus **density operator controllability implies pure-state controllability**, even if its definition is phrased using only mixed density operators.

The converse is false in general. For $N=4$, the full [compact symplectic group](../../../../../../compact-symplectic-group.md) $Sp(2)$ is transitive on the complex unit sphere: identify $\mathbb C^4$ with $\mathbb H^2$, extend any quaternionic unit vector to an orthonormal quaternionic basis, and map one such basis to another. This gives [pure-state controllability](../../../../../../pure-state-controllability.md). Yet the invariant in part (d) prevents it from connecting the indicated isospectral mixed [density operators](../../../../../../density-matrix.md), so it fails [density operator controllability](../../../../../../density-operator-controllability.md). This counterexample uses the full symplectic group, not an assertion that every parameter choice in part (c) generates it.

For $N=2$, the converse is true. Every [density operator](../../../../../../density-matrix.md) has the form $\rho=qI+(p-q)P$ for a rank-one $P$, with $p+q=1$. If $p\ne q$, pure-state control of $P$ controls its entire fixed-spectrum [unitary orbit of a density operator](../../../../../../unitary-orbit-of-a-density-operator.md). If $p=q=1/2$, the orbit contains only $I/2$. Therefore **the two controllability notions coincide for a qubit**. The Lie classification gives the same conclusion, since $Sp(1)=SU(2)$.

## ↑ Ancestors (11)

1. [E](../e.md)
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
