<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

At an [absorbing state](../../../../../../../absorbing-state.md), the remaining [absorption time](../../../../../../../absorption-time.md) is zero, so $e_0=e_n=0$. Multiplying the [linear recurrence relation](../../../../../../../linear-recurrence-relation.md) by three gives

$$
e_{k+1}-2e_k+e_{k-1}=-3.
$$

The second [finite difference](../../../../../../../finite-difference-split.md) of $k^2$ is two. A [particular solution](../../../../../../../particular-solution.md) is therefore $-3k^2/2$, while every solution of the corresponding homogeneous [linear recurrence relation](../../../../../../../linear-recurrence-relation.md) has the form $A+Bk$. The [boundary conditions](../../../../../../../boundary-condition.md) give $A=0$ and $B=3n/2$, hence

$$
\boxed{e_k=\frac32k(n-k),\qquad 0\leq k\leq n.}
$$

This is the [mean absorption time of a lazy symmetric random walk](../../../../../../../mean-absorption-time-of-a-lazy-symmetric-random-walk.md) with holding [probability](../../../../../../../probability.md) $1/3$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Mathematics III](../../../../mathematics-iii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
