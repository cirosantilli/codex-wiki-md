<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Remember the minimum node while scanning the remaining suffix:

```
function FindMin(xs: List): List
    require xs != nil
    best := xs
    p := xs.next
    while p != nil do
        if p.x < best.x then best := p
        p := p.next
    return best
```

The [loop invariant](../../../../../loop-invariant.md) says that the processed prefix is nonempty, `best` is a node of that prefix, and its key is no greater than any other processed key. The links are unchanged. Advancing `p` extends the prefix by one; the number of unprocessed nodes decreases. When it reaches `nil`, `best` is the minimum of the whole finite [singly linked list](../../../../../singly-linked-list.md). Strict comparison retains the first minimum among ties.

## ↑ Ancestors (12)

1. [A](../a.md)
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
