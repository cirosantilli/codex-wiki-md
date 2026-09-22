<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [binary search](../../../../../binary-search.md). Maintain an inclusive candidate interval `[lo,hi]`, initially `[0,n-1]`. Compare the target `v` once with the middle entry; a ternary comparison returns less than, equal to, or greater than. Equality ends successfully. Otherwise [sortedness](../../../../../sortedness.md) permits discarding the middle entry and the entire half on the wrong side:

```
lo := 0; hi := n-1;
WHILE lo <= hi DO
  mid := lo + (hi-lo) DIV 2;
  IF v = S[mid] THEN RETURN TRUE
  ELSIF v < S[mid] THEN hi := mid-1
  ELSE lo := mid+1
  END
END;
RETURN FALSE
```

The two written tests represent _one_ ternary comparison whose result is then inspected. The [loop invariant](../../../../../loop-invariant.md) says that every occurrence of `v`, if any, lies in the candidate interval. Initially it is true. The order comparison and [sortedness](../../../../../sortedness.md) preserve it after either discard. If the interval becomes empty, the [loop invariant](../../../../../loop-invariant.md) proves absence.

A failed comparison reduces a candidate interval of size $m$ to at most $\lfloor m/2\rfloor$. For $n\geq1$, at most $\lfloor\log_2 n\rfloor+1$ comparisons are needed; an empty input needs none. Hence

$$
\boxed{C(n)\leq\lfloor\log_2 n\rfloor+1=O(\log n)\quad(n\geq1).}
$$

The claim counts comparisons. Indexed access to an [array](../../../../../array-data-structure.md) also makes elapsed running time logarithmic in the usual model; a [linked list](../../../../../linked-list.md) representation would not give the same access cost.

## ↑ Ancestors (12)

1. [C](../c.md)
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
