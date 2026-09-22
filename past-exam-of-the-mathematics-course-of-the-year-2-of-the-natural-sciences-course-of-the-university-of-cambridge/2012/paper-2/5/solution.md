<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For integrable $f,g$, define their [convolution](../../../../convolution.md) by $(f*g)(x)=\int_{\mathbb R}f(y)g(x-y)dy$. Absolute integrability of the double integral permits [Fubini's theorem](../../../../fubini-s-theorem.md). With $s=x-y$,

$$
\begin{aligned}
\mathcal F[f*g](k)&=\int_{\mathbb R}\!\int_{\mathbb R}e^{-ikx}f(y)g(x-y)dy\,dx\\
&=\int_{\mathbb R}f(y)e^{-iky}dy\int_{\mathbb R}g(s)e^{-iks}ds=\widetilde f(k)\widetilde g(k).
\end{aligned}
$$

The [convolution theorem](../../../../convolution-theorem.md), together with uniqueness of the [Fourier transform](../../../../fourier-transform-split.md), therefore identifies the inverse transform of that product with $f*g$. With the stated convention the inverse carries $1/(2\pi)$, so there is no extra factor in the convolution itself.

Now take $f=e^{-|x|}$. For $x\geq0$, split the convolution at $y=0$ and $y=x$:

$$
\begin{aligned}
h(x)&=\int_{-\infty}^0e^{2y-x}dy+\int_0^xe^{-x}dy+\int_x^\infty e^{x-2y}dy\\
&=\frac12e^{-x}+xe^{-x}+\frac12e^{-x}=(1+x)e^{-x}.
\end{aligned}
$$

The convolution of two even functions is even, so the [self-convolution of a bilateral exponential](../../../../self-convolution-of-a-bilateral-exponential.md) gives

$$
\boxed{h(x)=(1+|x|)e^{-|x|}=\begin{cases}(1-x)e^x,&x<0,\\1,&x=0,\\(1+x)e^{-x},&x>0.\end{cases}}
$$

In particular the centre value is one; both pieces extend continuously there.

Splitting the Fourier integral at zero gives

$$
\widetilde f(k)=\int_0^\infty e^{-(1+ik)x}dx+\int_0^\infty e^{-(1-ik)x}dx=\frac2{1+k^2}.
$$

Hence $\widetilde h(k)=4/(1+k^2)^2$. The [Fourier inversion theorem](../../../../fourier-inversion-theorem.md) yields

$$
\boxed{h(x)=\frac2\pi\int_{-\infty}^{\infty}\frac{e^{ikx}}{(1+k^2)^2}dk.}
$$

The integral is absolutely convergent. At $x=0$ it gives $\int_{\mathbb R}(1+k^2)^{-2}dk=\pi/2$, providing a normalization check.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Paper 2](../../paper-2-split.md)
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
