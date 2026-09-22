<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Here “centroid” means the **[vertex centroid](../../../../../vertex-centroid.md)**, the arithmetic mean of the listed [vertices](../../../../../vertex-graph-theory.md), rather than the uniform-area [centroid](../../../../../centroid.md) of the polygon's interior:
```
centroid :: Polygon -> Point
centroid [] = error "centroid: empty vertex list"
centroid ps = (sx/n,sy/n)
  where
    (sx,sy) = foldr (\(x,y) (u,v) -> (x+u,y+v)) (0,0) ps
    n = fromIntegral (length ps)
```
The nonempty input restriction prevents division by zero; computing both sums and the length takes [linear time](../../../../../linear-time.md).

## ↑ Ancestors (12)

1. [F](../f.md)
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
