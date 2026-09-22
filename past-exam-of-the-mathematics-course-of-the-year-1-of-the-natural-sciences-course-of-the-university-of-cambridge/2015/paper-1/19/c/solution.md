<h1 id="19/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a_n=\ln[1+(-1)^n/n]$ and $S_N=\sum_{n=2}^Na_n$. Consecutive even and odd terms cancel exactly:

$$
a_{2j}=\ln\frac{2j+1}{2j},\qquad
a_{2j+1}=\ln\frac{2j}{2j+1}=-a_{2j}.
$$

Thus

$$
S_{2m+1}=0,\qquad S_{2m}=\ln\frac{2m+1}{2m}\longrightarrow0.
$$

Both parity subsequences have the same limit, so the full sequence of [partial sums](../../../../../partial-sum.md) converges and the sum is **zero**. This check is necessary: cancellation in fixed pairs alone does not always prove convergence of the original series.

For [absolute convergence](../../../../../absolute-convergence.md), each pair instead contributes

$$
|a_{2j}|+|a_{2j+1}|=2\ln\left(1+\frac1{2j}\right)
\geq\frac{2}{2j+1}.
$$

The inequality follows from $\ln(1+u)=\int_0^u(1+s)^{-1}ds\geq u/(1+u)$. The lower-bound series diverges by comparison with the [harmonic series](../../../../../harmonic-series.md). Therefore the [paired logarithmic series with zero sum](../../../../../paired-logarithmic-series-with-zero-sum.md) has

$$
\boxed{\text{conditional convergence, but not absolute convergence}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [19](../../19.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
