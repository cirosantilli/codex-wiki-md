<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [independent and identically distributed](../../../../independent-and-identically-distributed-random-variables.md) hypothesis factors the [joint probability mass function](../../../../joint-probability-mass-function.md):

$$
p_n(X_1,\ldots,X_n)=\prod_{i=1}^np(X_i),\qquad
\frac1n\log p_n(X_1,\ldots,X_n)=\frac1n\sum_{i=1}^n\log p(X_i).
$$

Symbols outside the [support of a probability distribution](../../../../support-of-a-probability-distribution.md) $p$ never occur, almost surely. On its finite positive [probability support](../../../../support-of-a-probability-distribution.md), $\log p(X_i)$ is bounded, so the [strong law of large numbers](../../../../strong-law-of-large-numbers.md) applies:

$$
\boxed{\frac1n\log p_n(X_1,\ldots,X_n)\longrightarrow
\sum_{x:p(x)>0}p(x)\log p(x)=-H(p)\quad\text{almost surely}.}
$$

This is the [asymptotic equipartition property](../../../../asymptotic-equipartition-property.md) with the sign appropriate to a [logarithm](../../../../logarithm.md) of a [probability mass](../../../../probability-mass.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
