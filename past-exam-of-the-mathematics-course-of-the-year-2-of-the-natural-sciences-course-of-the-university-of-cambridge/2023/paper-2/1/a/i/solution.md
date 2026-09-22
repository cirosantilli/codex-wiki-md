<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The weight cancels the denominator in the [Sturm-Liouville operator](../../../../../../sturm-liouville-operator.md). Two [integrations by parts](../../../../../../integration-by-parts.md), with real $p,q$, give the [Lagrange identity for a Sturm-Liouville operator](../../../../../../lagrange-identity-for-a-sturm-liouville-operator.md)

$$
\begin{aligned}
\langle f,\mathcal Lg\rangle_w-\langle\mathcal Lf,g\rangle_w
&=\int_a^b\left[-f^*(pg')'+(pf^{*\prime})'g\right]dx\\
&=\left[p\left(f^{*\prime}g-f^*g'\right)\right]_a^b.
\end{aligned}
$$

Thus the boundary form must vanish for every pair in the operator domain:

$$
\boxed{\left[p(f^{*\prime}g-f^*g')\right]_a^b=0.}
$$

Separated real [Robin boundary conditions](../../../../../../robin-boundary-condition.md) $A_s y(s)+B_s p(s)y'(s)=0$ at $s=a,b$, with $(A_s,B_s)\ne(0,0)$, make each endpoint contribution vanish. This includes [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) and [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md). Coupled conditions can also work: periodic $y(a)=y(b)$ and $p(a)y'(a)=p(b)y'(b)$ cancel the two endpoint contributions. For the regular problem, imposing a complete pair of such self-adjoint [boundary conditions](../../../../../../boundary-condition.md) gives a [self-adjoint differential operator](../../../../../../self-adjoint-differential-operator.md); the displayed identity is the boundary-form criterion.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
