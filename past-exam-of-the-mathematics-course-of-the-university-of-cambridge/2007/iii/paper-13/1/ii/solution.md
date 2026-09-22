<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With a cyclically oriented [independence digraph of events](../../../../../../independence-digraph-of-events.md), each event is independent of one of the other two. Independence is symmetric, so all three pairs are [independent events](../../../../../../independent-events.md). This does not imply mutual independence. Put $x=\mathbb P(A_1\cap A_2\cap A_3)$. The [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) gives

$$
\mathbb P(A_1^c\cap A_2^c\cap A_3^c)=1-3a+3a^2-x\geq1-3a+2a^2=(1-a)(1-2a),
$$

because $x\leq\mathbb P(A_1\cap A_2)=a^2$. Thus **the oriented case guarantees positive avoidance exactly when $0<a<1/2$**.

For sharpness, for any $1/2\leq a<1$ prescribe the law of the three event indicators by assigning mass $(1-a)^2$ to each of the three singleton success patterns, $(1-a)(2a-1)$ to each doubleton, $1-3a+3a^2$ to the tripleton, and zero to the zero-success pattern. All masses are nonnegative and their sum is one. Each marginal is

$$
(1-a)^2+2(1-a)(2a-1)+(1-3a+3a^2)=a,
$$

and each pair intersection has mass $(1-a)(2a-1)+(1-3a+3a^2)=a^2$. These events satisfy the oriented independence conditions and have zero avoidance [probability](../../../../../../probability.md).

The unoriented triangle imposes no independence conditions at all: every vertex is adjacent to every other. The [union bound](../../../../../../boole-s-inequality.md) gives positive avoidance if $3a<1$. To see that this is sharp for every $a\geq1/3$, use uniform measure on the circle of circumference one and take three arcs of length $a$ starting at $0,1/3,2/3$. They cover the circle. Hence **the unoriented case guarantees positive avoidance exactly when $0<a<1/3$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
