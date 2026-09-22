<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With the new right sides, the dual function is

$$
\theta_{\mathrm{new}}(\lambda,\mu)=\max\{10-\lambda,\ 8-\mu\},\qquad\lambda,\mu\geq0.
$$

Take $\lambda=\mu=t\to\infty$. Then $\theta_{\mathrm{new}}(t,t)=10-t\to-\infty$, so the minimization dual is **unbounded below**:

$$
\boxed{\inf\theta_{\mathrm{new}}=-\infty.}
$$

By [weak duality](../../../../weak-duality.md), any feasible [integer](../../../../integer-split.md) point with finite objective would have to have objective at most every dual value, which is impossible. Thus **the modified [integer](../../../../integer-split.md) program is infeasible and has no optimal solution**. This is an [infeasibility certificate from an unbounded Lagrangian dual](../../../../infeasibility-certificate-from-an-unbounded-lagrangian-dual.md).

There is also a direct certificate: the assignment equalities force $(a+b)\cdot x=9$, while the new bounds force it to be at most $3+5=8$. Even the modified linear relaxation is infeasible. The earlier $3.5,5.5$ problem also had no [integer](../../../../integer-split.md) solution, but there its fractional [feasible point](../../../../feasible-point.md) kept the dual value finite.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the integer programming course of the University of Oxford](../../../split.md)
5. [Integer programming course of the University of Oxford](../../../../integer-programming-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
