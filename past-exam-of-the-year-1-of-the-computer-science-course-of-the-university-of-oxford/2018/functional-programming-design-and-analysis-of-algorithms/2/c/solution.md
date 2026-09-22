<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two required equations are

```
zipWith f xs ys = map (uncurry f) (zip xs ys)
zip xs ys       = zipWith (,) xs ys
```

Either equation defines one operation from an independently defined other operation. They do **not** together supply an effective recursive definition of the intended operations. Substitution makes the first output constructor depend on itself without first emitting anything, so the mutually recursive program has the [bottom value](../../../../../bottom-value.md) as its least solution. At the level of equations they also fail to characterize the intended operations uniquely: returning `[]` for every call of either operation satisfies both equations, as does the intended [list zip](../../../../../list-zip.md). A constructor-producing base/step definition is essential for [productivity](../../../../../stream-productivity.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
