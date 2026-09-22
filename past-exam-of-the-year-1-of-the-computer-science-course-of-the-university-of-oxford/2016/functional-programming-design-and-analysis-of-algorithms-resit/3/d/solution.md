<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The parser recognizes exactly one leading operator character:
```
parseOp :: Parse Char
parseOp (c:cs)
  | c `elem` "+-*/" = Just (c,cs)
parseOp _ = Nothing
```
An empty input fails, and any later characters remain for the next parser. The last example printed in this part uses the name `parseInt`; its failure result does not change the requested operator parser.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
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
