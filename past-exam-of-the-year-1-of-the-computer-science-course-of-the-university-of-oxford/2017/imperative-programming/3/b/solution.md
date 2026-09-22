<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Treat removal of the first node separately; otherwise find its predecessor:

```
procedure Remove(x: List; var xs: List)
    require x is a node reachable from xs
    if xs = x then
        xs := x.next
    else
        p := xs
        while p.next != x do
            p := p.next
        p.next := x.next
    x.next := nil
```

In the search branch the [loop invariant](../../../../../loop-invariant.md) says that `p` is before `x` in the original [linked list](../../../../../linked-list.md), `x` is reachable from `p.next`, and no links have yet changed. The remaining link distance to `x` decreases at every advance, so membership of `x` guarantees a predecessor is found. Bypassing it removes exactly that cell, rather than an arbitrary equal-valued cell. Detaching `x.next` leaves a standalone removed node and preserves the relative order and [object identities](../../../../../object-identity.md) of all retained nodes.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
