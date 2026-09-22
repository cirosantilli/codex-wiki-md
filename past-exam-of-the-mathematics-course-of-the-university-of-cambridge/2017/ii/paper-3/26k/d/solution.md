<h1 id="26k/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The almost-sure bound gives $\tilde\theta_n-\hat\theta_n=o_{\mathbb P}(n^{-1/2})$, so [Slutsky theorem](../../../../../../slutsky-theorem.md) transfers both consistency and the asymptotic normal law to $\tilde\theta_n$. The [continuous mapping theorem](../../../../../../continuous-mapping-theorem.md) and [delta method](../../../../../../delta-method.md) then give

$$
\boxed{\psi(\tilde\theta_n)\xrightarrow{\mathbb P}\psi(\theta_0),\qquad
\sqrt n\bigl(\psi(\tilde\theta_n)-\psi(\theta_0)\bigr)
 \xrightarrow{d}\mathcal N\!\left(0,\frac{\psi'(\theta_0)^2}{I(\theta_0)}\right).}
$$

If $\psi'(\theta_0)=0$, the latter is the [Dirac measure](../../../../../../dirac-measure.md) at zero, conventionally a degenerate [normal distribution](../../../../../../normal-distribution.md); a nondegenerate second-order [limit](../../../../../../limit-of-a-function.md) would need a different normalization and extra smoothness.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
