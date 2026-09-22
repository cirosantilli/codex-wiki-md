<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [loop invariant](../../../../../loop-invariant.md) in [binary long division](../../../../../binary-long-division.md) says exactly where the true [integer](../../../../../integer-split.md) quotient $Q=\lfloor x/y\rfloor$ lies:

$$
x=qy+r,\quad0\leq r<y2^j
\quad\Longrightarrow\quad
\boxed{q\leq Q<q+2^j.}
$$

Halving `p` proposes the midpoint `q+p` of this candidate interval. The comparison `r >= y*p` is equivalent to `(q+p)*y <= x`, so it decides whether the quotient is in the upper or lower half. Adding `p` chooses the upper half; leaving `q` unchanged chooses the lower half. Thus [binary long division](../../../../../binary-long-division.md) is [binary search](../../../../../binary-search.md) for the last [integer](../../../../../integer-split.md) satisfying $qy\leq x$, deciding the quotient's [binary numeral system](../../../../../binary-numeral-system.md) digits from most significant to least significant. The doubling loop first finds a power-of-two interval containing that quotient.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2003](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
