<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Inside the supplied `PaymentsHash` class, scan until a matching node or the end of the chain. **A null return means the user has no record in this bucket.**

```
private def find(user: Int, head: PaymentsHash.Node): PaymentsHash.Node = {
  var p = head
  while (p != null && p.user != user) p = p.next
  p
}
```

The [loop invariant](../../../../../loop-invariant.md) says that every node already passed has a different user identity and `p` heads the unexamined suffix. [Short-circuit evaluation](../../../../../short-circuit-evaluation.md) of `&&` prevents dereferencing null. The [representation invariant](../../../../../representation-invariant.md) supplies an acyclic finite chain, so each unsuccessful step shortens that suffix and proves [algorithm termination](../../../../../algorithm-termination.md). The code changes no node fields.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
