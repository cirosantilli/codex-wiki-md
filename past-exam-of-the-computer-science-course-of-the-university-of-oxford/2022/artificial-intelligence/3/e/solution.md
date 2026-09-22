<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The conventional worst-case estimate is the [backtracking leaf bound](../../../../../backtracking-leaf-bound.md) given by the [product](../../../../../product-of-numbers.md) of the initial [constraint domain](../../../../../constraint-domain.md) sizes. Before exploiting any attacking-queen constraints, the three models give respectively

$$
\boxed{2^{N^2},\qquad (N^2)^N=N^{2N},\qquad N^N.}
$$

Model 1 has $N^2$ binary choices. Model 2 has $N$ labeled queens with $N^2$ possible cells each. Model 3 has $N$ row variables with $N$ possible columns each. The [rule of product](../../../../../rule-of-product.md) gives the displayed bounds; assigning variables in one prescribed order avoids multiplying again by the number of variable orderings.

With $k$ mutually nonattacking prescribed queens incorporated as singleton [constraint domains](../../../../../constraint-domain.md), the corresponding bounds improve to

$$
\boxed{2^{N^2-k},\qquad N^{2(N-k)},\qquad N^{N-k}.}
$$

In Model 1 only the $k$ prescribed occupied cells have been fixed in this estimate; immediate deletion of attacked cells tightens it further. In Model 3 consistent clues occupy $k$ distinct rows. If the clues are inconsistent, preprocessing can reject the instance immediately.

These are **upper bounds on leaves, rather than exact attained counts for a fully specified pruning implementation**. Ordinary [backtracking](../../../../../backtracking.md) rejects inconsistent partial assignments and often creates far fewer leaves; a stopped branch is itself a leaf even if not all variables were assigned. Such early leaves still obey the [backtracking leaf bound](../../../../../backtracking-leaf-bound.md), since distinct leaves describe disjoint nonempty families of full domain assignments when constraints are ignored. Counting only possible complete nonattacking assignments is a different question. For example, row/column restrictions alone reduce full assignments to at most $N!$ in Model 3, but that number does not directly count failed partial leaves. Exact counts depend on variable ordering and [constraint propagation](../../../../../constraint-propagation.md), neither of which is specified.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
