<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use parallel [arrays](../../../../../array-data-structure.md) for keys and their representative values, with only a prefix active:

```
override val capacity: Int = 1000
private val elements = new Array[Int](capacity)
private val representatives = new Array[Int](capacity)
private var used = 0
```

The chosen bound is an explicit implementation parameter of the [abstract data type](../../../../../abstract-data-type.md); another a-priori positive bound works identically. **The initial map is empty because `used == 0`.** Zero-filled unused cells are not members of the map, so zero and negative keys remain valid [integers](../../../../../integer-split.md). Use `DisjointSets` consistently as the trait name; the source's prose variation `DisjointSubsets` does not change the declared interface.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
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
