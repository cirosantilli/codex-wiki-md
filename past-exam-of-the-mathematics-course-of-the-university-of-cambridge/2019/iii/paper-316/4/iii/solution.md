<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For small $\alpha$, expand the defining integrand of the [Laplace coefficient](../../../../../../laplace-coefficient.md):

$$
(1-2\alpha\cos x+\alpha^2)^{-3/2}=1+3\alpha\cos x+O(\alpha^2).
$$

Hence

$$
b_{3/2}^{(1)}(\alpha)=\frac1\pi\int_0^{2\pi}\cos x[1+3\alpha\cos x+O(\alpha^2)]\,dx.
$$

The constant term integrates to zero and $\int_0^{2\pi}\cos^2x\,dx=\pi$, giving

$$
\boxed{b_{3/2}^{(1)}(\alpha)=3\alpha+O(\alpha^3).}
$$

There is no quadratic term: its factors are combinations of $\cos x$ and $\cos^3x$, which both integrate to zero over a period. The linear approximation is used for the distant planet, not for the closely spaced inner pair.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 316](../../../paper-316-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
