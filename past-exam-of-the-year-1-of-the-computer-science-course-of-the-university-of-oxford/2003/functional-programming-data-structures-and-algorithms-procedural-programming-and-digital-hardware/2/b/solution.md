<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [right fold](../../../../../list-fold.md) replaces the empty [list](../../../../../list-abstract-data-type.md) by a seed and each cons by an application of the combining [function](../../../../../function-split.md):

```
foldr :: (a -> b -> b) -> b -> [a] -> b
foldr op e [] = e
foldr op e (x:xs) = op x (foldr op e xs)
```

For example, `foldr op e [a,b,c] = op a (op b (op c e))`. The concise defining law is

$$
\boxed{\operatorname{foldr}\ op\ e\ (x:xs)=op\ x\ (\operatorname{foldr}\ op\ e\ xs),\qquad
\operatorname{foldr}\ op\ e\ []=e.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
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
