<h1 id="7d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For singularities $a<c_1<\cdots<c_N<b$, the Cauchy principal value is

$$
\boxed{
\operatorname{PV}\int_{-\infty}^{\infty}f(x)\,dx
=\lim_{\varepsilon\downarrow0}
\left[
\int_{-\infty}^{c_1-\varepsilon}f(x)\,dx+
\sum_{j=1}^{N-1}\int_{c_j+\varepsilon}^{c_{j+1}-\varepsilon}f(x)\,dx+
\int_{c_N+\varepsilon}^{\infty}f(x)\,dx
\right]},
$$

where the assumed tail [integrals](../../../../../../integral.md) make the two unbounded pieces meaningful. Equivalently, remove a symmetric interval of radius $\varepsilon$ about each $c_j$ and take the [limit](../../../../../../limit-of-a-function.md) of the remaining [integral](../../../../../../integral.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7D](../../7d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
