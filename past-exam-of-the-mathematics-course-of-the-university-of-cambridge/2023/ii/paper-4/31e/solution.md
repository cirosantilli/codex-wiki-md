<h1 id="31e/solution">Solution</h1>

↑ **Parent:** [31E](../31e.md)

Write the phase and amplitude as

$$
\phi(z)=\cosh z,
\qquad
f(z)=\frac1{z^2+16}.
$$

The [saddle point](../../../../../saddle-point.md) relevant to the contour is $z=0$, since $\phi'(z)=\sinh z$ and

$$
\phi(0)=1,
\qquad
\phi''(0)=1.
$$

The local [steepest-descent](../../../../../method-of-steepest-descent.md) direction is therefore vertical: with $z=iy$,

$$
\phi(iy)=\cos y=1-\frac{y^2}{2}+O(y^4).
$$

The given contour approaches the lines $\operatorname{Im}z=-\pi$ at its left end and $\operatorname{Im}z=\pi$ at its right end. The poles of $f$ are at $z=\pm4i$, outside the closed strip $|\operatorname{Im}z|\leq\pi$. The [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) therefore permits deformation to the contour consisting of the lower horizontal ray from $-\infty-i\pi$ to $-i\pi$, the vertical segment from $-i\pi$ to $i\pi$, and the upper horizontal ray from $i\pi$ to $\infty+i\pi$. On either horizontal ray,

$$
\cosh(p\pm i\pi)=-\cosh p,
$$

so those two integrals are exponentially small, of order $e^{-x}x^{-1/2}$.

The vertical segment, oriented upward, contributes

$$
i\int_{-\pi}^{\pi}\frac{e^{x\cos y}}{16-y^2}\,dy.
$$

Its real phase has a unique maximum at $y=0$. Since

$$
\frac1{16-y^2}=\frac1{16}+O(y^2),
$$

the [simple-saddle contribution in steepest descent](../../../../../simple-saddle-contribution-in-steepest-descent.md), equivalently the local [Gaussian integral](../../../../../gaussian-integral.md), gives

$$
I(x)
\sim \frac{i e^x}{16}
\int_{-\infty}^{\infty}e^{-xy^2/2}\,dy
=\boxed{\frac{i e^x}{16}\sqrt{\frac{2\pi}{x}}}
\qquad(x\to\infty).
$$

The factor $i$ comes from the upward tangent $dz=i\,dy$ of the deformed contour.

## ↑ Ancestors (10)

1. [31E](../31e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
