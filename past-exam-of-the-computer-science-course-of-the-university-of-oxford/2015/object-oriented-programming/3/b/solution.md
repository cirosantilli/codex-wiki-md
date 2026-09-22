<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let brick $i$ have positive [integer](../../../../../integer-split.md) width $w_i$. Regard its horizontal occupied region as $[x_i,x_i+w_i)$ and its vertical occupied region as $[y_i,y_i+1)$. These [half-open interval](../../../../../half-open-interval.md) conventions allow adjoining bricks to touch without overlapping. Since the vertical coordinates are [integers](../../../../../integer-split.md), two bricks can overlap only when they are on the same row. A suitable [predicate](../../../../../predicate.md) is

$$
\boxed{\operatorname{valid}(W)\iff
\forall i\ne j,\quad
 y_i\ne y_j\ \lor\ x_i+w_i\le x_j\ \lor\ x_j+w_j\le x_i.}
$$

Positive widths and nonnegative [integer](../../../../../integer-split.md) heights are the underlying domain conditions for a wall built on the baseplate. Distinct members of the [set](../../../../../set-split.md) are compared even if their `Brick` references happen to be identical: one brick specification can describe several placements. Testing [object identity](../../../../../object-identity.md) alone would miss two overlapping placements of the same specification.

For example, width-two bricks beginning at 0 and 2 on the same row satisfy the [predicate](../../../../../predicate.md); beginnings at 0 and 1 do not. The non-strict separation inequalities are essential because touching edges are permitted.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
