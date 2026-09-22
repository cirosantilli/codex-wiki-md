<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For integrable functions $u,v$, the [convolution theorem](../../../../convolution-theorem.md) in the chosen convention is

$$
\widehat{u*v}(s)=\widehat u(s)\widehat v(s),\qquad (u*v)(x)=\int_{\mathbb R}u(x-t)v(t)\,dt.
$$

Let $F(s,y)$ be the [Fourier transform](../../../../fourier-transform-split.md) of $f(\cdot,y)$ in the horizontal coordinate. Transforming [Laplace's equation](../../../../laplace-equation.md) gives

$$
F_{yy}-s^2F=0,\qquad F(s,0)=\frac2{1+s^2}.
$$

For $s\ne0$, exclude the growing exponential and obtain $F(s,y)=2e^{-|s|y}/(1+s^2)$. At $s=0$, continuity in frequency gives $F(0,y)=2$; a constant zero-frequency transform is compatible with spatial decay of $f$.

By the transform pair in part (a), the inverse transform of $e^{-|s|y}$ is the [Poisson kernel for the upper half-plane](../../../../poisson-kernel-for-the-upper-half-plane.md), $P_y(x)=y/[\pi(x^2+y^2)]$. Thus

$$
\boxed{f(x,y)=(P_y*e^{-|\cdot|})(x)=\frac y\pi\int_{\mathbb R}\frac{e^{-|t|}}{(x-t)^2+y^2}\,dt\quad(y>0).}
$$

The [Poisson extension of exponential boundary data](../../../../poisson-extension-of-exponential-boundary-data.md) is harmonic, approaches the continuous boundary data and decays at spatial infinity. For uniqueness, apply the [maximum principle for harmonic functions](../../../../maximum-principle-for-harmonic-functions.md) to the difference of two solutions on increasingly large half-discs: it is zero on the real boundary and uniformly small on the distant semicircle.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
