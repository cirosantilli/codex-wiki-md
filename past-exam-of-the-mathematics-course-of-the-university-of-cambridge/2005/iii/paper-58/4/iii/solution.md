<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [Pauli X gate](../../../../../../pauli-x-gate.md) interchanges the two basis [quantum states](../../../../../../quantum-state.md). Because the bit-flip outcome is a classical unobserved error rather than a coherent superposition, the [quantum bit-flip channel](../../../../../../quantum-bit-flip-channel.md) gives

$$
\boxed{\rho_2=(1-p)|\psi\rangle\langle\psi|+pX|\psi\rangle\langle\psi|X.}
$$

For $|\psi\rangle=\alpha|0\rangle+\beta|1\rangle$, its explicit [density matrix](../../../../../../density-matrix.md) is

$$
\rho_2=\begin{pmatrix}
(1-p)|\alpha|^2+p|\beta|^2&(1-p)\alpha\beta^*+p\beta\alpha^*\\
(1-p)\beta\alpha^*+p\alpha\beta^*&(1-p)|\beta|^2+p|\alpha|^2
\end{pmatrix}.
$$

For a pure reference [quantum state](../../../../../../quantum-state.md), the square of the paper's [quantum fidelity](../../../../../../fidelity-of-quantum-states.md) is $F^2=\langle\psi|\rho_2|\psi\rangle$. Therefore

$$
F^2=1-p+p|\langle\psi|X|\psi\rangle|^2.
$$

With $|\psi\rangle=\cos(\theta/2)|0\rangle+e^{i\phi}\sin(\theta/2)|1\rangle$, the [expectation](../../../../../../expected-value.md) is $\langle X\rangle=\sin\theta\cos\phi$, the $x$ component of the [Bloch vector](../../../../../../bloch-vector.md). Hence

$$
F^2(\theta,\phi)=1-p+p\sin^2\theta\cos^2\phi.
$$

“All possible [quantum states](../../../../../../quantum-state.md)” is interpreted as the rotationally invariant [uniform pure-qubit average](../../../../../../uniform-pure-qubit-average.md), with measure $d\mu=\sin\theta\,d\theta\,d\phi/(4\pi)$. Thus

$$
\begin{aligned}
\langle F^2\rangle&=1-p+\frac{p}{4\pi}\int_0^\pi\sin^3\theta\,d\theta\int_0^{2\pi}\cos^2\phi\,d\phi\\
&=1-p+\frac{p}{4\pi}\cdot\frac43\cdot\pi,
\end{aligned}
$$

so the [average pure-qubit fidelity of a bit-flip channel](../../../../../../average-pure-qubit-fidelity-of-a-bit-flip-channel.md) is

$$
\boxed{\langle F^2\rangle=1-\frac{2p}{3}.}
$$

Equivalently, rotational symmetry gives $\langle r_x^2\rangle=\langle r_y^2\rangle=\langle r_z^2\rangle=1/3$, since a pure-state [Bloch vector](../../../../../../bloch-vector.md) has unit length. The $X$ eigenstates are unchanged as [density matrices](../../../../../../density-matrix.md) and have fidelity one, while a [computational basis](../../../../../../computational-basis.md) [quantum state](../../../../../../quantum-state.md) has $F^2=1-p$; these provide checks on the angular expression. A uniform distribution in $\theta$ rather than in solid angle would produce the wrong ensemble average. The requested quantity is the [mean](../../../../../../expected-value.md) squared fidelity, not the square of the [mean](../../../../../../expected-value.md) unsquared fidelity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
