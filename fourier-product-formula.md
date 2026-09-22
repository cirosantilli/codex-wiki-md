# Fourier product formula

↑ **Parent:** [Convolution theorem](convolution-theorem.md)

For [Schwartz functions](schwartz-function.md) $f,g$ and the [Fourier transform](fourier-transform-split.md) convention $\widehat f(\xi)=\int f(x)e^{-ix\xi}\,dx$, the displayed formula exchanges a pointwise product for a [convolution](convolution.md). Substitute [Fourier inversion](fourier-inversion-theorem.md) for $g$ into the [Fourier transform](fourier-transform-split.md) of $fg$. [Fubini's theorem](fubini-s-theorem.md), justified by $\|f\|_1\|\widehat g\|_1<\infty$, gives

$$
\widehat{fg}(\xi)=\frac1{2\pi}\int\widehat g(\eta)\widehat f(\xi-\eta)\,d\eta.
$$

Unlike the [convolution theorem](convolution-theorem.md) $\widehat{f*g}=\widehat f\widehat g$, this version cannot be asserted for arbitrary pairs in $L^1$ without additional hypotheses, since their pointwise product need not be an [integrable function](lebesgue-integrable-function.md).

## ↑ Ancestors (7)

1. [Convolution theorem](convolution-theorem.md)
2. [Convolution](convolution.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-fourier-analysis-course-of-the-university-of-oxford/2023/1/a/i/solution.md)
