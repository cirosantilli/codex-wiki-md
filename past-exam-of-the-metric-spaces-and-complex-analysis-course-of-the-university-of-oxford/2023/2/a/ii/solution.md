<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

Let $(x_n)$ be any [sequence](../../../../../sequence.md) in the [compact metric space](../../../../../compact-metric-space.md) $X$. There must be an $x\in X$ such that every [open ball](../../../../../open-ball.md) about $x$ contains $x_n$ for infinitely many indices $n$. Otherwise, for each $x\in X$ choose a ball $B(x,r_x)$ containing only finitely many terms, counted by indices. These balls are an [open cover](../../../../../open-cover.md). A [finite subcover](../../../../../finite-subcover.md) would imply that only finitely many indices occur anywhere in $X$, a contradiction.

Now choose successively $n_k>n_{k-1}$ with $x_{n_k}\in B(x,1/k)$; infinitely many available indices make this possible. Then $d(x_{n_k},x)<1/k\to0$, so $(x_{n_k})$ is a [convergent subsequence](../../../../../convergent-subsequence.md). Thus

$$
\boxed{\text{compact metric space}\ \Longrightarrow\ \text{sequentially compact space}}.
$$

The proof counts indices rather than distinct points, so it also handles a value repeated infinitely often.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../../split.md)
6. [Metric spaces and complex analysis course of the University of Oxford](../../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
