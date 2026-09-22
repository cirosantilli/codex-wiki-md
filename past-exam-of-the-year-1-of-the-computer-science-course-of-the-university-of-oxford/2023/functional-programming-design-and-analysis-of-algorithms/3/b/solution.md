<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a distinct constructor for each mark, and reserve every bull before allocating any cow:
```
data Mark = Bull | Cow | Miss deriving (Eq,Show)

scoreWordle :: Eq a => [a] -> [a] -> [Mark]
scoreWordle secret guess = mark pairs pool
  where
    pairs = zip secret guess
    pool = [s | (s,g) <- pairs, s /= g]
    mark [] _ = []
    mark ((s,g):ps) available
      | s == g = Bull : mark ps available
      | otherwise = case pluck g available of
          Nothing -> Miss : mark ps available
          Just rest -> Cow : mark ps rest
```
The [multiset](../../../../../multiset.md) `pool` contains exactly the unused secret tokens after all bulls have been set aside. The recursive [invariant](../../../../../invariant-mathematics.md) is that `available` contains those tokens not yet allocated to cows. A successful `pluck` consumes one, and failure leaves the pool unchanged. This proves both multiplicity correctness and the priority of bulls over cows. Among duplicate non-bull guess tokens, the leftmost eligible ones receive cows. For secret `"alpha"` and guess `"aaabb"`, the result is **`[Bull,Cow,Miss,Miss,Miss]`**. This implements [duplicate-aware positional scoring](../../../../../duplicate-aware-positional-scoring.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
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
