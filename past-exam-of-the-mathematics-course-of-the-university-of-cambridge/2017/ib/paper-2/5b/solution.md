<h1 id="5b/solution">Solution</h1>

↑ **Parent:** [5B](../5b.md)

Oddness gives zero cosine coefficients. Integration by parts gives the sine [Fourier coefficients](../../../../../fourier-coefficient.md)

$$
b_n=\frac2\pi\int_0^\pi x\sin(nx)\,dx=\frac{2(-1)^{n+1}}n,
\qquad \boxed{x=2\sum_{n=1}^\infty\frac{(-1)^{n+1}}n\sin(nx)\quad(-\pi<x<\pi).}
$$

The [Fourier series](../../../../../fourier-series-split.md) of the piecewise smooth periodic extension converges to its value at interior continuity points. [Termwise integration](../../../../../termwise-integration.md) from 0 to $x$ is valid: on the interval between these points, which stays inside $(-\pi,\pi)$, the partial sums of $\sum(-1)^{n+1}\sin(nt)$ are uniformly bounded by the geometric-sum formula, since $|1+e^{it}|$ is bounded away from zero. The [Dirichlet test](../../../../../dirichlet-test.md) therefore gives uniform convergence there. Integrating gives

$$
x^2=4\sum_{n=1}^\infty\frac{(-1)^{n+1}}{n^2}(1-\cos nx).
$$

The integrated series is absolutely and uniformly convergent. Consequently

$$
\boxed{a_n=\frac{4(-1)^n}{n^2}\ (n\ge1),\qquad a_0=8\sum_{n=1}^\infty\frac{(-1)^{n-1}}{n^2}.}
$$

Independently, the constant [Fourier coefficient](../../../../../fourier-coefficient.md) is $a_0=\pi^{-1}\int_{-\pi}^\pi x^2\,dx=2\pi^2/3$. Comparison yields

$$
\boxed{\sum_{n=1}^\infty\frac{(-1)^{n-1}}{n^2}=\frac{\pi^2}{12},\qquad x^2=\frac{\pi^2}{3}+4\sum_{n=1}^\infty\frac{(-1)^n}{n^2}\cos nx.}
$$

The original sine series is not uniformly convergent on the whole open interval; that stronger assertion is unnecessary for the justified integration.

## ↑ Ancestors (10)

1. [5B](../5b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
