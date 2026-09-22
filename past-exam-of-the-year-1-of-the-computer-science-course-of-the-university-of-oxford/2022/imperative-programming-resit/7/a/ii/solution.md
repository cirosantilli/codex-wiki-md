<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Read and advance the [cursor](../../../../../../cursor.md) only when the [iterator](../../../../../../iterator.md) is asked for its next value:

```
def asIter[T](cur: Cursor[T]): Iter[T] = new Iter[T] {
  def hasNext: Boolean = cur.hasCurrent
  def next(): T = {
    require(cur.hasCurrent, "empty iterator")
    val answer = cur.current
    cur.next()
    answer
  }
}
```

The two abstract [sequences](../../../../../../sequence.md) are identical. A `next` call returns the old head and removes it, while `hasNext` only queries availability. No element is read at construction or during an availability test, and no later element is read while returning the current one. Thus the adapter is not too eager. The source's `Cursor.current` clause needs the implicit [precondition](../../../../../../precondition.md) that its [sequence](../../../../../../sequence.md) is nonempty; taking the head of an empty [sequence](../../../../../../sequence.md) is undefined. The checks above satisfy that requirement even without relying on the client convention.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
