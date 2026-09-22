<h1 id="6/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a pure predicate `p`, the ordinary [linked list](../../../../../../../linked-list.md) version copies only the surviving spine:
```
sml
fun filterO p ONil = ONil
  | filterO p (OCons (x, xs)) =
      if p x then OCons (x, filterO p xs)
      else filterO p xs;
```
For a [lazy list](../../../../../../../lazy-list.md), return a delayed computation. Searching for the next retained element begins only when this computation is forced:
```
sml
fun filterL p stream () =
    case stream () of
        LNil => LNil
      | LCons (x, rest) =>
          if p x then LCons (x, filterL p rest)
          else filterL p rest ();
```
A retained element has a delayed filtered tail, so the whole input is not forced at once. A long run of rejected elements must still be traversed to find the next match. If an infinite [lazy list](../../../../../../../lazy-list.md) has no matching element beyond the current position, forcing the next result does not terminate; laziness does not promise productivity for every predicate.

The destructive [mutable list](../../../../../../../mutable-list.md) version operates on the link reaching the current node:
```
sml
fun filterM p link =
    case !link of
        MNil => ()
      | MCons (x, tail) =>
          if p x then filterM p tail
          else (link := !tail; filterM p link);
```
When a node survives, recurse on its tail link. When it fails, bypass it by copying its successor into the same link and inspect that link again, which correctly handles several consecutive rejected nodes. **No new list nodes are allocated.** In particular, changing the root [ML reference type](../../../../../../../ml-reference-type.md) cell handles deletion of the head. These arguments assume finite acyclic input for the eager and destructive versions and a predicate that does not itself mutate the list. Aliases observe the mutations; a detached node is not promised to disappear from all external references.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [6](../../../6.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
