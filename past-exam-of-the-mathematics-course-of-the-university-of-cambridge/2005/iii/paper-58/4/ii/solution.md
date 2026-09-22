<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $\rho_1=|\psi\rangle\langle\psi|$ and $\rho_2=|\varphi\rangle\langle\varphi|$. A pure-state [density matrix](../../../../../../density-matrix.md) is a rank-one [orthogonal projector](../../../../../../orthogonal-projection.md), so $\rho_1^{1/2}=\rho_1$ and

$$
\rho_1\rho_2\rho_1=|\langle\psi|\varphi\rangle|^2\rho_1.
$$

Taking its square root and [trace](../../../../../../matrix-trace.md) yields the unsquared [quantum fidelity](../../../../../../fidelity-of-quantum-states.md)

$$
F=|\langle\psi|\varphi\rangle|.
$$

Use [unitary invariance of trace distance and fidelity](../../../../../../unitary-invariance-of-trace-distance-and-fidelity.md) to choose a basis of the span of the two [quantum states](../../../../../../quantum-state.md) in which $|\psi\rangle=|0\rangle$ and $|\varphi\rangle=c|0\rangle+s|1\rangle$, with $c=F\ge0$ and $s=\sqrt{1-c^2}\ge0$. Choosing state-vector phases to make the coefficients nonnegative does not change either [density matrix](../../../../../../density-matrix.md). On that span,

$$
\rho_1-\rho_2=\begin{pmatrix}s^2&-cs\\-cs&-s^2\end{pmatrix},\qquad (\rho_1-\rho_2)^2=s^2I.
$$

Its [eigenvalues](../../../../../../eigenvalue.md) are $s$ and $-s$, with zero [eigenvalues](../../../../../../eigenvalue.md) on the orthogonal complement. The positive square root of $\Delta^\dagger\Delta$ therefore has two [eigenvalues](../../../../../../eigenvalue.md) $s$, so the [trace distance](../../../../../../trace-distance.md) is $(s+s)/2=s$. Thus the [pure-state trace distance and fidelity identity](../../../../../../pure-state-trace-distance-and-fidelity-identity.md) is

$$
\boxed{D(\rho_1,\rho_2)=\sqrt{1-F(\rho_1,\rho_2)^2}.}
$$

Identical [pure quantum states](../../../../../../pure-state.md) give $F=1,D=0$; orthogonal [pure quantum states](../../../../../../pure-state.md) give $F=0,D=1$. If the span is one-dimensional, the identical-state result follows directly, so no second basis vector is required. This formula uses the unsquared fidelity convention in the paper; if fidelity denotes squared overlap instead, the square inside the formula is omitted.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
