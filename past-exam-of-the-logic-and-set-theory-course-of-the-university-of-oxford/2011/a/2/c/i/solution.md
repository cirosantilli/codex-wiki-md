<h1 id="a/2/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Extend the [first-order variable assignment](../../../../../../first-order-variable-assignment.md) recursively to [first-order terms](../../../../../../first-order-term.md) by

$$
\widetilde v(x_i)=v(x_i),\qquad\widetilde v(f(t))=f^{\mathcal A}(\widetilde v(t)).
$$

For atomic formulas, $\mathcal A\models t=s[v]$ exactly when $\widetilde v(t)=\widetilde v(s)$. Extend to the Boolean connectives by their [truth tables](../../../../../../truth-table.md), for example implication is false exactly when its antecedent is true and its consequent false. Quantifiers use modified [first-order variable assignments](../../../../../../first-order-variable-assignment.md):

$$
\begin{aligned}
\mathcal A\models\forall x_i\,\theta[v]&\iff\text{for every }a\in A,\quad\mathcal A\models\theta[v(x_i\mapsto a)],\\
\mathcal A\models\exists x_i\,\theta[v]&\iff\text{for some }a\in A,\quad\mathcal A\models\theta[v(x_i\mapsto a)].
\end{aligned}
$$

This recursion defines [satisfaction for a set structure](../../../../../../satisfaction-for-a-set-structure.md) for every [first-order formula](../../../../../../first-order-formula.md).

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [A](../../../../a.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the logic and set theory course of the University of Oxford](../../../../../split.md)
7. [Logic and set theory course of the University of Oxford](../../../../../../logic-and-set-theory-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
