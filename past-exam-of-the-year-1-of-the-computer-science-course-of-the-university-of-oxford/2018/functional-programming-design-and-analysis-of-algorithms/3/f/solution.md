<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

A [concatenation tree](../../../../../concatenation-tree.md) may contain arbitrarily many `Cat` and `Nil` nodes while denoting an empty or singleton [list](../../../../../list-abstract-data-type.md). For example, repeatedly wrap `One x` as `Cat Nil previous`. The output length stays one while the input size grows without bound. An arbitrary leaf could hide another `One`, so a correct general conversion cannot disregard unexamined branches. **Output length alone therefore cannot bound the work; input size must be included.**

## ↑ Ancestors (12)

1. [F](../f.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
