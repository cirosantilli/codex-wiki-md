<h1 id="9/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Taking the [Laplace transform](../../../../laplace-transform.md), using [linearity](../../../../linearity.md) and the preceding three formulas, gives

$$
p\bar x(p)-x(0)-\bar x(p)=\frac2{p^2}-\frac2{p^3}
=\frac{2(p-1)}{p^3}.
$$

Since $x(0)=0$, division by $p-1$ gives $\bar x(p)=2/p^3$ for $p\ne1$ in the domain of convergence. There is no genuine singularity at $p=1$: [continuity](../../../../continuous-function.md) of the [Laplace transform](../../../../laplace-transform.md) there supplies the same value. One can also first work with $\operatorname{Re}p>1$, where division is harmless.

The formula in part (iii) identifies $2/p^3$ as the [Laplace transform](../../../../laplace-transform.md) of $t^2$. By [uniqueness of the Laplace transform](../../../../uniqueness-of-the-laplace-transform.md),

$$
\boxed{\bar x(p)=\frac2{p^3},\qquad x(t)=t^2\quad(t\geq0).}
$$

As a direct check, $\dot x-x=2t-t^2$ and $x(0)=0$. Any two solutions of this [initial value problem](../../../../initial-value-problem.md) differ by $Ce^t$ and have the same initial value, forcing $C=0$. This also verifies uniqueness independently of transform inversion.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [9](../../9.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
