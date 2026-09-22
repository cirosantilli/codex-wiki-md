<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Assume `less` is a lawful strict comparison, for example a [strict weak order](../../../../../strict-weak-order.md), and the two input [linked lists](../../../../../linked-list.md) are disjoint and sorted by it. Allocate a result header and move existing data [linked list nodes](../../../../../linked-list-node.md); do not copy their values.
```
PROCEDURE Merge(less: LESS; q, r: List; VAR p: List);
VAR result: List; last, a, b: Tail;
BEGIN
  NEW(result); result.count := q.count + r.count;
  result.tail := NIL; last := result;
  a := q.tail; b := r.tail;
  WHILE (a # NIL) & (b # NIL) DO
    IF less(b,a) THEN
      last.tail := b; b := b.tail
    ELSE
      last.tail := a; a := a.tail
    END;
    last := last.tail
  END;
  IF a # NIL THEN last.tail := a ELSE last.tail := b END;
  q.tail := NIL; q.count := 0;
  r.tail := NIL; r.count := 0;
  p := result
END Merge;
```
The [loop invariant](../../../../../loop-invariant.md) says that the segment from `result.tail` through `last` is a sorted prefix of the desired [merge algorithm](../../../../../merge-algorithm.md), containing exactly the nodes already removed from the two unread chains. Every element of this prefix is no greater than either unread head. Choosing the smaller unread head maintains this property; choosing from `q` on a tie also gives [stable sorting](../../../../../stable-sorting.md).

At exit, at most one unread chain is nonempty, and its sorted suffix can be attached as a whole. Each original data [linked list node](../../../../../linked-list-node.md) occurs exactly once in the result, and its saved count is correct. Clearing the consumed headers prevents them from claiming ownership of the result's nodes.

$$
\boxed{\text{Sorted stable merge; time }O(|q|+|r|),\text{ one new header.}}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
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
