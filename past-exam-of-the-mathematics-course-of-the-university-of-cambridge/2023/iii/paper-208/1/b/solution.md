<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For every $0<\lambda<1/\alpha$, the [Chernoff bound](../../../../../../chernoff-bound.md) and the sub-exponential moment-generating bound give

$$
\mathbb P(X\geq t)
\leq\exp\left(-\lambda t+\frac{\lambda^2\nu}{2}\right).
$$

If $0<t\leq\nu/\alpha$, choose $\lambda=t/\nu$; at the endpoint, take a limit from below. This yields

$$
\mathbb P(X\geq t)\leq e^{-t^2/(2\nu)}.
$$

If $t>\nu/\alpha$, let $\lambda\uparrow1/\alpha$. Since $\nu/(2\alpha^2)<t/(2\alpha)$,

$$
-\frac t\alpha+\frac\nu{2\alpha^2}
\leq-\frac t{2\alpha},
$$

and hence $\mathbb P(X\geq t)\leq e^{-t/(2\alpha)}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
