<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the flattened Boolean [array](../../../../../../array-data-structure.md), the [abstraction function](../../../../../../abstraction-function.md) selects the true cells. A suitable [representation invariant](../../../../../../representation-invariant.md) requires the occupied cells to form a [order ideal](../../../../../../order-ideal.md): an occupied $(x,y)$ implies occupancy of every $(i,j)$ with $i\leq x,j\leq y$. Deleting a northeast rectangle preserves that property.

For column heights, the invariant is $N\geq h(0)\geq h(1)\geq\cdots\geq h(N-1)\geq0$, and the [abstraction function](../../../../../../abstraction-function.md) is $B=\{(x,y):0\leq x<N,\ 0\leq y<h(x)\}$. A legal move replaces every $h(i)$ for $i\geq x$ by $\min(h(i),y)$, preserving the invariant. This is an [order-ideal board representation](../../../../../../order-ideal-board-representation.md).

For a fair comparison, allow either representation a scalar cached token count: `Count` and `Legal` then take $O(1)$ in both. Without that cache, counting needs $\Theta(N^2)$ Boolean inspections versus $\Theta(N)$ height additions. A move takes $O(N^2)$ in the worst case in the flattened representation and $O(N)$ with heights. Displaying the full square takes $\Theta(N^2)$ character positions in either. Heights use **$\Theta(N)$ [array](../../../../../../array-data-structure.md) entries rather than $\Theta(N^2)$**, so they are superior for the requested operations; their initialization also takes only $\Theta(N)$ time.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Imperative programming (resit)](../../../../imperative-programming-resit-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
