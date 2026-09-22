<h1 id="21g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A,B$ be disjoint closed subsets of the [metric space](../../../../../../metric-space.md) $(X,d)$; the cases where one is empty are immediate. The distance functions

$$
d(x,A)=\inf_{a\in A}d(x,a),
\qquad
d(x,B)=\inf_{b\in B}d(x,b)
$$

are continuous, because each is 1-Lipschitz. Their sum is strictly positive: if both distances vanished, closedness would put $x$ in $A\cap B$. Therefore

$$
u(x)=\frac{d(x,A)}{d(x,A)+d(x,B)}
$$

is continuous, equals zero on $A$, and equals one on $B$. The sets

$$
u^{-1}([0,1/3))
\quad\text{and}\quad
u^{-1}((2/3,1])
$$

are disjoint open neighbourhoods of $A$ and $B$. Thus every metric space is a [normal topological space](../../../../../../normal-space.md); this is the [normality of every metric space](../../../../../../normality-of-every-metric-space.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [21G](../../21g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
