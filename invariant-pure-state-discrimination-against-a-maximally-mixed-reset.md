# Invariant-pure-state discrimination against a maximally mixed reset

↑ **Parent:** [Quantum state discrimination](quantum-state-discrimination.md)

Suppose one equally likely action returns a known normalized [pure state](pure-state.md) $|s\rangle$ unchanged, while another returns the [maximally mixed state](maximally-mixed-state.md) $I/d$. A [basic measurement](basic-measurement.md) in any [orthonormal basis](orthonormal-basis.md) containing $|s\rangle$ distinguishes them with success $1-1/(2d)$: guess the pure-state action on its basis label and the reset action on the remaining $d-1$ labels. The first action succeeds with [probability](probability.md) one and the second with [probability](probability.md) $(d-1)/d$.

The [Holevo–Helstrom theorem](holevo-helstrom-theorem.md) also proves optimality for these returned states. The [Hermitian](hermitian-operator.md) difference $|s\rangle\langle s|-I/d$ has [eigenvalues](eigenvalue.md) $1-1/d$ and $-1/d$ with [multiplicity](multiplicity-mathematics.md) $d-1$, hence [trace norm](trace-norm.md) $2(1-1/d)$. Its optimal equal-prior discrimination success is $1/2+\|\rho_0-\rho_1\|_1/4$. Random computational-basis permutations fix the uniform superposition, so they supply an example of the invariant action. This compares the returned states in the stated unassisted protocol; it makes no assertion about a more general channel-discrimination problem with an entangled ancillary probe.[§3.1.1, Theorem 3.4 and equation (3.20)](the-theory-of-quantum-information-by-john-watrous.md)

## ↑ Ancestors (6)

1. [Quantum state discrimination](quantum-state-discrimination.md)
2. [Quantum information theory](quantum-information-theory-split.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2019/quantum-information/1/d/iii/solution.md)
