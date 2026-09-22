<h1 id="19h/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Label the seven black intermediate vertices, from left to right and top to bottom within each column, by $a,b,c,d,e,f,g$: thus $a$ is directly below $r$, $b$ is the lower-left vertex, $c,d$ are the next upper and lower vertices, $e$ is the middle-right vertex, and $f,g$ are the upper-right and lower-right vertices.

For $x=4$, the following nonzero edge flows are feasible:

$$
\begin{array}{c|cccccccccc}
\text{edge}&sr&rc&cf&ft&sb&bd&de&et&dg&gt\\ \hline
\text{flow}&4&4&4&4&5&5&3&3&2&2.
\end{array}
$$

Their value is $9$. The cut with source side $\{s\}$ has capacity

$$
C(\{s\},V\setminus\{s\})=x+5=9.
$$

By the max-flow min-cut theorem,

$$
\boxed{\delta^*(4)=9}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [19H](../../../19h.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ib](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
