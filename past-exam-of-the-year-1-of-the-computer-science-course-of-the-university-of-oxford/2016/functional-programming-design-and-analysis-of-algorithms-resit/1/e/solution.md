<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write `u = take n xs`, `v = drop n xs`, and `len = length xs`. Part (c) gives `xs = u ++ v`; part (d) gives `length v = len-n` because $0\leq n\leq\mathrm{len}$. Use the finite-[list](../../../../../list-abstract-data-type.md) laws `take (length v) (v ++ w) = v`, `length (reverse v) = length v`, and `reverse (reverse v) = v`. Then [equational reasoning](../../../../../equational-reasoning.md) gives
```
reverse (take (len-n) (reverse xs))
= reverse (take (length v) (reverse (u ++ v)))
= reverse (take (length (reverse v)) (reverse v ++ reverse u))
= reverse (reverse v)
= v
= drop n xs
```
The first and second steps use the decomposition and the length equation; the third uses reversal of a concatenation; the fourth uses the stated take law. This is an algebraic proof using established laws, rather than a new [induction](../../../../../mathematical-induction.md) proof.

## ↑ Ancestors (12)

1. [E](../e.md)
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
