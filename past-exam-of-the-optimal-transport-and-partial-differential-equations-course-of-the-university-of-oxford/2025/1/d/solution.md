<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $d\mu=f(x)\,dx$, with $f\geq0$. Applying [polar coordinates](../../../../polar-coordinates.md) and [Fubini's theorem](../../../../fubini-s-theorem.md) gives, for bounded nonnegative measurable $h$,

$$
\int h\,d\widetilde\mu=\int_0^\infty h(r)g(r)\,dr,\qquad g(r)=\sigma_d r^{d-1}\int_{\mathbb S^{d-1}}f(r\theta)\,d\sigma(\theta)\quad(r>0).
$$

Also $\widetilde\mu(\{0\})=\mu(\{0\})=0$ by [absolute continuity of measures](../../../../absolute-continuity-of-measures.md). Extending $g$ by zero on the negative half-line proves

$$
\boxed{\widetilde\mu\ll\mathcal L^1.}
$$

Both radial [pushforward measures](../../../../pushforward-measure.md) have compact [support of a measure](../../../../support-of-a-measure.md), so [Brenier's theorem](../../../../brenier-theorem.md) on the line supplies a unique optimal [transport plan](../../../../transport-plan.md) and a [transport map](../../../../transport-map.md) $\tau$, unique $\widetilde\mu$-almost everywhere, with

$$
\boxed{\begin{aligned}d_2^2(\widetilde\mu,\widetilde\nu)&=\min_{s_\#\widetilde\mu=\widetilde\nu}\int_0^\infty|r-s(r)|^2\,d\widetilde\mu(r)\\&=\int_0^\infty|r-\tau(r)|^2\,d\widetilde\mu(r).\end{aligned}}
$$

In one dimension, the [gradient](../../../../gradient.md) of a [convex function](../../../../convex-function.md) is a [nondecreasing function](../../../../nondecreasing-function.md). Nonnegativity holds $\widetilde\mu$-almost everywhere because $\tau_\#\widetilde\mu=\widetilde\nu$ is carried by $[0,\infty)$. To choose a nonnegative, nondecreasing representative everywhere, let $F,G$ be the radial [cumulative distribution functions](../../../../cumulative-distribution-function.md) and use the [monotone rearrangement](../../../../monotone-rearrangement.md)

$$
\boxed{\tau(r)=G^{-1}(F(r)),\qquad G^{-1}(u)=\inf\{s\geq0:G(s)\geq u\}\quad(0<u<1).}
$$

At $F(r)=0$ set $\tau(r)=0$, and at $F(r)=1$ use the largest point of the [support of a measure](../../../../support-of-a-measure.md) $\widetilde\nu$. These choices preserve monotonicity and boundedness. Since $F$ is continuous, $F(R)$ has the [uniform distribution](../../../../continuous-uniform-distribution.md) on $(0,1)$ when $R$ has law $\widetilde\mu$, and the [quantile function](../../../../quantile-function.md) $G^{-1}$ sends this [uniform distribution](../../../../continuous-uniform-distribution.md) to $\widetilde\nu$. Thus this representative has the required [pushforward measure](../../../../pushforward-measure.md), even if the target has atoms.

## ↑ Ancestors (12)

1. [D](../d.md)
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
