<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $d=y-x$ and take $0<t\leq1$. Rearrange the defining inequality for a [strongly convex function](../../../../strongly-convex-function.md), applied to $x+td$:

$$
f(y)\geq f(x)+\frac{f(x+td)-f(x)}{t}+\frac\gamma2(1-t)\|d\|^2.
$$

Because $f$ is [differentiable](../../../../differentiable-function.md) at $x$, its [directional derivative](../../../../directional-derivative.md) in direction $d$ is

$$
\lim_{t\downarrow0}\frac{f(x+td)-f(x)}{t}=\nabla f(x)^Td.
$$

Taking the limit in the rearranged inequality gives

$$
\boxed{f(y)\geq f(x)+\nabla f(x)^T(y-x)+\frac\gamma2\|y-x\|^2.}
$$

This is the supporting [affine function](../../../../affine-function.md) inequality strengthened by a positive squared [Euclidean distance](../../../../euclidean-distance.md). **Differentiability at $x$ alone suffices**; no [derivative](../../../../derivative.md) at $y$ is used.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the optimisation for data science course of the University of Oxford](../../../split.md)
5. [Optimisation for data science course of the University of Oxford](../../../../optimisation-for-data-science-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
