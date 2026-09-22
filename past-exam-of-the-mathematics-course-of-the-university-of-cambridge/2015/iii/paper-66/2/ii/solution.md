<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use [one-bit remote preparation of real qubit states](../../../../../../one-bit-remote-preparation-of-real-qubit-states.md). Alice measures her [qubit](../../../../../../qubit.md) in the [orthonormal basis](../../../../../../orthonormal-basis.md)

$$
|\alpha_\theta\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle,\qquad|\beta_\theta\rangle=-\sin\theta|0\rangle+\cos\theta|1\rangle.
$$

Because this change of basis is real and orthogonal, the shared [Bell state](../../../../../../bell-state-split.md) has the expansion

$$
|\Phi^+\rangle=\frac{|\alpha_\theta\rangle_A|\alpha_\theta\rangle_B+|\beta_\theta\rangle_A|\beta_\theta\rangle_B}{\sqrt2}.
$$

Her [projective measurement](../../../../../../projective-measurement.md) gives each outcome with probability one half. She sends $m=0$ for the first outcome and $m=1$ for the second. Bob's conditional [pure state](../../../../../../pure-state.md) is respectively $|\alpha_\theta\rangle$ or $|\beta_\theta\rangle$.

For $m=0$ Bob does nothing. For $m=1$ he applies the fixed [unitary operator](../../../../../../unitary-operator.md)

$$
U=iY=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad U|\beta_\theta\rangle=|\alpha_\theta\rangle,
$$

where $Y$ is the [Pauli Y gate](../../../../../../pauli-y-gate.md). Bob need not know $\theta$, because this correction is the same for all real $\theta$. **Both outcomes produce the exact density operator $|\alpha_\theta\rangle\langle\alpha_\theta|$, using one classical bit and only local operations.**

This [remote state preparation](../../../../../../remote-state-preparation.md) consumes the shared [entangled state](../../../../../../entangled-state.md). Before receiving the bit, Bob has the mixture $(|\alpha_\theta\rangle\langle\alpha_\theta|+|\beta_\theta\rangle\langle\beta_\theta|)/2=I/2$, independent of $\theta$, as required by [quantum no-signalling](../../../../../../quantum-no-signalling.md). The real-state restriction is what permits a fixed unitary correction of the orthogonal outcome.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
