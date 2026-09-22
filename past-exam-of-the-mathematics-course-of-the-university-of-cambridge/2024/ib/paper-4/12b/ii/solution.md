<h1 id="12b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Fourier transformation gives

$$
(k^2+m^2)\widehat G(k)=1,
\qquad
\widehat G(k)=\frac1{k^2+m^2}.
$$

For $x>0$, close the inverse-transform contour in the upper half-plane and take the residue at $k=im$; for $x<0$, close it in the lower half-plane. This gives the [one-dimensional modified Helmholtz Green function](../../../../../../one-dimensional-modified-helmholtz-green-function.md)

$$
\boxed{G(x)=\frac{e^{-m|x|}}{2m}}.
$$

The same formula works for complex $m$ with $\operatorname{Re}m>0$: it decays at both ends, is continuous at zero, and its [derivative](../../../../../../derivative.md) has the jump $G'(0+)-G'(0-)=-1$ required by the delta source.

Convolution therefore yields

$$
\boxed{
u(x)=\frac1{2m}\int_{-\infty}^{\infty}
 e^{-m|x-y|}f(y)\,dy}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [12B](../../12b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
