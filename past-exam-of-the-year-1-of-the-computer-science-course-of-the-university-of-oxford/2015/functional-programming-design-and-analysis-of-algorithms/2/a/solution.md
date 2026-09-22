<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [sum type](../../../../../tagged-union.md) whose two constructors distinguish a number from an operator:
```
data Elem = Number Int | Operator Op
```
Then the supplied `Polish` and `RPolish` aliases can both be [lists](../../../../../list-abstract-data-type.md) of `Elem`. Constructor tags distinguish tokens without attempting to encode operators as special numeric values. The numeric type `Int` agrees with the supplied [abstract syntax tree](../../../../../abstract-syntax-tree.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
