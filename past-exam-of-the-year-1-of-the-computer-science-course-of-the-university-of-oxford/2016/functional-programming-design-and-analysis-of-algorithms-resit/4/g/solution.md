<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Apply the same [translation](../../../../../translation-geometry.md) to every [vertex](../../../../../vertex-graph-theory.md):
```
translate :: Point -> Polygon -> Polygon
translate (u,v) = map (\(x,y) -> (x+u,y+v))
```
Every [edge vector](../../../../../edge-vector.md) is unchanged because the added displacement cancels on subtraction. Hence lengths, angles, orientation and shape are preserved.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [4](../../4.md)
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
