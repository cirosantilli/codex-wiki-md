<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[List concatenation](../../../../../list-concatenation.md) exhausts one inner [list](../../../../../list-abstract-data-type.md) before reaching the next. For example, with rows `[0,2..]` and `[1]`, `concat` outputs the infinite even row and never reaches `1`. [First-occurrence duplicate removal](../../../../../first-occurrence-duplicate-removal.md) cannot recover a value that its input stream never supplies. Hence

$$
\boxed{\text{ordinary concatenation does not give a fair enumeration of infinite rows}.}
$$

The obstruction is separate from the undefined final tail in part (c): here a required distinct value is never emitted at all. A [fair enumeration](../../../../../fair-enumeration.md) must give every row and every element within it a finite opportunity to contribute.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
