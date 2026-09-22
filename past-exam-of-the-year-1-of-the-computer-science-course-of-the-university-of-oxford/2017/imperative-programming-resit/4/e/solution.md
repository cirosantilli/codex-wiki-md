<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The coefficient type is not assumed to be ordered, so do not require a sign or absolute-value operation beyond the supplied output routine. Parenthesize coefficients to keep negative or compound values unambiguous:

```
OutPoly(p):
    first = true
    while p != NIL:
        if p.coeff != 0:
            if not first: Out.String("+")
            Out.String("("); OutT(p.coeff); Out.String(")")
            if p.power != 0:
                Out.String("*x")
                if p.power != 1:
                    Out.String("^"); Out.Int(p.power)
            first = false
        p = p.next
    if first: OutT(0)
```

For example, the representation in the question can print **`(-1)+(1)*x^2`**, which denotes the same polynomial. If $T$ additionally provides ordered-real sign operations, cosmetic suppression of `+(-...)` and unit coefficients can produce `-1+x^2`. The generic routine already handles the zero polynomial and preserves the represented value without introducing those extra assumptions.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
