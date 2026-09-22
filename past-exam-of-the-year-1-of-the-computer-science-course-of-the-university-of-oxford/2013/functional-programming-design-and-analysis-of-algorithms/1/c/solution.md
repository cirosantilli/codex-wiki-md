<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Represent [Pascal's triangle](../../../../../pascal-s-triangle.md) by an infinite outer [lazy list](../../../../../lazy-list.md), each of whose elements is one finite row. Pad the preceding row with zero on its left and on its right, then add corresponding entries:

```
pascal :: [[Integer]]
pascal = iterate next [1]
  where
    -- Padding supplies the two boundary entries as well as the interior sums.
    next :: [Integer] -> [Integer]
    next row = zipWith (+) (0 : row) (row ++ [0])
```

Here `iterate next [1]` begins `[[1],[1,1],[1,2,1],[1,3,3,1],...]`. Every call to `next` receives a finite row, so its final zero is reachable. [Lazy evaluation](../../../../../lazy-evaluation.md) produces any requested finite prefix without trying to finish the infinite outer [list](../../../../../list-abstract-data-type.md).

Indexing rows and columns from zero, [Pascal's rule](../../../../../pascal-s-rule.md) says

$$
\boxed{\operatorname{pascal}_n=\left[\binom n0,\binom n1,\ldots,\binom nn\right],\qquad \binom{n+1}j=\binom n{j-1}+\binom nj.}
$$

Take out-of-range [binomial coefficients](../../../../../binomial-coefficient-split.md) to be zero. The seed is the zeroth row, and the padded [addition](../../../../../addition.md) implements this identity at every position, including the two boundaries. [Mathematical induction](../../../../../mathematical-induction.md) therefore proves every generated row correct. Using unbounded [integers](../../../../../integer-split.md) prevents overflow. Generating rows zero through $r$ takes $\Theta(r^2)$ arithmetic operations, with additional bit costs as the [binomial coefficients](../../../../../binomial-coefficient-split.md) grow.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
