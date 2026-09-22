# Logical failure of the three-qubit phase-flip repetition code

↑ **Parent:** [Phase-flip repetition code](phase-flip-repetition-code.md)

The [phase-flip repetition code](phase-flip-repetition-code.md) with codewords $|+++\rangle,|---\rangle$ corrects any one physical [Pauli Z gate](pauli-z-gate.md) error. Its two adjacent-pair [error syndromes](error-syndrome.md) cannot distinguish an error pattern from its three-bit complement. Minimum-weight recovery therefore leaves no residual error at weight zero or one, and leaves $Z_1Z_2Z_3$ at weight two or three. This residual operator exchanges the codewords, so inverse encoding gives a logical [Pauli X gate](pauli-x-gate.md). For independent physical phase errors of probability $\epsilon$, the decoded [quantum channel](quantum-channel.md) is $(1-p_L)\rho+p_LX\rho X$, where $p_L=3\epsilon^2(1-\epsilon)+\epsilon^3$. For $0<\epsilon<1/2$, $\epsilon-p_L=\epsilon(1-\epsilon)(1-2\epsilon)>0$.

## ↑ Ancestors (7)

1. [Phase-flip repetition code](phase-flip-repetition-code.md)
2. [Stabilizer code](stabilizer-code.md)
3. [Quantum error correction](quantum-error-correction-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-51/4/c/solution.md)
