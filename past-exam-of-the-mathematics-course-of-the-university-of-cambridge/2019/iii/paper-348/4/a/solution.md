<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [probability measures](../../../../../../probability-measure.md) $\mu,\nu$ on $\mathbb R^d$ with finite second [moments](../../../../../../moment.md), the [Knott–Smith optimality criterion](../../../../../../knott-smith-optimality-criterion.md) states that a [transport plan](../../../../../../transport-plan.md) $\pi\in\Pi(\mu,\nu)$ minimizes the quadratic cost $|x-y|^2$ if and only if there is a [proper convex function](../../../../../../proper-convex-function.md) $\Phi:\mathbb R^d\to\mathbb R\cup\{+\infty\}$ that is [sequentially lower semicontinuous](../../../../../../sequential-lower-semicontinuity.md) and satisfies

$$
\boxed{y\in\partial\Phi(x)\quad\text{for }\pi\text{-almost every }(x,y).}
$$

The [subdifferential](../../../../../../subdifferential.md) is characterized by

$$
y\in\partial\Phi(x)\quad\Longleftrightarrow\quad
\Phi(z)\geq\Phi(x)+y\cdot(z-x)\quad\text{for every }z\in\mathbb R^d,
$$

with $\Phi(x)<\infty$. Thus the [transport plan](../../../../../../transport-plan.md) is concentrated on the graph of the [subdifferential](../../../../../../subdifferential.md). No [absolute continuity of measures](../../../../../../absolute-continuity-of-measures.md) assumption on $\mu$ is needed. Multiplying the cost by $1/2$ leaves the criterion unchanged. The original quadratic optimal mapping result is [Knott and Smith, On the optimal mapping of distributions](https://link.springer.com/article/10.1007/BF00934745).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
