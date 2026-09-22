<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Represent the ranking criteria by a [tuple](../../../../../finite-tuple.md) in decreasing priority:

```
type Weight = (Int,Int,Int)

weight :: Results -> Weight
weight (Results _ scores) =
  (sum (map points scores),
   sum [gf - ga | (gf,ga) <- scores],
   sum (map fst scores))
  where
    points (gf,ga)
      | gf > ga   = 3
      | gf == ga  = 1
      | otherwise = 0
```

The components are **total points, total goal difference and total goals scored**. The [Haskell Ord class](../../../../../haskell-ord-class.md) compares [tuples](../../../../../finite-tuple.md) in [lexicographic order](../../../../../lexicographic-order.md), so a greater first component dominates all later components; only ties reach the next criterion. Exactly equal triples remain tied because no further ranking criterion was specified. In the supplied fixture data the descending triples are $(6,13,15)$, $(4,3,5)$, $(3,0,3)$, $(1,0,0)$, $(1,-3,4)$, $(1,-3,0)$ and $(0,-10,0)$, respectively for United, Athletic, City, Albion, Rovers, Corinthians and Thistle.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
