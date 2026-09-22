<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [closed unit ball](../../../../../closed-unit-ball.md) $\overline B_X$ first, and put $C=\overline{T(\overline B_X)}$. This is a [convex set](../../../../../convex-set-split.md) symmetric about zero. If $B_Y(y_0,r)\subseteq C$, then $-y_0\in C$, so taking midpoints gives

$$
B_Y(0,r/2)\subseteq C.
$$

Write $\delta=r/2$. By scaling,

$$
B_Y(0,2^{-j}\delta)\subseteq\overline{T(2^{-j}\overline B_X)}\qquad(j\geq1).
$$

Fix $y$ with $\|y\|<\delta/2$. Starting with $r_0=y$, recursively choose $x_j\in X$ such that

$$
\|x_j\|\leq2^{-j},\qquad
r_j=r_{j-1}-Tx_j,\qquad
\|r_j\|<2^{-j-1}\delta.
$$

At each step the previous residual lies in the open [ball](../../../../../ball-mathematics.md) on the left of the scaled inclusion, so the definition of [closure](../../../../../closure-topology.md) permits this approximation. The [series](../../../../../series-mathematics.md) $\sum_jx_j$ converges to some $x$ because $X$ is a [Banach space](../../../../../banach-space-split.md), and the [triangle inequality](../../../../../triangle-inequality.md) gives $\|x\|\leq\sum_j2^{-j}=1$. Continuity of $T$ gives $Tx=\lim_N\sum_{j=1}^NTx_j=y$, since $r_N\to0$. Thus

$$
B_Y(0,\delta/2)\subseteq T(\overline B_X).
$$

Scaling by $1/2$ now gives the slightly smaller open [ball](../../../../../ball-mathematics.md)

$$
\boxed{B_Y(0,\delta/4)\subseteq T(B_X(0,1)).}
$$

This proves the assertion whether the original [unit ball](../../../../../unit-ball.md) is taken open or closed. Only completeness of $X$ was used; the [normed space](../../../../../normed-vector-space-split.md) $Y$ need not be complete. The argument is [geometric correction for approximate surjectivity](../../../../../geometric-correction-for-approximate-surjectivity.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
