<h1 id="4/c/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Save the last entry, shift the others right in descending index order, and put the saved value at the left. Descending order prevents overwriting an unread entry.
```
PROCEDURE rotate(i, n, k: INTEGER);
VAR x: T; step, t: INTEGER;
BEGIN
  IF (k = 0) OR (k = n) THEN RETURN END;
  step := 0;
  WHILE step < k DO
    x := m[i+n-1];
    t := n-1;
    WHILE t > 0 DO
      m[i+t] := m[i+t-1];
      t := t-1
    END;
    m[i] := x;
    step := step+1
  END
END rotate;
```
For one pass, after the shifts at offsets greater than `t`, those positions contain the original preceding entries; offsets through `t` are still available, and `x` retains the original last entry. The [loop variant](../../../../../../loop-variant.md) `t` decreases to zero. The outer [loop invariant](../../../../../../loop-invariant.md) is that the segment has been rotated right by `step` places relative to its initial state. Repeating a one-step [cyclic permutation](../../../../../../cyclic-permutation.md) $k$ times therefore gives the required [array rotation](../../../../../../array-rotation.md). **The method uses one extra `T` variable and $O(kn)$ time**, with $O(1)$ auxiliary space. The early return avoids all accesses for an identity rotation.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
