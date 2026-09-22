<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A training observation is misclassified only if

$$
Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq0.
$$

The SVM constraint then forces $\widehat\xi_i\geq1$. Hence

$$
\mathbf1_{\{Y_i(\widehat\alpha+X_i^\top\widehat\beta)\leq0\}}
\leq\widehat\xi_i.
$$

Summing and dividing by $n$ proves $\widehat{\operatorname{Err}}_{\mathrm{tr}}\leq n^{-1}\sum_i\widehat\xi_i$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
