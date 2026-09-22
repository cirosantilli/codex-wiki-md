<h1 id="8b/solution">Solution</h1>

↑ **Parent:** [8B](../8b.md)

First suppose the integral of $g(\xi)/(\xi-z)$ converges, for example if $g\in L^1(\mathbb R)$. Substitute the complexified coordinates $x=(z+\bar a)/2$, $y=(z-\bar a)/(2i)$ into the [Poisson integral](../../../../../poisson-integral.md). The factorization of its denominator gives

$$
2u\!\left(\frac{z+\bar a}{2},\frac{z-\bar a}{2i}\right)=\frac1{i\pi}\int_{\mathbb R}g(\xi)\left(\frac1{\xi-z}-\frac1{\xi-\bar a}\right)d\xi.
$$

The given [Schwarz integral formula](../../../../../schwarz-integral-formula.md) therefore writes $f(z)$ as $(i\pi)^{-1}\int g(\xi)/(\xi-z)\,d\xi$ plus a constant. For $z=x+iy$, the real part of this integral is exactly the [Poisson integral](../../../../../poisson-integral.md), since

$$
\operatorname{Re}\frac1{i(\xi-z)}=\frac{y}{(\xi-x)^2+y^2}.
$$

The remaining constant has zero real part, giving $\boxed{f(z)=(i\pi)^{-1}\int_{\mathbb R}\frac{g(\xi)}{\xi-z}\,d\xi+ic}$ with $c\in\mathbb R$. The complex substitution is initially understood where the real-analytic harmonic function has its complexification; the holomorphic integral then continues the identity throughout the upper half-plane.

**Decay of $u$ alone does not guarantee convergence of the printed unregularized integral.** For example, choose a continuous $g$ which vanishes on $(-\infty,e]$ and equals $1/\log\xi$ for $\xi\ge e^2$, with continuous interpolation. It is bounded and tends to zero at both ends. Its [Poisson integral](../../../../../poisson-integral.md) tends to zero as $|z|\to\infty$ in the closed upper half-plane: split the boundary function into a small uniform tail and a compactly supported part. Nevertheless $\int^\infty g(\xi)/(\xi-z)\,d\xi$ diverges like $\log\log\xi$, even as a symmetric principal value. With only the stated decay assumptions, the always convergent version is

$$
\boxed{f(z)=\frac1{i\pi}\int_{\mathbb R}g(\xi)\left(\frac1{\xi-z}-\frac{\xi}{1+\xi^2}\right)d\xi+ic.}
$$

The subtracted kernel is real on the integration line, so it changes only the imaginary constant and leaves the [harmonic function](../../../../../harmonic-function.md) $u$ unchanged. The kernel difference is $O(\xi^{-2})$, which ensures convergence for bounded $g$.

## ↑ Ancestors (10)

1. [8B](../8b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
