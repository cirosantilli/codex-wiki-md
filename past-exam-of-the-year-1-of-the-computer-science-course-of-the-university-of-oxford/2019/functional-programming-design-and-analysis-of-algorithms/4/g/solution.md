<h1 id="4/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

For a **finite outer [list](../../../../../list-abstract-data-type.md)** of [proper lazy lists](../../../../../proper-lazy-list.md), use the fair binary product from part f:

```
cp :: [[a]] -> [[a]]
cp []       = [[]]
cp (xs:xss) = fairPair (:) xs (cp xss)
```

The empty family has one selection, the empty selection. For a nonempty finite family, each selection consists uniquely of one first-factor occurrence followed by a selection from the remaining factors. [Induction](../../../../../mathematical-induction.md) on the number of factors, together with the fairness of `fairPair`, proves that every such selection is produced and no invalid selection is introduced. Infinite factors are allowed: in particular, the three-factor example is enumerated fairly. If any factor is empty, the finite-family computation returns the empty product.

The printed hypothesis also permits an _infinite outer_ [proper lazy list](../../../../../proper-lazy-list.md). **No [function](../../../../../function-split.md) can satisfy the full enumeration requirement for all such inputs.** Take `repeat [0,1]`. Its mathematical [Cartesian product](../../../../../cartesian-product.md) contains every infinite binary sequence and is [uncountable](../../../../../uncountable-set.md). If a result [list](../../../../../list-abstract-data-type.md) enumerated these sequences as $z_0,z_1,\ldots$, the binary sequence $b$ with $b_i=1-z_i(i)$ would differ from the $i$-th listed sequence at position $i$, contradicting completeness. This is an [uncountability obstruction to enumerating infinite Cartesian products](../../../../../uncountability-obstruction-to-enumerating-infinite-cartesian-products.md). The finite-outer qualification is a necessary repair to the specification, not a restriction imposed for convenience by the code.

## ↑ Ancestors (12)

1. [G](../g.md)
2. [4](../../4.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
