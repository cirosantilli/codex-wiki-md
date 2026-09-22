<h1 id="3/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Use the [move-to-front heuristic](../../../../../move-to-front-heuristic.md). Replace only `recall` in `LinkedBook` by:
```
def recall(name: String): String = {
  require(name != null)
  val p = findPrev(name)
  require(p.next != null, "Name is not in the book")
  val found = p.next
  if (p ne header) {
    p.next = found.next
    found.next = header.next
    header.next = found
  }
  found.number
}
```
The search has the same [loop invariant](../../../../../loop-invariant.md) and [loop variant](../../../../../loop-variant.md) as before. Detach the existing [linked list node](../../../../../linked-list-node.md) before inserting it immediately after the [dummy header node](../../../../../sentinel-node.md). The branch for an already-first [linked list node](../../../../../linked-list-node.md) avoids linking it to itself. Every real contact still occurs exactly once with the same name/number binding, so the [representation invariant](../../../../../representation-invariant.md) and [abstraction function](../../../../../abstraction-function.md) are preserved at return. **No new [linked list node](../../../../../linked-list-node.md) is allocated, and an immediate repeated recall needs one name comparison.** The present recall still pays its original search cost; the gain is for later repeated access.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [3](../../3.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
