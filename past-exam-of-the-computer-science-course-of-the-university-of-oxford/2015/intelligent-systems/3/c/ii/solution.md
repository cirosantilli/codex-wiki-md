<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**True in some cases and false in others:** the two numerical inequalities do not guarantee a solution.

For an unsatisfiable example satisfying both inequalities, take six [variables](../../../../../../variable-mathematics.md), a [constraint domain](../../../../../../constraint-domain.md) with five values, and $k=4$, $m=3$, with [all-different constraints](../../../../../../all-different-constraint.md) on

$$
\{X_1,X_2,X_3,X_4\},\qquad
\{X_1,X_2,X_5,X_6\},\qquad
\{X_3,X_4,X_5,X_6\}.
$$

Any pair of the six [variables](../../../../../../variable-mathematics.md) occurs together in at least one of these scopes: view the [variables](../../../../../../variable-mathematics.md) as the three pairs $\{1,2\},\{3,4\},\{5,6\}$, and each scope as the union of two pairs. All six values must therefore be distinct. This is impossible with five available values, even though $5>4$ and $5>3$.

For a satisfiable example with the same $k,m,|D|$, take three disjoint groups of four [variables](../../../../../../variable-mathematics.md) and impose one [all-different constraint](../../../../../../all-different-constraint.md) on each group. Assign values $1,2,3,4$ separately in every group. All three constraints hold with $D=\{1,2,3,4,5\}$.

$$
\boxed{|D|>k\text{ and }|D|>m\text{ are insufficient.}}
$$

These examples concern the intended cases in which the antecedent holds; they do not rely on vacuous truth of an implication.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Intelligent systems](../../../../intelligent-systems-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
