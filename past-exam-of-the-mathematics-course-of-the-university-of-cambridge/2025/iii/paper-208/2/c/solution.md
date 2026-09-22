<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Chernoff bound](../../../../../../chernoff-bound.md) and part (b) give

$$
\mathbb P(f(X)\geq t)
\leq e^{-\lambda_*t}F(\lambda_*)
\leq3e^{-t/\sqrt{C_P(X)}}.
$$

Apply the same argument to $-f$ and use the [union bound](../../../../../../boole-s-inequality.md) to obtain

$$
\mathbb P(|f(X)|\geq t)
\leq6e^{-t/\sqrt{C_P(X)}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
