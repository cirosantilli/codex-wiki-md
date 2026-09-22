<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For integer [linked lists](../../../../../../linked-list.md), compare their heads and copy the smaller head, retaining the other list for the next step:
```
fun merge ([], ys) = ys
  | merge (xs, []) = xs
  | merge (xs as x :: xt, ys as y :: yt) =
      if x <= y then x :: merge (xt, ys)
      else y :: merge (xs, yt);
```
This [merge algorithm](../../../../../../merge-algorithm.md) preserves duplicates and chooses the left list on a tie, making it stable when elements have an ordering key. Each recursive step decreases the combined length. For correctness, the chosen head is no greater than either remaining head and therefore no greater than any remaining element; [structural induction](../../../../../../structural-induction.md) then proves that the result is ordered and contains exactly the elements of both inputs. For other element types, replace the integer comparison by a supplied ordering function. **Merge repeatedly emits the smaller head and reuses the remaining list when the other becomes empty.**

## ↑ Ancestors (11)

1. [A](../a.md)
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
