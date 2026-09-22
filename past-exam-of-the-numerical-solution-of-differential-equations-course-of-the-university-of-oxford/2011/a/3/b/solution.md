<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $s=\mu_x+\mu_y$. The update can be rearranged as

$$
\begin{aligned}
(1+s)U_{ij}^{m+1}-\frac{\mu_x}2(U_{i+1,j}^{m+1}+U_{i-1,j}^{m+1})-\frac{\mu_y}2(U_{i,j+1}^{m+1}+U_{i,j-1}^{m+1})
={}&(1-s)U_{ij}^m+\frac{\mu_x}2(U_{i+1,j}^m+U_{i-1,j}^m)+\frac{\mu_y}2(U_{i,j+1}^m+U_{i,j-1}^m).
\end{aligned}
$$

When $s\leq1$, the right side is a [convex combination](../../../../../convex-combination.md) of old values: its coefficients are nonnegative and sum to one. Assume all old values lie in $[U_{\min},U_{\max}]$. A new maximum $v>U_{\max}$ is interior because boundary values are zero and $U_{\max}\geq0$. At its node the left side is at least $(1+s)v-sv=v$, while the right side is at most $U_{\max}$, a contradiction. A new minimum $v<U_{\min}$ similarly makes the left side at most $v$ and the right side at least $U_{\min}$, again a contradiction.

The initial values satisfy the bounds by construction; [mathematical induction](../../../../../mathematical-induction.md) proves

$$
\boxed{U_{\min}\leq U_{ij}^m\leq U_{\max}\quad\text{at every node and time level}.}
$$

The new-time matrix is a [strictly diagonally dominant matrix](../../../../../strictly-diagonally-dominant-matrix.md) with positive diagonal and nonpositive off-diagonal entries, so the linear update is uniquely solvable. This [Crank-Nicolson maximum principle under a step restriction](../../../../../crank-nicolson-maximum-principle-under-a-step-restriction.md) concerns preservation of value bounds, which is a stronger requirement than scalar [A-stability](../../../../../a-stability.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
