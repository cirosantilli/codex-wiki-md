<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $a=\langle\psi|w\rangle=2^{-N/2}$, which is real and satisfies $0<a<1$ for $N\geq1$. The invariant two-dimensional span has orthonormal eigenvectors

$$
|+\rangle=\frac{|\psi\rangle+|w\rangle}{\sqrt{2(1+a)}},\qquad
|-\rangle=\frac{|\psi\rangle-|w\rangle}{\sqrt{2(1-a)}},
$$

with [eigenvalues](../../../../../../eigenvalue.md) $\Delta(1+a)$ and $\Delta(1-a)$. In this basis,

$$
|\psi\rangle=\sqrt{\frac{1+a}{2}}|+\rangle+\sqrt{\frac{1-a}{2}}|-\rangle,
\quad
|w\rangle=\sqrt{\frac{1+a}{2}}|+\rangle-\sqrt{\frac{1-a}{2}}|-\rangle.
$$

Transfer therefore requires the two evolved eigenphases to differ by an odd multiple of $\pi$:

$$
e^{-i2\Delta at}=-1.
$$

The first positive time is

$$
\boxed{t_0=\frac\pi{2\Delta a}=\frac{\pi\sqrt{2^N}}{2\Delta}.}
$$

Equivalently, exponentiating on the invariant span gives the full evolution

$$
e^{-iH_Gt}|\psi\rangle=e^{-i\Delta t}
\bigl[\cos(\Delta at)|\psi\rangle-i\sin(\Delta at)|w\rangle\bigr].
$$

At $t_0$ this is $-ie^{-i\Delta t_0}|w\rangle$, so the requested [global phase](../../../../../../global-phase.md) can be chosen as $\alpha=-\Delta t_0-\pi/2$ modulo $2\pi$. Since the two vectors are linearly independent, their relative coefficient cannot produce exact transfer at an earlier positive time. This is [continuous-time quantum search](../../../../../../continuous-time-quantum-search.md), with time proportional to the square root of the search-space dimension for fixed $\Delta$. Restoring units multiplies the stated time by $\hbar$. The degenerate zero-qubit case would already have $\psi=w$, so there would be no smallest positive transfer time; the formula concerns the nontrivial $N\geq1$ search.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
