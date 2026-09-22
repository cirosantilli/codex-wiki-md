<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Store a [complete binary tree](../../../../../complete-binary-tree.md) in an [array](../../../../../array-data-structure.md) $H[0..n)$, with children $2i+1,2i+2$ and parent $\lfloor(i-1)/2\rfloor$. The [max-heap](../../../../../max-heap.md) invariant says every parent's key is at least its children's keys. Consequently the root is a greatest-key item, and the height is $\lfloor\log_2 n\rfloor$.

Here is a pairwise-exchange implementation of `extractMax`:

```
extractMax(H, n):
    if n == 0: error "empty priority queue"
    answer = H[0]
    swap(H[0], H[n-1])
    n = n - 1
    i = 0
    while 2*i + 1 < n:
        j = 2*i + 1
        if j + 1 < n and key(H[j+1]) > key(H[j]):
            j = j + 1
        if key(H[i]) >= key(H[j]): break
        swap(H[i], H[j])
        i = j
    return (answer, n)
```

Only the root can initially violate [heap order](../../../../../heap-order.md). Each [heapify down](../../../../../sift-down.md) exchange promotes the larger child, making the previous position valid and moving the only possible violation down one level. It either stops at a valid position or reaches a leaf. The removed root is saved as `answer`, and reducing the active [array](../../../../../array-data-structure.md) length preserves the [complete binary tree](../../../../../complete-binary-tree.md) shape.

The [binary heap](../../../../../binary-heap.md) operation costs, with existing positions available for handle operations, are:

| Operation | Worst-case time |
| --- | --- |
| Empty initialization, `isEmpty`, `size` | $O(1)$ |
| `maximum` | $O(1)$ |
| `insert`, `increaseKey` | $O(\log(n+1))$ |
| `extractMax`, deletion by handle | $O(\log(n+1))$ |
| Build from $n$ arbitrary items by [bottom-up heap construction](../../../../../bottom-up-heap-construction.md) | $O(n)$ |

Insertion into the [binary heap](../../../../../binary-heap.md) places an item at the next leaf and moves it upward until [heap order](../../../../../heap-order.md) holds. Raising a key uses the same upward repair. Arbitrary deletion replaces its position by the final item and repairs upward or downward as necessary. A handle must be updated on exchanges; locating an item by value alone can require linear search. The boxed main bounds are $\boxed{\operatorname{maximum}:O(1),\quad\operatorname{insert},\operatorname{extractMax}:O(\log(n+1))}$. Dynamic [array](../../../../../array-data-structure.md) resizing is usually amortized or avoided by reserving sufficient capacity.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
