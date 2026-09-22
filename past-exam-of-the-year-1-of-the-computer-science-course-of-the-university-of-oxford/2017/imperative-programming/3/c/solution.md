<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [sentinel node](../../../../../sentinel-node.md) is a permanent header whose key is ignored and whose `next` field holds the first data node. Every data node then has a predecessor, including the first, so unlinking always updates a predecessor's `next` field.

```
function DelMin(hd: List): List
    require hd != nil and hd.next != nil
    bestPrev := hd
    p := hd.next
    while p.next != nil do
        if p.next.x < bestPrev.next.x then
            bestPrev := p
        p := p.next
    result := bestPrev.next
    bestPrev.next := result.next
    result.next := nil
    return result
```

The processed data prefix ends at `p`. Its minimum is `bestPrev.next`, and `bestPrev` remains that node's actual predecessor. This [loop invariant](../../../../../loop-invariant.md) is initialized by the first node and preserved when a strictly smaller next node is found. The unprocessed suffix length is a [loop variant](../../../../../loop-variant.md). At exit, the final splice removes the first minimum in one uniform case. This is [linked-list minimum extraction](../../../../../linked-list-minimum-extraction.md); it requires at least one data node, rather than treating the dummy header as an element.

## ↑ Ancestors (12)

1. [C](../c.md)
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
