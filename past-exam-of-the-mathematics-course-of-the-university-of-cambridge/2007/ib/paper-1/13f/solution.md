<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Integrate the entire function $e^{iz^2}$ around the positively oriented sector boundary: the real segment $0\to R$, the arc $Re^{i\theta}$ for $0\leq\theta\leq\pi/4$, and the radial segment back to zero. [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) gives

$$
\int_0^Re^{ix^2}\,dx+\int_{\mathrm{arc}}e^{iz^2}\,dz
-e^{i\pi/4}\int_0^Re^{-r^2}\,dr=0.
$$

The last term follows from $z=re^{i\pi/4}$ and $iz^2=-r^2$; its minus sign is the return orientation.

On the arc, $|e^{iz^2}|=e^{-R^2\sin(2\theta)}$. The supplied sine bound gives $\sin(2\theta)\geq4\theta/\pi$ throughout this sector, so

$$
\left|\int_{\mathrm{arc}}e^{iz^2}\,dz\right|
\leq R\int_0^{\pi/4}e^{-4R^2\theta/\pi}\,d\theta
=\frac\pi{4R}(1-e^{-R^2})\longrightarrow0.
$$

The Gaussian integral then yields $\int_0^\infty e^{ix^2}\,dx=e^{i\pi/4}\sqrt\pi/2$. Taking real and imaginary parts proves **both [Fresnel integrals](../../../../../fresnel-integral.md)**:

$$
\boxed{\int_0^\infty\cos x^2\,dx=\int_0^\infty\sin x^2\,dx=\sqrt{\frac\pi8}.}
$$

The contour estimate proves existence of the improper oscillatory integrals as well as their values; absolute convergence is neither asserted nor required.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
