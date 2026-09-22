<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Because $H_n|0^n\rangle=|\psi_0\rangle$,

$$
-H_nI_0H_n=2|\psi_0\rangle\langle\psi_0|-I,
$$

which is the [reflection operator](../../../../../../reflection-operator.md) in the line spanned by $|\psi_0\rangle$. Meanwhile $I_G$ changes the sign of every good basis state and fixes every bad basis state; on

$$
\mathcal P=\operatorname{span}_{\mathbb R}\{|\psi_G\rangle,|\psi_B\rangle\}
$$

it is the reflection in the $|\psi_B\rangle$ axis. Both reflections preserve $\mathcal P$, so their product $Q$ does too.

Write

$$
|\psi_0\rangle
=\sqrt{\frac{k}{N}}|\psi_G\rangle
+\sqrt{\frac{N-k}{N}}|\psi_B\rangle
=\sin\theta|\psi_G\rangle+\cos\theta|\psi_B\rangle,
\qquad
\sin\theta=\sqrt{\frac{k}{N}}.
$$

In [Euclidean geometry](../../../../../../euclidean-geometry.md), the composition of reflections in two lines through the origin has a [rotation matrix](../../../../../../rotation-matrix.md) through twice the oriented angle between the lines. Hence $Q$ rotates the good-bad plane by $2\theta$ from $|\psi_B\rangle$ toward $|\psi_G\rangle$. In particular, the [Grover rotation angle](../../../../../../grover-rotation-angle.md) formula is

$$
\boxed{Q^r|\psi_0\rangle
=\sin((2r+1)\theta)|\psi_G\rangle
+\cos((2r+1)\theta)|\psi_B\rangle.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
