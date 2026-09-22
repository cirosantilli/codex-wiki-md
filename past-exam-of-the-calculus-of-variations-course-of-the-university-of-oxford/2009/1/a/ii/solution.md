<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [strictly convex function](../../../../../strictly-convex-function.md) satisfies the same inequality strictly whenever $x\ne y$ and $0<t<1$.

For the unlabelled Hessian criterion, [convexity](../../../../../convex-function.md) implies $F(z_0+th)+F(z_0-th)-2F(z_0)\geq0$. Divide by $t^2$ and let $t\to0$ to obtain $h^TD^2F(z_0)h\geq0$ for every $h$. Thus the [Hessian matrix](../../../../../hessian-matrix.md) is [positive semidefinite](../../../../../positive-semidefinite-matrix.md).

Conversely, if every Hessian is [positive semidefinite](../../../../../positive-semidefinite-matrix.md), Taylor's [integral](../../../../../integral-split.md) formula with $h=z-z_0$ gives

$$
F(z)-F(z_0)-DF(z_0)\cdot h=\int_0^1(1-t)h^TD^2F(z_0+th)h\,dt\geq0.
$$

The allowed supporting-plane characterization then proves

$$
\boxed{F\text{ convex}\iff D^2F(z)\text{ positive semidefinite for all }z.}
$$

For the [integral](../../../../../integral-split.md) inequality put $m=(b-a)^{-1}\int_a^bu$. The supporting tangent at $m$ gives $F(u(x))\geq F(m)+F'(m)(u(x)-m)$ [almost everywhere](../../../../../almost-everywhere.md). Integrating cancels the linear term, so

$$
\boxed{F\left(\frac1{b-a}\int_a^bu\right)\leq\frac1{b-a}\int_a^bF(u).}
$$

This is [Jensen's inequality](../../../../../jensen-s-inequality.md). It remains valid with value $+\infty$ on the right: the affine lower bound has [integrable](../../../../../integrability.md) negative part, so the extended [integral](../../../../../integral-split.md) is well-defined.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
