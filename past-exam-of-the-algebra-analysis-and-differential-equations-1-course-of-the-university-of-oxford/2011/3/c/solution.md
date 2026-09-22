<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N$ count everyone present, including the host. The grouping, seating and departure conditions give the [modular congruences](../../../../modular-congruence.md)

$$
N\equiv4\pmod5,\qquad N\equiv3\pmod9,\qquad N\equiv1\pmod2.
$$

The first two imply $N=39+45k$, and oddness forces $k$ even. By the [Chinese remainder theorem](../../../../chinese-remainder-theorem.md), the complete solution is

$$
\boxed{N\equiv39\pmod{90}.}
$$

Because not every invitee attended, at most $y-1$ guests came, so $N\leq y$. For $y=120$, the only positive possibility is **39 people**. It is feasible: seven groups of five and one of four; three tables of ten and one of nine; nineteen departing pairs and the host.

For $y=150$, both **39 and 129 people** are possible. The latter uses twenty-five groups of five and one of four, three tables of ten and eleven of nine, and sixty-four departing pairs. Thus the larger invitation count destroys uniqueness; it does not force a different attendance.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
