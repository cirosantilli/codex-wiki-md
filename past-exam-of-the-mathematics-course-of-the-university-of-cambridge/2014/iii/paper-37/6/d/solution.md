<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply the condition after the usual [clause](../../../../../../clause-of-a-boolean-formula.md) normalization, so each variable has at most one singleton [clause](../../../../../../clause-of-a-boolean-formula.md). For a variable with such a [clause](../../../../../../clause-of-a-boolean-formula.md), make its favored [literal](../../../../../../boolean-literal.md) true with [probability](../../../../../../probability.md) $p>1/2$; for other variables use a fair value. Make these choices independently. Then every singleton is satisfied with [probability](../../../../../../probability.md) $p$.

Each [literal](../../../../../../boolean-literal.md) of a proper two-variable [clause](../../../../../../clause-of-a-boolean-formula.md) is true with [probability](../../../../../../probability.md) at least $1-p$. Independence bounds the [probability](../../../../../../probability.md) that both are false by $p^2$, so the [clause](../../../../../../clause-of-a-boolean-formula.md) is satisfied with [probability](../../../../../../probability.md) at least $1-p^2$. Tautologies have [probability](../../../../../../probability.md) one. Thus the expected fraction satisfied is at least $\min(p,1-p^2)$. One term increases and the other decreases, so their intersection maximizes this bound:

$$
p=1-p^2\quad\Longrightarrow\quad\boxed{p=\frac{\sqrt5-1}{2}\approx0.618034.}
$$

The [method of conditional probabilities](../../../../../../method-of-conditional-probabilities.md) also works with these biased [probabilities](../../../../../../probability.md): before fixing a variable, the current expectation is the weighted average of its two [conditional expectations](../../../../../../conditional-expectation.md), so choosing the larger cannot decrease it. Each [clause](../../../../../../clause-of-a-boolean-formula.md) contributes a constant-degree expression in $p$; since $p^2=1-p$, these expectations can be compared exactly in the fixed quadratic field $\mathbb Q(\sqrt5)$ with polynomial bit complexity. The final deterministic assignment therefore has

$$
\boxed{\text{approximation ratio }\frac{\sqrt5-1}{2}.}
$$

This is the [golden ratio approximation for MAX-2SAT](../../../../../../golden-ratio-approximation-for-max-2sat.md), under the stated restriction on normalized singleton [clauses](../../../../../../clause-of-a-boolean-formula.md). Arbitrary conflicting singleton [clauses](../../../../../../clause-of-a-boolean-formula.md) do not admit the same independent-bias guarantee.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
