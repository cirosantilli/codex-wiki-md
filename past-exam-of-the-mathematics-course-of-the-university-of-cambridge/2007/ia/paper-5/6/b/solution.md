<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Carry the list as an immutable accumulator instead of storing it in a reference:
```
fun snackerPure m =
    let
      fun collect (Snack x, acc) = x :: acc
        | collect (Lunch (a, b), acc) =
            collect (b, collect (a, acc))
        | collect (Feast (a, b, c), acc) =
            collect (c, collect (b, collect (a, acc)))
    in
      collect (m, [])
    end;
```
For any initial accumulator `acc`, [structural induction](../../../../../../structural-induction.md) shows that `collect(m,acc)` equals the final reference content obtained by traversing `m` left to right and prepending each snack to a reference initially containing `acc`. At `Lunch` and `Feast`, the accumulator passed to each child is the result of all earlier children, exactly matching the imperative sequencing. Thus the result is the **reverse of the left-to-right list of snack labels**, just as for the original `snacker`; returning the ordinary left-to-right list would be incorrect. The code uses no mutable cells and is polymorphic, with type `'a meal -> 'a list`.

## ↑ Ancestors (11)

1. [B](../b.md)
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
