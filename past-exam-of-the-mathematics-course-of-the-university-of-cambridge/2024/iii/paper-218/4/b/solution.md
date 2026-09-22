<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [separating hyperplane](../../../../../../separating-hyperplane.md) for signed data satisfies $Y_i(\gamma_0+X_i^T\beta)>0$ for every $i$; its geometric set is $\{x:\gamma_0+x^T\beta=0\}$. The plot marks three [support vectors](../../../../../../support-vector.md). At the shown fit they lie on the two [support-vector-machine margin boundaries](../../../../../../support-vector-machine-margin-boundaries.md), so their signed functional margins satisfy

$$
Y_iX_i^{*T}\widehat\gamma=1.
$$

The solid line is the decision hyperplane $X^{*T}\widehat\gamma=0$, while the dashed parallel lines are $X^{*T}\widehat\gamma=1$ and $X^{*T}\widehat\gamma=-1$.

If $\lambda=0$, every parameter vector with all margins at least one has zero hinge loss. Scaling or changing a separating vector can therefore give another minimizer, so the objective need not select the displayed maximum-margin direction or the same three lines. Positive quadratic regularization selects a finite, minimum-norm compromise.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
