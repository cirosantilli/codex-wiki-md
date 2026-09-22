<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Transform convention and derivatives.** Use the [Fourier transform](../../../../fourier-transform-split.md) pair

$$
\boxed{\widetilde f(k)=\int_{-\infty}^{\infty}f(x)e^{-ikx}\,dx,\qquad f(x)=\frac1{2\pi}\int_{-\infty}^{\infty}\widetilde f(k)e^{ikx}\,dk.}
$$

For sufficiently decaying $f,f'$ with integrable second [derivative](../../../../derivative.md), two applications of [integration by parts](../../../../integration-by-parts.md) give

$$
\begin{aligned}
\widetilde{f''}(k)&=[f'e^{-ikx}]_{-\infty}^{\infty}+ik\int_{-\infty}^{\infty}f'e^{-ikx}\,dx\\
&=ik[f e^{-ikx}]_{-\infty}^{\infty}+(ik)^2\widetilde f(k)=\boxed{-k^2\widetilde f(k)}.
\end{aligned}
$$

The identity also holds for [tempered distributions](../../../../tempered-distribution.md), which is the setting needed for the [Dirac delta function](../../../../dirac-delta-function.md) boundary data.

**Upper half-plane solution.** Take the [Fourier transform](../../../../fourier-transform-split.md) in $x$ only, writing $\Phi(k,y)=\widetilde\phi(k,y)$. [Laplace's equation](../../../../laplace-equation.md) becomes $\Phi_{yy}-k^2\Phi=0$. For $k\ne0$, discard the exponentially growing solution and use $\Phi(k,0)=1$, the [Fourier transform](../../../../fourier-transform-split.md) of the [Dirac delta function](../../../../dirac-delta-function.md). This gives $\Phi(k,y)=e^{-|k|y}$. The value at $k=0$ can be set to its continuous limit one. Pointwise decay of $\phi$ as $y\to\infty$ does not require this individual transformed value to decay: the total integral in $x$ remains one while the profile spreads.

The inverse [Fourier transform](../../../../fourier-transform-split.md) now yields, for $y>0$,

$$
\phi(x,y)=\frac1{2\pi}\int_{-\infty}^{\infty}e^{-|k|y}e^{ikx}\,dk=\frac1\pi\int_0^\infty e^{-ky}\cos(kx)\,dk.
$$

Evaluate the last [integral](../../../../integral-split.md) as the real part of $\int_0^\infty e^{-(y-ix)k}\,dk=(y-ix)^{-1}$:

$$
\boxed{\phi(x,y)=\frac{y}{\pi(x^2+y^2)},\qquad y>0.}
$$

This is the [Poisson kernel for the upper half-plane](../../../../poisson-kernel-for-the-upper-half-plane.md). Its boundary condition is a [distributional convergence](../../../../weak-convergence-of-distributions.md), rather than an ordinary value at $(0,0)$: for a smooth compactly supported test [function](../../../../function-split.md) $g$,

$$
\int_{-\infty}^{\infty}\phi(x,y)g(x)\,dx=\frac1\pi\int_{-\infty}^{\infty}\frac{g(yt)}{1+t^2}\,dt\longrightarrow g(0).
$$

The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) applies because $g$ is bounded and $(1+t^2)^{-1}$ is integrable. Also $0\leq\phi(x,y)\leq1/(\pi y)$, proving the required decay as $y\to\infty$.

**Direct verification.** Differentiating the rational expression gives

$$
\phi_{xx}=\frac{2y(3x^2-y^2)}{\pi(x^2+y^2)^3},\qquad\phi_{yy}=\frac{2y(y^2-3x^2)}{\pi(x^2+y^2)^3}.
$$

Their sum is zero throughout $y>0$, so the solution is a [harmonic function](../../../../harmonic-function.md) there.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
