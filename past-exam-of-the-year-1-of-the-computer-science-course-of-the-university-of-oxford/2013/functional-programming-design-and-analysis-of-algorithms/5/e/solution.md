<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Split a [graph path](../../../../../path-in-a-graph.md) of length at most $2k$ into two consecutive parts of length at most $k$, allowing a zero-length part. Conversely, concatenating two such parts gives a [walk](../../../../../walk-in-a-graph.md) of length at most $2k$ and hence the same [reachability](../../../../../reachability-in-a-graph.md). Therefore

$$
\boxed{P_{2k}=P_k\odot P_k.}
$$

Start at $P_1=I\lor E$, then square to obtain $P_2,P_4,P_8,\ldots$. Stop at equality of successive [matrices](../../../../../matrix.md), or after the length bound reaches $n-1$. The invariant is now $P=P_{2^r}$ after $r$ squarings. Equality implies closure under composition, and the included [identity matrix](../../../../../identity-matrix.md) ensures [reflexivity](../../../../../reflexive-relation.md).

For the same elementary dense [Boolean matrix multiplication](../../../../../boolean-matrix-multiplication.md) and equality stopping test, the cost is

$$
\boxed{T_{\mathrm{square}}=\Theta\!\left(n^3(1+\log(m+1))\right),\qquad \text{space}=\Theta(n^2).}
$$

The additive constant covers the final stability check and the cases $m=0,1$. Thus, with $m\geq2$, the number of cubic passes falls from $\Theta(m)$ to $\Theta(\log m)$. In terms of $n$ alone the worst-case bound improves from $\Theta(n^4)$ to $\Theta(n^3\log n)$ for these implementations. A directed chain also requires logarithmically many squarings. This comparison uses ordinary triple-loop multiplication, rather than a faster [matrix multiplication](../../../../../matrix-multiplication.md) method.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
