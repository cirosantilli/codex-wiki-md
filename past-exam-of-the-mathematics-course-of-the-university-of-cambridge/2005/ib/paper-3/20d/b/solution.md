<h1 id="20d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [dual linear program](../../../../../../dual-linear-program.md) is

$$
\boxed{\begin{aligned}\text{minimize }&11y_1+16y_2+29y_3,\\\text{subject to }&-3y_2+9y_3\geq4,\\&y_1+2y_2-2y_3\geq1,\\&-11y_1-7y_2+10y_3\geq-9,\\&y_1,y_2,y_3\geq0.\end{aligned}}
$$

The negatives of the final slack payoff coefficients give $\boxed{y^*=(1,2/3,2/3)}$. Its three dual constraints are equalities, and its objective is $11+32/3+58/3=41$. Equality with the primal objective proves optimality by [weak duality](../../../../../../weak-duality.md), independently of tableau sign conventions. It is also the [complementary slackness](../../../../../../complementary-slackness.md) certificate, with all primal variables and all dual variables strictly positive.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20D](../../20d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
