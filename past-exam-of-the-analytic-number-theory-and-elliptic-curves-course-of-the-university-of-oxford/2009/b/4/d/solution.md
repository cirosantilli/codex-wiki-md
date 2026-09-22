<h1 id="b/4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Choose the blocks

$$
\boxed{x_n=p^{\lfloor\log_p n\rfloor}\quad(n\geq1).}
$$

If $p^k\leq n<p^{k+1}$, then $|x_n|_p=p^{-k}$, so $x_n\to0$ in $\mathbb Q_p$. By the [ultrametric inequality](../../../../../ultrametric-inequality.md), for $N\geq M$,

$$
\left|\sum_{n=M}^{N}x_n\right|_p
\leq\max_{M\leq n\leq N}|x_n|_p\longrightarrow0
\quad(M\to\infty).
$$

The [partial sums](../../../../../partial-sum.md) are [Cauchy sequence](../../../../../cauchy-sequence.md), and [completeness](../../../../../completeness.md) of $\mathbb Q_p$ proves convergence of $\sum x_n$.

In the real series of [p-adic absolute values](../../../../../p-adic-absolute-value.md), the block $p^k\leq n<p^{k+1}$ contains $(p-1)p^k$ equal terms of size $p^{-k}$. Its sum is $p-1$, independently of $k$. Infinitely many such positive block sums force divergence. This exhibits [p-adic convergence without summable absolute values](../../../../../p-adic-convergence-without-summable-absolute-values.md): the criterion is that the terms tend to zero, rather than real absolute summability.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
