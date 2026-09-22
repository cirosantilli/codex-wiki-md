<h1 id="4f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $t>0$, monotonicity gives $\{X\geq k\}=\{e^{tX}\geq e^{tk}\}$. Apply [Markov inequality](../../../../../../markov-inequality.md) to the nonnegative variable $e^{tX}$:

$$
\boxed{\mathbb P(X\geq k)\leq e^{-tk}\mathbb E[e^{tX}]}.
$$

If the [expectation](../../../../../../expected-value.md) is infinite, the bound remains true but uninformative. At $t=0$ the right side is one, so that endpoint follows directly. Minimizing over $t\geq0$ gives the [Chernoff bound](../../../../../../chernoff-bound.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4F](../../4f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
