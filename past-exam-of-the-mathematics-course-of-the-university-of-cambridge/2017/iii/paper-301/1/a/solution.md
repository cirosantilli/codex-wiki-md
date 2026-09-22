<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [natural units](../../../../../../natural-units.md) $\hbar=c=1$ and the [Minkowski metric](../../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(1,-1,-1,-1)$ throughout. An Abelian [gauge transformation](../../../../../../gauge-transformation.md) is $A_\mu\mapsto A_\mu+\partial_\mu\chi$. For a sufficiently regular $\chi$, commuting the [partial derivatives](../../../../../../partial-derivative.md) gives $F_{\mu\nu}\mapsto F_{\mu\nu}$, so the [Maxwell Lagrangian](../../../../../../maxwell-lagrangian.md) is invariant pointwise.

Vary the [action](../../../../../../action.md) with respect to the [electromagnetic four-potential](../../../../../../electromagnetic-four-potential.md), using variations of [compact support](../../../../../../compact-support.md) or vanishing on the [boundary](../../../../../../boundary-of-a-set.md). The antisymmetry of the [electromagnetic field tensor](../../../../../../electromagnetic-field-tensor.md) gives

$$
\delta\mathcal L=-\frac12F^{\mu\nu}\delta F_{\mu\nu}=-F^{\mu\nu}\partial_\mu\delta A_\nu.
$$

After [integration by parts](../../../../../../integration-by-parts.md), $\delta S=\int d^4x\,(\partial_\mu F^{\mu\nu})\delta A_\nu$. The [principle of stationary action](../../../../../../principle-of-stationary-action.md) therefore gives the source-free [Maxwell equations](../../../../../../maxwell-equations.md),

$$
\boxed{\partial_\mu F^{\mu\nu}=0\iff\Box A^\nu-\partial^\nu(\partial_\mu A^\mu)=0.}
$$

In the [Lorenz gauge](../../../../../../lorenz-gauge-condition.md), $\partial_\mu A^\mu=0$, this becomes $\Box A_\nu=0$ with $\Box=\partial_\mu\partial^\mu$. The PDF's name “Lorentz gauge” denotes the usual [Lorenz gauge](../../../../../../lorenz-gauge-condition.md), named after Lorenz. Residual [gauge transformations](../../../../../../gauge-transformation.md) preserve it when $\Box\chi=0$; this condition is not itself a complete removal of the gauge freedom.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
