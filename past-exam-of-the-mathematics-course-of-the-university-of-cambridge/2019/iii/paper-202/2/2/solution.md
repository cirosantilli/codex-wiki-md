<h1 id="2/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Because $\|b'\|_\infty<\infty$, the function $b$ is [Lipschitz continuous](../../../../../../lipschitz-continuity.md). the [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md), proved by iteration on

$$
x^{(0)}(t)=x_0+w(t),\qquad
x^{(n+1)}(t)=x_0+w(t)+\int_0^tb(x^{(n)}(s))ds
$$

converges uniformly on every compact interval. The usual factorial estimate proves convergence for arbitrary interval length, and the [Gronwall inequality](../../../../../../gronwall-inequality.md) proves uniqueness. Thus there is a unique global continuous solution.

For $w=W$, induction shows that $X_t^{(n)}$ is $\mathcal F_t$-measurable: its value uses only $(W_s)_{s\leq t}$ and earlier iterates up to time $t$. The pointwise limit $X_t$ is therefore $\mathcal F_t$-measurable. Hence **$X$ is adapted to $(\mathcal F_t)$**.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
