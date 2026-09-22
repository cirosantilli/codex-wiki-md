<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First include the closing [edge](../../../../../edge-of-a-graph.md) exactly once:
```
edges :: Polygon -> [(Point,Point)]
edges [] = []
edges ps = zip ps (tail ps ++ [head ps])

perimeter :: Polygon -> Double
perimeter = total . edges
  where total [] = 0
        total ((p,q):es) = distBetween p q + total es

perimeterFold :: Polygon -> Double
perimeterFold = foldr (\(p,q) s -> distBetween p q + s) 0 . edges
```
The recursive version and [right fold](../../../../../list-fold.md) both sum the [Euclidean distances](../../../../../euclidean-distance.md) between consecutive [vertices](../../../../../vertex-graph-theory.md), including the last-to-first pair. They take [linear time](../../../../../linear-time.md). The empty-list convention gives zero, although an empty list is not a valid [polygon](../../../../../polygon.md).

## ↑ Ancestors (12)

1. [D](../d.md)
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
