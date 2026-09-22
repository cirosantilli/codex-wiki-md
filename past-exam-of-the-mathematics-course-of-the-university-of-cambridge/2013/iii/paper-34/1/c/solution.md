<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The joint [prior predictive distribution](../../../../../../bayesian-model-evidence.md) is the [Bayesian model evidence](../../../../../../bayesian-model-evidence.md), obtained by integrating over the shared parameter:

$$
\begin{aligned}
p(\mathbf y\mid\alpha,\beta)
&=\alpha\beta^\alpha\int_{\max(\beta,M)}^\infty
\theta^{-(\alpha+n+1)}\,d\theta\\
&=\boxed{\frac{\alpha\beta^\alpha}
{(\alpha+n)\max(\beta,M)^{\alpha+n}}},
\qquad y_j>0.
\end{aligned}
$$

It is zero otherwise. This [uniform-Pareto model evidence](../../../../../../uniform-pareto-model-evidence.md) is a joint density, not the product of separately marginalized observation densities: mixing over the common parameter induces dependence.

## ↑ Ancestors (11)

1. [C](../c.md)
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
