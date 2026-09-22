<h1 id="6e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Unmodified [Hebbian learning](../../../../../../hebbian-learning.md) reinforces correlated input and output but has no mechanism limiting synaptic strength. The second rule adds activity-dependent negative feedback and stabilizes the [norm](../../../../../../norm.md) at an input-scale-independent value, provided the input keeps exciting the output. The third has a cubic weight penalty independent of the instantaneous output; its equilibrium [norm](../../../../../../norm.md) instead depends on the strength of the input [second moment](../../../../../../second-moment.md).

For the third averaged rule, an equilibrium along [eigenvector](../../../../../../eigenvector.md) $i$ has radial linearized [eigenvalue](../../../../../../eigenvalue.md) $-2\lambda_i/\tau$ and transverse [eigenvalues](../../../../../../eigenvalue.md) $(\lambda_j-\lambda_i)/\tau$. Thus a positive simple largest [eigenvalue](../../../../../../eigenvalue.md) gives stable equilibria in its two opposite directions, whereas lower eigen-directions are unstable to larger components. With generic initial weights, it learns the dominant correlation direction, linking the rule to [principal component analysis](../../../../../../principal-component-analysis.md). These are idealized normalization and feature-extraction mechanisms, not claims that biological synapses implement these exact equations.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
