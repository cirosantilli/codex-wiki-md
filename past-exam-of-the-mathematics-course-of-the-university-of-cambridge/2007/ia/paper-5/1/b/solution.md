<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split the list into two contiguous halves, sort each recursively, and use the [merge algorithm](../../../../../../merge-algorithm.md) from part (a):
```
fun mergesort [] = []
  | mergesort [x] = [x]
  | mergesort xs =
      let
        val k = List.length xs div 2
        val left = List.take (xs, k)
        val right = List.drop (xs, k)
      in
        merge (mergesort left, mergesort right)
      end;
```
`List.length` counts elements, `List.take(xs,k)` returns the first $k$ elements and `List.drop(xs,k)` returns the remaining suffix. Since $0<k<n$ when $n\ge2$, both recursive inputs are smaller and differ in length by at most one. [Mathematical induction](../../../../../../mathematical-induction.md) on length proves that each half is sorted without losing elements, and the correctness of the [merge algorithm](../../../../../../merge-algorithm.md) proves the same for the combined result. Contiguous splitting and left-biased equal-key merging preserve the original relative order of equal keys. **This is a stable top-down [merge sort](../../../../../../merge-sort.md).**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
