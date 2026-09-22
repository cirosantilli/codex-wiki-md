# Single-point exchange in polynomial minimax approximation

↑ **Parent:** [Remez algorithm](remez-algorithm.md)

Suppose a reference [polynomial](polynomial-split.md) $q$ has nonzero alternating errors of magnitude $|h|$, and another point $\eta$ has error magnitude $M>|h|$. Insert $\eta$ and delete a reference point so that the retained errors, in spatial order, still alternate. Solving the new alternation equations gives the displayed strict increase in reference height, with $w_j=\prod_{k\ne j}(z_j-z_k)^{-1}$ on the new ordered set. To prove this, apply the order-$(n+1)$ [divided difference](divided-difference.md) to the old and new degree-at-most-$n$ [polynomials](polynomial-split.md). Both vanish, so the new signed height is the sum of the old errors times $w_j$, divided by $\sum_j(-1)^jw_j$. All these signed weight products have one sign. Its absolute value is therefore the positive weighted average of one value $M$ and $n+1$ values $|h|$.

For an interior $\eta$, replace the endpoint of its containing reference interval with the same error sign. If $\eta$ is exterior, replace the nearest endpoint when the signs agree; if they disagree, insert $\eta$ and drop the farthest endpoint. These rules preserve ordered alternation. The nearest point with the same sign need not be an adjacent point on an irregular grid, and an unqualified nearest-same-sign replacement does not ensure the strict increase.

## ↑ Ancestors (7)

1. [Remez algorithm](remez-algorithm.md)
2. [Best uniform approximation](best-uniform-approximation.md)
3. [Uniform approximation](uniform-approximation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-approximation-of-functions-course-of-the-university-of-oxford/2011/3/solution.md)
- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2008/a/4/a/solution.md)
- [Solution](past-exam-of-the-approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford/2010/a/3/b/solution.md)
