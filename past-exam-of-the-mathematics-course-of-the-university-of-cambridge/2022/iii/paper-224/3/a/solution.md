<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [type](../../../../../../type-information-theory.md) of $x_1^n\in A^n$ is its empirical mass function

$$
\widehat P_{x_1^n}(a)
=\frac1n\sum_{i=1}^n\mathbf1_{\{x_i=a\}},
\qquad a\in A.
$$

For a product source $Q^{\otimes n}$,

$$
\begin{aligned}
Q^{\otimes n}(x_1^n)
&=\prod_{i=1}^nQ(x_i)
=\prod_{a\in A}Q(a)^{n\widehat P_{x_1^n}(a)}\\
&=2^{-n\{H(\widehat P_{x_1^n})+D(\widehat P_{x_1^n}\Vert Q)\}},
\end{aligned}
$$

with the usual convention that the probability is zero if the string uses a symbol outside the support of $Q$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
