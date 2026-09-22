<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Repeated [constant time](../../../../../constant-time.md) insertion constructs the representation:
```
fromList :: [a] -> List a
fromList = foldr cons nil
```
The [right fold](../../../../../list-fold.md) preserves order because `cons` prepends its argument. On a finite length-$n$ [list](../../../../../list-abstract-data-type.md), there are $n$ calls of `cons`; completely constructing the result takes **$\Theta(n)$ time** and $O(n)$ constructors. This claim concerns finite inputs, not productivity of conversion from an infinite [lazy list](../../../../../lazy-list.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
