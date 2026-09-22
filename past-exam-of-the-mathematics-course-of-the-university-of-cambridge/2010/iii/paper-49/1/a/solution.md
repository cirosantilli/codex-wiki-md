<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $N=2^n$ and $|s\rangle=N^{-1/2}\sum_{x=0}^{N-1}|x\rangle$. The initial [Hadamard gates](../../../../../../hadamard-gate.md) prepare $|s\rangle$ in the search register and $|-\rangle$ in the final [quantum ancilla](../../../../../../quantum-ancilla.md). Since the [Pauli X gate](../../../../../../pauli-x-gate.md) satisfies $X|-\rangle=-|-\rangle$, the [Boolean quantum oracle](../../../../../../boolean-quantum-oracle.md) acts by [quantum phase kickback](../../../../../../phase-kickback.md):

$$
U_f(|x\rangle|-\rangle)=(-1)^{f(x)}|x\rangle|-\rangle.
$$

For a single marked entry this is the [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) $O_a=I-2|a\rangle\langle a|$ on the search register. The ancilla stays separate and unchanged throughout.

The [Grover diffusion operator](../../../../../../grover-diffusion-operator.md) is $V=2|s\rangle\langle s|-I$, because $H^{\otimes n}|0^n\rangle=|s\rangle$. The PDF circuit places one diffusion after each oracle call, so the state before measurement is

$$
(VO_a)^k|s\rangle\otimes|-\rangle.
$$

In the supplied [amplitude amplification theorem](../../../../../../amplitude-amplification.md), take $|\psi\rangle=|s\rangle$ and $|\phi\rangle=|a\rangle$. Their overlap has modulus $1/\sqrt N$, so the [Grover rotation angle](../../../../../../grover-rotation-angle.md) is $\theta=\arcsin(N^{-1/2})$. A [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) therefore gives

$$
\boxed{\mathbb P(\text{output }a)=\sin^2((2k+1)\theta).}
$$

The inverse sine here is applied to the overlap of the two different states. The converted TeX's self-overlap in the angle definition is a transcription error; the original PDF has $|\langle\phi|\psi\rangle|$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
