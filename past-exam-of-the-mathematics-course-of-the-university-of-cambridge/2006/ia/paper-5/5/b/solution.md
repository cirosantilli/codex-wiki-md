<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Generate every [permutation](../../../../../../permutation.md) of the tail, then insert its missing head at every possible position. The helper preserves order among the elements already present:
```
sml
fun insertEverywhere x [] = [[x]]
  | insertEverywhere x (y :: ys) =
      (x :: y :: ys) ::
      List.map (fn zs => y :: zs) (insertEverywhere x ys);

fun permutations [] = [[]]
  | permutations (x :: xs) =
      List.concat
        (List.map (insertEverywhere x) (permutations xs));
```
The first helper result inserts $x$ before $y$; the mapped recursive results put $y$ back at the front and insert $x$ farther along. For a list of length $k$, it yields exactly $k+1$ positions. The empty list has one [permutation](../../../../../../permutation.md), itself, so the base result is `[[]]`, not `[]`.

For correctness, use [structural induction](../../../../../../structural-induction.md). Any [permutation](../../../../../../permutation.md) of `x :: xs` has a unique position containing $x$. Removing that position leaves a [permutation](../../../../../../permutation.md) of `xs`, supplied by the induction hypothesis; reinserting $x$ at its unique position reconstructs the required output. With distinct input elements, neither the tail [permutation](../../../../../../permutation.md) nor the insertion position can be duplicated, so each output occurs once. Consequently **a length-$n$ input yields exactly $n!$ permutations**, in an unrestricted order. The explicit output is large; this is not a polynomial-time enumeration with respect to $n$ alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
