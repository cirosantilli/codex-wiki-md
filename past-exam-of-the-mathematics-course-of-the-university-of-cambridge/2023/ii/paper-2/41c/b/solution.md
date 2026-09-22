<h1 id="41c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiating the truncated Fourier expansion gives

$$
u_x=\sum_{m=-d}^di\pi m\widehat u_m e^{i\pi mx}.
$$

The $n$th Fourier coefficient of the product $cu_x$ is the [discrete convolution](../../../../../../discrete-convolution.md)

$$
i\pi\sum_{m=-d}^dm\widehat c_{n-m}\widehat u_m.
$$

Projecting the advection equation onto modes $|n|\leq d$ therefore gives

$$
\frac{d\widehat u_n}{dt}
=-i\pi\sum_{m=-d}^dm\widehat c_{n-m}\widehat u_m.
$$

Thus

$$
\boxed{\frac{d\widehat{\mathbf u}}{dt}
=i\pi B\widehat{\mathbf u}},
\qquad
\boxed{B_{nm}=-m\widehat c_{n-m}}.
$$

Equivalently, if

$$
C_{nm}=\widehat c_{n-m},
\qquad
D=\operatorname{diag}(-d,-d+1,\ldots,d),
$$

then

$$
\boxed{B=-CD}.
$$

This is the [Fourier spectral method for variable-coefficient advection](../../../../../../fourier-spectral-method-for-variable-coefficient-advection.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [41C](../../41c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
