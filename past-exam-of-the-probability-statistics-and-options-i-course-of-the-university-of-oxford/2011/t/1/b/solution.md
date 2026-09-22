<h1 id="t/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $x^*=(0,3,4,0,5)^T$. By [strong duality](../../../../../strong-duality.md), an optimal dual vector $y^*$ exists. [Complementary slackness](../../../../../complementary-slackness.md) at $x^*$ makes the dual constraints equalities at indices $2,3,5$, where $x_j^*>0$. The vector $\widehat x=(0,1,2,0,3)^T$ has exactly that same support. It is nonnegative and satisfies $A\widehat x=\widehat b$, while $y^*$ remains dual feasible because dual feasibility depends on $A,c$, not on the right-hand side. Hence

$$
c^T\widehat x=(A^Ty^*)^T\widehat x=\widehat b^Ty^*.
$$

The objective gap is zero, so **$\widehat x$ is optimal for the modified programme**. This is [support-preserving right-hand-side changes in linear programming](../../../../../support-preserving-right-hand-side-changes-in-linear-programming.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [T](../../../t.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
