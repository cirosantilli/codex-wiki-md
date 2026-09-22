<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Membership is exactly whether the bucket search finds an entry:

```
def isInBook(name: String): Boolean = {
  find(name, table(hash(name))) != null
}
```

By the bucket-placement [representation invariant](../../../../../representation-invariant.md), an entry with this name can occur only in this bucket. The `find` contract therefore proves **true exactly for keys in the map's domain**, with no state change. One hash calculation and one bucket traversal suffice; no insertion is performed during the query.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
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
