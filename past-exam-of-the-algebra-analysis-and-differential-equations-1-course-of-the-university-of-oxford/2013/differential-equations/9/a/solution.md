<h1 id="differential-equations/9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Inside the half-plane of convergence, the differentiation theorem for the [Laplace transform](../../../../../laplace-transform.md) permits differentiation with respect to the transform variable. Since $\partial_p e^{-pt}=-te^{-pt}$,

$$
\boxed{\overline x'(p)=-\int_0^\infty t x(t)e^{-pt}\,dt=\mathcal L[-tx(t)](p).}
$$

Repeating the argument, or applying induction using $\partial_p^n e^{-pt}=(-t)^n e^{-pt}$, gives

$$
\boxed{\overline x^{(n)}(p)=\int_0^\infty(-t)^n x(t)e^{-pt}\,dt
=(-1)^n\mathcal L[t^n x(t)](p),\qquad n\geq1.}
$$

The identities hold for $\operatorname{Re}p>0$, within the stated convergence half-plane. The usual transform differentiation theorem uses an interior margin in the real part of $p$ to control the polynomial factors in $t$; it makes no assertion on the boundary $\operatorname{Re}p=0$.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
