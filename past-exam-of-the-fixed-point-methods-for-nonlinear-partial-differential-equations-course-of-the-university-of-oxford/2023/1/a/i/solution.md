<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Banach fixed-point theorem](../../../../../contraction-mapping-theorem.md) states that a [contraction mapping](../../../../../contraction-mapping.md) $T:X\to X$ of a nonempty [complete metric space](../../../../../complete-metric-space.md) $(X,d)$ has a unique [fixed point](../../../../../fixed-point.md), and [iterations of a map](../../../../../iterated-function.md) $x_{n+1}=T(x_n)$ converge to it from every $x_0\in X$. Precisely, assume a single constant $q\in[0,1)$ satisfies $d(Tx,Ty)\leq qd(x,y)$ for every $x,y\in X$.

Induction gives $d(x_{n+1},x_n)\leq q^n d(x_1,x_0)$. The [triangle inequality](../../../../../triangle-inequality.md) and the [geometric series](../../../../../geometric-series.md) therefore give, for $m>n$,

$$
d(x_m,x_n)\leq\sum_{j=n}^{m-1}q^j d(x_1,x_0)
\leq\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md). By [completeness](../../../../../completeness.md) it converges to some $x_*\in X$. The [contraction mapping](../../../../../contraction-mapping.md) is a [continuous map](../../../../../continuous-map.md), so $Tx_*=\lim_n Tx_n=\lim_n x_{n+1}=x_*$. If $y_*$ is another [fixed point](../../../../../fixed-point.md), then $d(x_*,y_*)\leq qd(x_*,y_*)$, forcing $x_*=y_*$. Letting $m\to\infty$ in the estimate also gives the [contraction iteration error bound](../../../../../contraction-iteration-error-bound.md):

$$
\boxed{Tx_*=x_*,\qquad d(x_n,x_*)\leq\frac{q^n}{1-q}d(x_1,x_0).}
$$

If $q=0$, $T$ is constant and the [sequence](../../../../../sequence.md) reaches its unique [fixed point](../../../../../fixed-point.md) after the first step; this also removes any ambiguity about $0^0$ in the displayed estimate at $n=0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../split.md)
6. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
