<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reversibly test whether the measured integer $x$ is a nontrivial divisor of $N$, and phase-flip exactly those computational basis states. This implements the good-subspace reflection in classical and quantum polynomial time. The reflection in $C_N|0^n\rangle$ is

$$
C_N(2|0^n\rangle\langle0^n|-I)C_N^\dagger,
$$

which is polynomial size by the stated assumption.

Here $\sin^2\theta=\sin^2(\pi/10)$, so $\theta=\pi/10$. Two amplification iterations give

$$
(2\cdot2+1)\theta=\frac\pi2.
$$

The final measurement therefore returns a nontrivial factor with certainty whenever $N$ is composite. Only two uses each of $C_N,C_N^\dagger$ up to a constant factor and polynomial-size verification circuits are required, so the complete algorithm is polynomial in $n$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
