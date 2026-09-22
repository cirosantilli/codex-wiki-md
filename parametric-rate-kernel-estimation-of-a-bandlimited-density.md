# Parametric-rate kernel estimation of a bandlimited density

↑ **Parent:** [Flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md)

Let a bounded [probability density function](probability-density-function.md) have [Fourier transform](fourier-transform.md) supported in the plateau of a [flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md). At fixed [smoothing bandwidth](smoothing-bandwidth.md) one, the [convolution theorem](convolution-theorem.md) gives $K*f=f$, so the [kernel density estimator](kernel-density-estimation.md) is pointwise unbiased. Its [variance](variance-split.md) is at most $\|f\|_\infty\|K\|_2^2/n$, and the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) proves the displayed rate. An explicit example is $f(x)=(1-\cos x)/(\pi x^2)$, with value $1/(2\pi)$ at zero and transform $(1-|t|)_+$. Direct inverse Fourier integration gives the formula. The function is nonnegative, integrable and has integral one because its transform at zero is one. Compact frequency support also gives bounded derivatives of every order.

## ↑ Ancestors (9)

1. [Flat-top kernel for density estimation](flat-top-kernel-for-density-estimation.md)
2. [Kernel for density estimation](kernel-for-density-estimation.md)
3. [Density estimation](density-estimation.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/2/solution.md)
