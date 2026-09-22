<h1 id="5j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For log-likelihood $\ell(\beta;Y)$, the [score function](../../../../../../informant-function.md) and [Fisher information matrix](../../../../../../fisher-information-matrix.md) are

$$
U(\beta)=\nabla_\beta\ell(\beta;Y),
\qquad
\mathcal I(\beta)
=-\mathbb E_\beta[\nabla_\beta^2\ell(\beta;Y)]
=\operatorname{cov}_\beta(U(\beta)).
$$

The [Fisher scoring](../../../../../../scoring-algorithm.md) iteration replaces the observed Hessian in Newton's method by its expectation:

$$
\boxed{\beta^{(m+1)}
=\beta^{(m)}
+\mathcal I(\beta^{(m)})^{-1}U(\beta^{(m)})}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5J](../../5j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
