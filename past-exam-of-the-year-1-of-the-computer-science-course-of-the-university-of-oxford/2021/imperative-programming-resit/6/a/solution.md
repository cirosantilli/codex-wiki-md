<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [iterator pattern](../../../../../iterator-pattern.md) exposes sequential traversal through a small interface while hiding the representation of the underlying data. A client asks whether another entry is available and requests the next entry; it need not know whether the producer uses an [array](../../../../../array-data-structure.md), [linked list](../../../../../linked-list.md), tree or generated [sequence](../../../../../sequence.md).

The key design benefit is **[encapsulation](../../../../../encapsulation-computer-programming.md) of traversal state and representation**. The same consuming [algorithm](../../../../../algorithm-split.md) can work through the interface for different producers, and each traversal can keep its own cursor state when a fresh [iterator](../../../../../iterator.md) is supplied. This independence requires separate consumption states; two references to one [iterator](../../../../../iterator.md) share a cursor.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
