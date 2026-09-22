<h1 id="9h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [independence](../../../../../../independent-random-variables.md) of the two [simple random walks](../../../../../../simple-random-walk.md), [linearity of expectation](../../../../../../linearity-of-expectation.md), and symmetry of their transition probabilities,

$$
\begin{aligned}
\mathbb E Z
&=\sum_{n=0}^{\infty}\mathbb P(X_n=Y_n)\\
&=\sum_{n=0}^{\infty}\sum_{x\in\mathbb Z}p_{0x}(n)^2\\
&=\sum_{n=0}^{\infty}\sum_{x\in\mathbb Z}p_{0x}(n)p_{x0}(n).
\end{aligned}
$$

The [Chapman-Kolmogorov equation](../../../../../../chapman-kolmogorov-equation.md) identifies the inner sum as $p_{00}(2n)$, so

$$
\boxed{\mathbb E Z=\sum_{n=0}^{\infty}p_{00}(2n)}.
$$

A [simple random walk on the integer line](../../../../../../simple-random-walk-on-the-integer-line.md) can return to $0$ only at an [even](../../../../../../even-number.md) time. Since it is recurrent at $0$, part (a) gives

$$
\sum_{m=0}^{\infty}p_{00}(m)=\sum_{n=0}^{\infty}p_{00}(2n)=\infty.
$$

Therefore $\boxed{\mathbb E Z=\infty}$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9H](../../9h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
