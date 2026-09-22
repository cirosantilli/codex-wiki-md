<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The balance recurrence is

$$
\pi_i=\pi_{i+1}+\pi_0q_{i+1}.
$$

Working down from $N-1$ gives $\pi_i=\pi_0P(T_1>i)$. Since the sum of these tails is $E[T_1]$, the unique invariant law is

$$
\boxed{\pi_i=\frac{P(T_1>i)}{E[T_1]}=
\frac{\sum_{j=i+1}^Nq_j}{\sum_{j=1}^Njq_j}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
