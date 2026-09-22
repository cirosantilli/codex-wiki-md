<h1 id="33b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An [interval map](../../../../../../interval-map.md) $F:I\to I$ has a [horseshoe](../../../../../../horseshoe-for-an-interval-map.md) if there are two [closed subintervals](../../../../../../closed-real-interval.md) $J_0,J_1\subseteq I$ with disjoint interiors such that

$$
F(J_i)\supseteq J_0\cup J_1
\qquad(i=0,1).
$$

It is [chaotic in Glendinning's sense](../../../../../../glendinning-chaos.md) if some positive [iterate](../../../../../../iterated-function.md) $F^n$ has a horseshoe.

Suppose $a<b<c$ are the points of a [3-cycle](../../../../../../periodic-point-of-an-interval-map.md) and put $J_0=[a,b]$, $J_1=[b,c]$. There are two possible cyclic orders. If

$$
a\mapsto b\mapsto c\mapsto a,
$$

then the [intermediate value theorem](../../../../../../intermediate-value-theorem.md) gives

$$
J_0\longrightarrow J_1,
\qquad
J_1\longrightarrow J_0\cup J_1.
$$

Consequently both $F^2(J_0)$ and $F^2(J_1)$ contain $J_0\cup J_1$. If instead

$$
a\mapsto c\mapsto b\mapsto a,
$$

then

$$
J_0\longrightarrow J_0\cup J_1,
\qquad
J_1\longrightarrow J_0,
$$

and again both second images contain $J_0\cup J_1$. Thus in either cyclic order $F^2$ has a horseshoe.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [33B](../../33b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
