<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Start with a one-cell, possibly unnormalized representation, then carry:

```
function MakeNum(t: integer): number
    require t >= 0
    new(result, 1)
    result[0] := t
    Normal(result)
    return result
```

Before normalization its represented value is exactly `t`. [Carry normalization of a digit array](../../../../../carry-normalization-of-a-digit-array.md) preserves that value and grows storage when needed. Zero returns a valid nonempty representation containing zero. A negative input is outside this nonnegative-number abstraction.

## ↑ Ancestors (12)

1. [D](../d.md)
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
