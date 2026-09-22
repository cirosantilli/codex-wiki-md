<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

By the definition of [convolution](../../../../../../convolution.md) and [Fourier inversion](../../../../../../fourier-inversion-theorem.md),

$$
\begin{aligned}
\mathcal F^{-1}(\widetilde f*\widetilde g)(t)
&=\frac1{2\pi}\int_{\mathbb R}\int_{\mathbb R}\widetilde f(\eta)\widetilde g(\omega-\eta)e^{i\omega t}\,d\eta\,d\omega\\
&=\frac1{2\pi}\left[\int_{\mathbb R}\widetilde f(\eta)e^{i\eta t}d\eta\right]\left[\int_{\mathbb R}\widetilde g(\nu)e^{i\nu t}d\nu\right]\\
&=\boxed{2\pi f(t)g(t)}.
\end{aligned}
$$

The second line uses $\nu=\omega-\eta$. The factor $2\pi$ comes from the inverse-transform normalization. This is the product form of the [convolution theorem](../../../../../../convolution-theorem.md), initially justified for sufficiently decaying functions and extended when the indicated products and convolutions exist.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
