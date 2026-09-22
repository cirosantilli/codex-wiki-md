<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The profile is an even [function](../../../../function-split.md), so its [Fourier transform](../../../../fourier-transform-split.md) is real and

$$
\widehat T(\omega)=2\int_0^2(1-x/2)\cos(\omega x)\,dx.
$$

For $\omega\ne0$, [integration by parts](../../../../integration-by-parts.md) gives

$$
\int_0^2(1-x/2)\cos(\omega x)\,dx
=\frac1{2\omega}\int_0^2\sin(\omega x)\,dx
=\frac{1-\cos(2\omega)}{2\omega^2}.
$$

Therefore

$$
\boxed{\widehat T(\omega)=\begin{cases}\displaystyle\frac{2\sin^2\omega}{\omega^2},&\omega\ne0,\\2,&\omega=0.\end{cases}}
$$

At zero, direct integration gives the area of the triangle, namely two; the displayed quotient has the same limit. In particular **$\widehat T(\omega)\geq0$ for every real frequency**. This is the [Fourier transform of a triangular function](../../../../fourier-transform-of-a-triangular-function.md).

One can also see the nonnegative square structurally: $T=\tfrac12\mathbf1_{[-1,1]}*\mathbf1_{[-1,1]}$, so the [convolution theorem](../../../../convolution-theorem.md) gives $\widehat T=\tfrac12(2\sin\omega/\omega)^2$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
