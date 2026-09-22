<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume $X$ is [square-integrable](../../../../../square-integrable-function.md). Since $X$ and $Y$ have the same [probability distribution](../../../../../probability-distribution-split.md), $Y$ is also [square-integrable](../../../../../square-integrable-function.md) and $\mathbb E[Y^2]=\mathbb E[X^2]$. The product $XY$ is [integrable](../../../../../integrability.md) by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md).

We use the defining test-function identity for [conditional expectation](../../../../../conditional-expectation.md): for bounded $\mathcal G$-[measurable](../../../../../measurability.md) $H$, $\mathbb E[XH]=\mathbb E[YH]$. Take $H=Y\mathbf1_{\{|Y|\leq m\}}$ and let $m\to\infty$. The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), with bounds $|XY|$ and $Y^2$, gives

$$
\mathbb E[XY]=\mathbb E[Y^2].
$$

This is the extension of the [conditional expectation](../../../../../conditional-expectation.md) pull-out identity to this [square-integrable](../../../../../square-integrable-function.md) multiplier. Consequently

$$
\mathbb E[(X-Y)^2]
=\mathbb E[X^2]-2\mathbb E[XY]+\mathbb E[Y^2]
=\mathbb E[X^2]-\mathbb E[Y^2]=0.
$$

A nonnegative [random variable](../../../../../random-variable-split.md) with zero [expectation](../../../../../expected-value-split.md) is zero [almost surely](../../../../../almost-sure-convergence.md). Hence

$$
\boxed{X=Y\quad\text{almost surely}.}
$$

Geometrically, this is the equality case in the [L2 space](../../../../../l2-space-is-a-hilbert-space.md) [orthogonal projection](../../../../../orthogonal-projection.md) interpretation of [conditional expectation](../../../../../conditional-expectation.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability, measure and martingales course of the University of Oxford](../../../../split.md)
6. [Probability, measure and martingales course of the University of Oxford](../../../../../probability-measure-and-martingales-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
