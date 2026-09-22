<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use two indices, initially the first and last positions of the ordered [sequence](../../../../../sequence.md). The two elements occupy distinct positions, so continue only while `i < j`:

```
i := 0; j := n-1;
WHILE i < j DO
  t := S[i] + S[j];
  IF t = x THEN RETURN TRUE
  ELSIF t < x THEN i := i+1
  ELSE j := j-1
  END
END;
RETURN FALSE
```

The [loop invariant](../../../../../loop-invariant.md) is: a solution exists in the original input if and only if one exists with both indices in `[i,j]`. If `S[i]+S[j] < x`, then `S[i]+S[k] <= S[i]+S[j] < x` for every `k <= j`, so index `i` cannot belong to a remaining solution. If the sum is too large, `S[k]+S[j] >= S[i]+S[j] > x` for every `k >= i`, so index `j` cannot belong to one. This proves preservation of the [loop invariant](../../../../../loop-invariant.md). Equality gives the desired pair, and an interval with fewer than two positions contains none.

Every unsuccessful iteration decreases the [loop variant](../../../../../loop-variant.md) `j-i` by one, so there are at most $n-1$ sum comparisons and only [constant space](../../../../../constant-space.md) is needed. Duplicate values are permitted if they occupy distinct positions. Under exact constant-cost real arithmetic and endpoint access,

$$
\boxed{\text{two-pointer two-sum uses }O(n)\text{ time and }O(1)\text{ auxiliary space}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
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
