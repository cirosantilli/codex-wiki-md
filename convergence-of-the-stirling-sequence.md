# Convergence of the Stirling sequence

↑ **Parent:** [Stirling formula](stirling-formula.md)

The positive [sequence](sequence.md) $a_n=\sqrt n(n/e)^n/n!$ has logarithmic increments

$$
u_n=\ln\frac{a_{n+1}}{a_n}=\left(n+\frac12\right)\ln\left(1+\frac1n\right)-1.
$$

The [rational lower bound for the natural logarithm](rational-lower-bound-for-the-natural-logarithm.md) proves $u_n>0$. For $n>1$, the [Taylor series](taylor-series.md) gives

$$
u_n=\sum_{k=2}^{\infty}\frac{(-1)^k}{n^k}\frac{k-1}{2k(k+1)}.
$$

Since $0<(k-1)/[2k(k+1)]<1/2$, a [geometric series](geometric-series.md) bounds $u_n<1/[2n(n-1)]\leq n^{-2}$ for $n\geq2$. The [comparison test for series](comparison-test-for-series.md) therefore proves $\sum u_n<\infty$. The finite [telescoping sum](telescoping-sum.md) $\ln a_{n+1}=-1+\sum_{k=1}^n u_k$ shows that $a_n$ increases to a finite positive [limit](limit-of-a-function.md). This argument establishes the existence of the constant in [Stirling's formula](stirling-formula.md); its value $1/\sqrt{2\pi}$ requires an independent identification.

## ↑ Ancestors (8)

1. [Stirling formula](stirling-formula.md)
2. [Asymptotic equivalence](asymptotic-equivalence.md)
3. [Asymptotic analysis](asymptotic-analysis.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/19/f/solution.md)
