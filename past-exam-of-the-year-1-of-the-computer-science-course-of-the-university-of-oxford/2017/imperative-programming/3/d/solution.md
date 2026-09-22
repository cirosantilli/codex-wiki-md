<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Repeatedly detach the minimum and append that very node to a separate output chain:

```
function Sort(xs: List): List
    allocate dummy headers remaining and output
    remaining.next := xs
    output.next := nil
    tail := output
    while remaining.next != nil do
        p := DelMin(remaining)
        tail.next := p
        tail := p
    return output.next
```

The [loop invariant](../../../../../loop-invariant.md) says that the output and remaining chains contain disjoint subsets of the original data nodes, together containing every original node exactly once. The output is nondecreasing, its final key is no larger than any remaining key, and `tail` points to its final node, or to the dummy header when empty. Its outgoing link is `nil` because `DelMin` detaches the returned node. Appending the remaining minimum preserves all these properties; the remaining node count decreases by one.

At exit the output is the complete sorted bag. This iterative [selection sort](../../../../../selection-sort.md) preserves duplicate occurrences and, with first-minimum tie handling, their original relative order. It uses $\Theta(N^2)$ time and $O(1)$ auxiliary nodes. “Increasing” here means nondecreasing when equal keys occur.

## ↑ Ancestors (12)

1. [D](../d.md)
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
