<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An [instrumental variable](../../../../../../instrumental-variable.md) $G$ supplies variation in an [exposure](../../../../../../exposure.md) $B$ that can be used for [causal inference](../../../../../../causal-inference-split.md) about its effect on $Y$. Its three core requirements are:

- **[Instrument relevance](../../../../../../instrument-relevance.md):** $G$ changes the distribution of $B$; in a simple linear model this requires a nonzero first-stage association.
- **[Instrumental-variable independence](../../../../../../instrumental-variable-independence.md):** $G$ is independent of unmeasured common causes of $B$ and $Y$, or independent of the relevant [potential outcomes](../../../../../../potential-outcome.md) conditional on specified measured covariates.
- **[Exclusion restriction](../../../../../../exclusion-restriction.md):** interventions on $G$ affect $Y$ only through $B$, with no other causal pathway. In [potential outcomes](../../../../../../potential-outcome.md) notation, $Y(b,g)=Y(b)$.

**Relevance, independence, and exclusion are the core instrumental-variable assumptions.** They do not by themselves identify an arbitrary population-average effect. For a binary instrument and treatment, [instrumental-variable monotonicity](../../../../../../instrumental-variable-monotonicity.md) and the usual [consistency in causal inference](../../../../../../consistency-in-causal-inference.md) assumptions can identify a [local average treatment effect](../../../../../../local-average-treatment-effect.md); stronger effect-homogeneity or structural-model assumptions are needed for other effect interpretations.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
