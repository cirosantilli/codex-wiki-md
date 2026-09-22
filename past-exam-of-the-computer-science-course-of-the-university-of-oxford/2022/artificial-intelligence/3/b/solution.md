<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret MyAC as doing at least one initial sweep, then repeating while the preceding sweep deleted a value. Its loop guard otherwise has no initialized truth condition. Both procedures apply the same support-based deletion rule, so both preserve every solution and terminate because finite [constraint domains](../../../../../constraint-domain.md) only shrink. Both return false on a detected empty [constraint domain](../../../../../constraint-domain.md); neither successful return establishes satisfiability.

If a sweep changes no [constraint domain](../../../../../constraint-domain.md), every directed arc has been revised against unchanged [constraint domains](../../../../../constraint-domain.md), so all arcs satisfy [arc consistency](../../../../../arc-consistency.md). Conversely, [AC-3](../../../../../ac-3.md) places every potentially affected incoming arc back on its work list after a deletion. Its empty work list therefore also establishes [arc consistency](../../../../../arc-consistency.md). When both run to successful completion, they compute the same [arc-consistency closure](../../../../../arc-consistency-closure.md), independently of revision order. To see maximality, any subdomains of the initial [constraint domains](../../../../../constraint-domain.md) that satisfy [arc consistency](../../../../../arc-consistency.md) survive every revision: each of their values retains a support inside those subdomains. Thus neither procedure can delete a value belonging to any such fixed point. Early failure may leave different intermediate [constraint domains](../../../../../constraint-domain.md), but both failures correctly prove impossibility.

Their scheduling costs differ. [AC-3](../../../../../ac-3.md) directs work toward arcs that may have lost supports, with standard [time complexity](../../../../../time-complexity.md) $O(v+ed^3)$. The [full-sweep arc consistency](../../../../../full-sweep-arc-consistency.md) method revisits all $2e$ arcs after even one remote change. There are at most $vd$ value deletions, so at most $vd+1$ sweeps; a direct implementation including a scan for empty [constraint domains](../../../../../constraint-domain.md) costs

$$
\boxed{O\bigl((vd+1)(ed^2+v)\bigr).}
$$

If empty-domain detection is maintained during revisions rather than rescanned, the familiar comparison is $O(ved^3)$ versus $O(ed^3)$, apart from initialization. These are upper bounds, not exact costs on every input.

In practice MyAC is simple and may have low overhead or benefit from a fortunate sweep order. It can also waste many scans after changes propagate slowly opposite to that order. [AC-3](../../../../../ac-3.md) incurs work-list bookkeeping but normally avoids those unrelated revisions. Both inherit the inability of [arc consistency](../../../../../arc-consistency.md) to decide arbitrary [constraint satisfaction problems](../../../../../constraint-satisfaction-problem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
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
