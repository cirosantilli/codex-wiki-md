<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**`inits` is not a direct [list fold](../../../../../list-fold.md):** `inits undefined = [] : undefined` has a defined outer constructor, while `foldr c z undefined` is $\bot$.

**Both `pinits` and `ninits` are direct [list folds](../../../../../list-fold.md):**
```
pinitsFold :: [a] -> [[a]]
pinitsFold = foldr (\x yss -> [] : map (x:) yss) []

ninitsFold :: [a] -> [[a]]
ninitsFold = foldr (\x yss -> [x] : map (x:) yss) []
```
For `pinits`, the combining function is exactly the recursive step above. For `ninits`, expand `inits xs = [] : ninits xs` and use

$$
\operatorname{map}(x:)([]:yss)=[x]:\operatorname{map}(x:)yss.
$$

Neither step needs to inspect `yss` before producing its first outer constructor. Thus the definitions satisfy the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md) on partial as well as total [lazy lists](../../../../../lazy-list.md).

## ↑ Ancestors (12)

1. [F](../f.md)
2. [1](../../1.md)
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
