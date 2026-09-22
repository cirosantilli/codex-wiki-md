<h1 id="15a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With the [Fourier transform](../../../../../../fourier-transform.md) convention of 5A, use the printed [Fourier inversion](../../../../../../fourier-inversion-theorem.md) formula directly. The possible choice of values at $s=\pm1$ has no effect on the integral. Integration over the support gives

$$
g(x)=\frac1{2\pi}\int_{-1}^1(e^s-e^{-s})e^{-isx}ds
=\frac1\pi\left[\frac{\sinh(1-ix)}{1-ix}-\frac{\sinh(1+ix)}{1+ix}\right].
$$

Combining the two fractions yields

$$
\boxed{g(x)=\frac{2i}{\pi(1+x^2)}\bigl(x\sinh1\cos x-\cosh1\sin x\bigr).}
$$

In particular $g$ is imaginary-valued and odd, as expected from the real odd transformed function with this inverse-transform sign.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [15A](../../15a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
