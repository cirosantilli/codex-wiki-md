<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\omega=e^{2\pi i/3}$. The positive-exponent [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) gives $|\xi\rangle=3^{-1/2}\sum_{y=0}^2\omega^{2y}|y\rangle$. Reindexing the [cyclic shift operator](../../../../../../cyclic-shift-operator.md) gives

$$
S|\xi\rangle=\frac1{\sqrt3}\sum_{z=0}^2\omega^{2(z-1)}|z\rangle=\omega^{-2}|\xi\rangle=\omega|\xi\rangle.
$$

Thus **$|\xi\rangle$ is an eigenstate with eigenvalue $\omega$**, with this sign fixed by the printed [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) convention.

Prepare the first two [qutrits](../../../../../../qutrit.md) in $(\operatorname{QFT}_3|0\rangle)^{\otimes2}$ and the answer [qutrit](../../../../../../qutrit.md) in $|\xi\rangle$. The [modular-addition quantum oracle](../../../../../../modular-addition-quantum-oracle.md) applies $S^{f(x_1,x_2)}$ to the answer. Its [eigenvalue](../../../../../../eigenvalue.md) produces [quantum phase kickback](../../../../../../phase-kickback.md), leaving

$$
\frac13\sum_{x_1,x_2=0}^2\omega^{a_1x_1+a_2x_2}|x_1,x_2\rangle\otimes|\xi\rangle
=\operatorname{QFT}_3|a_1\rangle\otimes\operatorname{QFT}_3|a_2\rangle\otimes|\xi\rangle.
$$

Apply $\operatorname{QFT}_3^{-1}$ to each input [qutrit](../../../../../../qutrit.md), then measure them in the [computational basis](../../../../../../computational-basis.md). The result is

$$
\boxed{(a_1,a_2)\text{ with probability }1.}
$$

The preparation, inverse transforms and measurements are independent of $f$, and there is exactly one use of $U_f$. This is [qutrit linear-function identification](../../../../../../qutrit-linear-function-identification.md), the ternary version of [Bernstein-Vazirani phase kickback](../../../../../../bernstein-vazirani-phase-kickback.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
