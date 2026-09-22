<h1 id="gaussian-peak-behind-stirling-s-formula">Gaussian peak behind Stirling's formula</h1>

↑ **Parent:** [Stirling formula](stirling-formula.md)

Repeated [integration by parts](integration-by-parts.md) gives the [Gamma integral](gamma-integral.md)

$$
n!=\int_0^\infty t^n e^{-t}\,dt.
$$

The logarithm of its integrand is $n\log t-t$, whose unique maximum is at $t=n$. Write $t=n+\sqrt n\,s$. For fixed $s$ and large $n$, a [Taylor expansion](taylor-expansion.md) gives

$$
n\log\left(1+\frac{s}{\sqrt n}\right)-s\sqrt n
=-\frac{s^2}{2}+\frac{s^3}{3\sqrt n}+O(n^{-1}).
$$

The [Big O notation](big-o-notation.md) here is for a fixed $s$, or uniformly for $s$ in a fixed bounded interval. It does not claim a uniform approximation over the entire growing integration domain. Consequently the peak, divided by its height, approaches $e^{-s^2/2}$.

<a id="image-the-peak-of-a-factorial-integral-approaches-a-gaussian-after-recentering-and-rescaling"></a>
![](stirling-gamma-gaussian-peak.png)

**[Figure 9](#image-the-peak-of-a-factorial-integral-approaches-a-gaussian-after-recentering-and-rescaling). The peak of a factorial integral approaches a Gaussian after recentering and rescaling**. The plotted functions are $K_n(s)=\exp(n\log(1+s/\sqrt n)-s\sqrt n)$ for $s>-\sqrt n$, with zero outside their domains. Each has peak height one. They are rescaled integrands, not normalized [probability density functions](probability-density-function.md).

The exact substitution gives

$$
n!=n^n e^{-n}\sqrt n\int_{-\sqrt n}^{\infty}
\exp\left(n\log\left(1+\frac{s}{\sqrt n}\right)-s\sqrt n\right)\,ds.
$$

Replacing the integral by the [Gaussian integral](gaussian-integral.md) $\int_{\mathbb R}e^{-s^2/2}\,ds=\sqrt{2\pi}$ produces $S_n$. Thus the estimate is peak height $n^ne^{-n}$ times width $\sqrt n$ times the area of a standard Gaussian peak. This is [Laplace's method](laplace-s-method.md) in a concrete form; controlling the integral's tails justifies the replacement. The next terms, including their products after exponentiation, produce the [Stirling correction by Gaussian moments](stirling-correction-by-gaussian-moments.md).

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

- [Stirling formula](stirling-formula.md)
