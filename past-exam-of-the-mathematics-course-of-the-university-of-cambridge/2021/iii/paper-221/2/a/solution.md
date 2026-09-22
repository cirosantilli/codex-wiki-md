<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Conditionally on $X$, a valid [instrumental variable](../../../../../../instrumental-variable.md) $Z$ must satisfy three core conditions.

- [Instrument relevance](../../../../../../instrument-relevance.md): $Z$ changes the conditional distribution of $A$, for example $\operatorname{Cov}(Z,A\mid X)\ne0$ on a set of positive probability.
- [Instrumental-variable independence](../../../../../../instrumental-variable-independence.md): $Z$ is independent of latent outcome causes and the relevant [potential outcomes](../../../../../../potential-outcome.md), for example $Z\mathrel\perp\{Y(a):a\}\mid X$.
- The [exclusion restriction](../../../../../../exclusion-restriction.md): $Z$ affects $Y$ only through $A$, written $Y(a,z)=Y(a)$.

Together with [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md) and [positivity in causal inference](../../../../../../positivity-assumption.md), these assumptions make variation in $A$ induced by $Z$ causally interpretable. In the displayed graph, relevance is the edge $Z\to A$, independence is the absence of a path from $Z$ to $U$ after conditioning on $X$, and exclusion is the absence of a direct $Z\to Y$ edge.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
