<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Represent a [binary search tree](../../../../../../binary-search-tree.md) by:
```
sml
datatype ('k, 'v) dict = Empty
    | Branch of ('k, 'v) dict * 'k * 'v * ('k, 'v) dict;
```
Assume the provided `lookup d key` returns `NONE` or `SOME value`, and `update d (key, value)` returns the updated [binary search tree](../../../../../../binary-search-tree.md). Traverse the first dictionary, retaining only a key with the same value in the second:
```
sml
fun intersection equal d1 d2 =
    let
        fun visit Empty result = result
          | visit (Branch (left, key, value, right)) result =
              let
                  val r1 = visit left result
                  val r2 =
                      case lookup d2 key of
                          NONE => r1
                        | SOME other =>
                            if equal (value, other)
                            then update r1 (key, value)
                            else r1
              in
                  visit right r2
              end
    in
        visit d1 Empty
    end;
```
For equality-type values, call `intersection (op =) d1 d2`. An explicit value comparison parameter also handles values for which [Standard ML](../../../../../../standard-ml.md) does not define built-in equality. This distinguishes absent keys from defined values without reserving a sentinel value.

Every inserted entry belongs to both input dictionaries with the same value, so the result agrees with each. Conversely, each common equal-valued entry is visited in `d1`, found in `d2`, and inserted. Any dictionary agreeing with both can contain only those entries. Thus **the result is exactly the largest common dictionary**, not merely an intersection of key sets. If `d1` has $m$ entries, lookup height is $h_2$, and maximum result-tree height during insertion is $h_r$, the [time complexity](../../../../../../time-complexity.md) is $O(m(1+h_2+h_r))$ for constant-cost comparisons. Logarithmic heights require a balancing assumption; an ordinary unbalanced [binary search tree](../../../../../../binary-search-tree.md) can have linear height.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
