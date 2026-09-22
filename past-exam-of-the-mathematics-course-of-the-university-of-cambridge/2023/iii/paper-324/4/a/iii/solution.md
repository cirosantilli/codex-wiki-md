<h1 id="4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Since the [Hadamard gate](../../../../../../../hadamard-gate.md) conjugates $X$ to $Z$,

$$
V_n=e^{i\pi(X\otimes X)/n},
\qquad
W_n=e^{i\pi(X\otimes Z)/n}.
$$

For $n=1$, each exponential is $-I$, so

$$
V_1W_1=I=e^{iA_1},
\qquad
\boxed{A_1=0}.
$$

For $n=2$,

$$
V_2=iX\otimes X,
\qquad
W_2=iX\otimes Z.
$$

Using $XZ=-iY$ gives

$$
V_2W_2=-I\otimes XZ=iI\otimes Y
=\exp\left(i\frac\pi2I\otimes Y\right),
$$

so one convenient logarithm is

$$
\boxed{A_2=\frac\pi2I\otimes Y}.
$$

Both products are [Clifford operations](../../../../../../../clifford-gate.md): the first is the identity and the second is a one-qubit [Pauli Y gate](../../../../../../../pauli-y-gate.md) up to global phase.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
