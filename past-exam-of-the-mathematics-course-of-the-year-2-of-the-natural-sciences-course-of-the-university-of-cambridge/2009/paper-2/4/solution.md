<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Cauchy's integral theorem](../../../../cauchy-s-integral-theorem.md) states that a [holomorphic function](../../../../holomorphic-function-split.md) on a simply connected domain has zero [contour integral](../../../../contour-integral.md) around every closed piecewise smooth curve in that domain. One proof begins with the [Cauchy theorem for a triangle](../../../../cauchy-theorem-for-a-triangle.md). Subdivide a triangle into four equal triangles. Their oriented boundary integrals sum to the original integral because internal edges cancel, so choose a nested subtriangle carrying at least one quarter of the preceding integral's modulus. At stage $n$, its perimeter and diameter are $P/2^n,d/2^n$, and the nested triangles converge to a point $z_0$. Complex differentiability gives $f(z)=f(z_0)+f'(z_0)(z-z_0)+\epsilon(z)(z-z_0)$, with $\epsilon(z)\to0$. The affine terms have primitives and integrate to zero. Therefore $|I_n|\leq\sup|\epsilon|\,Pd/4^n$, while $|I_0|\leq4^n|I_n|$. Letting $n\to\infty$ proves $I_0=0$. Triangulation cancels internal edges for polygonal contours; local primitives and deformation through the domain extend the result to the stated piecewise smooth curves. Simple connectedness ensures the necessary contractions do not pass through a missing point.

Apply the theorem to $e^{-az^2}$ on the rectangle between heights zero and $\rho$, with vertical sides at $\operatorname{Re}z=\pm R$. On either vertical side,

$$
|e^{-az^2}|=e^{-aR^2+a(\operatorname{Im}z)^2}\leq e^{-aR^2+a\rho^2}.
$$

The modulus of each side integral is at most $|\rho|e^{-aR^2+a\rho^2}\to0$. Both horizontal integrals converge absolutely. The two horizontal orientations are opposite, so the limit gives $I(\rho,a)=I(0,a)$, also for negative $\rho$. This is [Gaussian contour translation](../../../../gaussian-contour-translation.md).

Now complete the square:

$$
-ax^2+i\nu x=-a\left(x-\frac{i\nu}{2a}\right)^2-\frac{\nu^2}{4a}.
$$

The substitution $z=x-i\nu/(2a)$ moves the path to height $-\nu/(2a)$. Its Gaussian integral equals the real-axis integral by the preceding result. Hence

$$
\boxed{\int_{-\infty}^{\infty}e^{-ax^2+i\nu x}dx=\sqrt{\frac\pi a}\,e^{-\nu^2/(4a)},\qquad a>0,\ \nu\in\mathbb R.}
$$

This also gives the [Fourier transform of a Gaussian](../../../../fourier-transform-of-a-gaussian.md) in the convention with no prefactor in the forward transform.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
