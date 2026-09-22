<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\varepsilon>0$, the [triangle inequality](../../../../../../triangle-inequality.md) and the [union bound](../../../../../../boole-s-inequality.md) give

$$
\begin{aligned}
\mathbb P\bigl(|(X_n+Y_n)-(X+Y)|>\varepsilon\bigr)
&\leq\mathbb P(|X_n-X|>\varepsilon/2)
+\mathbb P(|Y_n-Y|>\varepsilon/2)\\
&\longrightarrow0.
\end{aligned}
$$

Thus $\boxed{X_n+Y_n\longrightarrow X+Y\text{ in probability}}$. This proves closure of [convergence in probability](../../../../../../convergence-in-probability.md) under addition. No [independence](../../../../../../independent-random-variables.md) is needed; the [random variables](../../../../../../random-variable-split.md) are compared on their given common [probability space](../../../../../../probability-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
