<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

In one dimension, $u\in W^{1,2}$ has an absolutely continuous bounded representative. For any smooth zero-endpoint [test function](../../../../../test-function.md) $\eta$, the functions $u+t\eta$ are admissible and arbitrarily close to $u$ for small $t$. Local minimality forces the [first variation](../../../../../first-variation.md) to vanish. Differentiation under the [integral](../../../../../integral-split.md) is valid because $u,\eta$ are bounded and the derivative terms are integrable, giving the weak [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md)

$$
\boxed{\int_0^1\bigl(2u'\eta'+4xu^3\eta\bigr)\,dx=0.}
$$

In distributional form this says $(2u')'=4xu^3$. The fundamental theorem for [weak derivatives](../../../../../weak-derivative.md), or the fundamental lemma applied after subtracting an antiderivative, gives a constant $C$ with

$$
\boxed{u'(x)=C+2\int_0^x t\,u(t)^3\,dt\quad\text{almost everywhere}.}
$$

This is the integrated [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). The boundary difference $u(1)-u(0)=2$ determines

$$
C=2-2\int_0^1(1-t)t\,u(t)^3\,dt.
$$

The weak identity extends to all zero-trace $W^{1,2}$ [test functions](../../../../../test-function.md) by [density](../../../../../density.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the calculus of variations course of the University of Oxford](../../../../split.md)
6. [Calculus of variations course of the University of Oxford](../../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
