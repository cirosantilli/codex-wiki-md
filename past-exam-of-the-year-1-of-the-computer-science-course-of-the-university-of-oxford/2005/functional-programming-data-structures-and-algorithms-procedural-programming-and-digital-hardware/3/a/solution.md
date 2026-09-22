<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

To agree with the example, preserve the first occurrence of each value. This [first-occurrence duplicate removal](../../../../../first-occurrence-duplicate-removal.md) is a [right fold](../../../../../list-fold.md):

```
remalldups = foldr step []
  where step x ys = x : filter (/= x) ys
```

The folded tail has no repetitions by the [induction hypothesis](../../../../../induction-hypothesis.md). The [list filter](../../../../../list-filter.md) removes any occurrence of the new head from that tail; prepending the head then gives exactly one occurrence of it, in its first input position. Other values retain their relative order. For the supplied example the intermediate folded results, from right to left, are `[1]`, `[3,1]`, `[2,3,1]`, and `[1,2,3]`. Thus

$$
\boxed{\operatorname{remalldups}[1,2,3,1]=[1,2,3].}
$$

Under [lazy evaluation](../../../../../lazy-evaluation.md), constructing `x : ...` does not first demand the folded tail. That observation is essential for the infinite cases below. The alternative step that first asks whether `x` belongs to the folded tail would lose this property and would also keep last occurrences instead of matching the stated example.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
