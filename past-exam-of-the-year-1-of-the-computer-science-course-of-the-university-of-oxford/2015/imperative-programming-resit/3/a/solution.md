<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Return the exclusive endpoint of the [maximal initial run](../../../../../maximal-initial-run.md):
```
PROCEDURE Run(a, b: INTEGER): INTEGER;
VAR c: INTEGER;
BEGIN
  IF a = b THEN RETURN b END;
  c := a+1;
  WHILE c < b DO
    IF u[c-1] > u[c] THEN RETURN c END;
    c := c+1
  END;
  RETURN c
END Run;
```
The [loop invariant](../../../../../loop-invariant.md) is $a<c\leq b$ and $u[a..c)$ is nondecreasing. An unsuccessful adjacent-order test extends the run by one; a strict descent at $c$ prevents any extension across it. If $c=b$, the whole segment is a run. The [loop variant](../../../../../loop-variant.md) is $b-c$.

$$
\boxed{u[a..\operatorname{Run}(a,b))\text{ is the maximal initial run}.}
$$

For a run of length $s>0$, the [running time](../../../../../running-time.md) is $\Theta(s)$, including at most one failed extension test; an empty segment takes $\Theta(1)$.

## ↑ Ancestors (12)

1. [A](../a.md)
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
