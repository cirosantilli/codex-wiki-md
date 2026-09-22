<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $w=u-v$ and $r=f-g$. Subtraction of the two [boundary value problems](../../../../boundary-value-problem-split.md) gives $-w''+w+u^3-v^3=r$, with $w(0)=w(1)=0$. Multiply by $w$ and apply [integration by parts](../../../../integration-by-parts.md):

$$
\int_0^1(-w'')w\,dx=-[w'w]_0^1+\int_0^1(w')^2\,dx=\int_0^1(w')^2\,dx.
$$

Consequently the required [energy identity](../../../../energy-identity.md) is

$$
\int_0^1\left((w')^2+w^2+(u^3-v^3)w\right)dx=\int_0^1rw\,dx.
$$

The nonlinear term is nonnegative pointwise, since

$$
(u^3-v^3)(u-v)=(u-v)^2(u^2+uv+v^2),\qquad u^2+uv+v^2=(u+v/2)^2+3v^2/4\geq0.
$$

This is the [monotonicity energy estimate for a semilinear Dirichlet problem](../../../../monotonicity-energy-estimate-for-a-semilinear-dirichlet-problem.md) for the [monotone function](../../../../monotonic-function.md) $s\mapsto s^3$. Apply [Young's inequality for products](../../../../young-s-inequality-for-products.md), $rw\leq(r^2+w^2)/2$, inside the last [integral](../../../../integral-split.md) and discard the nonnegative nonlinear term. Moving $\tfrac12\int_0^1w^2dx$ to the left gives

$$
\int_0^1(u'-v')^2dx+\frac12\int_0^1(u-v)^2dx\leq\frac12\int_0^1(f-g)^2dx.
$$

In particular, equal forcing gives $w=0$, proving [uniqueness](../../../../uniqueness.md) and a quantitative [continuous dependence on forcing](../../../../continuous-dependence-on-forcing.md) estimate for this [boundary value problem](../../../../boundary-value-problem-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical solutions of partial differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solutions of partial differential equations course of the University of Oxford](../../../../numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
