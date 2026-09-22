<h1 id="14e/solution">Solution</h1>

↑ **Parent:** [14E](../14e.md)

The [Fourier coefficients](../../../../../fourier-coefficient.md) satisfy $a_0=a_n=0$ and

$$
b_n=\frac1\pi\left(\int_0^\pi\sin(n\theta)\,d\theta-\int_\pi^{2\pi}\sin(n\theta)\,d\theta\right)
=\frac{2[1-(-1)^n]}{\pi n}.
$$

Thus the [square wave](../../../../../square-wave.md) has [Fourier series](../../../../../fourier-series-split.md)

$$
\boxed{f(\theta)\sim\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac{\sin(n\theta)}n}.
$$

It equals $f$ away from its [jump discontinuities](../../../../../jump-discontinuity.md), and converges to $0$ at the jumps. The assigned endpoint values do not affect its [Fourier coefficients](../../../../../fourier-coefficient.md).

For the [Poisson equation](../../../../../poisson-equation.md), use [separation of variables](../../../../../separation-of-variables.md) $\phi=\sum_{n\text{ odd}}b_nR_n(r)\sin(n\theta)$. The radial equation is $r^2R_n''+rR_n'-n^2R_n=r^2$. Its bounded solution with zero [Dirichlet boundary condition](../../../../../dirichlet-boundary-condition.md) at $r=1$ is

$$
R_n(r)=\frac{r^n-r^2}{n^2-4}.
$$

Indeed the negative power is excluded at the centre, and the boundary fixes the coefficient of $r^n$. No resonance at $n=2$ occurs because only odd modes are forced. Therefore

$$
\boxed{\phi(r,\theta)=\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}
\frac{r^n-r^2}{n(n^2-4)}\sin(n\theta)}.
$$

This is a [Poisson equation on a disk with angular forcing](../../../../../poisson-equation-on-a-disk-with-angular-forcing.md). The series converges uniformly on the closed disk: for $n\ge3$ each term is bounded by a constant times $n^{-3}$. Its first spatial derivatives also converge uniformly. For instance the radial derivative and $r^{-1}$ times the angular derivative of each term are bounded by constants times $n^{-2}$; the $n=1$ harmonic term is smooth in Cartesian coordinates. It defines a function with zero boundary data and the required [weak formulation](../../../../../weak-formulation.md). Applying the [Laplacian](../../../../../laplacian.md) to finite partial sums gives the [Fourier partial sums](../../../../../fourier-partial-sum.md) of $f$, which converge in $L^2$; passing to the limit against smooth compactly supported test functions verifies the [Poisson equation](../../../../../poisson-equation.md). It holds classically off the jump rays and the centre, where the forcing is locally constant. It cannot be interpreted as a global classical equation with continuous second derivatives for discontinuous forcing. Uniqueness follows from the zero-boundary [Dirichlet energy](../../../../../dirichlet-energy.md) identity for the difference of two solutions.

Finally [orthogonality](../../../../../orthogonal-vectors.md) gives $\int_0^{2\pi}f(\theta)\sin(n\theta)\,d\theta=\pi b_n$. The radial integral is

$$
\int_0^1R_n(r)r\,dr
=\frac{1}{n^2-4}\left(\frac1{n+2}-\frac14\right)
=-\frac1{4(n+2)^2}.
$$

Uniform convergence of $\phi$ and boundedness of $f$ justify integration term by term, so

$$
\boxed{\int_{r\le1}f\phi\,dA
=-\frac4\pi\sum_{\substack{n\ge1\\n\text{ odd}}}\frac1{n^2(n+2)^2}}.
$$

The negative sign also agrees with $\int\phi\Delta\phi=-\int|\nabla\phi|^2$. The original PDF's radial denominator is $n^2-4$; the converted TeX's $n^2-1$ is a transcription error.

## ↑ Ancestors (10)

1. [14E](../14e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
