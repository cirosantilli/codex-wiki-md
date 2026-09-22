<h1 id="36a/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The classical [canonical partition function](../../../../../../../canonical-partition-function.md) uses one phase-space cell $h^2$ per state. In [polar coordinates](../../../../../../../polar-coordinates.md),

$$
\begin{aligned}
Z_1
&=\frac1{h^2}
\int_{\mathbb R^2}e^{-\beta p^2/(2m)}\,d^2p
\int_{r<R}e^{-\beta\kappa r^2/2}\,d^2x\\
&=\frac1{h^2}
\left(\frac{2\pi m}{\beta}\right)
\left(2\pi\int_0^Rr e^{-\beta\kappa r^2/2}\,dr\right)\\
&=\boxed{
\frac{4\pi^2m}{h^2\beta^2\kappa}
\left(1-e^{-\beta\kappa R^2/2}\right)
}.
\end{aligned}
$$

Equivalently, using $h=2\pi\hbar$,

$$
Z_1=\frac{m}{\hbar^2\beta^2\kappa}
\left(1-e^{-\beta\kappa R^2/2}\right).
$$

This is the [particle in a finite two-dimensional harmonic trap](../../../../../../../particle-in-a-finite-two-dimensional-harmonic-trap.md) partition function.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [36A](../../../36a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
