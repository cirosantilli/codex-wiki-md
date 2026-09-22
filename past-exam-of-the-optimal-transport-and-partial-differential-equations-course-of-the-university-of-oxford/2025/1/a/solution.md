<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Compact [support of a measure](../../../../support-of-a-measure.md) gives finite second [absolute moments](../../../../absolute-moment.md) for both [probability measures](../../../../probability-measure.md). Since the source satisfies [absolute continuity of measures](../../../../absolute-continuity-of-measures.md) with respect to [Lebesgue measure](../../../../lebesgue-measure.md), [Brenier's theorem](../../../../brenier-theorem.md) identifies the quadratic [Kantorovich optimal transport problem](../../../../kantorovich-optimal-transport-problem.md) with the [Monge optimal transport problem](../../../../monge-optimal-transport-problem.md):

$$
\boxed{\begin{aligned}d_2^2(\mu,\nu)&=\min_{\pi\in\Gamma(\mu,\nu)}\int|x-y|^2\,d\pi(x,y)\\&=\min_{S_\#\mu=\nu}\int|x-S(x)|^2\,d\mu(x)=\int|x-T(x)|^2\,d\mu(x).\end{aligned}}
$$

Here $S_\#\mu$ is the [pushforward measure](../../../../pushforward-measure.md). The optimal [transport plan](../../../../transport-plan.md) is unique and equals $(\operatorname{Id},T)_\#\mu$. The optimal [transport map](../../../../transport-map.md) is **unique up to a $\mu$-null set**, with

$$
\boxed{T=\nabla u\quad\mu\text{-almost everywhere},\qquad u\text{ convex}.}
$$

The [gradient](../../../../gradient.md) of this [convex function](../../../../convex-function.md) is [c-cyclically monotone](../../../../c-cyclical-monotonicity.md) for $c(x,y)=|x-y|^2$ on a full-measure set. In particular, summing the two supporting inequalities for the [convex function](../../../../convex-function.md) gives $(T(x)-T(x'))\cdot(x-x')\geq0$ wherever both [gradients](../../../../gradient.md) exist. No regularity of the target beyond the stated [probability measure](../../../../probability-measure.md) assumptions is needed.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the optimal transport and partial differential equations course of the University of Oxford](../../../split.md)
5. [Optimal transport and partial differential equations course of the University of Oxford](../../../../optimal-transport-and-partial-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
