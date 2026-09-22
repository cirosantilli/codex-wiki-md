# Dyadic phase-gate identification

↑ **Parent:** [Quantum phase estimation](quantum-phase-estimation.md)

For the [phase gate](phase-gate.md) $R_a=\operatorname{diag}(1,e^{2\pi ia/2^n})$, apply powers $R_a^{2^{n-1}},\ldots,R_a$ to a [uniform quantum superposition](uniform-quantum-superposition.md) on $n$ qubits. Binary positional weights multiply the phases into $e^{2\pi iax/2^n}$ on basis vector $|x\rangle$. The inverse [quantum Fourier transform](quantum-fourier-transform.md) returns $|a\rangle$ exactly, by [orthogonality of roots of unity](orthogonality-of-roots-of-unity.md). Preparing the powers by repeated applications uses $2^n-1$ copies of $R_a$; this does not claim a number of gate calls polynomial in $n$. If $a$ is odd, its powers generate the entire set of dyadic phase gates because $a$ has a [modular inverse](modular-multiplicative-inverse.md) modulo $2^n$.

## ↑ Ancestors (6)

1. [Quantum phase estimation](quantum-phase-estimation.md)
2. [Quantum Fourier transform](quantum-fourier-transform.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-49/4/a/solution.md)
