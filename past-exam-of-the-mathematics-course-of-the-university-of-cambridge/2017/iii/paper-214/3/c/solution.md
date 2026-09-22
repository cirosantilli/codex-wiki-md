<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Group the random resistance cost by unoriented [edges](../../../../../../edge-of-a-graph.md). For $e=\{x,y\}$, its resistance contributes once whenever the walk traverses it in either direction. Pathwise,

$$
\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=\sum_{\{x,y\}\in E}R_{\mathrm{eff}}(x,y)\bigl(S(x,y)+S(y,x)\bigr).
$$

The [graph](../../../../../../graph-split.md) is finite and the commute has finite [expected value](../../../../../../expected-value.md). [Linearity of expectation](../../../../../../linearity-of-expectation.md), or [Tonelli theorem](../../../../../../tonelli-theorem.md) for these nonnegative terms, therefore permits taking expectations of the sum. By the [directed edge occupation in a random-walk commute](../../../../../../directed-edge-occupation-in-a-random-walk-commute.md), both directed traversal counts have [expected value](../../../../../../expected-value.md) $R_{\mathrm{eff}}(a,z)$. Thus

$$
\mathbb E_a\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=2R_{\mathrm{eff}}(a,z)\sum_{e\in E}R_{\mathrm{eff}}(e).
$$

Apply [Foster's theorem](../../../../../../foster-s-theorem.md) from part (a) to obtain

$$
\boxed{\mathbb E_a\sum_{t=0}^{\tau-1}R_{\mathrm{eff}}(X_t,X_{t+1})=2(n-1)R_{\mathrm{eff}}(a,z).}
$$

The factor two counts the two orientations of each [edge](../../../../../../edge-of-a-graph.md). It would be lost by treating the expected directed count in part (b) as an expected count for both directions together. The same distinct-terminal and simple-random-walk conventions from part (b) remain in force.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 214](../../../paper-214-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
