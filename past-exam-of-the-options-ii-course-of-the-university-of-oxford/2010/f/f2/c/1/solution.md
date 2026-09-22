<h1 id="f/f2/c/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work on the positive orthant, where all real powers in $g$ are defined. To justify a global maximum, enlarge the constraint set to the compact simplex

$$
K=\{x_i\geq0:\sum_i p_ix_i=1\}.
$$

It is closed and bounded since $x_i\leq1/p_i$. The product $g$ extends continuously to $K$, is zero at every boundary point where a coordinate vanishes, and equals $1$ at $(1,\ldots,1)$. Hence a maximum exists and lies in the positive interior. For $n=1$ the constraint gives $x_1=1$ directly.

For $n\geq2$, at an interior maximum the [Lagrange multiplier](../../../../../../lagrange-multiplier.md) equations are

$$
\partial_i g=\frac{p_ig}{x_i}=\lambda p_i.
$$

All $p_i$ and $g$ are positive, so all $x_i$ are equal. The constraint and $\sum_i p_i=1$ make their common value $1$. Thus the only possible maximizer has value $1$, proving

$$
\boxed{g(x)\leq1\quad\text{on }M,}
$$

with equality exactly when every $x_i=1$. The source writes $g$ on all of $\mathbb R^n$; for general noninteger exponents its relevant real-valued domain is the positive orthant used here.

## ↑ Ancestors (14)

1. [1](../1.md)
2. [C](../../c.md)
3. [F2](../../../f2.md)
4. [F](../../../../f.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
