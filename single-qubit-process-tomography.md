# Single-qubit process tomography

↑ **Parent:** [Quantum state tomography](quantum-state-tomography.md)

To identify the physical channel $\rho\mapsto V\rho V^\dagger$ of a single-[qubit](qubit.md) [unitary gate](quantum-logic-gate.md), prepare each of the three positive [Pauli matrix](pauli-matrices.md) [eigenstates](eigenstate.md) and estimate each output Pauli [expectation](expected-value.md). Their nine means are

$$
R_{ij}=\frac12\operatorname{Tr}(\sigma_iV\sigma_jV^\dagger),\qquad i,j\in\{x,y,z\}.
$$

They determine the [Bloch vector](bloch-vector.md) [rotation](rotation-mathematics.md) $\boldsymbol r\mapsto R\boldsymbol r$, hence the channel on all states. If two gates have the same channel, their relative unitary commutes with all three [Pauli matrices](pauli-matrices.md): commuting with $Z$ forces it diagonal and commuting with $X$ forces equal diagonal entries. Thus they differ by a scalar [global phase](global-phase.md), proving uniqueness up to that phase. This procedure needs no controlled gate or [eigenstate](eigenstate.md) of the unknown gate. Estimating its bounded measurement means to error $\epsilon$ with fixed confidence uses order $\epsilon^{-2}$ repetitions. It determines the relative [eigenphases](eigenphase.md) but cannot determine an overall [eigenvalue](eigenvalue.md) phase from uncontrolled gate access alone.

## ↑ Ancestors (6)

1. [Quantum state tomography](quantum-state-tomography.md)
2. [Measurement in quantum mechanics](quantum-measurement-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-57/4/d/solution.md)
