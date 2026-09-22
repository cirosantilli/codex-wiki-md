<h1 id="a/3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Give $H_0^1$ the equivalent [Hilbert space](../../../../../../hilbert-space-split.md) norm $\|u\|_H=\|\nabla u\|_2$, using the [Poincaré inequality](../../../../../../poincare-inequality.md). Define

$$
a(u,v)=\int_\Omega\nabla u\cdot\nabla v+\int_\Omega(b\cdot\nabla u)v,\qquad\ell(v)=\int_\Omega fv.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|a(u,v)|\leq(1+C_P\|b\|_\infty)\|u\|_H\|v\|_H$ and $|\ell(v)|\leq C_P\|f\|_2\|v\|_H$.

For $\varphi\in C_0^\infty(\Omega)$, the definition of [weak divergence](../../../../../../weak-divergence.md), applied to $\varphi^2/2$, gives

$$
\int_\Omega(b\cdot\nabla\varphi)\varphi=-\frac12\int_\Omega(\operatorname{div}b)\varphi^2\geq0.
$$

The left side is continuous in the $H_0^1$ norm. Approximate any $u\in H_0^1$ by [test functions](../../../../../../test-function.md) and pass to the limit on the left to obtain $\int(b\cdot\nabla u)u\geq0$. This density argument is essential: local integrability of $\operatorname{div}b$ alone does not justify treating $(\operatorname{div}b)u^2$ as integrable for arbitrary $u\in H_0^1$.

Consequently $a(u,u)\geq\|u\|_H^2$, so $a$ is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) supplies a unique [weak solution](../../../../../../weak-solution.md) with $\boxed{\|\nabla u\|_2\leq C_P\|f\|_2}$. The reusable estimate is [coercivity from a drift with nonpositive weak divergence](../../../../../../coercivity-from-a-drift-with-nonpositive-weak-divergence.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [A](../../../../a.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
