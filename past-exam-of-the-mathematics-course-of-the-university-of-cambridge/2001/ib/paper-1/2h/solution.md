<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

For the real even [function](../../../../../function-split.md), let $s_N=a_0/2+\sum_{n=1}^Na_n\cos nx$. [Fourier orthogonality](../../../../../fourier-orthogonality.md) gives $\int_{-\pi}^{\pi}\cos nx\,dx=0$ for $n\geq1$ and $\int_{-\pi}^{\pi}\cos nx\cos mx\,dx=\pi\delta_{nm}$. Consequently

$$
\frac1\pi\int_{-\pi}^{\pi}s_N^2\,dx=\frac{a_0^2}{2}+\sum_{n=1}^Na_n^2.
$$

For an even [square-integrable function](../../../../../square-integrable-function.md), the complete [Fourier cosine series](../../../../../fourier-cosine-series.md) converges in the [L2 norm](../../../../../l2-norm.md); hence its norms converge. Taking $N\to\infty$ proves [Parseval's identity](../../../../../parseval-identity.md) in the required normalization:

$$
\boxed{\frac1\pi\int_{-\pi}^{\pi}f(x)^2\,dx=\frac{a_0^2}{2}+\sum_{n=1}^{\infty}a_n^2}.
$$

This limit argument avoids multiplying an infinite series without a justification of [L2 norm](../../../../../l2-norm.md) convergence.

For the quadratic [function](../../../../../function-split.md), the [Fourier coefficients](../../../../../fourier-coefficient.md) are

$$
a_0=\frac1\pi\int_{-\pi}^{\pi}x^2\,dx=\frac{2\pi^2}{3},\qquad
a_n=\frac2\pi\int_0^\pi x^2\cos nx\,dx=\frac{4(-1)^n}{n^2}.
$$

The last equality follows from two [integrations by parts](../../../../../integration-by-parts.md), using $\sin n\pi=0$. Thus

$$
\boxed{x^2=\frac{\pi^2}{3}+4\sum_{n=1}^{\infty}\frac{(-1)^n}{n^2}\cos nx\quad(-\pi\leq x\leq\pi)}.
$$

This [Fourier series](../../../../../fourier-series-split.md) is [absolutely convergent](../../../../../absolute-convergence.md); the periodically extended quadratic is continuous, so it represents its values also at the endpoints. Substituting its coefficients into [Parseval's identity](../../../../../parseval-identity.md) gives

$$
\frac{2\pi^4}{5}=\frac{2\pi^4}{9}+16\sum_{n=1}^{\infty}\frac1{n^4},
\qquad \boxed{\sum_{n=1}^{\infty}\frac1{n^4}=\frac{\pi^4}{90}}.
$$

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
