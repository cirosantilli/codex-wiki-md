<h1 id="11g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We argue by contradiction using the previous [subsequence](../../../../../../subsequence.md) construction. If $X$ is not [complete](../../../../../../completeness.md), choose a [Cauchy sequence](../../../../../../cauchy-sequence.md) with no limit in $X$. None of its $d_m$ can be zero: if $d_m=0$, then $d(x_m,x_n)\to0$, giving a limit in $X$. The construction therefore produces pairwise distinct $y_j$ with

$$
d(y_{m+1},y_{n+1})\leq\tfrac12d(y_m,y_n).
$$

Let $Y=\{y_1,y_2,\ldots\}$. **This subset is closed in $X$.** Indeed, if a point $x\notin Y$ lay in its [closure](../../../../../../closure-topology.md), there would be points of $Y$ tending to $x$. Their indices must be unbounded, because the distance from $x$ to any finite subset of $Y$ is positive. Passing to increasing indices gives a [convergent subsequence](../../../../../../convergent-subsequence.md) of the original [Cauchy sequence](../../../../../../cauchy-sequence.md). Part (a) would then make the whole sequence converge to $x$, a contradiction.

Now define $F:Y\to Y$ by $F(y_j)=y_{j+1}$. Distinctness makes this well-defined, and the displayed inequality makes it a [contraction mapping](../../../../../../contraction-mapping.md) with constant at most $1/2$. It has no [fixed point](../../../../../../fixed-point.md), contradicting the assumed property of closed subsets. Consequently

$$
\boxed{X\text{ is complete}.}
$$

This is the converse direction of [contraction property of closed subsets characterizes completeness](../../../../../../contraction-property-of-closed-subsets-characterizes-completeness.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11G](../../11g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
