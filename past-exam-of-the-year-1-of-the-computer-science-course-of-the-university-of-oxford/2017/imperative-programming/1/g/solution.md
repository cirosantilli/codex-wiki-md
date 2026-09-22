<h1 id="1/g/solution">Solution</h1>

↑ **Parent:** [G](../g.md)

Normalize a copy, skip high-order zero blocks, print the highest block ordinarily, and pad all remaining blocks:

```
procedure OutNum(n: number)
    z := CopyNum(n)
    Normal(z)
    i := len(z)-1
    while i > 0 and z[i] = 0 do
        i := i-1
    Out.Int(z[i])
    i := i-1
    while i >= 0 do
        place := base div 10
        while place > 0 do
            digit := (z[i] div place) mod 10
            Out.Char(character('0' + digit))
            place := place div 10
        i := i-1
```

Here `Out.Int` writes an ordinary unpadded decimal integer, and `character('0' + digit)` denotes its decimal digit character. Since $base=10^k$ for $k\geq1$, the inner loop writes exactly $k$ characters per lower block. This [power-of-ten digit-block formatting](../../../../../power-of-ten-digit-block-formatting.md) retains internal zeros: base-$1000$ digits $[4,0,12]$ print as **`12000004`**, not `1204`. An all-zero array prints exactly **`0`**. The caller's original array is preserved.

## ↑ Ancestors (12)

1. [G](../g.md)
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
