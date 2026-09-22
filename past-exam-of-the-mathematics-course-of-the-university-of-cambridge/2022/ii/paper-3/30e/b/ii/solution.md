<h1 id="30e/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set $t=zs$. Then

$$
\Gamma'(z)
=e^{z\log z}
\int_0^\infty
\frac{\log z+\log s}{s}
e^{z(\log s-s)}\,ds.
$$

The fixed phase

$$
\phi(s)=\log s-s
$$

has its unique maximum at $s=1$, with

$$
\phi(1)=-1,
\qquad
\phi''(1)=-1.
$$

The amplitude at the maximum is $\log z$. The interior-maximum form of [Laplace's method](../../../../../../../laplace-s-method.md) gives

$$
\Gamma'(z)
\sim e^{z\log z}e^{-z}\log z
\sqrt{\frac{2\pi}{z}}.
$$

Thus

$$
\boxed{
\Gamma'(z)\sim
\sqrt{\frac{2\pi}{z}},e^{z\log z-z}\log z
},
$$

so $\boxed{a=2\pi}$. This is the [Laplace asymptotic for the derivative of the Gamma function](../../../../../../../laplace-asymptotic-for-the-derivative-of-the-gamma-function.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [30E](../../../30e.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
