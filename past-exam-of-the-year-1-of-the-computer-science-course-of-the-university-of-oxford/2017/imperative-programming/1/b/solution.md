<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The pointer argument must be passed by reference, because it is replaced:

```
procedure Lengthen(var n: number)
    old := n
    L := len(old)
    new(result, 2*L)
    for i := 0 to L-1 do
        result[i] := old[i]
    for i := L to 2*L-1 do
        result[i] := 0
    n := result
```

The low-order coefficients are preserved and the newly allocated high-order coefficients are zero, so the [digit-array integer representation](../../../../../digit-array-integer-representation.md) has the same value. The allocation remains nonempty because $L\geq1$. Neither allocation nor an uninitialized high-order cell may be assumed to contain zero. Any other reference to the old array still denotes that old array; the code does not free storage through an alias.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
