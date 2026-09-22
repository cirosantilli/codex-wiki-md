<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

For a [periodic potential](../../../../../periodic-potential.md), the Hamiltonian commutes with every lattice translation. The three primitive translations are commuting [unitary operators](../../../../../unitary-operator.md), so within each [energy eigenspace](../../../../../energy-eigenspace.md) one can choose simultaneous translation eigenstates. Their [eigenvalues](../../../../../eigenvalue.md) have modulus one and can be written $e^{i\boldsymbol k\cdot\boldsymbol a_i}$. Translation by any lattice vector then gives

$$
\psi_{n\boldsymbol k}(\boldsymbol r+\boldsymbol l)=e^{i\boldsymbol k\cdot\boldsymbol l}\psi_{n\boldsymbol k}(\boldsymbol r),\qquad\boxed{\psi_{n\boldsymbol k}=e^{i\boldsymbol k\cdot\boldsymbol r}u_{n\boldsymbol k}(\boldsymbol r),\quad u(\boldsymbol r+\boldsymbol l)=u(\boldsymbol r).}
$$

This proves Bloch's theorem in its eigenbasis form; arbitrary superpositions inside a degenerate eigenspace need not themselves have a single Bloch wavevector.

The [reciprocal lattice](../../../../../reciprocal-lattice.md) consists of vectors $\boldsymbol g$ with $\boldsymbol g\cdot\boldsymbol a_i\in2\pi\mathbb Z$. Changing $\boldsymbol k$ to $\boldsymbol k+\boldsymbol g$ and $u$ to $e^{-i\boldsymbol g\cdot\boldsymbol r}u$ gives the same physical wavefunction with a periodic new $u$. The [eigenvalue problem](../../../../../eigenvalue-problem.md) on one cell has a [discrete set](../../../../../discrete-subset.md) of levels, giving bands indexed by $n$, and this equivalence yields $E_n(\boldsymbol k+\boldsymbol g)=E_n(\boldsymbol k)$. A reciprocal-lattice [fundamental domain](../../../../../fundamental-domain.md), conventionally a [Brillouin zone](../../../../../brillouin-zone.md), therefore labels inequivalent wavevectors.

[Periodic boundary conditions](../../../../../periodic-boundary-conditions.md) in physical volume $\mathcal V$ give one allowed wavevector per reciprocal-space volume $(2\pi)^3/\mathcal V$. Including the two spin states, there are $2\mathcal V\,d^3k/(2\pi)^3$ states; **per unit physical volume** the count is the printed $2\,d^3k/(2\pi)^3$. Each occupied state carries charge $-e$ and [velocity](../../../../../velocity.md) $\hbar^{-1}\nabla_kE_n$, so

$$
\boxed{\boldsymbol j=-e\frac2{(2\pi)^3}\int_Bn(\boldsymbol k)\boldsymbol v(\boldsymbol k)\,d^3k.}
$$

For a full band, the integral of $\nabla_kE_n$ is a boundary integral. Opposite faces of a reciprocal fundamental cell have equal energies by periodicity and opposite normals, so their contributions cancel. Hence **a full band carries zero [electric current](../../../../../electric-current.md)**.

## ↑ Ancestors (10)

1. [33D](../33d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
