<h1 id="33b/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Set

$$
I_0=[x_0,x_1],\qquad I_1=[x_1,x_3],\qquad I_2=[x_3,x_2].
$$

Their covering graph is

$$
I_0\longrightarrow I_1,I_2,\qquad
I_1\longrightarrow I_0,I_1,I_2,\qquad
I_2\longrightarrow I_0,I_1,
$$

with [adjacency matrix](../../../../../../../adjacency-matrix-of-a-directed-graph.md)

$$
A=\begin{pmatrix}0&1&1\\1&1&1\\1&1&0\end{pmatrix}.
$$

The closed walks $I_1\to I_1\to I_1$ and $I_1\to I_0\to I_1$ give a [horseshoe from two closed covering walks](../../../../../../../horseshoe-from-two-closed-covering-walks.md) for $F^2$, so $F$ must be [chaotic](../../../../../../../glendinning-chaos.md). Since

$$
\operatorname{tr}A=1,
\qquad
\operatorname{tr}(A^3)=13,
$$

[counting cycles in an interval covering graph](../../../../../../../counting-cycles-in-an-interval-covering-graph.md) gives

$$
\frac{13-1}{3}=\boxed4
$$

distinct 3-cycles in the minimum case, attained by the corresponding [connect-the-dots interval map](../../../../../../../connect-the-dots-interval-map.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [33B](../../../33b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
