<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Start with $P_1=I\lor E$ and repeatedly apply part (b), keeping a fresh output [matrix](../../../../../matrix.md). A simple implementation is

```
P := I OR E
repeat:
    Q := P OR boolean_product(P, E)
    if Q = P: return P
    P := Q
```

At the start of each iteration, $P=P_k$ for the current length bound $k$. The update produces $P_{k+1}$, proving the [loop invariant](../../../../../loop-invariant.md) by [mathematical induction](../../../../../mathematical-induction.md). If $Q=P$, every [edge](../../../../../edge-of-a-graph.md) extension of a known [graph path](../../../../../path-in-a-graph.md) is already known. Repeating the same update then makes no further change, so every longer [graph path](../../../../../path-in-a-graph.md) is represented as well.

Every reachable pair of distinct [vertices](../../../../../vertex-graph-theory.md) has a [simple path](../../../../../path-in-a-graph.md) of at most $n-1$ [edges](../../../../../edge-of-a-graph.md): a repeated [vertex](../../../../../vertex-graph-theory.md) allows the intervening part to be deleted. Thus the process stabilizes after finitely many updates and returns

$$
\boxed{R[i,j]=\text{true precisely when }j\text{ is reachable from }i,\text{ including }i=j.}
$$

This is the [reflexive transitive closure](../../../../../reflexive-transitive-closure.md). An alternative stopping rule is to stop once the length bound is at least $n-1$, avoiding a final equality-detection iteration. For $n=0$ or $1$, $P_1$ already suffices.

## ↑ Ancestors (12)

1. [C](../c.md)
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
