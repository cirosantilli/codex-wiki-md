<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [contraction mapping theorem](../../../../contraction-mapping-theorem.md) states that a self-map $T$ of a nonempty [complete metric space](../../../../complete-metric-space.md) with a uniform contraction constant $q<1$ has a unique [fixed point](../../../../fixed-point.md) $p$. For every starting point, the iteration $x_{n+1}=Tx_n$ converges to $p$, with $d(x_n,p)\leq q^nd(x_1,x_0)/(1-q)$.

For the [cosine fixed-point iteration](../../../../cosine-fixed-point-iteration.md), any real $x_0$ gives $x_1\in[-1,1]$. This [closed interval](../../../../closed-real-interval.md) is [complete](../../../../completeness.md), and cosine maps it into $[\cos1,1]\subseteq[-1,1]$. The [mean value theorem](../../../../mean-value-theorem.md) gives

$$
|\cos x-\cos y|\leq\sin(1)|x-y|\qquad(x,y\in[-1,1]),
$$

with $\sin(1)<1$. Apply the [contraction mapping theorem](../../../../contraction-mapping-theorem.md) to the tail starting at $x_1$. Therefore $\boxed{x_n\to p,\quad p=\cos p}$ for every real initial value. Numerically $p\approx0.739085$. The global real-line [derivative](../../../../derivative.md) bound is only one; entering the [invariant interval](../../../../invariant-interval.md) supplies the strict uniform bound needed by the theorem.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../split.md)
5. [Fixed point methods for nonlinear partial differential equations course of the University of Oxford](../../../../fixed-point-methods-for-nonlinear-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
