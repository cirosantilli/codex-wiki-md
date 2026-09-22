<h1 id="2/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let there be $k$ inner [lists](../../../../../../list-abstract-data-type.md), of lengths $\ell_1,\ldots,\ell_k$, and let $N=\sum_j\ell_j$. Evaluate the whole output [list](../../../../../../list-abstract-data-type.md) spine, taking each input element as an already available value. The defining equation `(x:xs) ++ ys = x : (xs ++ ys)` shows that [list concatenation](../../../../../../list-concatenation.md) traverses its left operand, sharing its right operand.

The [right fold](../../../../../../list-fold.md) puts each original inner [list](../../../../../../list-abstract-data-type.md) on the left of exactly one concatenation. Thus its total element traversal is proportional to $N$, and visiting the outer [list](../../../../../../list-abstract-data-type.md) costs $k$:

$$
\boxed{T_{\mathrm{right}}=\Theta(k+N).}
$$

The $k$ term matters when many inner [lists](../../../../../../list-abstract-data-type.md) are empty. With $k$ rows each of length $r$, the bound is $\Theta(k+kr)$. In particular, with uniformly bounded positive row length it is linear in $k$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
