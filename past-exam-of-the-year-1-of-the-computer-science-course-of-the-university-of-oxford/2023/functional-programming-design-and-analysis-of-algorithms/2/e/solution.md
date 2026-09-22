<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Define the ordered [merge algorithm](../../../../../merge-algorithm.md) explicitly:
```
mergePos :: [Integer] -> [Integer] -> [Integer]
mergePos [] ys = ys
mergePos xs [] = xs
mergePos xs@(x:xt) ys@(y:yt)
  | x <= y = x : mergePos xt ys
  | otherwise = y : mergePos xs yt

ilv :: Seq a -> Seq a -> Seq a
ilv s t v = mergePos (map (2*) (s v))
                    (map (\j -> 2*j+1) (t v))
```
The first sequence occupies even positions and the second occupies odd positions. Within each transformed [list](../../../../../list-abstract-data-type.md), order is preserved; merging puts all positions for a queried token into increasing order. The two transformed lists have disjoint parities, so equality cannot occur between their heads on valid inputs. The length assumption ensures that these positions describe the intended interleaved sequence without a gap at its finite end.

## ↑ Ancestors (12)

1. [E](../e.md)
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
