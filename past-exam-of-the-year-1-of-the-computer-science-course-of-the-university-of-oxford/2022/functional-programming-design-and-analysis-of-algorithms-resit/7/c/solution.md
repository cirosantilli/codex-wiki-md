<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $N=|V|$ and replace every [edge](../../../../../edge-of-a-graph.md) weight by **$w'(e)=Nw(e)+1$**. Call the supplied shortest-path routine once using these new weights, and return its path in the original graph. For every path $P$,

$$
w'(P)=Nw(P)+|P|,
$$

where $|P|$ is its number of [edges](../../../../../edge-of-a-graph.md). Positive original weights imply positive transformed weights, so a shortest route can be taken to be simple and has at most $N-1$ [edges](../../../../../edge-of-a-graph.md). Distinct integral original weights of paths differ by at least one. Thus if $w(P)<w(Q)$ for simple paths, then

$$
w'(Q)-w'(P)=N\bigl(w(Q)-w(P)\bigr)+|Q|-|P|\ge N-(N-1)>0.
$$

For equal original weights, the transformed comparison is exactly the comparison of hop counts. Therefore every transformed shortest path minimises original weight first and number of [edges](../../../../../edge-of-a-graph.md) second, proving the [integer-weight shortest-path tie-breaking lemma](../../../../../integer-weight-shortest-path-tie-breaking-lemma.md). The transformation costs $O(N+|E|)$ time, followed by one subroutine call. Weights gain only $O(\log N)$ bits; exact arithmetic should be used if multiplying machine-sized weights might overflow. If $t$ is unreachable, it remains unreachable.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
