<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the one-layer softmax fit, write its class logits as $z_k=a_k+b_k^Tx$. Then

$$
\log\frac{p_1(x)}{p_0(x)}
=(a_1-a_0)+(b_1-b_0)^Tx.
$$

Thus an equivalent [logistic regression](../../../../../../logistic-regression.md) classifier predicts a click exactly when

$$
\delta_0+\delta^Tx\geq0,
\qquad
\delta_0=a_1-a_0,
\quad \delta=b_1-b_0.
$$

Using one reference class removes the common-logit-shift non-identifiability. Subject to the usual full-rank and no-separation conditions, the logistic parameter is identifiable. It uses four effective parameters rather than an eight-parameter redundant softmax representation, has a convex loss, and gives directly interpretable log-odds coefficients, so it is preferable for this binary linear classifier.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
