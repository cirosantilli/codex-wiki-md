<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First recode the labels as $y_i=2Y_i-1\in\{-1,1\}$; with labels $0$ and $1$, the displayed constraints for class zero can never hold. Add an unpenalized intercept $b$ so that the separating hyperplane need not pass through the origin, and solve

$$
\min_{b,\beta}\frac12\|\beta\|_2^2
\quad\text{subject to}\quad
y_i(b+X_i^T\beta)\geq1.
$$

Centering and scaling predictor columns is also advisable because the Euclidean penalty depends on their units.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
