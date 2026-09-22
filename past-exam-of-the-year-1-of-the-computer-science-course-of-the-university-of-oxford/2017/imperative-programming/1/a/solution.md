<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Allocate a fresh array and copy every digit:

```
function CopyNum(n: number): number
    new(result, len(n))
    for i := 0 to len(n)-1 do
        result[i] := n[i]
    return result
```

Every coefficient in the [digit-array integer representation](../../../../../digit-array-integer-representation.md) is unchanged, so the value is unchanged. The new array shares no storage with `n`; assigning one pointer to the other would instead create [reference aliasing](../../../../../reference-aliasing.md). Since the entries are integers, copying the entries also gives the required [deep copy](../../../../../deep-copy.md) of this representation.

## ↑ Ancestors (12)

1. [A](../a.md)
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
