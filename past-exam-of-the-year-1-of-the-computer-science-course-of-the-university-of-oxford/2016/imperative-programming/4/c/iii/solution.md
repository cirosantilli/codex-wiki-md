<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Replace the sole recursive call by updates to the current segment's parameters:
```
PROCEDURE rotate(i, n, k: INTEGER);
VAR a, b: INTEGER;
BEGIN
  WHILE (k > 0) AND (k < n) DO
    a := n-k; b := k;
    IF a = b THEN
      blockswap(i, i+a, a);
      RETURN
    ELSIF a < b THEN
      blockswap(i, i+b, a);
      n := b; k := b-a
    ELSE
      blockswap(i, i+a, b);
      i := i+b; n := a; k := b
    END
  END
END rotate;
```
The [loop invariant](../../../../../../loop-invariant.md) is that every position outside the current unresolved segment already has its final value, while rotating the current segment by the current `k` completes the original [array rotation](../../../../../../array-rotation.md). The block decompositions in part (ii) prove preservation. The positive unresolved length decreases in each continuing branch; the equal-block branch finishes immediately. **The same rotation now uses $O(1)$ auxiliary space**, including control storage, and leaves the rest of the [array](../../../../../../array-data-structure.md) untouched.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
