<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $A=R(k-1,\ell)$, $B=R(k,\ell-1)$ and consider any coloring of $K_{A+B}$. Choose a vertex $v$. Among its $A+B-1$ neighbors, either at least $A$ are joined to it by red edges, or at least $B$ by blue edges.

In the red case, the induced [complete graph](../../../../../complete-graph.md) on those neighbors contains either a red $K_{k-1}$, which joins with $v$ to make a red $K_k$, or a blue $K_\ell$. The blue case similarly gives a red $K_k$ or a blue $K_{\ell-1}$ which extends with $v$ to a blue $K_\ell$. Hence every coloring has the required configuration, and

$$
\boxed{R(k,\ell)\leq R(k-1,\ell)+R(k,\ell-1).}
$$

This is the [Ramsey number recursion](../../../../../ramsey-number-recursion.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
