<h1 id="5/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the abstract state be the [set](../../../../../../set-split.md) $B$ of occupied coordinate pairs. For the Boolean [array](../../../../../../array-data-structure.md), the [abstraction function](../../../../../../abstraction-function.md) is $\alpha(occupied)=\{(x,y):occupied(y)(x)\}$. Its [representation invariant](../../../../../../representation-invariant.md) requires an $N\times N$ Boolean [array](../../../../../../array-data-structure.md) and the downward-closure property

$$
(x,y)\in B\ \Longrightarrow\ (i,j)\in B
\quad\text{whenever }0\leq i\leq x,\ 0\leq j\leq y.
$$

Thus $B$ is an [order ideal](../../../../../../order-ideal.md) for the coordinatewise [partial order](../../../../../../partially-ordered-set.md). Removing an upper-right rectangle preserves this property. The empty [set](../../../../../../set-split.md) is allowed after the losing move.

For the row-boundary [array](../../../../../../array-data-structure.md), the [abstraction function](../../../../../../abstraction-function.md) and [representation invariant](../../../../../../representation-invariant.md) are

$$
\alpha(row)=\{(x,y):0\leq y<N,\ 0\leq x<row(y)\},
\qquad N\geq row(0)\geq\cdots\geq row(N-1)\geq0.
$$

The [array](../../../../../../array-data-structure.md) has length $N$. Removing at $(x,y)$ replaces each `row(j)` for $j\geq y$ by $\min(row(j),x)$. Earlier rows are unchanged. This both implements the abstract removal and preserves the nonincreasing boundary.

Without a cached count, the Boolean representation takes $\Theta(N^2)$ for `Count`, $O(1)$ for `Legal`, $O(N^2)$ worst-case for `Move`, and $\Theta(N^2)$ for a full-grid `Display`. The boundary representation takes $\Theta(N)$ for `Count`, $O(1)$ for `Legal`, $O(N)$ worst-case for `Move`, and $\Theta(N^2)$ for the same full-grid `Display`. Their [space complexities](../../../../../../space-complexity.md) are respectively $\Theta(N^2)$ and $\Theta(N)$. A scalar cached total makes `Count` $O(1)$ in either representation if each move updates it consistently. The implementation below uses that cache with the boundary [array](../../../../../../array-data-structure.md), so it achieves **constant-time `Count` and `Legal`, linear worst-case `Move`, and linear storage**. Full-grid output still takes quadratic time because it emits quadratic many cell positions.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Imperative programming resit](../../../../imperative-programming-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
