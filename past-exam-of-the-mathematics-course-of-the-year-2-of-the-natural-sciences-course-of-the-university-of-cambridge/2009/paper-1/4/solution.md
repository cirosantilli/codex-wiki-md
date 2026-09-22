<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Choose the [Fourier transform](../../../../fourier-transform-split.md) convention $\widehat f(k)=\int_{\mathbb R}e^{-ikx}f(x)dx$, with inverse $(2\pi)^{-1}\int e^{ikx}\widehat f(k)dk$. For absolutely integrable $f_1,f_2$, [Fubini's theorem](../../../../fubini-s-theorem.md) permits the substitution $s=x-y$ in the convolution transform:

$$
\begin{aligned}
\widehat{f_1*f_2}(k)
&=\int_{\mathbb R}\int_{\mathbb R}e^{-ikx}f_1(y)f_2(x-y)dy\,dx\\
&=\left[\int_{\mathbb R}e^{-iky}f_1(y)dy\right]\left[\int_{\mathbb R}e^{-iks}f_2(s)ds\right].
\end{aligned}
$$

This proves the [convolution theorem](../../../../convolution-theorem.md) in the chosen convention.

Take $q(x)=\tfrac12e^{-|x|}$. Splitting its transform at zero gives $\widehat q(k)=\tfrac12[(1+ik)^{-1}+(1-ik)^{-1}]=(1+k^2)^{-1}$. Thus the desired inverse is $q*q$. For $x\geq0$, split the convolution integral at $y=0$ and $y=x$:

$$
(q*q)(x)=\frac14\left[\frac{e^{-x}}2+xe^{-x}+\frac{e^{-x}}2\right]=\frac14(1+x)e^{-x}.
$$

The result is even, so

$$
\boxed{\mathcal F^{-1}\!\left[\frac1{(1+k^2)^2}\right](x)=\frac14(1+|x|)e^{-|x|}.}
$$

Different normalization conventions alter the transform prefactors, which is why the convention was stated explicitly.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2009](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
