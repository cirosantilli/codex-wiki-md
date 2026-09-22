<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The zero [Fourier coefficient](../../../../../fourier-coefficient.md) is $u_0=0$. For a nonzero integer $r$, integrate the two constant halves:

$$
\begin{aligned}
u_r&=\frac{1\,\mathrm V}{4\,\mathrm s}\left[\int_0^{2\,\mathrm s}e^{-ir\omega t}\,dt-\int_{2\,\mathrm s}^{4\,\mathrm s}e^{-ir\omega t}\,dt\right]\\
&=\frac{1-(-1)^r}{i\pi r}\,\mathrm V.
\end{aligned}
$$

Consequently

$$
\boxed{u_0=0,\qquad
u_r=\begin{cases}-2i/(\pi r)\,\mathrm V,&r\text{ odd},\\0,&r\ne0\text{ even}.\end{cases}}
$$

The [complex Fourier series](../../../../../complex-fourier-series.md) is $g(t)\sim\sum_{r\in\mathbb Z}u_re^{ir\pi t/(2\,\mathrm s)}$. The negative-index coefficients are the [complex conjugates](../../../../../complex-conjugate.md) of the positive-index ones, as required for a real signal. Combining each pair gives the equivalent real expansion

$$
g(t)\sim\frac{4\,\mathrm V}{\pi}\sum_{j=0}^{\infty}\frac{\sin[(2j+1)\pi t/(2\,\mathrm s)]}{2j+1}.
$$

At a jump, [pointwise convergence of a piecewise smooth Fourier series](../../../../../pointwise-convergence-of-a-piecewise-smooth-fourier-series.md) gives zero, the average of the two one-sided limits. The value assigned to $g$ at isolated jumps does not affect its [Fourier coefficients](../../../../../fourier-coefficient.md) or [mean-square signal power](../../../../../signal-power.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 3](../../../paper-3-split.md)
4. [2024](../../../split.md)
5. [Past exam of the year 2 of the earth sciences (geology) course of the University of Oxford](../../../../split.md)
6. [Year 2 of the earth sciences (geology) course of the University of Oxford](../../../../../year-2-of-the-earth-sciences-geology-course-of-the-university-of-oxford.md)
7. [Earth sciences (geology) course of the University of Oxford](../../../../../earth-sciences-geology-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
