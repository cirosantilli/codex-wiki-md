<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The time $T_R$ is a [stopping time](../../../../../../stopping-time.md), because $\{T_R\leq n\}=\bigcup_{k\leq n}\{M_k\geq R\}\in\mathcal F_n$. Apply the [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) to the bounded time $T_R\wedge n$:

$$
1=\mathbb E M_{T_R\wedge n}
\geq R\,\mathbb P(T_R\leq n).
$$

On $\{T_R\leq n\}$ the stopped value is at least $R$, and elsewhere it is nonnegative. Letting $n\to\infty$ gives the [maximal bound for a nonnegative martingale](../../../../../../maximal-bound-for-a-nonnegative-martingale.md):

$$
\boxed{\mathbb P(T_R<\infty)\leq\frac1R.}
$$

**Stop at a bounded time first, then pass to the increasing event.** This avoids assuming [uniform integrability](../../../../../../uniform-integrability.md) of the original process. For $0<R\leq1$, $T_R=0$ and the bound simply says $1\leq1/R$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
