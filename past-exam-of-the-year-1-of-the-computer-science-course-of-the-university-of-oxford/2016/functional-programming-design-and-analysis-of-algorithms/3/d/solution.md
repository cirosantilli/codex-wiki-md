<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Map each current first-position value with the first function, then swap the functions when descending to the other [algebraic data type](../../../../../algebraic-data-type.md):
```
mapZig :: (a -> c) -> (b -> d) -> Zig a b -> Zig c d
mapZig _ _ Nil = Nil
mapZig f g (Cins x zs) = Cins (f x) (mapZag g f zs)

mapZag :: (a -> c) -> (b -> d) -> Zag a b -> Zag c d
mapZag _ _ Nal = Nal
mapZag f g (Cans x zs) = Cans (f x) (mapZig g f zs)
```
All four [type variables](../../../../../type-variable.md) are independent: mapping may change both element types. There is no `Enum` or numeric constraint on the mapping functions themselves; constraints arise only from particular arguments such as `succ` or `(+2)`. The [mutual recursion](../../../../../mutual-recursion.md) preserves every constructor and applies the intended function at each alternating position. The results are **`Cins 3 (Cans 'B' (Cins 4 Nal))`** and **`Cans "D" (Cins True (Cans "E" Nil))`**, respectively.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
