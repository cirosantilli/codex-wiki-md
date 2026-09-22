<h1 id="10d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let

$$
H_n=H^{\otimes n},
\qquad
|s\rangle=H_n|0^n\rangle
=\frac1{\sqrt N}\sum_{x\in B_n}|x\rangle,
$$

where $H$ is the [Hadamard gate](../../../../../../hadamard-gate.md). For a computational-basis string $z$, define the phase reflection

$$
I_z=I-2|z\rangle\langle z|.
$$

Thus $I_0$ changes the sign of $|0^n\rangle$, while $I_{x_0}$ changes the sign of the marked state.

Conjugating $I_0$ by $H_n$ reflects in the hyperplane perpendicular to $|s\rangle$, so

$$
-H_nI_0H_n=2|s\rangle\langle s|-I
$$

is the [Grover diffusion operator](../../../../../../grover-diffusion-operator.md), the reflection about $|s\rangle$. The [Grover iteration operator](../../../../../../grover-s-algorithm.md)

$$
Q=(2|s\rangle\langle s|-I)I_{x_0}
$$

is the product of two reflections. It acts as a rotation through $2\theta$ in the plane spanned by the marked state $|x_0\rangle$ and the normalized uniform superposition of unmarked states, where

$$
\sin\theta=\frac1{\sqrt N}.
$$

It is the identity up to sign on the orthogonal complement of that plane.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10D](../../10d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
