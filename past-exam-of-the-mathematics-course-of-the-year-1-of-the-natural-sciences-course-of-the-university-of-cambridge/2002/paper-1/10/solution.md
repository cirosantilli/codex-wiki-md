<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

Put $\tau=t+b$ and $q=x+a$. For $\theta=f(t)e^{-q^2/(4\tau)}$, [partial differentiation](../../../../partial-derivative.md) gives

$$
\theta_t=\left(f'+\frac{q^2f}{4\tau^2}\right)e^{-q^2/(4\tau)},\qquad \theta_{xx}=\left(-\frac f{2\tau}+\frac{q^2f}{4\tau^2}\right)e^{-q^2/(4\tau)}.
$$

The [heat equation](../../../../heat-equation.md) therefore requires $f'=-f/(2\tau)$, giving $f=C/\sqrt{|t+b|}$ on an interval not containing $-b$. A decaying spatial [Gaussian function](../../../../gaussian-function.md) uses $t+b>0$, so $f=C/\sqrt{t+b}$ there.

The initial profile is a difference of two translated [Gaussian functions](../../../../gaussian-function.md). Set $b=1/4$, $a=-2$ and $a=2$, with respective constants $C=1/2$ and $C=-1/2$. The [superposition principle](../../../../superposition-principle.md) gives

$$
\boxed{\theta(x,t)=\frac{e^{-(x-2)^2/(1+4t)}-e^{-(x+2)^2/(1+4t)}}{\sqrt{1+4t}},\qquad t\geq0.}
$$

This is an [odd pair of Gaussian profiles under diffusion](../../../../odd-pair-of-gaussian-profiles-under-diffusion.md), obtained from [Gaussian initial data for the heat equation](../../../../gaussian-initial-data-for-the-heat-equation.md). It is [odd](../../../../odd-function.md) in $x$, vanishes at zero, is positive for $x>0$ and negative for $x<0$. The two lobes broaden and decrease in height, and $\theta(x,t)\to0$ at every fixed $x$ as $t\to\infty$. Their extrema move; they do not remain exactly at $\pm2$.

<a id="10/image-diffusion-of-two-gaussian-profiles-with-opposite-signs"></a>
![](../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2002/paper-1-odd-gaussian-diffusion.png)

**[Figure 2](#10/image-diffusion-of-two-gaussian-profiles-with-opposite-signs). Diffusion of two Gaussian profiles with opposite signs**. Original plots at several times show the odd symmetry, decreasing amplitudes and widening lobes.

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 1 of the natural sciences course of the University of Cambridge](../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
