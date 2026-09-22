<h1 id="6/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

For the implementations above the value is
```
List('1', '3', '5', '7', '9')
```
The first half-[iterator](../../../../../iterator.md) returns the odd-position characters while consuming the even-position characters as its required skips. By the time it is exhausted, it has consumed the entire shared underlying [iterator](../../../../../iterator.md). The second half-[iterator](../../../../../iterator.md) consequently has no entries left when concatenation reaches it. **Sharing one source does not create two independent traversals.** Neither constructor consumes anything, so it also does not shift the first output before iteration begins. The source's implementation references here should be read as parts (d) and (e); the printed reference to (c) and (d) is a cross-reference slip.

## ↑ Ancestors (12)

1. [F](../f.md)
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
