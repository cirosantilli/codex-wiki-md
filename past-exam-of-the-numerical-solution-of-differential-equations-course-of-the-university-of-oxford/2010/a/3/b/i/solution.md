<h1 id="a/3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $M_0=\sup_xu_0(x)<\infty$ and assume $\lambda(1+pM_0^{p-1})\leq1$. Suprema are understood where the printed maxima on the infinite domain are not attained. We prove the invariant interval $0\leq U_j^m\leq M_0$ simultaneously with the stated speed bound.

Suppose the interval property holds at time $m$. By the [mean value theorem](../../../../../../mean-value-theorem.md), the divided difference

$$
a_j^m=\frac{f(U_j^m)-f(U_{j-1}^m)}{U_j^m-U_{j-1}^m}
$$

is between $1$ and $1+pM_0^{p-1}$; when the two states coincide define it as $f'(U_j^m)$. The update is the [convex combination](../../../../../../convex-combination.md)

$$
U_j^{m+1}=(1-\lambda a_j^m)U_j^m+\lambda a_j^mU_{j-1}^m.
$$

Both coefficients are nonnegative and sum to one, so the same interval property holds at time $m+1$. It is true initially and hence for all times by induction. Therefore

$$
\boxed{\lambda\sup_j|1+p(U_j^m)^{p-1}|\leq\lambda(1+pM_0^{p-1})\leq1\quad\text{for every }m.}
$$

The propagated nonnegativity is essential; it keeps the flux increasing on the entire range of the numerical solution.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../../split.md)
7. [Numerical solution of differential equations course of the University of Oxford](../../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
8. [Year 3 of the mathematics course of the University of Oxford](../../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
