<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On $(-\pi,\pi)$ the [function](../../../../../../function-split.md) is [odd](../../../../../../odd-function.md), so its mean and all its [cosine](../../../../../../cosine.md) [Fourier coefficients](../../../../../../fourier-coefficient.md) vanish:

$$
a_0=0,\qquad a_n=0\quad(n\geq1).
$$

The assigned endpoint value does not affect these [integrals](../../../../../../integral-split.md). The product of the two [odd functions](../../../../../../odd-function.md) $x|x|$ and $\sin nx$ is [even](../../../../../../even-function.md), hence the [sine](../../../../../../sine.md) [Fourier coefficients](../../../../../../fourier-coefficient.md) are

$$
b_n=\frac2\pi\int_0^\pi x^2\sin nx\,dx.
$$

Two applications of [integration by parts](../../../../../../integration-by-parts.md) give

$$
\begin{aligned}
\int_0^\pi x^2\sin nx\,dx
&=\left[-\frac{x^2\cos nx}{n}\right]_0^\pi+\frac2n\int_0^\pi x\cos nx\,dx\\
&=-\frac{\pi^2(-1)^n}{n}+\frac2n\left[\frac{x\sin nx}{n}+\frac{\cos nx}{n^2}\right]_0^\pi\\
&=-\frac{\pi^2(-1)^n}{n}+\frac{2[(-1)^n-1]}{n^3}.
\end{aligned}
$$

Therefore

$$
\boxed{f(x)\sim\sum_{n=1}^{\infty}\left[\frac{2\pi(-1)^{n+1}}n+\frac{4[(-1)^n-1]}{\pi n^3}\right]\sin nx.}
$$

The [periodic extension](../../../../../../periodic-extension.md) has a [jump discontinuity](../../../../../../jump-discontinuity.md) at every odd multiple of $\pi$: its left and right limits are $\pi^2$ and $-\pi^2$. Its assigned value at each such point is $-\pi^2$. Thus it is [odd](../../../../../../odd-function.md) away from these points, but it is not a globally [odd function](../../../../../../odd-function.md) pointwise. The [Fourier series](../../../../../../fourier-series-split.md) will take the midpoint value zero at these jumps.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
