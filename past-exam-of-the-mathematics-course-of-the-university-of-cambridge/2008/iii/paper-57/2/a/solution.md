<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $L=2^N$ and define $\theta=\arcsin\sqrt{M/L}$. The normalized good and bad [vectors](../../../../../../vector.md) have disjoint [computational basis](../../../../../../computational-basis.md) supports, so they are [orthogonal](../../../../../../orthogonal-vectors.md). Counting the terms in the uniform [quantum superposition](../../../../../../quantum-superposition.md) gives

$$
\boxed{|\phi\rangle=\sin\theta\,|\Psi_g\rangle+\cos\theta\,|\Psi_b\rangle,\qquad\sin\theta=\sqrt{M/2^N}.}
$$

Since $V_0=I-2|0^N\rangle\langle0^N|$, the [Hadamard transform](../../../../../../hadamard-transform.md) gives $-H^{\otimes N}V_0H^{\otimes N}=2|\phi\rangle\langle\phi|-I$, the [Grover diffusion operator](../../../../../../grover-diffusion-operator.md). On the ordered [orthonormal basis](../../../../../../orthonormal-basis.md) $(|\Psi_g\rangle,|\Psi_b\rangle)$, the two [reflection operators](../../../../../../reflection-operator.md) have [matrices](../../../../../../matrix.md)

$$
U_f=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\qquad 2|\phi\rangle\langle\phi|-I=\begin{pmatrix}-\cos2\theta&\sin2\theta\\\sin2\theta&\cos2\theta\end{pmatrix}.
$$

Their product is

$$
\boxed{G=\begin{pmatrix}\cos2\theta&\sin2\theta\\-\sin2\theta&\cos2\theta\end{pmatrix}.}
$$

This is a plane [rotation](../../../../../../rotation-mathematics.md) through angle $-2\theta$ in the displayed coordinate convention, with the invariant good-bad plane preserved by both operators. In particular its action sends $(\sin a,\cos a)$ to $(\sin(a+2\theta),\cos(a+2\theta))$. Induction therefore gives the [Grover rotation angle](../../../../../../grover-rotation-angle.md) formula

$$
G^n|\phi\rangle=\sin((2n+1)\theta)|\Psi_g\rangle+\cos((2n+1)\theta)|\Psi_b\rangle.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
