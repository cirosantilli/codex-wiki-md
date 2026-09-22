<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E$ be the underlying [Banach space](../../../../../banach-space-split.md). By the [Laplace-transform formula for a semigroup resolvent](../../../../../laplace-transform-formula-for-a-semigroup-resolvent.md),

$$
R_\lambda f=\int_0^\infty e^{-\lambda s}P_sf\,ds,\qquad
\|R_\lambda\|\leq\int_0^\infty e^{-\lambda s}\,ds=\frac1\lambda.
$$

These are [Bochner integrals](../../../../../bochner-integral.md), defined for every $f\in E$ and $\lambda>0$. The [contraction semigroup](../../../../../contraction-semigroup.md) bound and [semigroup property](../../../../../semigroup-property.md) give

$$
R_\lambda R_\mu f
=\int_0^\infty\int_0^\infty e^{-\lambda s-\mu t}P_{s+t}f\,dt\,ds.
$$

Interchanging and regrouping these [Bochner integrals](../../../../../bochner-integral.md) is justified by the integrable bound $e^{-\lambda s-\mu t}\|f\|$, whose integral is $\|f\|/(\lambda\mu)$. For $\lambda\ne\mu$, set $v=s+t$ and evaluate the inner scalar integral:

$$
\begin{aligned}
R_\lambda R_\mu f
&=\int_0^\infty\left(\int_0^ve^{-\lambda s-\mu(v-s)}\,ds\right)P_vf\,dv\\
&=\frac1{\mu-\lambda}\int_0^\infty(e^{-\lambda v}-e^{-\mu v})P_vf\,dv\\
&=\frac{R_\lambda f-R_\mu f}{\mu-\lambda}.
\end{aligned}
$$

Since $f$ was arbitrary, the [resolvent identity](../../../../../resolvent-identity.md) follows:

$$
\boxed{R_\lambda-R_\mu=(\mu-\lambda)R_\lambda R_\mu.}
$$

For $\lambda=\mu$, both sides vanish, so that case holds as well.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the stochastic analysis and partial differential equations course of the University of Oxford](../../../../split.md)
6. [Stochastic analysis and partial differential equations course of the University of Oxford](../../../../../stochastic-analysis-and-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
