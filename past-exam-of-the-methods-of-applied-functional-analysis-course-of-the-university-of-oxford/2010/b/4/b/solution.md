<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

This is the [fixed point theorem for summably Lipschitz iterates](../../../../../fixed-point-theorem-for-summably-lipschitz-iterates.md). Put $x_n=A^nx_0$ and $d=\|x_1-x_0\|$. For $n\geq1$,

$$
\|x_{n+1}-x_n\|=\|A^nx_1-A^nx_0\|\leq\alpha_nd.
$$

Consequently, for $m>n\geq1$,

$$
\|x_m-x_n\|\leq d\sum_{k=n}^{m-1}\alpha_k.
$$

Summability makes the tails tend to zero, so $(x_n)$ is a [Cauchy sequence](../../../../../cauchy-sequence.md). Since $M$ is closed in a [Banach space](../../../../../banach-space-split.md), $x_n\to x\in M$. The $n=1$ hypothesis makes $A$ a [Lipschitz map](../../../../../lipschitz-continuity.md), hence continuous; passing to the limit in $x_{n+1}=Ax_n$ gives $x=Ax$.

If $y$ is another [fixed point](../../../../../fixed-point.md), then $\|x-y\|\leq\alpha_n\|x-y\|$ for every $n$. Since $\alpha_n\to0$, eventually $\alpha_n<1$ and thus $x=y$. Finally let $m\to\infty$ in the tail estimate:

$$
\boxed{\|x-x_n\|\leq\left(\sum_{k\geq n}\alpha_k\right)\|x_1-x_0\|\quad(n\geq1).}
$$

The map itself need not be a [contraction mapping](../../../../../contraction-mapping.md); its successive iterates provide the summable error bound.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../split.md)
6. [Methods of applied functional analysis course of the University of Oxford](../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
