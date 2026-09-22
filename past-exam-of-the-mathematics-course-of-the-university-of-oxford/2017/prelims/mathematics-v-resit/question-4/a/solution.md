<h1 id="question-4/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

For a nonzero integer $k$, direct [integration](../../../../../../integral-split.md) gives

$$
\int_{-\pi}^{\pi}\cos(kx)\,dx=0,\qquad
\int_{-\pi}^{\pi}\sin(kx)\,dx=0,
$$

whereas $\int_{-\pi}^{\pi}1\,dx=2\pi$. The [product-to-sum formulas](../../../../../../product-to-sum-formula.md)

$$
\begin{aligned}
2\cos(mx)\cos(nx)&=\cos((m-n)x)+\cos((m+n)x),\\
2\sin(mx)\sin(nx)&=\cos((m-n)x)-\cos((m+n)x),\\
2\sin(mx)\cos(nx)&=\sin((m+n)x)+\sin((m-n)x)
\end{aligned}
$$

therefore establish [Fourier orthogonality](../../../../../../fourier-orthogonality.md): for positive integers $m,n$,

$$
\begin{aligned}
\int_{-\pi}^{\pi}\cos(mx)\cos(nx)\,dx&=\pi\delta_{mn},\\
\int_{-\pi}^{\pi}\sin(mx)\sin(nx)\,dx&=\pi\delta_{mn},\\
\int_{-\pi}^{\pi}\sin(mx)\cos(nx)\,dx&=0.
\end{aligned}
$$

Here $\delta_{mn}$ is the [Kronecker delta](../../../../../../kronecker-delta.md). In particular the [constant function](../../../../../../constant-function.md) is orthogonal to every nonconstant [sine](../../../../../../sine.md) and [cosine](../../../../../../cosine.md) in this system. Integrating the given [Fourier series](../../../../../../fourier-series-split.md), then multiplying it by $\cos(mx)$ or $\sin(mx)$ and integrating, isolates its [Fourier coefficients](../../../../../../fourier-coefficient.md). Using the permitted interchange of the [sum](../../../../../../sum.md) and [integral](../../../../../../integral-split.md) gives

$$
\boxed{a_0=\frac1\pi\int_{-\pi}^{\pi}f(x)\,dx},\qquad
\boxed{a_n=\frac1\pi\int_{-\pi}^{\pi}f(x)\cos(nx)\,dx},\qquad
\boxed{b_n=\frac1\pi\int_{-\pi}^{\pi}f(x)\sin(nx)\,dx}\quad(n\geq1).
$$

If $f$ is an [even function](../../../../../../even-function.md), then $f(x)\sin(nx)$ is an [odd function](../../../../../../odd-function.md), while $f(x)\cos(nx)$ is an [even function](../../../../../../even-function.md). Thus

$$
\boxed{b_n=0,\qquad a_n=\frac2\pi\int_0^\pi f(x)\cos(nx)\,dx\quad(n\geq0)}.
$$

The [Fourier series](../../../../../../fourier-series-split.md) consequently reduces to a [Fourier cosine series](../../../../../../fourier-cosine-series.md).

## ↑ Ancestors (12)

1. [a](../a.md)
2. [Question 4](../../question-4.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
