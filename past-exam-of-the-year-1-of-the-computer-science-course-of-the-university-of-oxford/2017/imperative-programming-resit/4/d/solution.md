<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Distribute every term of one input across every term of the other, using the same private accumulator:

```
mulPoly(x,y):
    r = NIL
    p = x
    while p != NIL:
        q = y
        while q != NIL:
            accumulate(r,p.coeff*q.coeff,p.power+q.power)
            q = q.next
        p = p.next
    return r
```

The inner-loop invariant says that the current result contains all products from earlier nodes of `x`, plus the current `x` node multiplied by the processed prefix of `y`. The outer invariant is the corresponding statement for completed rows of products. The [distributive property](../../../../../distributive-property.md) then proves correctness. Powers add, equal powers combine, zero products and cancellations disappear. Both input lists are only read, and an empty input gives the zero polynomial.

There are $mn$ coefficient products. If at most $u$ result nodes are present at a time, the simple unsorted accumulator costs $O(mn(1+u))$, with $u\leq mn$; it is correct without claiming a linear-time multiplication.

## ↑ Ancestors (12)

1. [D](../d.md)
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
