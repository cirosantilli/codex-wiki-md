<h1 id="section-b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

Use the real [Fourier series](../../../../../fourier-series-split.md) convention $f(x)\sim a_0/2+\sum_{n\geq1}[a_n\cos(n\pi x)+b_n\sin(n\pi x)]$ for period two. The [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
a_0=\int_0^1 2x\,dx=1,\quad a_n=\int_0^1 2x\cos(n\pi x)\,dx=\frac{2[(-1)^n-1]}{n^2\pi^2},\quad b_n=\int_0^1 2x\sin(n\pi x)\,dx=\frac{2(-1)^{n+1}}{n\pi}.
$$

The last two [integrals](../../../../../integral-split.md) follow by [integration by parts](../../../../../integration-by-parts.md). Thus the [Fourier series of a half-wave rectified ramp](../../../../../fourier-series-of-a-half-wave-rectified-ramp.md) is

$$
f(x)\sim\frac12-\frac4{\pi^2}\sum_{r=0}^\infty\frac{\cos((2r+1)\pi x)}{(2r+1)^2}+\frac2\pi\sum_{n=1}^\infty\frac{(-1)^{n+1}}n\sin(n\pi x).
$$

On $(-1,1)$, $f(x)=|x|+x$. Its [even](../../../../../even-function.md) part is $f_e(x)=|x|$ and its [odd](../../../../../odd-function.md) part is $f_o(x)=x$, so the cosine and sine terms separate:

$$
\boxed{f_e(x)=\frac12-\frac4{\pi^2}\sum_{r=0}^\infty\frac{\cos((2r+1)\pi x)}{(2r+1)^2},\qquad f_o(x)=\frac2\pi\sum_{n=1}^\infty\frac{(-1)^{n+1}}n\sin(n\pi x).}
$$

At a jump, the [Fourier series](../../../../../fourier-series-split.md) converges to the average of the one-sided limits. Thus the first series for $f$ takes the value $1$ at odd integers, while the [Fourier series of a periodic sawtooth](../../../../../fourier-series-of-a-periodic-sawtooth.md) for $f_o$ takes the value $0$ there. The even function has a continuous periodic extension.

At $x=0$, the formula for $f_e$ gives $0=1/2-(4/\pi^2)\sum_{r\geq0}(2r+1)^{-2}$. At $x=1/2$, the formula for $f_o$ has only odd-index terms and gives $1/2=(2/\pi)\sum_{r\geq0}(-1)^r/(2r+1)$. Hence

$$
\boxed{\sum_{r=0}^\infty\frac1{(2r+1)^2}=\frac{\pi^2}{8},\qquad\sum_{r=0}^\infty\frac{(-1)^r}{2r+1}=\frac\pi4.}
$$

## ↑ Ancestors (13)

1. [8](../8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
