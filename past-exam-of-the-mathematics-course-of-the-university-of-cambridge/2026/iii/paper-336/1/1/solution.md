<h1 id="1/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write the [Schläfli contour integral for Legendre polynomials](../../../../../../schlafli-contour-integral-for-legendre-polynomials.md) as

$$
P_n(\mu)=\frac1{2\pi i}\oint
\frac{e^{n\phi(z)}}{2^{n}(z-\mu)}\,dz,
\qquad
\phi(z)=\log\frac{z^2-1}{z-\mu}.
$$

The [saddle points](../../../../../../saddle-point.md) satisfy

$$
\phi'(z)=\frac{2z}{z^2-1}-\frac1{z-\mu}=0,
\qquad
z^2-2\mu z+1=0.
$$

For $\mu=\cos\theta$, they are $z_\pm=e^{\pm i\theta}$. Deforming the contour through both conjugate saddles and using the local Gaussian contributions from the [method of steepest descent](../../../../../../method-of-steepest-descent.md) gives conjugate exponentials. Their sum is the [Debye asymptotic for Legendre polynomials](../../../../../../debye-asymptotic-for-legendre-polynomials.md)

$$
\boxed{
P_n(\cos\theta)
\sim
\sqrt{\frac{2}{\pi n\sin\theta}}
\cos\left[\left(n+\frac12\right)\theta-\frac\pi4\right]}.
$$

Both saddles are required for the real oscillatory answer.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
