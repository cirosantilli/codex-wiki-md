<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Even and odd original positions become consecutive new positions:
```
evens :: Seq a -> Seq a
evens s v = map (`div` 2) (filter even (s v))

odds :: Seq a -> Seq a
odds s v = map (`div` 2) (filter odd (s v))
```
An occurrence at $2j$ belongs to `evens` at position $j$; one at $2j+1$ belongs to `odds` at position $j$. Thus the formulas preserve increasing position order and produce the specified finite examples. For infinite occurrence lists, filtering can search forever when no further position of the chosen parity exists. Consequently these otherwise direct formulas need not preserve [productivity](../../../../../stream-productivity.md) for every query.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
