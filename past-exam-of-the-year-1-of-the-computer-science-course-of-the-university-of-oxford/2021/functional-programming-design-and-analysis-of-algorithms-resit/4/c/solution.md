<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The embedding is a [right fold](../../../../../list-fold.md) interpreting each source constructor by its new counterpart:
```
list' :: [a] -> List a
list' = foldr cons' nil'
```
[Induction](../../../../../mathematical-induction.md) on the finite source [list](../../../../../list-abstract-data-type.md) proves that querying index $i$ returns its $i$th element exactly when $i$ lies in range. The empty case is `nil'`; the cons case shifts every tail index as established in part (b). This is the only part of Question 4 whose implementation uses the conventional [list](../../../../../list-abstract-data-type.md) type.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
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
