<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Each entry contributes a choice between omission and inclusion. Use [list concatenation](../../../../../list-concatenation.md) as $\oplus$, so that [Cartesian lifting of a binary operation to lists](../../../../../cartesian-lifting-of-a-binary-operation-to-lists.md) joins every choice from an earlier position to every choice from later positions:

```
crossAppend :: [[a]] -> [[a]] -> [[a]]
crossAppend xss yss = [xs ++ ys | xs <- xss, ys <- yss]

f :: a -> [[a]]
f x = [[],[x]]

subs :: [a] -> [[a]]
subs xs = foldr crossAppend [[]] (map f xs)
```

The seed is `[[]]`, because the empty [list](../../../../../list-abstract-data-type.md) has one [subsequence](../../../../../subsequence.md), namely `[]`, and concatenating the empty [list](../../../../../list-abstract-data-type.md) changes nothing. If `rest` lists the [subsequences](../../../../../subsequence.md) of the tail, `crossAppend [[],[x]] rest` lists all omissions of `x` first and all inclusions second. For `[a,b,c]`, the last position changes fastest, producing the specified order `[], [c], [b], [b,c], [a], [a,c], [a,b], [a,b,c]`. Repeated input values can give equal [subsequences](../../../../../subsequence.md) at distinct choices of positions; those repetitions are retained. Thus

$$
\boxed{\operatorname{subs}=\operatorname{foldr}\ X_{++}\ [[]]\circ\operatorname{map}f.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
