# Nondegenerate phase-flip correction in the Steane code

↑ **Parent:** [Steane code](steane-code.md)

Write the [Steane code](steane-code.md) basis as uniform [quantum superpositions](quantum-superposition.md) over a binary [linear code](linear-code.md) $D$ and a disjoint coset $t+D$, where $D$ is the even-weight part of the length-seven [Hamming code](hamming-code.md). For $Z(w)=\bigotimes_{j=1}^7Z_j^{w_j}$, diagonal [Pauli Z gates](pauli-z-gate.md) cannot connect the two cosets. Within coset $t_a+D$, the overlap is

$$
\langle\psi_a|Z(w)|\psi_a\rangle=(-1)^{w\cdot t_a}|D|^{-1}\sum_{x\in D}(-1)^{w\cdot x}.
$$

If $w\notin D^\perp$, translation by a word $x_0\in D$ with $w\cdot x_0=1$ negates this sum, so it vanishes. Since the [dual code](dual-code.md) $D^\perp$ is the length-seven [Hamming code](hamming-code.md) of minimum [Hamming distance](hamming-distance.md) three, every nonzero $w$ of [Hamming weight](hamming-weight.md) one or two has vanishing overlap. Taking $u,v$ from $\{0,e_1,\ldots,e_7\}$ proves the displayed identity. The eight two-dimensional error images are [orthogonal](orthogonal-vectors.md), so their [projective measurement](projective-measurement.md) determines the [error syndrome](error-syndrome.md) without revealing the logical state; applying the identified [phase flip](pauli-z-gate.md) again recovers every code state. This proves [nondegenerate quantum error-correcting code](nondegenerate-quantum-error-correcting-code.md) behaviour for the identity and all single-site [phase flips](pauli-z-gate.md), including their coherent linear span.

## ↑ Ancestors (7)

1. [Steane code](steane-code.md)
2. [Stabilizer code](stabilizer-code.md)
3. [Quantum error correction](quantum-error-correction-split.md)
4. [Quantum theory](quantum-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/5/b/solution.md)
