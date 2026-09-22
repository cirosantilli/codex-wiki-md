<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [mathematical induction](../../../../../mathematical-induction.md) on $n$, which is finite even when the [list](../../../../../list-abstract-data-type.md) is infinite. At $n=0$, the left side is `[] ++ xs = xs`. For the successor step, an empty [list](../../../../../list-abstract-data-type.md) gives `[]`; for `x:xs`, the defining equations and [list concatenation](../../../../../list-concatenation.md) give
```
take (n+1) (x:xs) ++ drop (n+1) (x:xs)
= (x : take n xs) ++ drop n xs
= x : (take n xs ++ drop n xs)
= x : xs
```
The last step applies the [induction hypothesis](../../../../../induction-hypothesis.md) to the tail. A [bottom value](../../../../../bottom-value.md) tail is allowed: for a wholly undefined list and a positive count both sides are undefined. Thus the equality is observationally valid for finite and infinite [lists](../../../../../list-abstract-data-type.md); no evaluation of an infinite length is used.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
