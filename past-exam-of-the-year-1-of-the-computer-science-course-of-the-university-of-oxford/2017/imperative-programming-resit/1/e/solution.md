<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

First normalize fresh copies of the two components. The following output helpers print a reduced rational with no `/1`, suppress a zero radical term, and suppress a unit radical coefficient:

```
OutRat(q):
    Out.Int(q.num)
    if q.den != 1: Out.String("/"); Out.Int(q.den)

OutIrr(x):
    r = mkRat(x.rat.num,x.rat.den)
    b = mkRat(x.irr.num,x.irr.den)
    if b.num == 0:
        OutRat(r); return
    if r.num != 0: OutRat(r)
    if b.num < 0: Out.String("-")
    else if r.num != 0: Out.String("+")
    c = mkRat(abs(b.num),b.den)
    if c.num != c.den:
        OutRat(c); Out.String("*")
    Out.String("sqrt(5)")
```

Thus the examples print **`1/2+1/2*sqrt(5)`** and **`2`**; zero prints `0`, and pure unit radicals print `sqrt(5)` or `-sqrt(5)`. The positive-denominator invariant makes the coefficient sign test reliable. Input records are not mutated.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
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
