<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat u(k,y)=\int_{\mathbb R}u(x,y)e^{-ikx}\,dx$ and inverse factor $1/(2\pi)$. [Laplace equation](../../../../../laplace-equation.md) gives $\widehat u_{yy}-k^2\widehat u=0$. Selecting its decaying Fourier branch gives $\widehat u(k,y)=\widehat u_0(k)e^{-|k|y}$, the standard bounded solution for bounded continuous boundary data. The inverse transform of the multiplier is the [Poisson kernel for the upper half-plane](../../../../../poisson-kernel-for-the-upper-half-plane.md):

$$
\frac1{2\pi}\int_{\mathbb R}e^{ikx-|k|y}\,dk
=\frac1\pi\int_0^\infty e^{-ky}\cos(kx)\,dk
=\frac{y}{\pi(x^2+y^2)}.
$$

The [convolution theorem](../../../../../convolution-theorem.md) therefore gives the [Poisson integral](../../../../../poisson-integral.md)

$$
\boxed{u(x,y)=\int_{\mathbb R}u_0(t)\frac{y}{\pi[(x-t)^2+y^2]}\,dt.}
$$

For suitably regular boundary data, this kernel is an approximate identity as $y\downarrow0$, recovering $u_0$.

For $a>0$, contour integration gives $\widehat u_0(k)=(\pi/a)e^{-a|k|}$. Multiplication by $e^{-y|k|}$ and inversion yield

$$
\boxed{u(x,y)=\frac{y+a}{a[x^2+(y+a)^2]}.}
$$

The stated form assumes $a>0$; if $a<0$, replace it by $|a|$ because the boundary function only depends on $a^2$. The case $a=0$ has singular boundary data and is outside this regular calculation.

The transform argument requires a growth condition. A [zero-boundary harmonic function with pointwise vertical decay](../../../../../zero-boundary-harmonic-function-with-pointwise-vertical-decay.md) shows that the printed conditions alone do not ensure uniqueness:

$$
v(x,y)=\operatorname{Im}e^{(x+iy)^2}=e^{x^2-y^2}\sin(2xy)
$$

vanishes at $y=0$ and tends to zero as $y\to\infty$ for every fixed $x$. It can be added without changing those conditions, but its growth in $x$ excludes it from the bounded solution class. The displayed Poisson integral is the standard bounded solution for regular bounded boundary data; pointwise vertical decay by itself cannot justify a uniqueness claim.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
