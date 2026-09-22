<h1 id="9e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The arithmetic--geometric mean inequality gives $x_n\geq1$ from $n=2$ onward. For $x>1$,

$$
1<\frac12(x+x^{-1})<x,
$$

so the tail decreases to a [limit](../../../../../../limit-of-a-function.md) $L\geq1$. Passing to the recurrence gives $2L=L+L^{-1}$, hence $L=1$.

For the subadditive [sequence](../../../../../../sequence.md), $0\leq x_n/n\leq x_1$, so it is bounded. The [Fekete lemma](../../../../../../fekete-s-lemma.md) can be proved directly here as follows. Let $\alpha=\inf_kx_k/k$. Fix $k$ and write $n=qk+r$, $0\leq r<k$. Then

$$
\frac{x_n}{n}\leq\frac{qx_k+x_r}{qk+r}\longrightarrow\frac{x_k}{k}.
$$

**Thus $\limsup x_n/n\leq\alpha$, while the definition gives $\liminf x_n/n\geq\alpha$. Hence $x_n/n\to\alpha$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
