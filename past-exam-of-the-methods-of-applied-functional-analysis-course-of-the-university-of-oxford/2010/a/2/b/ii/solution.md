<h1 id="a/2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $g=(g_1,\ldots,g_n)$ for the continuous representatives of the [weak derivatives](../../../../../../weak-derivative.md). Integrating the preceding identity over $B=B(0,1)$ gives

$$
|B|u_\varepsilon(x)=\int_Bu_\varepsilon(y)\,dy+\int_B\int_0^1(\rho_\varepsilon*g)(y+t(x-y))\cdot(x-y)\,dt\,dy.
$$

The first term converges to $\int_Bu$ because $u_\varepsilon\to u$ in $L^1$. For fixed $x$, all segments in the second term lie in a compact set. Continuity of $g$ implies $\rho_\varepsilon*g\to g$ uniformly on that set. Hence every $x$ has the finite limit

$$
U(x)=\frac1{|B|}\left(\int_Bu(y)\,dy+\int_B\int_0^1g(y+t(x-y))\cdot(x-y)\,dt\,dy\right).
$$

The same argument is uniform for $x$ in any fixed compact set: all the segments then lie in a common compact set. Thus $u_\varepsilon\to U$ locally uniformly, so $U$ is continuous; the local $L^1$ convergence also gives $U=u$ [almost everywhere](../../../../../../almost-everywhere.md).

Passing to the limit in the segment identity, and taking its endpoints to be $x$ and $x+h$, gives

$$
U(x+h)-U(x)-g(x)\cdot h=\int_0^1[g(x+th)-g(x)]\cdot h\,dt=o(|h|).
$$

Therefore $U$ is [differentiable](../../../../../../differentiable-function.md) with continuous [gradient](../../../../../../gradient.md) $g$: $\boxed{U\in C^1,\quad U=u\text{ almost everywhere},\quad\nabla U=g}$. This is the [continuous weak gradient gives a C1 representative](../../../../../../continuous-weak-gradient-gives-a-c1-representative.md) criterion.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
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
