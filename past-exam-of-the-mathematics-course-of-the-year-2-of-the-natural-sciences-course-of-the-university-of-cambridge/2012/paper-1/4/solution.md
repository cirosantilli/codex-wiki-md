<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Complete the square in the [Fourier transform](../../../../fourier-transform-split.md) exponent:

$$
-\lambda x^2-ikx=-\lambda\left(x+\frac{ik}{2\lambda}\right)^2-\frac{k^2}{4\lambda}.
$$

The supplied shifted [Gaussian integral](../../../../gaussian-integral.md) therefore gives

$$
\boxed{\widehat f(k)=\sqrt{\frac\pi\lambda}\exp\left(-\frac{k^2}{4\lambda}\right).}
$$

This is the [Fourier transform of a Gaussian](../../../../fourier-transform-of-a-gaussian.md), with angular-wavenumber convention $e^{-ikx}$.

Take the spatial [Fourier transform](../../../../fourier-transform-split.md) of the [heat equation](../../../../heat-equation.md). Two [integrations by parts](../../../../integration-by-parts.md), with decaying fields and first derivatives at infinity, give $\mathcal F[\psi_{xx}]=-k^2\widetilde\psi$. Thus each mode satisfies the [ordinary differential equation](../../../../ordinary-differential-equation.md)

$$
\boxed{\partial_t\widetilde\psi(k,t)=-k^2\widetilde\psi(k,t).}
$$

Inserting the transformed [initial condition](../../../../initial-condition.md) and integrating the time equation gives

$$
\boxed{\widetilde\psi(k,t)=\sqrt{\frac\pi\lambda}\exp\left[-\left(t+\frac1{4\lambda}\right)k^2\right].}
$$

Finally set $A=t+1/(4\lambda)>0$. The [inverse Fourier transform](../../../../inverse-fourier-transform.md), evaluated by the same Gaussian identity, gives

$$
\begin{aligned}
\psi(x,t)&=\frac1{2\pi}\sqrt{\frac\pi\lambda}\int_{-\infty}^{\infty}e^{-Ak^2+ikx}dk\\
&=\frac1{2\sqrt{\lambda A}}e^{-x^2/(4A)}.
\end{aligned}
$$

Equivalently the [Gaussian initial data for the heat equation](../../../../gaussian-initial-data-for-the-heat-equation.md) evolve as

$$
\boxed{\psi(x,t)=\frac1{\sqrt{1+4\lambda t}}\exp\left[-\frac{\lambda x^2}{1+4\lambda t}\right],\qquad t>0.}
$$

The profile broadens and its peak decreases, while its total [integral](../../../../integral-split.md) remains $\sqrt{\pi/\lambda}$, as required by [diffusion](../../../../diffusion.md) without loss on the whole line. Direct differentiation verifies the equation and the initial limit.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
