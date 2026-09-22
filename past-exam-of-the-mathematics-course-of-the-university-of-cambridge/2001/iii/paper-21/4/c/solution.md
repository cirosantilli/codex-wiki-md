<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**True.** The unit-time increments $Z_k=B_k-B_{k-1}$ are [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with standard [normal distribution](../../../../../../normal-distribution.md), hence integrable with mean zero. The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) gives $B_n/n\to0$ almost surely at integer times.

To control the intervals between integers, put $M_n=\sup_{0\leq u\leq1}|B_{n+u}-B_n|$. [Stationary increments](../../../../../../stationary-increments.md) and the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) give $\mathbb E M_n^2\leq4$. Thus the [Markov inequality](../../../../../../markov-inequality.md) yields

$$
\sum_{n=1}^\infty\mathbb P(M_n>\varepsilon n)\leq\frac4{\varepsilon^2}\sum_{n=1}^\infty n^{-2}<\infty.
$$

The [Borel-Cantelli lemma](../../../../../../borel-cantelli-lemmas.md), followed by a countable intersection over positive rational $\varepsilon$, implies $M_n/n\to0$ almost surely. For $n\leq t\leq n+1$,

$$
\frac{|B_t|}{t}\leq\frac{|B_n|+M_n}{n}.
$$

Both terms tend to zero on the same probability-one event, proving $\boxed{B_t/t\to0\text{ almost surely}}$ for continuous time as well.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
