<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Emit separators only between terms, with a special case for the empty sum:

```
procedure OutRat(m,n)
    Out.Int(m)
    Out.String("/")
    Out.Int(n)

procedure OutEgypt(e)
    if e.i = 0 then
        Out.String("0")
    else
        for j := 0 to e.i-1 do
            if j > 0 then Out.String("+")
            Out.String("1/")
            Out.Int(e.x[j])
```

Ordinary unpadded decimal output and the [greedy Egyptian fraction expansion](../../../../../greedy-egyptian-fraction-expansion.md) give **`5/7 = 1/2+1/5+1/70`** for that input. The final newline is supplied by the caller. Stored duplicate denominators, if present in another valid representation, are printed as separate [unit fraction](../../../../../unit-fraction.md) occurrences.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
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
