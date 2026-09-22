<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [heapsort](../../../../../heapsort.md), use the usual [array](../../../../../array-data-structure.md) representation of a [max-heap](../../../../../max-heap.md), indexed from zero, with children $2i+1,2i+2$. Build the [max-heap](../../../../../max-heap.md) from the last internal node towards the root, using [heapify down](../../../../../sift-down.md). The three build stages are

```
start                    [2,7,3,2,8,1]
sift at index 2          [2,7,3,2,8,1]
sift at index 1          [2,8,3,2,7,1]
sift at index 0          [8,7,3,2,2,1]
```

At index zero, the value `2` moves below `8` and then below `7`. Next exchange the root with the last active element, shorten the active [heap](../../../../../heap-data-structure.md), and restore [heap order](../../../../../heap-order.md). A vertical separator below distinguishes the active prefix from its sorted final suffix.

| Removed maximum | After root exchange | After restoring [heap order](../../../../../heap-order.md) |
| --- | --- | --- |
| $8$ | `1,7,3,2,2 | 8` | `7,2,3,1,2 | 8` |
| $7$ | `2,2,3,1 | 7,8` | `3,2,2,1 | 7,8` |
| $3$ | `1,2,2 | 3,7,8` | `2,1,2 | 3,7,8` |
| $2$ | `2,1 | 2,3,7,8` | `2,1 | 2,3,7,8` |
| $2$ | `1 | 2,2,3,7,8` | `1 | 2,2,3,7,8` |

The trace chooses the left child when equal children tie; other tie conventions can give different intermediate [heaps](../../../../../heap-data-structure.md) with the same sorted output.

For [quicksort](../../../../../quicksort.md), use the head as pivot and partition the remaining elements into those strictly less than it and those greater than or equal to it, retaining their order within each partition. This specifies how the duplicate `2` is handled:

```
pivot 2:  [1]       | 2 | [7,3,2,8]
pivot 7:  [3,2]     | 7 | [8]
pivot 3:  [2]       | 3 | []
```

Empty and singleton [lists](../../../../../list-abstract-data-type.md) are already sorted. Returning from the recursive calls gives

```
Q [3,2]       = [2] ++ [3] ++ []       = [2,3]
Q [7,3,2,8]   = [2,3] ++ [7] ++ [8]   = [2,3,7,8]
Q [2,7,3,2,8,1] = [1] ++ [2] ++ [2,3,7,8]
```

For [counting sort](../../../../../counting-sort.md), count keys $1$ through $8$. After reading each input key, the count vector is

```
initial: (0,0,0,0,0,0,0,0)
read 2:  (0,1,0,0,0,0,0,0)
read 7:  (0,1,0,0,0,0,1,0)
read 3:  (0,1,1,0,0,0,1,0)
read 2:  (0,2,1,0,0,0,1,0)
read 8:  (0,2,1,0,0,0,1,1)
read 1:  (1,2,1,0,0,0,1,1)
```

The cumulative counts are $(1,3,4,4,4,4,5,6)$. For the usual [stable sorting](../../../../../stable-sorting.md) version with zero-based output indices, scan the input from right to left, place a key $k$ at position $C[k]-1$, and decrement $C[k]$. The successive placements are `1` at $0$, `8` at $5$, the later `2` at $2$, `3` at $3$, `7` at $4$, and the earlier `2` at $1$. The final answer for all three [sorting algorithms](../../../../../sorting-algorithm.md) is

$$
\boxed{[1,2,2,3,7,8].}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [5](../../5.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
