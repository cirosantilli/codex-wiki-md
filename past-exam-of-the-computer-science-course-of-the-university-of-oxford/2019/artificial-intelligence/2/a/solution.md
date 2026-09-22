<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $Q=\{1,\ldots,n\}^2$ be the board squares and let $\operatorname{Attack}(p,q)$ mean that the absolute coordinate differences are $(1,2)$ or $(2,1)$.

**One [variable](../../../../../variable-mathematics.md) per knight.** Use $X_1,\ldots,X_k$, with each [constraint domain](../../../../../constraint-domain.md) equal to $Q$. For every pair $i<j$, require

$$
X_i\ne X_j,\qquad\neg\operatorname{Attack}(X_i,X_j).
$$

Every satisfying assignment places $k$ distinct nonattacking knights, and any such placement gives an assignment after labelling its knights. This has only $k$ [variables](../../../../../variable-mathematics.md) and $O(k^2)$ [binary constraints](../../../../../binary-constraint.md), but domains of size $n^2$. Relabelling the knights gives $k!$ assignments for the same unlabelled board, so the representation contains considerable redundancy.

**One [Boolean variable](../../../../../boolean-variable.md) per square.** Use $Y_q\in\{0,1\}$ for every $q\in Q$. Impose the [cardinality constraint](../../../../../cardinality-constraint.md)

$$
\sum_{q\in Q}Y_q=k,
$$

and for every knight-attack pair $p,q$ impose $Y_p+Y_q\leq1$. There are $n^2$ [variables](../../../../../variable-mathematics.md), each with a two-element [constraint domain](../../../../../constraint-domain.md), and only $O(n^2)$ local attack restrictions, because each square attacks at most eight others. The single counting constraint is a global constraint, not a [binary constraint](../../../../../binary-constraint.md).

The square encoding avoids knight-label redundancy and has sparse local attack relations; the knight encoding uses fewer [variables](../../../../../variable-mathematics.md) when $k$ is small and makes single-knight moves natural. Both are exact representations of the [nonattacking knights problem](../../../../../nonattacking-knights-problem.md). Neither may impose one knight per row: several knights can legally share a row.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
