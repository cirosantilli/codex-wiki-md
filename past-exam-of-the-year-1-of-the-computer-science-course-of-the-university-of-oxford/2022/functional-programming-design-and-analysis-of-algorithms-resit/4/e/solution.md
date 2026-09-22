<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Apply the supplied bitonic-merging fact directly:
```
merge :: Ord a => [a] -> [a]
merge xs = rounds (levels (length xs)) xs
  where
    levels n
      | n <= 1    = 0
      | otherwise = 1 + levels (n `div` 2)
    order (x,y)
      | x <= y    = (x,y)
      | otherwise = (y,x)
    pass = unpairs . map order . pairs . riffle
    rounds 0 ys = ys
    rounds r ys = rounds (r-1) (pass ys)
```
For length $n=2^k$, `levels n = k`. Each `pass` performs exactly the required shuffle and adjacent compare-exchange operations. The supplied fact therefore proves that `rounds k` yields ascending order from a [bitonic sequence](../../../../../bitonic-sequence.md). Each pass preserves the [multiset](../../../../../multiset.md) of entries and costs $\Theta(n)$, giving **$\Theta(n\log n)$ time** for $n\ge2$. Length one needs no pass. The definition also harmlessly returns `[]` on empty input.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
