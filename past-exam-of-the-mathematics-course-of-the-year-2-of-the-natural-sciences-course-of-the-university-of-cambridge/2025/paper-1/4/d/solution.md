<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [Translation property of the Fourier transform](../../../../../translation-property-of-the-fourier-transform.md) gives

$$
\begin{aligned}
\widetilde r(k)&=\widetilde u(k)\sum_{n=1}^4e^{ik(4n-10)}\\
&=\frac{4\sin^2k}{k^2}\left(e^{-6ik}+e^{-2ik}+e^{2ik}+e^{6ik}\right)\\
&=\boxed{\frac{16\sin^2k}{k^2}\cos(4k)\cos(2k)},\qquad \boxed{\widetilde r(0)=16}.
\end{aligned}
$$

For the remaining [integral](../../../../../integral-split.md), the same [Translation property of the Fourier transform](../../../../../translation-property-of-the-fourier-transform.md) identifies $e^{20ik'}\widetilde g(k')$ as the [Fourier transform](../../../../../fourier-transform-split.md) of $g(x+20)$. By the product form of the [convolution theorem](../../../../../convolution-theorem.md), with inverse normalization $1/(2\pi)$,

$$
\int_{\mathbb R}e^{20ik'}\widetilde g(k')\widetilde r(k-k')\,dk'=2\pi\,\mathcal F\{g(x+20)r(x)\}(k).
$$

But $g(x+20)$ is supported in $[-21,-19]$, whereas the four translated [triangular functions](../../../../../triangular-function.md) making up $r$ are all supported in $[-8,8]$. Their product is identically zero. Therefore the requested [integral](../../../../../integral-split.md) is $\boxed{0}$ for every real $k$.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
