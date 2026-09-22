<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Treat the live [array](../../../../../array-data-structure.md) segment as a [FIFO queue](../../../../../fifo-queue.md) of runs. Remove its first two runs, append their merged result, and repeat:
```
PROCEDURE Sort(a, b: INTEGER; VAR c, d: INTEGER);
VAR x, y, z: INTEGER;
BEGIN
  c := a; d := b;
  WHILE c < d DO
    x := Run(c, d);
    IF x = d THEN RETURN END;
    y := Run(x, d);
    z := y-c;
    Merge(c, x, y, d);
    c := y;
    d := d+z
  END
END Sort;
```
Compute both run boundaries before writing the destination, which starts at the old `d`. The untouched suffix $u[y..d)$ is followed by the new merged run. The endpoints returned in `c,d` always describe the live [sequence](../../../../../sequence.md); obsolete values before `c` are ignored. As allowed, assume enough destination capacity.

For example, $[3,1,4,2]$ becomes the live [sequence](../../../../../sequence.md) $[2,1,3,4]$, then $[1,2,3,4]$. The first merge combines $[3]$ and $[1,4]$, and the second combines $[2]$ and $[1,3,4]$.

$$
\boxed{u[c..d)\text{ contains the sorted input and }d-c=b-a.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
