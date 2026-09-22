<h1 id="30j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The stopping rule ensures that the returned function belongs to

$$
\mathcal H
=\left\{\sum_{m=1}^M\beta_mh_m:
\beta_m\geq0,\ \sum_m\beta_m\leq1,\ h_m\in B\right\}.
$$

Indeed, when adding the next coefficient would make the sum exceed one, the algorithm returns the preceding sum, and at the first step it returns zero.

Since each $h_m$ takes values in $\{-1,1\}$, every $f\in\mathcal H$ satisfies $|f(x)|\leq1$. On $[-1,1]$, the map $z\mapsto e^{-z}$ is $\exp(1)$-Lipschitz. The expected [Rademacher complexity](../../../../../../rademacher-complexity.md) generalization inequality followed by the [Rademacher contraction lemma](../../../../../../rademacher-contraction-lemma.md) gives

$$
\mathbb ER_\phi(\widehat f)
\leq\mathbb E\widehat R_\phi(\widehat f)
+2e\,\mathbb E\widehat R(\mathcal H(X_{1:n})).
$$

A linear functional attains the same supremum over a set and its convex hull. Since $B=-B$, adjoining zero and allowing total coefficient at most one does not increase the supremum, so the [Rademacher complexity of a convex hull](../../../../../../rademacher-complexity-of-a-convex-hull.md) gives

$$
\widehat R(\mathcal H(x_{1:n}))
\leq\widehat R(B(x_{1:n}))
\leq r_B.
$$

Combining the two bounds proves

$$
\boxed{
\mathbb ER_\phi(\widehat f)
\leq\mathbb E\widehat R_\phi(\widehat f)+2\exp(1)r_B}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30J](../../30j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
