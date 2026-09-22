# Clean subset superposition preparation

↑ **Parent:** [Known-subset Grover search](known-subset-grover-search.md)

Suppose a known list of $2^m$ distinct $n$-bit strings $a_j$ is available and [computational basis](computational-basis.md) transpositions on $n+m$ [qubits](qubit.md) have polynomial-size implementations. Start with the [uniform superposition state](uniform-superposition-state.md) of index labels $j$, leaving the data zero. First swap $|0^n,j\rangle$ with $|a_j,j\rangle$ for each nonzero $a_j$. Next, for each $j\ne0$, swap $|a_j,j\rangle$ with $|a_j,0^m\rangle$. Distinct index labels separate the first-stage pairs, and distinct data strings separate the second-stage pairs. Thus no later transposition disturbs an earlier term. At most $2^{m+1}-1$ transpositions prepare the uniform data state and return the [quantum ancilla](quantum-ancilla.md) to zero. For $m=O(\log n)$ the [quantum circuit](quantum-circuit-split.md) has polynomial size. This assumes the list is available; a membership predicate alone does not supply it.

## ↑ Ancestors (6)

1. [Known-subset Grover search](known-subset-grover-search.md)
2. [Grover's algorithm](grover-s-algorithm.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/2/d/solution.md)
