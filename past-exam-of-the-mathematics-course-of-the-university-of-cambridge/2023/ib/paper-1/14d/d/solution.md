<h1 id="14d/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $\psi(x)=Ce^{-\alpha x^2}$,

$$
\psi''=(4\alpha^2x^2-2\alpha)\psi.
$$

The stationary [Schrödinger equation](../../../../../../schrodinger-equation.md) becomes

$$
\left[
\frac{\hbar^2\alpha}{m}
+\left(k-\frac{2\hbar^2\alpha^2}{m}\right)x^2
\right]\psi=E\psi.
$$

Hence, choosing the positive root and a positive normalization constant,

$$
\alpha=\frac1\hbar\sqrt{\frac{mk}{2}},
\qquad
E=\hbar\sqrt{\frac{k}{2m}},
\qquad
C=\left(\frac{2\alpha}{\pi}\right)^{1/4}.
$$

The state is even, so $\langle x\rangle=\langle p\rangle=0$. The Gaussian [integrals](../../../../../../integral.md) give

$$
(\Delta x)^2=\frac1{4\alpha},
\qquad
(\Delta p)^2=\hbar^2\alpha,
$$

and therefore $\Delta x\Delta p=\hbar/2$. These values are collected in [gaussian eigenstate for a quadratic potential](../../../../../../gaussian-eigenstate-for-a-quadratic-potential.md).

Finally, equality in the derivation of the uncertainty relation requires the centred [vectors](../../../../../../vector.md) to be linearly dependent with a purely imaginary proportionality constant. Thus for some $s>0$,

$$
(\widehat p-p_0)\psi=is(\widehat x-x_0)\psi.
$$

In position space this says

$$
\psi'=\left(\frac{ip_0}{\hbar}-\frac{s(x-x_0)}{\hbar}\right)\psi,
$$

whose normalizable solutions are

$$
\psi(x)=C_0\exp\left(\frac{ip_0x}{\hbar}-\frac{s(x-x_0)^2}{2\hbar}\right).
$$

**Thus every saturating state is Gaussian up to translation, a plane-wave factor, and an overall phase, as in the [equality case of the Heisenberg uncertainty relation](../../../../../../equality-case-of-the-heisenberg-uncertainty-relation.md).**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [14D](../../14d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
