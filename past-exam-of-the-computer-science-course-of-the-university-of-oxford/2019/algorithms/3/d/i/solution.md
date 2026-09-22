<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume the standard nonempty instance convention $1\leq k\leq n$, and set $d(v,v)=0$. Start with no centers. Pick any city still farther than $2r^*$ from every selected center, add it as a center, and mark every city within distance $2r^*$ of it as covered. Stop when all cities are covered.

Distinct chosen centers have pairwise distance greater than $2r^*$. Fix an optimal [set](../../../../../../set-split.md) of $k$ centers and assign each city to one optimal center within distance $r^*$. Two cities assigned to the same center have distance at most $2r^*$ by the [triangle inequality](../../../../../../triangle-inequality.md). Thus no two chosen centers can be assigned to that same optimal center. The [pigeonhole principle](../../../../../../pigeonhole-principle.md) shows that **the greedy procedure selects at most $k$ centers and has radius at most $2r^*$**. If fewer than $k$ are selected, add arbitrary distinct cities; this cannot worsen the radius.

With the supplied radius, a straightforward implementation updates coverage in $O(n)$ time per selected center, hence takes $O(nk)$ distance tests. The argument also handles $r^*=0$. It is the packing bound underlying the [metric k-center problem](../../../../../../metric-k-center-problem.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
