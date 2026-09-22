<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Only the first constructor needs to be inspected:
```
headZig :: Zig a b -> a
headZig (Cins x _) = x
headZig Nil = error "headZig: empty input"

headZag :: Zag a b -> a
headZag (Cans x _) = x
headZag Nal = error "headZag: empty input"
```
The first [type parameter](../../../../../type-parameter.md) is the type of the first element in either [algebraic data type](../../../../../algebraic-data-type.md). The source examples therefore return **`1` and `"C"`**, respectively. These functions are partial at empty inputs, as allowed by the stated nonempty-input requirement.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
