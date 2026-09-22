<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take the initial removed set to be empty, as required by the displayed equality in this [discrete SIR epidemic on a graph](../../../../../../discrete-sir-epidemic-on-a-graph.md). If initially removed individuals are allowed, add their indicators $Y_i(0)$ to the final-removal count; an isolated initially removed [vertex](../../../../../../vertex-graph-theory.md) already shows why this correction is necessary. Condition on a fixed initial infection vector.

Given the history through time $k$, the [union bound](../../../../../../boole-s-inequality.md) over currently infected [neighbours](../../../../../../neighbour-of-a-vertex.md) gives

$$
\mathbb E[X_i(k+1)\mid\mathcal F_k]
\leq\beta\sum_jA_{ij}X_j(k).
$$

Write $u(k)=\mathbb E X(k)$. Taking [expectations](../../../../../../expected-value.md) and iterating this componentwise inequality for the nonnegative [adjacency matrix of a graph](../../../../../../adjacency-matrix.md) gives $u(k)\leq(\beta A)^kX(0)$.

A [vertex](../../../../../../vertex-graph-theory.md) is infected at most once, and an infection lasts exactly one step before permanent removal. Hence $Y_i(\infty)=\sum_{k\geq0}X_i(k)$ under the stated initial convention. The [Tonelli theorem](../../../../../../tonelli-theorem.md) now gives

$$
\boxed{\mathbb P(Y_i(\infty)=1)
=\mathbb P(i\text{ is ever infected})
\leq\sum_{k=0}^\infty\sum_j
\beta^k(A^k)_{ij}X_j(0)}.
$$

The [walk count from powers of an adjacency matrix](../../../../../../walk-count-from-powers-of-an-adjacency-matrix.md) explains the terms: all possible transmission [walks](../../../../../../walk-in-a-graph.md) are counted, including [walks](../../../../../../walk-in-a-graph.md) that overcount because removal prevents reinfection. This is the [adjacency-matrix bound for a discrete SIR epidemic](../../../../../../adjacency-matrix-bound-for-a-discrete-sir-epidemic.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
