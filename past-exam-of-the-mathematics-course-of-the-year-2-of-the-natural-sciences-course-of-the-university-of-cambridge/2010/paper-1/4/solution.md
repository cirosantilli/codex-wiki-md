<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Split the [Fourier transform](../../../../fourier-transform-split.md) integral at zero:

$$
\boxed{\widehat g(k)=\int_0^\infty e^{-(\lambda+ik)x}dx+\int_0^\infty e^{-(\lambda-ik)x}dx=\frac{2\lambda}{\lambda^2+k^2}.}
$$

By [Fourier inversion](../../../../fourier-inversion-theorem.md) applied to this pair, or by the [residue theorem](../../../../residue-theorem.md), the other transform is

$$
\boxed{\widehat h(k)=\frac\pi\mu e^{-\mu|k|}.}
$$

For example, inversion with $\lambda=\mu$ gives $\int e^{ikx}(k^2+\mu^2)^{-1}dk=(\pi/\mu)e^{-\mu|x|}$; evenness supplies the desired sign convention.

Take the spatial [Fourier transform](../../../../fourier-transform-split.md) of the [Laplace equation](../../../../laplace-equation.md). For $y>0$ it gives $\widehat\psi_{yy}-k^2\widehat\psi=0$. Removing the exponentially growing solution and matching the boundary gives

$$
\widehat\psi(k,y)=\widehat f(k)e^{-|k|y}.
$$

At $k=0$ this formula is interpreted by continuity; a single transform value does not alter the inverse integral. The previous transform pair identifies

$$
\mathcal F^{-1}[e^{-|k|y}](x)=\frac1\pi\frac{y}{x^2+y^2}=P_y(x),
$$

the [Poisson kernel for the upper half-plane](../../../../poisson-kernel-for-the-upper-half-plane.md). The [convolution theorem](../../../../convolution-theorem.md) therefore gives the [Poisson integral](../../../../poisson-integral.md)

$$
\boxed{\psi(x,y)=\frac y\pi\int_{\mathbb R}\frac{f(u)}{(x-u)^2+y^2}du.}
$$

This is the bounded harmonic solution for bounded decaying data, or the corresponding solution in an appropriate Fourier class. Such a growth condition matters if vertical decay is interpreted only pointwise: the nonzero [harmonic function](../../../../harmonic-function.md) $e^{x^2-y^2}\sin(2xy)=\operatorname{Im}e^{(x+iy)^2}$ vanishes on the real axis and tends to zero for fixed $x$ as $y\to\infty$, but grows rapidly in $x$ and has no ordinary spatial [Fourier transform](../../../../fourier-transform-split.md). It can be excluded by requiring boundedness; the stated pointwise limits alone would not establish uniqueness.

For the interval data, direct integration gives the [Poisson extension of interval boundary data](../../../../poisson-extension-of-interval-boundary-data.md)

$$
\boxed{\psi(x,y)=\frac c\pi\left[\arctan\frac{a-x}{y}+\arctan\frac{a+x}{y}\right],\qquad y>0.}
$$

As $y\downarrow0$ it approaches $c$ for $|x|<a$, zero for $|x|>a$, and $c/2$ at $x=\pm a$. At those jump points the prescribed isolated values cannot be attained by a continuous extension; they do not affect the integral. The solution decays vertically, with $\psi\sim2ac/(\pi y)$ for fixed $x$ and large $y$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
