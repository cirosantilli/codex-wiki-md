<h1 id="12a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The transform factors as $s^{-2}(s+2)^{-2}$, whose inverse factors are $t$ and $te^{-2t}$. The [Laplace convolution theorem](../../../../../../convolution-theorem.md) gives

$$
f(t)=\int_0^t\tau(t-\tau)e^{-2(t-\tau)},d\tau,
$$

and direct integration produces

$$
f(t)=\frac14\bigl(t-1+(t+1)e^{-2t}\bigr),
$$

confirming part (b).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [12A](../../12a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
