<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the intended [hierarchical Bayesian model](../../../../../../hierarchical-bayesian-model.md): the breed parameters are conditionally independent given $\alpha,\beta$, and observations are independent given their breed parameters. Put $m_i=\max(\beta,M_i)$. The [uniform-Pareto model evidence](../../../../../../uniform-pareto-model-evidence.md) factorizes over breeds:

$$
\boxed{p(\mathbf y_1,\ldots,\mathbf y_I\mid\alpha,\beta)
=\prod_{i=1}^I\frac{\alpha\beta^\alpha}
{(\alpha+n_i)m_i^{\alpha+n_i}}.}
$$

Identical marginal [prior distributions](../../../../../../prior-probability.md) alone would not determine this product; [conditional independence](../../../../../../conditional-independence.md) is the additional assumption.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
