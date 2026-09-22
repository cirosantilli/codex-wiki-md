<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $B_0$ and $R_0=L(\mathrm{bagHeader.next})$ describe the entry state. The [postcondition](../../../../../postcondition.md) is: **the [multiset](../../../../../multiset.md) is empty; the returned chain is sorted nondecreasingly; its node [sequence](../../../../../sequence.md) is a [permutation](../../../../../permutation.md) of $R_0$**. Thus it has exactly the original [multiset](../../../../../multiset.md) of data and preserves all duplicates. Strict increase is impossible when the [multiset](../../../../../multiset.md) contains repeated values.

```
def getAllSorted(): Node = {
  var head: Node = null
  var tail: Node = null
  while (bagHeader.next != null) {
    val nextSmallest = findMin(bagHeader.next)
    delete(nextSmallest)
    nextSmallest.next = null
    if (head == null) head = nextSmallest
    else tail.next = nextSmallest
    tail = nextSmallest
  }
  head
}
```

The [loop invariant](../../../../../loop-invariant.md) partitions the original node identities into the remaining [multiset](../../../../../multiset.md) and the returned-prefix chain. The latter is sorted, its last node is `tail`, and every datum in it is no larger than every remaining datum. Selecting a minimum and appending that detached node preserves all these facts. The [loop variant](../../../../../loop-variant.md) is the number of real nodes remaining in the [multiset](../../../../../multiset.md), decreasing by one. When it reaches zero the [string prefix](../../../../../string-prefix.md) contains the entire original node set, proving the [postcondition](../../../../../postcondition.md). An initially empty [multiset](../../../../../multiset.md) returns null.

This is linked-list [selection sort](../../../../../selection-sort.md). Its time is $\Theta(m^2)$ in general, from successive scans of lengths $m,m-1,\ldots,1$, and it uses constant auxiliary space: it relinks original nodes instead of allocating a new node for each item.

## ↑ Ancestors (12)

1. [E](../e.md)
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
