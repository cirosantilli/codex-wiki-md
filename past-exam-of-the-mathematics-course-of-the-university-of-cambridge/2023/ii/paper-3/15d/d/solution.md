<h1 id="15d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

After the first [Hadamard gate](../../../../../../hadamard-gate.md) and the [controlled unitary gate](../../../../../../controlled-unitary-gate.md), the state is

$$
\frac1{\sqrt2}
\left(|0\rangle|\psi\rangle
+e^{i\theta}|1\rangle|\psi\rangle\right).
$$

The final Hadamard gate gives

$$
\boxed{
\frac12\left[
(1+e^{i\theta})|0\rangle
+(1-e^{i\theta})|1\rangle
\right]|\psi\rangle.}
$$

Hence the [Hadamard test](../../../../../../hadamard-test.md) returns one with probability

$$
\boxed{
\Pr(1)=\frac{|1-e^{i\theta}|^2}{4}
=\frac{1-\cos\theta}{2}
=\sin^2\frac\theta2.}
$$

If $U|\psi\rangle=|\psi\rangle$, then $\theta=0$ and the outcome is zero with certainty. If $U|\psi\rangle=-|\psi\rangle$, then $\theta=\pi$ modulo $2\pi$ and the outcome is one with certainty. The single measurement therefore distinguishes the two promised cases exactly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
