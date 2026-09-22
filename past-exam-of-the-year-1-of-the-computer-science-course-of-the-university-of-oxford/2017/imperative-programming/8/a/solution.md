<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Store the current list in a mutable field; insertion and deletion can use its head:

```
class MSet[T](contents: List[T]) {
  protected var data: List[T] = contents

  def add(x: T): Unit = {
    data = x :: data
  }

  def delete(): T = data match {
    case x :: xs => data = xs; x
    case Nil => throw new NoSuchElementException("MSet.delete")
  }
}
```

The [representation invariant](../../../../../representation-invariant.md) interprets the list by its [multiset](../../../../../multiset.md) of occurrences; order is immaterial and duplicates remain distinct occurrences. `add` increases one multiplicity, while `delete` returns and removes one occurrence. The field is protected so the minimum-search subclass in part (d) can inspect it. Both successful updates take $O(1)$ list operations. Deleting from an empty bag raises an explicit exception.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
