<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the [HHL algorithm](../../../../../../hhl-algorithm.md) to have runtime polynomial in $\log N$, the Hermitian matrix $A$ must be invertible, have a [condition number](../../../../../../condition-number.md) $\kappa$ bounded by $\operatorname{poly}(\log N)$, and be a [sparse matrix](../../../../../../sparse-matrix.md) with its nonzero entries efficiently accessible by an oracle. The normalized state $|b\rangle$ must also be preparable in $\operatorname{poly}(\log N)$ time. With precision costs suppressed, these assumptions let HHL prepare, with high probability,

$$
\boxed{|\xi\rangle=\frac{A^{-1}|b\rangle}
{\|A^{-1}|b\rangle\|}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
