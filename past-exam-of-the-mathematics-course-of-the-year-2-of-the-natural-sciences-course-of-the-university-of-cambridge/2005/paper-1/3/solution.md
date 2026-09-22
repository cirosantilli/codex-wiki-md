<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the convention

$$
\widehat f(k)=\int_{\mathbb R}f(x)e^{-ikx}dx,\qquad f(x)=\frac1{2\pi}\int_{\mathbb R}\widehat f(k)e^{ikx}dk.
$$

These are the [Fourier transform](../../../../fourier-transform-split.md) and [inverse Fourier transform](../../../../inverse-fourier-transform.md) for suitably integrable data. Assuming the required ordinary transforms exist and the lower derivatives vanish at both ends, [integration by parts](../../../../integration-by-parts.md) gives $\widehat{g'}=[ge^{-ikx}]_{-\infty}^{\infty}+ik\widehat g=ik\widehat g$. Repeating this argument yields

$$
\boxed{\widehat{g^{(n)}}(k)=(ik)^n\widehat g(k).}
$$

The decay assumptions are used to discard the boundary terms at each step.

For positive diffusivity $\alpha$, transforming the [heat equation](../../../../heat-equation.md) gives $\partial_t\widehat f=-\alpha k^2\widehat f$. Thus $\widehat f(k,t)=e^{-\alpha k^2t}\widehat f_0(k)$, where $f_0(x)=f(x,0)$. The [convolution theorem](../../../../convolution-theorem.md) and the [Gaussian heat kernel](../../../../gaussian-heat-kernel.md) give

$$
\boxed{f(x,t)=\frac1{\sqrt{4\pi\alpha t}}\int_{\mathbb R}e^{-(x-\xi)^2/(4\alpha t)}f_0(\xi)\,d\xi,\qquad t>0.}
$$

For $f_0(x)=e^{-x^2}$, the [Fourier transform of a Gaussian](../../../../fourier-transform-of-a-gaussian.md) is $\sqrt\pi e^{-k^2/4}$. Multiplying by the heat factor and inverting gives the [Gaussian initial data for the heat equation](../../../../gaussian-initial-data-for-the-heat-equation.md) solution

$$
\boxed{f(x,t)=\frac1{\sqrt{1+4\alpha t}}\exp\left[-\frac{x^2}{1+4\alpha t}\right].}
$$

It recovers the initial profile as $t\downarrow0$ and preserves its spatial integral $\sqrt\pi$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
