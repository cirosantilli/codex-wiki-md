<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [precondition](../../../../../precondition.md) is **`n != null` and $n\in L(\mathrm{bagHeader.next})$**, using node identity rather than datum equality. Search for its predecessor:

```
def delete(n: Node): Unit = {
  var previous = bagHeader
  while (previous.next ne n) {
    previous = previous.next
  }
  previous.next = n.next
  n.next = null
}
```

The [loop invariant](../../../../../loop-invariant.md) states that `previous` is the header or a preceding real node, and $n\in L(\mathrm{previous.next})$. The [loop variant](../../../../../loop-variant.md) is the number of links from `previous` to `n` minus one. The [precondition](../../../../../precondition.md) guarantees that this search reaches the predecessor before a null dereference. Replacing its successor by `n.next` bypasses exactly the requested node; clearing the removed node's link detaches it for later reuse. The order and identities of every other node remain unchanged. In abstract terms, only the multiplicity of `n.datum` decreases, by one. The worst-case time is linear; the pointer modification itself is constant-time.

## ↑ Ancestors (12)

1. [C](../c.md)
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
