<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a finite acyclic [linked list](../../../../../linked-list.md) define the node [sequence](../../../../../sequence.md), retaining [software object](../../../../../software-object.md) identities, by

$$
L(\mathrm{null})=[],\qquad L(u)=u:L(u.\mathrm{next}).
$$

Then scan without changing any links:

```
def findMin(first: Node): Node = {
  require(first != null)
  var best = first
  var cursor = first.next
  while (cursor != null) {
    if (cursor.datum < best.datum) best = cursor
    cursor = cursor.next
  }
  best
}
```

At each [while loop](../../../../../while-loop.md) head, write $L(\mathrm{first})=P\mathbin{++}L(\mathrm{cursor})$. The [loop invariant](../../../../../loop-invariant.md) says $P$ is nonempty, `best` belongs to $P$, and its datum is no larger than that of every node in $P$. Initially $P$ contains only `first`; comparing the next node extends the processed [string prefix](../../../../../string-prefix.md) and preserves minimality. The [loop variant](../../../../../loop-variant.md) $|L(\mathrm{cursor})|$ strictly decreases. At exit the whole [list](../../../../../list-abstract-data-type.md) is processed, so **the returned reference identifies a minimum node**. Ties retain the earliest minimum. Time is linear in the number of nodes and auxiliary space is constant.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
