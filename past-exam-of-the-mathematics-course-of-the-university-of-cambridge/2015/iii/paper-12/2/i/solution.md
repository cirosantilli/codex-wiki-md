<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [normalized Fourier analysis on a finite abelian group](../../../../../../normalized-fourier-analysis-on-a-finite-abelian-group.md), identifying $A$ with its [indicator function](../../../../../../indicator-function.md) $a=\mathbf1_A$ on the [cyclic group](../../../../../../cyclic-group.md) $\mathbb Z_n$. The conventions are

$$
\mathbb E_xh(x)=\frac1n\sum_{x\in\mathbb Z_n}h(x),\qquad
\widehat h(r)=\mathbb E_xh(x)\omega^{-rx},\qquad
(h*k)(x)=\mathbb E_yh(y)k(x-y).
$$

The last operation is [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md). With these conventions the [Fourier coefficients on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) use a normalized average, while sums over frequencies use counting measure.

Expanding the [normalized convolution on a finite group](../../../../../../normalized-convolution-on-a-finite-group.md) and putting $z=x-y$ gives

$$
\widehat f(r)=\mathbb E_x\mathbb E_y a(y)a(x-y)\omega^{-rx}
=\bigl(\mathbb E_y a(y)\omega^{-ry}\bigr)\bigl(\mathbb E_z a(z)\omega^{-rz}\bigr)
=\widehat a(r)^2.
$$

For the [translation of a function](../../../../../../translation-of-a-function.md) $g(x)=f(x-u)$, putting $z=x-u$ yields

$$
\widehat g(r)=\mathbb E_z f(z)\omega^{-r(z+u)}=\omega^{-ru}\widehat f(r).
$$

**The two transforms are therefore**

$$
\boxed{\widehat f(r)=\widehat A(r)^2,\qquad \widehat g(r)=\omega^{-ru}\widehat A(r)^2.}
$$

The negative sign in the translation factor follows from the negative sign in our [Fourier coefficient on a finite abelian group](../../../../../../fourier-coefficient-on-a-finite-abelian-group.md) convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
