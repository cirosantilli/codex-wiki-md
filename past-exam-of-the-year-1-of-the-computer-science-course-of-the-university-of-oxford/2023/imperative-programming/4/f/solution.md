<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Update an existing node, otherwise append one fresh node while preserving the cycle:

```
def store(name: String, number: String): Unit = {
  val p = find(name)
  if (p != null) p.number = number
  else {
    val fresh = new Node(name, number, null)
    if (last == null) {
      fresh.next = fresh
      last = fresh
    } else {
      fresh.next = last.next
      last.next = fresh
      last = fresh
    }
  }
}
```

For an existing name, changing only its number realizes replacement in the abstract [partial function](../../../../../partial-function.md). On an empty book, the new node points to itself, establishing a singleton cycle. On a nonempty book, its successor becomes the old first node and the old last points to it; advancing `last` leaves the first node unchanged and closes the enlarged cycle. Since a full search established absence, name uniqueness is preserved. Thus the [postcondition](../../../../../postcondition.md) is exactly the old book with this name mapped to the supplied number, and all other entries unchanged. A store takes $O(K)$ [running time](../../../../../running-time.md) for the name search and $O(1)$ additional pointer work.

## ↑ Ancestors (12)

1. [F](../f.md)
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
