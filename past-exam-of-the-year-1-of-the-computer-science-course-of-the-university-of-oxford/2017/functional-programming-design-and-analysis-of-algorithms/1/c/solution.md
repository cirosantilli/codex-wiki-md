<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Generate each row of [Pascal's triangle](../../../../../pascal-s-triangle.md) from its predecessor, padding at opposite ends before adding corresponding entries:

```
pascal :: Num a => [[a]]
pascal = iterate next [1]
  where
    next :: Num a => [a] -> [a]
    next row = zipWith (+) (0:row) (row ++ [0])
```

The boundary sums are the old endpoint plus zero, and the interior sums satisfy [Pascal's rule](../../../../../pascal-s-rule.md). [Induction](../../../../../mathematical-induction.md) on the iteration number therefore gives the rows of [binomial coefficients](../../../../../binomial-coefficient-split.md). The outer [lazy list](../../../../../lazy-list.md) is infinite, with each finite row available on demand. Instantiate `a` as `Integer` for exact arbitrarily large entries; bounded machine integers eventually overflow.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
