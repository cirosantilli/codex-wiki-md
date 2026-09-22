<h1 id="30a/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every $N$,

$$
f(\xi)=\sum_{n=0}^Nf_n(\xi-x_0)^n+r_N(\xi),
\qquad
r_N(\xi)=o((\xi-x_0)^N).
$$

Integrating the finite sum gives

$$
\int_{x_0}^x f(\xi)\,d\xi
=\sum_{n=0}^N\frac{f_n}{n+1}(x-x_0)^{n+1}
+\int_{x_0}^x r_N(\xi)\,d\xi.
$$

For every $\varepsilon>0$, sufficiently close to $x_0$ one has $|r_N(\xi)|\leq\varepsilon|\xi-x_0|^N$, so the last integral is $o(|x-x_0|^{N+1})$. This proves the integrated expansion.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [30A](../../../30a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
