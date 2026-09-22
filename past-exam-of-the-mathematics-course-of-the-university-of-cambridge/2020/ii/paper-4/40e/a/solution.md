<h1 id="40e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Termwise differentiation of a Fourier series](../../../../../../termwise-differentiation-of-a-fourier-series.md) multiplies a mode by its wavenumber, so

$$
\boxed{\widehat{(f_x)}_{m,n}=i\pi m\widehat f_{m,n},
\qquad
\widehat{(f_y)}_{m,n}=i\pi n\widehat f_{m,n}}.
$$

The [convolution theorem](../../../../../../convolution-theorem.md) turns pointwise multiplication into [discrete convolution](../../../../../../discrete-convolution.md):

$$
h=fg
=\sum_{p,q}\sum_{r,s}\widehat f_{p,q}\widehat g_{r,s}
 e^{i\pi(p+r)x+i\pi(q+s)y},
$$

so

$$
\boxed{\widehat h_{m,n}
=\sum_{p,q\in\mathbb Z}\widehat f_{p,q}\widehat g_{m-p,n-q}}.
$$

The assumed [real analyticity](../../../../../../real-analytic-function.md) justifies these termwise operations through rapid decay of the [Fourier coefficients](../../../../../../fourier-coefficient.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40E](../../40e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
