<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A general single-[qubit](../../../../../../qubit.md) [quantum gate](../../../../../../quantum-logic-gate.md) belongs to $U(2)$. Remove its [global phase](../../../../../../global-phase.md) to obtain $V\in SU(2)$; the displayed expression in the question is literally a special-unitary gate and represents a general physical gate up to that phase. Every $V\in SU(2)$ can be written

$$
V=\begin{pmatrix}u&v\\-v^*&u^*\end{pmatrix},\qquad |u|^2+|v|^2=1,
$$

and consequently

$$
V=q_0 I-i(q_x\sigma_x+q_y\sigma_y+q_z\sigma_z),\qquad q_0,q_x,q_y,q_z\in\mathbb R,\quad q_0^2+q_x^2+q_y^2+q_z^2=1.
$$

Choose $\theta$ with $q_0=\cos(\theta/2)$ and $\|q\|=\sin(\theta/2)$, and set $n=q/\|q\|$ when $q\ne0$. The [Pauli matrix multiplication law](../../../../../../pauli-matrix-multiplication-law.md) shows $(n\cdot\sigma)^2=\|n\|^2I=I$. Applying part (a) proves

$$
\boxed{U=e^{i\chi}e^{-i\theta(n\cdot\sigma)/2},\qquad \|n\|=1.}
$$

For $q=0$, $V=\pm I$ and any axis can be used with angle zero or $2\pi$. Thus the phase-free gate is a [rotation gate](../../../../../../rotation-gate.md) by angle $\theta$ about the unit axis $n$. An arbitrary exact $U(2)$ operator also needs the scalar phase $e^{i\chi}$, which cannot in general be produced by a traceless [Quantum Hamiltonian](../../../../../../hamiltonian-quantum-mechanics.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
