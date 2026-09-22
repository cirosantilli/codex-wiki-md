<h1 id="14b/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Fourier transform](../../../../../../../fourier-transform.md) convention $\widetilde h(k)=\int_{\mathbb R}e^{-ikx}h(x)\,dx$, with inverse $(2\pi)^{-1}\int_{\mathbb R}e^{ikx}\widetilde h(k)\,dk$. Splitting at the origin, with $a>0$ to ensure convergence, gives

$$
\widetilde h(k)=\int_{-\infty}^0e^{(a-ik)x}\,dx+\int_0^\infty e^{-(a+ik)x}\,dx=\frac1{a-ik}+\frac1{a+ik}.
$$

Thus

$$
\boxed{\widetilde h(k)=\frac{2a}{a^2+k^2}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [14B](../../../14b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ib](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
