<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Join either two halves or successive pairs:
```
unhalve :: ([a],[a]) -> [a]
unhalve (xs,ys) = xs ++ ys

unpairs :: [(a,a)] -> [a]
unpairs = foldr (\(x,y) zs -> x:y:zs) []
```
By the defining property of `splitAt`, concatenating the two halves restores the original [list](../../../../../list-abstract-data-type.md). For `unpairs`, [structural induction](../../../../../structural-induction.md) on the even input proves that its first pair restores its first two elements and the recursive result restores the rest. Thus both requested [function compositions](../../../../../function-composition.md) are the identity. Fully consuming either result takes at most [linear time](../../../../../linear-time.md); [list concatenation](../../../../../list-concatenation.md) only copies the left half once.

## ↑ Ancestors (12)

1. [B](../b.md)
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
