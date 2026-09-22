<h1 id="17b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\alpha=\pi(m+1)/n$, which lies strictly between zero and $\pi$. On the lower ray $z=x$, the integral is $I_R=\int_0^R x^m/(1+x^n)dx$. On the upper ray $z=xe^{2\pi i/n}$, the positive boundary orientation runs from $R$ down to zero. Since $z^n=x^n$, that contribution is $-e^{2i\alpha}I_R$. The circular contribution vanishes by part (b); hence

$$
(1-e^{2i\alpha})I=-\frac{2\pi i}{n}e^{i\alpha}.
$$

Use $1-e^{2i\alpha}=-2ie^{i\alpha}\sin\alpha$ to obtain

$$
\boxed{\int_0^\infty\frac{x^m}{1+x^n}\,dx
=\frac\pi{n\sin[\pi(m+1)/n]}}.
$$

The result is positive as expected. Convergence near zero follows from $m\ge0$, so both endpoint limits used in the [contour](../../../../../../complex-integration-contour.md) argument are justified.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [17B](../../17b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
