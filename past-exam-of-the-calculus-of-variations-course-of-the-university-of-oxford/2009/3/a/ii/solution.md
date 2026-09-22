<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A [strong local minimizer of a variational integral](../../../../../strong-local-minimizer-of-a-variational-integral.md) is an admissible $\bar u$ for which the same conclusion holds whenever $\|v-\bar u\|_\infty<\rho$. Every strong local minimizer is weak, because Sobolev closeness implies uniform closeness. A [global minimizer](../../../../../global-minimizer.md) is both, and the converse implication from weak to strong is not generally valid.

If the integrand is independent of $u$, a weak local minimizer has vanishing [first variation](../../../../../first-variation.md):

$$
\int_a^bf_v(x,\bar u'(x))\varphi'(x)dx=0\quad(\varphi\in C_0^\infty(a,b)).
$$

The bounded [function](../../../../../function-split.md) $h(x)=f_v(x,\bar u'(x))$ therefore has zero [distributional derivative](../../../../../distributional-derivative.md), so is constant [almost everywhere](../../../../../almost-everywhere.md). For an elementary test-[function](../../../../../function-split.md) argument, any smooth compactly supported $\psi$ of [integral](../../../../../integral-split.md) zero is the [derivative](../../../../../derivative.md) of a compactly supported smooth $\varphi$. Hence $\int h\psi=0$; subtracting a fixed unit-[integral](../../../../../integral-split.md) [test function](../../../../../test-function.md) from arbitrary tests shows that $h$ agrees with one constant against every test. The fundamental lemma then gives

$$
\boxed{f_v(x,\bar u'(x))=c\quad\text{almost everywhere}.}
$$

This is the [first integral for a variational integrand independent of the function value](../../../../../first-integral-for-a-variational-integrand-independent-of-the-function-value.md).

A [point of convexity](../../../../../point-of-convexity.md) $v_0$ of a differentiable real [function](../../../../../function-split.md) $g$ has a globally supporting tangent: $g(v)\geq g(v_0)+g'(v_0)(v-v_0)$ for every $v$. The [Weierstrass necessary condition](../../../../../weierstrass-necessary-condition.md) for a strong minimum says that $\bar u'(x)$ is such a point for $v\mapsto f(x,\bar u(x),v)$ for almost every $x$. Equivalently, the [Weierstrass excess function](../../../../../weierstrass-excess-function.md) is nonnegative at every trial slope.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
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
