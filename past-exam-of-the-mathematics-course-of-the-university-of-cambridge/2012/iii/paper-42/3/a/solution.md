<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [decision problem](../../../../../../decision-problem.md) belongs to [NP](../../../../../../np-complexity.md) if every yes-instance has a polynomial-length certificate verifiable by a deterministic [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md). It is [NP-hard](../../../../../../np-hardness.md) if every problem in [NP](../../../../../../np-complexity.md) has a [polynomial-time many-one reduction](../../../../../../polynomial-time-many-one-reduction.md) to it. It is [NP-complete](../../../../../../np-completeness.md) if it is both [NP-hard](../../../../../../np-hardness.md) and in [NP](../../../../../../np-complexity.md).

A [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md) for any [NP-complete](../../../../../../np-completeness.md) problem would therefore give one for every problem in [NP](../../../../../../np-complexity.md), implying $\mathrm P=\mathrm{NP}$. Conversely, if $\mathrm P=\mathrm{NP}$, all [NP-complete](../../../../../../np-completeness.md) decision problems have polynomial-time algorithms. **[NP-completeness](../../../../../../np-completeness.md) does not unconditionally prove that polynomial-time solution is impossible.** Optimization problems such as minimum tour cost are described as [NP-hard](../../../../../../np-hardness.md), while their threshold decision versions can be [NP-complete](../../../../../../np-completeness.md).

For a minimization problem with nonnegative costs, an [approximation algorithm](../../../../../../approximation-algorithm.md) of ratio $\alpha\geq1$ is a [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md) returning a feasible solution of cost at most $\alpha$ times the optimum on every instance. For maximization, one often uses $\alpha\geq1$ with value at least $\mathrm{OPT}/\alpha$; an equivalent convention uses ratios at most one. The metric-tour question uses the minimization convention.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
