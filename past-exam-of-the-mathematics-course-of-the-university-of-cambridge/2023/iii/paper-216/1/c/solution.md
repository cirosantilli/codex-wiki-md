<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a decision $x$ in the [unit ball](../../../../../../unit-ball.md), [conditional expectation](../../../../../../conditional-expectation.md) under the posterior gives

$$
\mathbb E[(x^T\beta)^2\mid Y]
=x^T\mathbb E[\beta\beta^T\mid Y]x
=x^T(C+mm^T)x.
$$

The symmetric [positive semidefinite matrix](../../../../../../positive-semidefinite-matrix.md) $C+mm^T$ has a [Rayleigh quotient](../../../../../../rayleigh-quotient.md) maximized over $\lVert x\rVert\leq1$ by any unit [eigenvector](../../../../../../eigenvector.md) corresponding to its largest [eigenvalue](../../../../../../eigenvalue.md). [Bayes decision rule](../../../../../../bayes-decision-rule.md) therefore chooses any such eigenvector for the stated utility.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
