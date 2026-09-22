<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Carry the number of original snacks still to skip, returning it together with the reconstructed subtree. Zero means that the replacement has already happened:
```
fun glut k meal replacement =
    let
      fun visit (t, 0) = (t, 0)
        | visit (Snack x, j) =
            if j = 1 then (replacement, 0)
            else (Snack x, j - 1)
        | visit (Lunch (a, b), j) =
            let val (a1, j1) = visit (a, j)
                val (b1, j2) = visit (b, j1)
            in (Lunch (a1, b1), j2) end
        | visit (Feast (a, b, c), j) =
            let val (a1, j1) = visit (a, j)
                val (b1, j2) = visit (b, j1)
                val (c1, j3) = visit (c, j2)
            in (Feast (a1, b1, c1), j3) end
    in
      if k < 1 then raise Subscript
      else
        let val (answer, remaining) = visit (meal, k)
        in if remaining = 0 then answer else raise Subscript end
    end;
```
The successive bindings explicitly establish left-to-right counting. Before the target is reached, each original snack decreases the counter by one; at the target the subtree becomes `replacement` and the counter becomes zero. Subsequent subtrees are returned unchanged, and newly inserted snacks are never counted. [Structural induction](../../../../../../structural-induction.md) on the helper's subtree establishes this invariant and proves the specified one-based substitution. The result has type `int -> 'a meal -> 'a meal -> 'a meal`. Since unaltered original snacks remain, their label type must agree with the replacement's label type.

The behavior for an invalid index is not specified in the PDF; this implementation deliberately raises `Subscript` for $k\le0$ or too few snacks. For valid input, **exactly the $k$th original snack in left-to-right order is replaced**. Sharing untouched immutable subtrees is semantically equivalent to a fresh structural copy.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [6](../../6.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
