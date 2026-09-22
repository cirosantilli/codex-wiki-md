<h1 id="26g/solution">Solution</h1>

↑ **Parent:** [26G](../26g.md)

Because the centered [normal distribution](../../../../../normal-distribution.md) density $g_t$ is nonnegative and has integral one, [Fubini's theorem](../../../../../fubini-s-theorem.md) and translation invariance give

$$
\begin{aligned}
\|f*g_t\|_1
&\leq\int_{\mathbb R}\int_{\mathbb R}|f(x-y)|g_t(y)\,dy\,dx\\
&=\int_{\mathbb R}g_t(y)\|f\|_1\,dy
=\|f\|_1.
\end{aligned}
$$

Thus $f*g_t\in L^1$.

Use the angular-frequency convention

$$
\widehat f(\xi)=\int_{\mathbb R}f(x)e^{-ix\xi}\,dx.
$$

The [convolution theorem](../../../../../convolution-theorem.md) and the Gaussian transform give

$$
\widehat{f*g_t}(\xi)=\widehat f(\xi)e^{-t\xi^2/2}.
$$

Since $|\widehat f(\xi)|\leq\|f\|_1$, this product is integrable. Moreover, absolute integrability justifies exchanging the integrals:

$$
\begin{aligned}
\frac1{2\pi}\int_{\mathbb R}\widehat f(\xi)e^{-t\xi^2/2}e^{ix\xi}\,d\xi
&=\int_{\mathbb R}f(z)
\left[\frac1{2\pi}\int_{\mathbb R}e^{-t\xi^2/2}e^{i(x-z)\xi}\,d\xi\right]dz\\
&=\int_{\mathbb R}f(z)g_t(x-z)\,dz\\
&=(f*g_t)(x).
\end{aligned}
$$

This proves the [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) for the convolution directly.

Now additionally suppose $\widehat f\in L^1$. For every $x$, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) gives

$$
\lim_{t\downarrow0}(f*g_t)(x)
=\frac1{2\pi}\int_{\mathbb R}\widehat f(\xi)e^{ix\xi}\,d\xi.
$$

Fourier inversion identifies the right-hand side with $f(x)$ for [Lebesgue almost everywhere](../../../../../almost-everywhere.md) $x$. Therefore the [Gaussian approximate identity](../../../../../gaussian-approximate-identity.md) satisfies

$$
\boxed{f*g_t(x)\longrightarrow f(x)\quad\text{for almost every }x.}
$$

## ↑ Ancestors (10)

1. [26G](../26g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
