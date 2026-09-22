# Convolution theorem

↑ **Parent:** [Convolution](convolution.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Convolution_theorem)

For [Lebesgue integrable functions](lebesgue-integrable-function.md) $f,g$ on $\mathbb R$, use the [Fourier transform](fourier-transform.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-2\pi ix\xi}\,dx$. Then

$$
\widehat{f*g}(\xi)=\widehat f(\xi)\widehat g(\xi).
$$

Thus the [integral](integral.md) combining all translated products becomes an ordinary multiplication at each [frequency](frequency.md). Different [Fourier transform](fourier-transform.md) normalizations can place a constant in this identity; fixing the convention prevents that ambiguity. Its use in filtering is illustrated by [Brad Osgood, Stanford EE261, Lecture 9, convolution and Fourier-domain filtering](https://see.stanford.edu/materials/lsoftaee261/transcripts/TheFourierTransformAndItsApplications-Lecture09.pdf).

For the [indicator function](indicator-function.md) $q=\mathbf1_{[0,1]}$,

$$
\widehat q(\xi)=e^{-\pi i\xi}\operatorname{sinc}(\xi),\qquad \operatorname{sinc}(\xi)=\frac{\sin(\pi\xi)}{\pi\xi},
$$

with $\operatorname{sinc}(0)=1$. Therefore the [triangular function](triangular-function.md) $q*q$ has [Fourier transform](fourier-transform.md) $e^{-2\pi i\xi}\operatorname{sinc}^2(\xi)$. The extra factor of the [sinc function](sinc-function.md) improves the large-frequency bound from a constant times $1/|\xi|$ to one times $1/|\xi|^2$, matching the smoother output in the overlap picture. [Fourier decay of repeated interval convolutions](fourier-decay-of-repeated-interval-convolutions.md) extends this calculation to further repetitions.

For a proof outline, [Fubini's theorem](fubini-s-theorem.md) permits exchanging the two [integrals](integral.md) because the integral of $|f(y)g(x-y)|$ over $(x,y)$ is $\|f\|_1\|g\|_1<\infty$. Set $u=x-y$ in the inner [integral](integral.md):

$$
\begin{aligned}
\widehat{f*g}(\xi)&=\int_{\mathbb R}\!\int_{\mathbb R}f(y)g(x-y)e^{-2\pi ix\xi}\,dy\,dx\\
&=\int_{\mathbb R}\!\int_{\mathbb R}f(y)g(u)e^{-2\pi i(y+u)\xi}\,du\,dy\\
&=\widehat f(\xi)\widehat g(\xi).
\end{aligned}
$$

The factorization of the [complex exponential](complex-exponential-function.md) is the mechanism behind the simplification. The [discrete convolution](discrete-convolution.md) version similarly turns coefficient sums into products of [generating functions](generating-function.md).

**Table of contents**

- [Exponential kernel convolved with an interval indicator](exponential-kernel-convolved-with-an-interval-indicator.md)
- [Gamma density from repeated exponential convolution](gamma-density-from-repeated-exponential-convolution.md)

## ↑ Ancestors (6)

1. [Convolution](convolution.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (34)

- [Convolution](convolution.md)
- [Convolution of distributions with a compactly supported factor](convolution-of-distributions-with-a-compactly-supported-factor.md)
- [Flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md)
- [Fourier analysis](fourier-analysis-split.md)
- [Fourier decay of repeated interval convolutions](fourier-decay-of-repeated-interval-convolutions.md)
- [Gaussian filtering Fourier multiplier](gaussian-filtering-fourier-multiplier.md)
- [Parametric-rate kernel estimation of a bandlimited density](parametric-rate-kernel-estimation-of-a-bandlimited-density.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/15d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-4/15d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/14d/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-1/14d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-2/30a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-30/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-69/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-4/15d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-82/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-67/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/14b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-3/20f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-2/4b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/40e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-2/14a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-4/12a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-4/26g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1/1a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-2/11f/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-3/14a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/14a/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-2/14b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-129/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/23h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/23h/d/i/solution.md)
