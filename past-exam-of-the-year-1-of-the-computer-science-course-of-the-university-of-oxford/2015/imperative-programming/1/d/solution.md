<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $L$ be the final output length, $k$ the number of emitted markers, and $s$ the number of pending handles. Each pending [subtree](../../../../../subtree.md) contributes at least one future marker, so

$$
k+s\leq L\leq\operatorname{LEN}(\mathrm{out}).
$$

Store output from the low end and the [stack](../../../../../stack-data-structure.md) from the high end of the same [array](../../../../../array-data-structure.md). A pop frees one cell before the next write. For a fork, the two pushed children each account for at least one of the remaining markers. Thus the two regions never overlap.
```
PROCEDURE PreorderShared(t: Tree; VAR out: ARRAY OF INTEGER;
                         VAR count: INTEGER);
VAR top, cap: INTEGER; p: Tree;
BEGIN
  cap := LEN(out); count := 0;
  top := cap-1; out[top] := t;
  WHILE top < cap DO
    p := out[top]; INC(top);
    IF p = 0 THEN
      out[count] := 0; INC(count)
    ELSE
      out[count] := 1; INC(count);
      DEC(top); out[top] := nodes[p-1].right;
      DEC(top); out[top] := nodes[p-1].left
    END
  END
END PreorderShared;
```
The [loop invariant](../../../../../loop-invariant.md) includes `count <= top`, with pending handles in `out[top..cap)` and final markers in `out[0..count)`. The preceding accounting proves every intermediate write also respects [array bounds](../../../../../array-bounds.md). This uses the [integer](../../../../../integer-split.md) handle representation chosen in part (b). Simply putting a [pointer](../../../../../pointer-computer-programming.md) into a genuinely [Boolean](../../../../../boolean-data-type.md)-typed cell would not be valid [Oberon](../../../../../oberon-programming-language.md).

$$
\boxed{\text{One result array suffices; additional working storage is }O(1).}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
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
