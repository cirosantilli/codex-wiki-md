<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Equal side lengths alone are insufficient: a nonsquare rhombus is not a [regular polygon](../../../../../regular-polygon.md). Use the [regular polygon edge rotation criterion](../../../../../regular-polygon-edge-rotation-criterion.md): for $n\geq3$, successive nonzero [edge vectors](../../../../../edge-vector.md) must be related by the same [rotation](../../../../../rotation-mathematics.md) through either $2\pi/n$ or $-2\pi/n$.
```
regular :: Polygon -> Bool
regular ps
  | length ps < 3 = False
  | otherwise = norm2 (head es) > 0 && (fits 1 || fits (-1))
  where
    es = [ (u-x,v-y) | ((x,y),(u,v)) <- edges ps ]
    angle = 2*pi / fromIntegral (length ps)
    norm2 (x,y) = x*x+y*y
    close x y = abs (x-y) <= 1e-10 * max 1 (max (abs x) (abs y))
    same (x,y) (u,v) = close x u && close y v
    turn s (x,y) = (cos angle*x - s*sin angle*y,
                    s*sin angle*x + cos angle*y)
    fits s = and (zipWith (\a b -> same (turn s a) b)
                          es (tail es ++ [head es]))
```
With exact real coordinates and exact equality in `same`, this is an if-and-only-if test for an ordinary convex [regular polygon](../../../../../regular-polygon.md), in either boundary orientation. The displayed `Double` implementation tests that condition to the stated tolerance; it cannot promise exact geometric classification near the tolerance boundary. Both orientations are needed, and using the fundamental turn $2\pi/n$ excludes regular star traversals. A repeated zero-length side fails the exact criterion.

## ↑ Ancestors (12)

1. [E](../e.md)
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
