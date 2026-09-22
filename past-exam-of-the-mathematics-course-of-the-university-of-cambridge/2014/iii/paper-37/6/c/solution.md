<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the usual nonempty-[clause](../../../../../../clause-of-a-boolean-formula.md) convention and normalize repeated [literals](../../../../../../boolean-literal.md) within a [clause](../../../../../../clause-of-a-boolean-formula.md); tautologies are always satisfied. If empty [clauses](../../../../../../clause-of-a-boolean-formula.md) are admitted, discard them first: they contribute nothing to any assignment or to the optimum. Let $m$ be the resulting number of [clause](../../../../../../clause-of-a-boolean-formula.md) occurrences.

Assign independent fair truth values. A singleton [clause](../../../../../../clause-of-a-boolean-formula.md) is satisfied with [probability](../../../../../../probability.md) $1/2$, a proper two-variable [clause](../../../../../../clause-of-a-boolean-formula.md) with [probability](../../../../../../probability.md) $3/4$, and a tautology with [probability](../../../../../../probability.md) one. By [linearity of expectation](../../../../../../linearity-of-expectation.md), the expected number satisfied is at least $m/2$, hence at least $\mathrm{OPT}/2$.

To derandomize, use the [method of conditional probabilities](../../../../../../method-of-conditional-probabilities.md). After some variables have been fixed, let $F$ be the conditional expected number of satisfied [clauses](../../../../../../clause-of-a-boolean-formula.md). For the next variable the two [conditional expectations](../../../../../../conditional-expectation.md) $F_0,F_1$ satisfy $F=(F_0+F_1)/2$. Fix the value with the larger expectation. This never decreases $F$. When all variables have been fixed, $F$ is the actual integer number of satisfied [clauses](../../../../../../clause-of-a-boolean-formula.md), so

$$
\boxed{\text{the algorithm satisfies at least }m/2\ge\mathrm{OPT}/2\text{ clauses}.}
$$

Compute each [conditional expectation](../../../../../../conditional-expectation.md) by summing the [probabilities](../../../../../../probability.md) of the [clauses](../../../../../../clause-of-a-boolean-formula.md). Each has at most two variables, so its contribution is computed in constant time; scanning all [clauses](../../../../../../clause-of-a-boolean-formula.md) for each variable gives $O(nm)$ arithmetic operations. This is a polynomial-time [approximation algorithm](../../../../../../approximation-algorithm.md) with [approximation ratio](../../../../../../approximation-ratio.md) $1/2$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
