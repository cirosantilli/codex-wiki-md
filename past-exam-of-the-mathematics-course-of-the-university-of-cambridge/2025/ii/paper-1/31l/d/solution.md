<h1 id="31l/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [hinge loss](../../../../../../hinge-loss.md) $\phi(t)=\max(0,1-t)$ is one-Lipschitz. Centering it at zero and applying the contraction lemma gives

$$
\mathcal R_n(\phi\circ H)\leq\mathcal R_n(H).
$$

For an empirical risk minimizer and a population minimizer, the standard expected ERM inequality with the $1/n$ Rademacher convention used in part (a) is

$$
\mathbb E R_\phi(\widehat h)-R_\phi(h^*)
\leq2\mathcal R_n(\phi\circ H).
$$

Part (c) consequently yields

$$
\mathbb E R_\phi(\widehat h)-R_\phi(h^*)
\leq\frac{2C^2s}{\sqrt n}.
$$

**Thus $K=2C^2s$ for this normalization of Rademacher complexity.**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31L](../../31l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
