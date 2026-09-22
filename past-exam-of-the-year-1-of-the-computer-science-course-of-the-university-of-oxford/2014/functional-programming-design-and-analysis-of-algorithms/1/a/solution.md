<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The two constructors encode a [natural number](../../../../../natural-number.md) by its number of successors. [Structural recursion](../../../../../structural-recursion.md) replaces the zero constructor by zero and every successor by one [addition](../../../../../addition.md):

```
convert :: Natural -> Integer
convert Zero     = 0
convert (Succ n) = 1 + convert n
```

[Structural induction](../../../../../structural-induction.md) gives $\boxed{\operatorname{convert}(\operatorname{Succ}^n\operatorname{Zero})=n}$. The output uses unbounded [integers](../../../../../integer-split.md), so there is no machine-word overflow.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
