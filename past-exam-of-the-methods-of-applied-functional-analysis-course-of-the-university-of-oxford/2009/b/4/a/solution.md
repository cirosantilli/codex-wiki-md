<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Banach's fixed-point theorem](../../../../../contraction-mapping-theorem.md) states that a map $T:Y\to Y$ on a nonempty [complete metric space](../../../../../complete-metric-space.md) with $d(Tx,Ty)\le qd(x,y)$ for a constant $0\le q<1$ has a unique [fixed point](../../../../../fixed-point.md), approached from every starting point by iteration.

Choose $x_0$ and let $x_{n+1}=Tx_n$. Induction gives $d(x_{n+1},x_n)\le q^nd(x_1,x_0)$. For $m>n$, the triangle inequality and [geometric series](../../../../../geometric-series.md) give

$$
d(x_m,x_n)\le\frac{q^n}{1-q}d(x_1,x_0).
$$

Thus the [sequence](../../../../../sequence.md) is Cauchy and converges by completeness to some $x_*$. The contraction estimate implies [continuity](../../../../../continuous-function.md), so $Tx_*=\lim Tx_n=\lim x_{n+1}=x_*$. If $y_*$ were another [fixed point](../../../../../fixed-point.md), $d(x_*,y_*)\le qd(x_*,y_*)$ would force equality of the points. Passing $m\to\infty$ also yields the quantitative error estimate

$$
\boxed{d(x_n,x_*)\le\frac{q^n}{1-q}d(x_1,x_0).}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
