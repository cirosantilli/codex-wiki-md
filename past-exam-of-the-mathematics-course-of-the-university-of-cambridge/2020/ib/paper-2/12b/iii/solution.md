<h1 id="12b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $w=z-1$. Then

$$
f(z)=\frac1{(w+1)(w-1)}
=-\frac1{1-w^2}.
$$

Thus

$$
\boxed{f(z)=-\sum_{n=0}^{\infty}(z-1)^{2n}},
\qquad 0<|z-1|<1.
$$

This is actually a [Taylor series](../../../../../../taylor-series.md), because $z=1$ is a regular point. The point $z=0$ is a [simple pole](../../../../../../simple-pole.md). At infinity,

$$
f(1/w)=\frac{w^2}{1-2w}
$$

extends analytically to $w=0$, so infinity is a [removable singularity](../../../../../../removable-singularity.md) of $f$, with extended value zero.

For the real integral, first write

$$
\frac{2-\cos\theta}{5-4\cos\theta}
=\frac14+\frac{3}{4(5-4\cos\theta)}.
$$

Let

$$
J=\int_0^{2\pi}\frac{d\theta}{5-4\cos\theta}.
$$

With $z=e^{i\theta}$,

$$
J=\oint_{|z|=1}\frac{dz}{i(-2z^2+5z-2)}.
$$

The denominator has roots $1/2$ and $2$, so only $1/2$ lies inside the contour. Its [residue](../../../../../../residue.md) is $1/(3i)$, and the [residue theorem](../../../../../../residue-theorem.md) gives

$$
J=2\pi i\frac1{3i}=\frac{2\pi}{3}.
$$

Consequently

$$
\boxed{\int_0^{2\pi}\frac{2-\cos\theta}{5-4\cos\theta}\,d\theta
=\frac{\pi}{2}+\frac34\frac{2\pi}{3}
=\pi}.
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [12B](../../12b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
