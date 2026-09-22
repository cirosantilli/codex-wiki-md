<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use a [linear search](../../../../../linear-search.md) over every pair of [array indices](../../../../../array-index.md).
```
PROCEDURE SearchAll(x: INTEGER; VAR i, j: INTEGER): BOOLEAN;
VAR r, c: INTEGER;
BEGIN
  FOR r := 0 TO M-1 DO
    FOR c := 0 TO N-1 DO
      IF f[r,c] = x THEN i := r; j := c; RETURN TRUE END
    END
  END;
  RETURN FALSE
END SearchAll;
```
For a worst-case lower bound, consider an input in which every inspected element differs from $x$. If an element remains uninspected, changing just that element to $x$ gives an indistinguishable execution requiring the opposite answer. Therefore a correct exact [search algorithm](../../../../../search-algorithm.md) must inspect all $MN$ elements in the worst case.

The printed phrase “at least $O(MN)$” uses the upper-bound notation for a lower-bound claim. Its precise interpretation is

$$
\boxed{\text{Worst-case lower bound }\Omega(MN);\quad\text{the scan takes }\Theta(MN).}
$$

This is an [adversary argument](../../../../../adversary-argument.md) for access to arbitrary independent [array](../../../../../array-data-structure.md) entries.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
