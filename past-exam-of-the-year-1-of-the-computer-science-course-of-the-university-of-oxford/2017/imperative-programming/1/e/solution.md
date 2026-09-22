<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Add corresponding coefficients, treating missing coefficients as zero:

```
function Add(a, b: number): number
    L := max(len(a), len(b))
    new(result, L)
    for i := 0 to L-1 do
        result[i] := 0
        if i < len(a) then result[i] := result[i] + a[i]
        if i < len(b) then result[i] := result[i] + b[i]
    Normal(result)
    return result
```

By the [digit-array integer representation](../../../../../digit-array-integer-representation.md), the raw result has value $\operatorname{val}(a)+\operatorname{val}(b)$. [Carry normalization of a digit array](../../../../../carry-normalization-of-a-digit-array.md) produces a normalized result, including any final carry. Both input arrays remain unchanged, so the operation also works when `a` and `b` alias each other.

## ↑ Ancestors (12)

1. [E](../e.md)
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
