<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Inside `LinkedListBook`, traverse without modifying the head or any node:

```
def printBook(): Unit = {
  var p = list
  while (p != null) {
    println(p.name + ":" + p.number)
    p = p.next
  }
}
```

The [loop invariant](../../../../../loop-invariant.md) is that precisely the prefix before `p` has been printed, once per node, in list order; `p` heads the remaining suffix. The [null-terminated linked list](../../../../../null-terminated-linked-list.md) invariant proves termination and prevents duplicate output through cycles. An empty list prints nothing. The [abstraction function](../../../../../abstraction-function.md) is unchanged, and the traversal takes $O(K)$ node visits for $K$ entries.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
