<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the vortex aspect ratio as $\chi$ to distinguish it from cylindrical radius. The [Kida vortex](../../../../../../kida-vortex.md) core flow is

$$
u_x=\frac{3\Omega}{2\chi(\chi-1)}y,
\qquad
u_y=-\frac{3\Omega\chi}{2(\chi-1)}x.
$$

As $\chi\to\infty$, $u_x\to0$ and $u_y\to-(3/2)\Omega x$, recovering [Keplerian shear](../../../../../../keplerian-shear.md).

For a fluid particle,

$$
\ddot x=-\left[\frac{3\Omega}{2(\chi-1)}\right]^2x.
$$

It therefore circulates around an ellipse with angular frequency $3\Omega/[2(\chi-1)]$ and period

$$
\boxed{T_{\rm vort}=\frac{4\pi(\chi-1)}{3\Omega}}.
$$

For a perturbation depending only on $z,t$, horizontal pressure gradients vanish. Linearization gives

$$
\boxed{\partial_tu_x'
=\Omega\left[2-\frac{3}{2\chi(\chi-1)}\right]u_y'},
$$



$$
\boxed{\partial_tu_y'
=-\Omega\left[2-\frac{3\chi}{2(\chi-1)}\right]u_x'}.
$$

Taking $\mathbf u'\propto e^{-i\omega t}$ yields

$$
\boxed{\omega^2=\Omega^2
\left[2-\frac{3}{2\chi(\chi-1)}\right]
\left[2-\frac{3\chi}{2(\chi-1)}\right]}.
$$

The first bracket is positive for $\chi>3/2$, while the second is negative for $1<\chi<4$. Their product is therefore negative, so $\omega$ is imaginary and the mode grows precisely when

$$
\boxed{\frac32<\chi<4}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
