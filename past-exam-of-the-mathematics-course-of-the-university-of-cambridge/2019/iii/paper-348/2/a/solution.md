<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $J_T(x)=|\det DT(x)|$, the absolute [Jacobian determinant](../../../../../../jacobian-determinant.md). Under the usual meaning of a $C^1$ map on domains, the injective [area formula](../../../../../../area-formula-geometric-measure-theory.md) gives, for any nonnegative measurable $a$,

$$
\int_X a(T(x))J_T(x)\,dx=\int_Y a(y)\,dy.
$$

This version of the [change of variables formula](../../../../../../change-of-variables-formula.md) does not require $DT$ to be nonsingular everywhere. A $C^1$ map is a [locally Lipschitz function](../../../../../../locally-lipschitz-function.md), and the formula applies by exhaustion if the domains are unbounded. For non-open $X$, one needs the corresponding extension or regularity interpretation of the stated $C^1$ assumption.

First suppose $f(x)=g(T(x))J_T(x)$ almost everywhere with respect to [Lebesgue measure](../../../../../../lebesgue-measure.md). For each bounded nonnegative measurable $a$,

$$
\int_X a(T(x))f(x)\,dx
=\int_X a(T(x))g(T(x))J_T(x)\,dx
=\int_Y a(y)g(y)\,dy.
$$

Taking [indicator functions](../../../../../../indicator-function.md) proves $T_\#\mu=\nu$.

Conversely, the [area formula](../../../../../../area-formula-geometric-measure-theory.md) shows that the measure $\widetilde\mu$ with [probability density function](../../../../../../probability-density-function.md) $g(T(x))J_T(x)$ has total mass one and satisfies $T_\#\widetilde\mu=\nu$. The assumed equality $T_\#\mu=\nu$ then implies $\mu=\widetilde\mu$, since the measurable [bijection](../../../../../../bijection.md) $T$ has a measurable inverse on these domains. Equivalently, apply both [pushforward measure](../../../../../../pushforward-measure.md) identities to $T(A)$ for each [Borel set](../../../../../../borel-set.md) $A\subseteq X$. Uniqueness of the [Radon-Nikodym derivative](../../../../../../radon-nikodym-derivative.md) yields

$$
\boxed{T_\#\mu=\nu\quad\Longleftrightarrow\quad f(x)=g(T(x))|\det DT(x)|\ \text{Lebesgue-almost everywhere}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 348](../../../paper-348-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
