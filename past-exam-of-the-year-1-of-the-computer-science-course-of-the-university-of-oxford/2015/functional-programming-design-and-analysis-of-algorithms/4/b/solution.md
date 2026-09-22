<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Enumerate finite shells of constant coordinate sum:
```
triples :: [(Integer, Integer, Integer)]
triples =
  [(a, b, k-a-b) |
     k <- [0..],
     a <- [0..k],
     b <- [0..k-a]]
```
Here [natural numbers](../../../../../natural-number.md) include zero. Every generated coordinate is nonnegative. Conversely, a given triple $(a,b,c)$ occurs in exactly the shell $k=a+b+c$ and at exactly those loop indices $a,b$. Each shell contains only finitely many triples, so every triple is reached after finitely many earlier outputs. This is [fair enumeration](../../../../../fair-enumeration.md), unlike nesting three unrestricted infinite lists. For the positive-integer convention, add one to each generated coordinate.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
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
