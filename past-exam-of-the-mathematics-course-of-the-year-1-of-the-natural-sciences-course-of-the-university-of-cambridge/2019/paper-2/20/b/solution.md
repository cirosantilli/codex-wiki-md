<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the Gaussian ansatz, [partial differentiation](../../../../../partial-derivative.md) gives

$$
T_t=(F'-x^2FH')e^{-x^2H},\qquad
T_{xx}=F(-2H+4x^2H^2)e^{-x^2H}.
$$

Cancel the positive exponential and compare the constant and quadratic powers of $x$ in the [diffusion equation](../../../../../diffusion-equation-split.md). The two coupled [ordinary differential equations](../../../../../ordinary-differential-equation.md) are

$$
\boxed{F'=-2\kappa FH,\qquad H'=-4\kappa H^2}.
$$

The initial profile requires $F(0)=T_0$ and $H(0)=L^{-2}$. The second equation is a [separable differential equation](../../../../../separable-differential-equation.md):

$$
\frac{d}{dt}\left(\frac1H\right)=4\kappa,
\qquad \boxed{H(t)=\frac1{L^2+4\kappa t}}.
$$

Substitute this into the first equation and integrate its [logarithmic derivative](../../../../../logarithmic-derivative.md):

$$
\ln\frac{F(t)}{T_0}=-2\kappa\int_0^t\frac{ds}{L^2+4\kappa s}
=-\frac12\ln\frac{L^2+4\kappa t}{L^2}.
$$

Thus

$$
\boxed{F(t)=\frac{T_0L}{\sqrt{L^2+4\kappa t}}},
$$

and the solution is

$$
\boxed{T(x,t)=\frac{T_0L}{\sqrt{L^2+4\kappa t}}\exp\left[-\frac{x^2}{L^2+4\kappa t}\right]},\qquad t\geq0.
$$

This is [Gaussian diffusion of a smooth initial profile](../../../../../gaussian-diffusion-of-a-smooth-initial-profile.md): its width grows while its peak decreases. The [Gaussian integral](../../../../../gaussian-integral.md) gives $\int_{-\infty}^{\infty}T(x,t)\,dx=\sqrt\pi T_0L$, independent of time, which checks conservation of the total amount under the [diffusion equation](../../../../../diffusion-equation-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
