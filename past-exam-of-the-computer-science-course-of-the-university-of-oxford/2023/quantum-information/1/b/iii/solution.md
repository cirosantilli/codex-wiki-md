<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Alice uses [conjugate-basis steering of a Bell pair](../../../../../../conjugate-basis-steering-of-a-bell-pair.md). Write the desired [orthonormal basis](../../../../../../orthonormal-basis.md) for Bob as $|\psi\rangle=a|0\rangle+b|1\rangle$ and $|\psi^\perp\rangle=c|0\rangle+d|1\rangle$. Entrywise [complex conjugation](../../../../../../complex-conjugation.md) in the [computational basis](../../../../../../computational-basis.md) gives Alice's [orthonormal basis](../../../../../../orthonormal-basis.md)

$$
|\overline\psi\rangle=\overline a|0\rangle+\overline b|1\rangle,
\qquad
|\overline{\psi^\perp}\rangle=\overline c|0\rangle+\overline d|1\rangle.
$$

For either $|u\rangle$ in Bob's chosen [orthonormal basis](../../../../../../orthonormal-basis.md), the corresponding unnormalized conditional [quantum state](../../../../../../quantum-state.md) is

$$
(\langle\overline u|_A\otimes I_B)|\phi_+\rangle_{AB}
=\frac1{\sqrt2}\sum_{j=0}^1\langle\overline u|j\rangle|j\rangle_B
=\frac{|u\rangle_B}{\sqrt2}.
$$

Its squared [norm](../../../../../../norm.md) is $1/2$. Thus **Alice measures in the complex-conjugate basis**, obtaining the required Bob [pure states](../../../../../../pure-state.md) with [probability](../../../../../../probability.md) $1/2$ each. Averaging over Alice's undisclosed outcome leaves Bob's [density matrix](../../../../../../density-matrix-split.md) equal to $I/2$, consistent with the [no-communication theorem](../../../../../../no-communication-theorem.md).

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
