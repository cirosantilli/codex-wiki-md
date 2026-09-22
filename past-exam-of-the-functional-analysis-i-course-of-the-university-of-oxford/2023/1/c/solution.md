<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $(x_n)$ be a [Cauchy sequence](../../../../cauchy-sequence.md) in the [graph norm](../../../../graph-norm.md), and set $y_n=Tx_n$. Since

$$
\|y_n-y_m\|_Y\leq\|x_n-x_m\|_T,
$$

$(y_n)$ is a [Cauchy sequence](../../../../cauchy-sequence.md) in the [Banach space](../../../../banach-space-split.md) $Y$. Write $y_n\to y\in Y$.

Use the bounded [right inverse](../../../../right-inverse.md) to remove the part seen by $T$:

$$
w_n=x_n-Sy_n,\qquad Tw_n=Tx_n-TSy_n=y_n-y_n=0.
$$

Thus $w_n\in W$, and the [operator norm](../../../../operator-norm.md) bound gives

$$
\|w_n-w_m\|_X\leq\|x_n-x_m\|_X+\|S\|\|y_n-y_m\|_Y
\leq(1+\|S\|)\|x_n-x_m\|_T.
$$

The assumed [completeness](../../../../completeness.md) of $W$ supplies $w\in W$ with $w_n\to w$ in $\|\cdot\|_X$. Put $x=w+Sy\in X$. The [linearity](../../../../linearity.md) of $T$ and the [right inverse](../../../../right-inverse.md) identity give $Tx=y$. Therefore

$$
\|x_n-x\|_T\leq\|w_n-w\|_X+(1+\|S\|)\|y_n-y\|_Y\longrightarrow0.
$$

We have proved the [completeness of a graph norm from a bounded right inverse](../../../../completeness-of-a-graph-norm-from-a-bounded-right-inverse.md):

$$
\boxed{(X,\|\cdot\|_T)\text{ is a Banach space}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis I course of the University of Oxford](../../../split.md)
5. [Functional analysis I course of the University of Oxford](../../../../functional-analysis-i-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
