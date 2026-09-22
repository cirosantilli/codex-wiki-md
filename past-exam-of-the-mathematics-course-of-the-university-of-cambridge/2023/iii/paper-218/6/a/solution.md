<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The binary [regression functions](../../../../../../regression-function.md) are the [conditional class probabilities](../../../../../../conditional-class-probability.md)

$$
\eta_1(x)=\mathbb P(Y=1\mid X=x)=\mathbb E(Y\mid X=x),
\qquad
\eta_0(x)=1-\eta_1(x).
$$

Under zero-one loss, the [Bayes classifier](../../../../../../bayes-classifier.md) is

$$
C^*(x)=\mathbf1_{\{\eta_1(x)\geq1/2\}},
$$

with arbitrary tie breaking. Its [Bayes decision boundary](../../../../../../bayes-decision-boundary.md) is

$$
\boxed{\{x:\eta_1(x)=\eta_0(x)\}
=\{x:\eta_1(x)=1/2\}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
