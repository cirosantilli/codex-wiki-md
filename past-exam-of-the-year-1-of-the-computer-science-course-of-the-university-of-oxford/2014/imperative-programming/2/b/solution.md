<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix the top-right corner $(i,j)$ and a bottom boundary $k$. A width $w$ is feasible precisely when every row $m\in[i,k)$ has at least $w$ consecutive true entries ending at column $j$. Thus the largest feasible width is the minimum of those [row run lengths](../../../../../row-run-length.md), and the area is that width times $k-i$.
```
def maxRectangleAt(i: Int, j: Int): Int = {
  var k = i
  var width = j + 1
  var best = 0
  while (k < N) {
    width = math.min(width, rowCount(k)(j))
    k += 1
    best = math.max(best, (k - i) * width)
  }
  best
}
```
At the loop head, the [loop invariant](../../../../../loop-invariant.md) is $i\leq k\leq N$,

$$
\begin{aligned}
\mathrm{width}&=\min\bigl(\{j+1\}\cup\{\mathrm{rowCount}(m)(j):i\leq m<k\}\bigr),\\
\mathrm{best}&=\max\bigl(\{0\}\cup\{(h-i)\min_{i\leq m<h}\mathrm{rowCount}(m)(j):i<h\leq k\}\bigr).
\end{aligned}
$$

The initial cap $j+1$ makes the empty-prefix case well-defined and cannot restrict any actual run. Each iteration incorporates one new row and tests its corresponding bottom boundary. The [loop variant](../../../../../loop-variant.md) is $N-k$, so

$$
\boxed{\mathrm{best}=\max_{i<k\leq N}(k-i)\min_{i\leq m<k}\mathrm{rowCount}(m)(j),\qquad O(N).}
$$

A zero width contributes area zero, covering the case where no nonempty all-true [rectangle](../../../../../rectangle.md) starts at that corner.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
