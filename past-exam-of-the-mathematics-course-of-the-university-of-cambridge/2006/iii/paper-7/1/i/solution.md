<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Identify the [circle](../../../../../../circle.md) with $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and use normalized [Fourier coefficients](../../../../../../fourier-coefficient.md) and [convolution](../../../../../../convolution.md):

$$
\widehat f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t)e^{-int}\,dt,\qquad (f*g)(t)=\frac1{2\pi}\int_{-\pi}^{\pi}f(t-s)g(s)\,ds.
$$

For $0\leq r<1$, summing two [geometric series](../../../../../../geometric-series.md) gives the [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md):

$$
1+\sum_{n\geq1}r^n(e^{int}+e^{-int})=\frac1{1-re^{it}}+\frac1{1-re^{-it}}-1=\frac{1-r^2}{1-2r\cos t+r^2}=P_r(t).
$$

This [Fourier series](../../../../../../fourier-series-split.md) converges absolutely and uniformly for each fixed $r<1$. Consequently we can integrate it term by term in the [convolution](../../../../../../convolution.md); the substitution $u=t-s$ gives

$$
\boxed{(f*P_r)(t)=\sum_{n\in\mathbb Z}\widehat f(n)r^{|n|}e^{int}.}
$$

The resulting series is itself absolutely and uniformly convergent, since $|\widehat f(n)|\leq\|f\|_\infty$ and $\sum_n r^{|n|}<\infty$.

The [Poisson kernel on the circle](../../../../../../poisson-kernel-on-the-circle.md) is nonnegative and has normalized integral one, as its constant [Fourier coefficient](../../../../../../fourier-coefficient.md) is one. Its mass concentrates near zero. Indeed, for $r\geq1/2$ and $\delta\leq|s|\leq\pi$,

$$
0\leq P_r(s)=\frac{1-r^2}{(1-r)^2+2r(1-\cos s)}\leq\frac{1-r^2}{1-\cos\delta}.
$$

Hence its normalized integral outside $(-\delta,\delta)$ tends to zero as $r\uparrow1$. Given $\eta>0$, [uniform continuity](../../../../../../uniform-continuity.md) of $f$ gives a $\delta>0$ such that $|f(t-s)-f(t)|<\eta$ whenever the circular distance of $s$ from zero is less than $\delta$. Splitting the [convolution](../../../../../../convolution.md) error into this arc and its complement yields

$$
\sup_t|(f*P_r)(t)-f(t)|\leq\eta+2\|f\|_\infty\frac1{2\pi}\int_{\delta\leq|s|\leq\pi}P_r(s)\,ds.
$$

The second term tends to zero, and $\eta$ is arbitrary. Thus **the Abel sums converge uniformly to $f$**, or $\boxed{\|f*P_r-f\|_\infty\to0}$. This is [uniform Poisson summability of continuous circle functions](../../../../../../uniform-poisson-summability-of-continuous-circle-functions.md): positivity, unit mass and concentration supply the required [approximate identity](../../../../../../approximate-identity.md) argument.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
