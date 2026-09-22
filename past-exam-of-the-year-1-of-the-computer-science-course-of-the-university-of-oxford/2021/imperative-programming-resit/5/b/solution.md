<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split the index range at its middle:
```
def MakeTree(u: Array[Int], a: Int, b: Int): Tree = {
  require(0 <= a && a <= b && b <= u.length)
  if (a == b) null
  else {
    val middle = a + (b - a) / 2
    new Tree(u(middle),
             MakeTree(u, a, middle),
             MakeTree(u, middle + 1, b))
  }
}
```
For $N=b-a>0$, the child sizes are $\lfloor N/2\rfloor$ and $N-1-\lfloor N/2\rfloor$, differing by at most one. [Induction](../../../../../mathematical-induction.md) gives the same property at every descendant, so **the result is nearly balanced**. Its inorder traversal is the initial subrange, then $u(middle)$, then the final subrange, reproducing exactly $u[a..b)$ with every occurrence retained.

There is one nonempty [recursive call](../../../../../recursive-call.md) per constructed node and one constant-time base call per empty child position. Therefore construction takes **$\Theta(N)$ time for $N\geq1$**, or $\Theta(N+1)$ including the empty case, and allocates exactly $N$ nodes. The balanced [recursion](../../../../../recursion-computer-science.md) has logarithmic stack depth. The input [array](../../../../../array-data-structure.md) need not be sorted: the required property concerns [subtree](../../../../../subtree.md) sizes and inorder order, not a search-tree ordering.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
