<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The two abstract methods are
```
def hasNext: Boolean
def next(): T
```
The first reports availability; the second returns and consumes the next entry, or throws a `NoSuchElementException` if none exists. Other standard [iterator](../../../../../iterator.md) operations are supplied in terms of this interface. Repeated availability checks must not lose entries, although they may perform preparatory internal work.[Iterator, abstract members hasNext and next; class-level mutation and reuse contract](../../../../../scala-2-13-iterator-api-documentation.md)

## ↑ Ancestors (12)

1. [B](../b.md)
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
