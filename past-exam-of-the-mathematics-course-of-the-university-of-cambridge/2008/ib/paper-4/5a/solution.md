<h1 id="5a/solution">Solution</h1>

↑ **Parent:** [5A](../5a.md)

For the [half-range Fourier cosine series](../../../../../half-range-fourier-cosine-series.md) on $(0,1)$, the coefficients are

$$
a_0=2\int_0^1x^2\,dx=\frac23,\qquad a_n=2\int_0^1x^2\cos(n\pi x)\,dx.
$$

Two integrations by parts, with $k=n\pi$, give

$$
\int_0^1x^2\cos(kx)\,dx=-\frac2k\int_0^1x\sin(kx)\,dx=\frac{2(-1)^n}{k^2}.
$$

Thus

$$
\boxed{x^2=\frac13+\frac4{\pi^2}\sum_{n=1}^{\infty}\frac{(-1)^n\cos(n\pi x)}{n^2}.}
$$

The even, $2$-periodic extension is continuous and piecewise continuously differentiable, so the [Fourier series](../../../../../fourier-series-split.md) converges to it, including at $x=1$. Equivalently, the summable coefficient bound gives [uniform convergence](../../../../../uniform-convergence.md) and permits taking the limit from the interior. Evaluating at $x=1$, where $(-1)^n\cos(n\pi)=1$, yields

$$
1=\frac13+\frac4{\pi^2}\sum_{n=1}^{\infty}\frac1{n^2},\qquad \boxed{\sum_{n=1}^{\infty}\frac1{n^2}=\frac{\pi^2}{6}.}
$$

This is the [Basel problem](../../../../../basel-problem.md).

## ↑ Ancestors (10)

1. [5A](../5a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
