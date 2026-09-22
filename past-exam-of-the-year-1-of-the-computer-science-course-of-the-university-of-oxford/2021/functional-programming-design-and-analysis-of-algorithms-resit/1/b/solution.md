<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**Yes.** Define the combining [function](../../../../../function-split.md) as follows:
```
takeP :: (a -> Bool) -> [a] -> [a]
takeP p = foldr step []
  where
    step x rest = if p x then x : rest else []
```
For the fusion derivation use the identity reconstruction `foldr (:) []`, take $f=\operatorname{takeWhile}\ p$, and choose the displayed `step` as $h$. The [function](../../../../../function-split.md) $f$ is strict in the input [list](../../../../../list-abstract-data-type.md), $f([])=[]$, and its cons equation is exactly $f(x:xs)=h\ x\ (f(xs))$. Fusion gives the implementation. On a false test, `step` does not demand the folded tail, so the implementation can terminate after a finite [list prefix](../../../../../prefix-of-a-list.md) even when the remaining [list](../../../../../list-abstract-data-type.md) is infinite or undefined. An undefined [predicate](../../../../../predicate.md) result at a tested element makes both definitions undefined.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
