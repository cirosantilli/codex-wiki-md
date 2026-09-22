<h1 id="7/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

There is an index slip in the source: starting with $G_1$ and performing steps $1,\ldots,n$ produces the final graph $G_{n+1}$. Write $H$ for that final graph. The literal assertion for $G_n$ can fail: take a triangle with $\ell(xz)=3$, $\ell(xy)=2$, $\ell(yz)=1$. Before the final step the extra edge $yz$ remains; only the final deletion removes it.

The invariant is that $x$ and $y$ remain connected. Choose a simple $xy$ [graph path](../../../../../path-in-a-graph.md) $P$ in $H$. If an edge of $H$ did not lie in $P$, then at its processing time $P$ was still present and avoided that edge. The algorithm would therefore have deleted it, a contradiction. Thus every edge of $H$ lies in $P$. **The final graph is precisely an $xy$ path and possibly isolated vertices.**

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [7](../../../7.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
