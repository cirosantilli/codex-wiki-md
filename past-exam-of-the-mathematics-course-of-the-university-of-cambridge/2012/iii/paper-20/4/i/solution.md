<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $\mathbb T=\mathbb R/(2\pi\mathbb Z)$ and $|k|_1=\sum_j|k_j|$. A [Diophantine frequency vector](../../../../../../diophantine-frequency-vector.md) satisfies

$$
\boxed{|k\cdot\omega|\ge\gamma |k|_1^{-\tau}\quad
(k\in\mathbb Z^n\setminus\{0\}).}
$$

Changing the norm only changes the admissible $\gamma$. The bound excludes resonances and quantifies the [small divisors](../../../../../../small-divisor.md) in the inverse of $\mathcal D_\omega$.

A periodic solution necessarily has zero-mean right-hand side, because the integral of each angular derivative vanishes. Conversely, if $\langle g\rangle=0$, expand its [Fourier series](../../../../../../fourier-series-split.md):

$$
g(x)=\sum_k g_ke^{ik\cdot x},\qquad
f(x)=f_0+\sum_{k\ne0}\frac{g_k}{i\,k\cdot\omega}e^{ik\cdot x}.
$$

The [Diophantine condition](../../../../../../diophantine-frequency-vector.md) makes every denominator nonzero. These are all differentiable periodic solutions: any difference satisfies $\mathcal D_\omega h=0$ and has no nonzero [Fourier coefficient](../../../../../../fourier-coefficient.md). Thus **a solution exists exactly for zero-mean $g$, and is unique up to a constant**; setting $\langle f\rangle=0$ fixes it. The analytic conclusion is on every strictly smaller complex strip, not necessarily the original boundary strip.

Shifting each contour in the [Fourier coefficient](../../../../../../fourier-coefficient.md) integral toward the appropriate edge of the complex strip gives

$$
|g_k|\le |g|_\sigma e^{-\sigma|k|_1}.
$$

Hence for $0<\delta<\sigma$,

$$
|f-\langle f\rangle|_{\sigma-\delta}
\le\frac{|g|_\sigma}{\gamma}\sum_{k\ne0}|k|_1^\tau e^{-\delta|k|_1}.
$$

This converges normally, including differentiated series on any still smaller strip, and proves both holomorphic extension and $\mathcal D_\omega f=g$. Real-valuedness follows from $g_{-k}=\overline{g_k}$ and the corresponding identity for $f_k$.

An explicit bound is obtained by counting lattice shells. The number of $k$ with $|k|_1=m$ is at most

$$
2^n\binom{m+n-1}{n-1}\le A_n m^{n-1},\qquad
A_n=\frac{2^n n^{n-1}}{(n-1)!}.
$$

Put $s=n+\tau$ and $p=s-1\ge0$. For $p>0$, $m^p e^{-\delta m/2}\le(2p/(e\delta))^p$; for $p=0$ use the bound $1$. Since $\sum_{m\ge1}e^{-\delta m/2}=(e^{\delta/2}-1)^{-1}\le2/\delta$, this gives

$$
\boxed{|f-\langle f\rangle|_{\sigma-\delta}
\le \frac{C_{n,\tau}}{\gamma\,\delta^{n+\tau}}|g|_\sigma,\qquad
C_{n,\tau}=2A_n\left(\frac{2(n+\tau-1)}e\right)^{n+\tau-1}.}
$$

Use $0^0=1$ in this constant when $n=1,\tau=0$. The estimate is valid for every positive $\delta$; optimality of the exponent is not needed. For a unit-period [flat torus](../../../../../../flat-torus.md), insert the factors $2\pi$ in both the Fourier exponent and denominator and adjust the constant.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
