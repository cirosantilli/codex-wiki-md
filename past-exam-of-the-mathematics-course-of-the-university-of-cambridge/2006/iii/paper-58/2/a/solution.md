<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Denote the normalized initial field by $|F\rangle$, and its shifted packets by

$$
|F_-\rangle=\frac1{\sqrt k}\sum_{n=1}^k|n\rangle,\qquad
|F_+\rangle=\frac1{\sqrt k}\sum_{n=3}^{k+2}|n\rangle.
$$

Here the photon-number kets are [orthogonal](../../../../../../orthogonal-vectors.md) [Fock states](../../../../../../fock-state.md). Counting shared number labels gives

$$
\langle F|F_-\rangle=\langle F|F_+\rangle=r_k=\frac{k-1}{k},\qquad
\langle F_-|F_+\rangle=s_k=\frac{\max(k-2,0)}k.
$$

After the interaction, linearity gives the joint state

$$
|\Omega\rangle=\frac1{\sqrt2}\left[
|0\rangle(\alpha|F\rangle+\beta|F_+\rangle)
+|1\rangle(\alpha|F_-\rangle-\beta|F\rangle)\right].
$$

Take the [partial trace](../../../../../../partial-trace.md) over the field. Put $d=|\alpha|^2-|\beta|^2$ and $c=\alpha\beta^*+\alpha^*\beta$. In the ordered [qubit](../../../../../../qubit.md) basis $(|0\rangle,|1\rangle)$, the reduced [density matrix](../../../../../../density-matrix.md) is

$$
\boxed{\rho=\frac12\begin{pmatrix}
1+r_kc&r_kd+s_k\alpha^*\beta-\alpha\beta^*\\
r_kd+s_k\alpha\beta^*-\alpha^*\beta&1-r_kc
\end{pmatrix}.}
$$

For example, its upper off-diagonal entry is half the overlap of the field accompanying $|1\rangle$ with the field accompanying $|0\rangle$, fixing the conjugation order. The [trace](../../../../../../matrix-trace.md) is one, and positivity follows because this is the [partial trace](../../../../../../partial-trace.md) of a normalized [pure state](../../../../../../pure-state.md). For $k\ge2$, $s_k=1-2/k$; at $k=1$ it is zero, not the continuation $-1$. This is the [photon-number reference for a Hadamard gate](../../../../../../photon-number-reference-for-a-hadamard-gate.md) channel, not an actual coherent-state packet.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
