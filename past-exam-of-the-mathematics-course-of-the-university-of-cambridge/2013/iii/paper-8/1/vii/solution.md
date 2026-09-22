<h1 id="1/vii/solution">Solution</h1>

↑ **Parent:** [Vii](../vii.md)

Use the transform convention $F(\lambda)=\int_{\mathbb R}f(t)e^{-i\lambda t}\,dt$. The given [Fourier inversion theorem](../../../../../../fourier-inversion-theorem.md) gives

$$
f(t)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{it\lambda}\,d\lambda.
$$

Here $F$ is continuous, vanishes at both endpoints and belongs to $L^2[-\pi,\pi]$. It therefore defines a continuous periodic function. Its [Fourier coefficient](../../../../../../fourier-coefficient.md) at index $-n$ is $f(n)$. By part (i),

$$
P_N(\lambda)=\sum_{|n|\leq N}f(n)e^{-in\lambda}\longrightarrow F(\lambda)
\quad\text{in }L^2.
$$

Pair this convergence with $e^{it\lambda}$. Since that function has normalized $L^2$ norm one, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields, uniformly in $t$,

$$
\left|f(t)-\frac1{2\pi}\int_{-\pi}^{\pi}P_N(\lambda)e^{it\lambda}\,d\lambda\right|
\leq\|F-P_N\|_2\longrightarrow0.
$$

The elementary integral is the [sinc function](../../../../../../sinc-function.md),

$$
\frac1{2\pi}\int_{-\pi}^{\pi}e^{i(t-n)\lambda}\,d\lambda
=D(t-n).
$$

Thus the [sampling expansion by periodic Fourier projection](../../../../../../sampling-expansion-by-periodic-fourier-projection.md) is

$$
\boxed{f(t)=\sum_{n\in\mathbb Z}f(n)D(t-n).}
$$

There is no pointwise interchange with an unproved [Fourier series](../../../../../../fourier-series-split.md): the calculation first uses finite sums and then an $L^2$ limit.

The convergence can also be made absolute. [Parseval's identity](../../../../../../parseval-identity.md) gives $\sum_n|f(n)|^2=\|F\|_2^2$, and [Bessel's inequality](../../../../../../bessel-s-inequality.md) applied to $e^{it\lambda}$ gives $\sum_n|D(t-n)|^2\leq1$. Hence

$$
\sum_{|n|>N}|f(n)D(t-n)|
\leq\left(\sum_{|n|>N}|f(n)|^2\right)^{1/2}\longrightarrow0
$$

uniformly in $t$. At an integer argument, $D$ is one at zero and zero at the other integers, so the expansion interpolates the samples exactly.

## ↑ Ancestors (11)

1. [Vii](../vii.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
