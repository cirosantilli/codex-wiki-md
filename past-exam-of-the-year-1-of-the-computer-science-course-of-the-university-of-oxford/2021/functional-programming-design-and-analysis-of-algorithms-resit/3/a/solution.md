<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The empty family has one choice, the empty selection:
```
cp :: [[a]] -> [[a]]
cp = foldr extend [[]]
  where
    extend choices suffixes = [x:ys | x <- choices, ys <- suffixes]
```
A selection from the whole family consists uniquely of a choice from its first member and a selection from the remaining family. This bijection proves the combining equation and completeness by [induction](../../../../../mathematical-induction.md). If a member family is empty, there are no selections. The base is `[[]]`, not `[]`: otherwise every [Cartesian product](../../../../../cartesian-product.md) would incorrectly be empty.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
