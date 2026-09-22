<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Choose the bounded, nonnegative [nondecreasing function](../../../../nondecreasing-function.md) $\tau$ from part (d), and define

$$
h(r)=\int_0^r\tau(s)\,ds,\qquad U(x)=h(|x|).
$$

The [function](../../../../function-split.md) $h$ is [convex](../../../../convex-function.md) and nondecreasing. For $0\leq a\leq1$, the [triangle inequality](../../../../triangle-inequality.md), monotonicity, and [convexity](../../../../convex-function.md) give

$$
U((1-a)x+ay)\leq h((1-a)|x|+a|y|)\leq(1-a)U(x)+aU(y).
$$

Hence $U$ is a [convex function](../../../../convex-function.md). By the [gradient of a radial function](../../../../gradient-of-a-radial-function.md) formula and the [fundamental theorem of calculus](../../../../fundamental-theorem-of-calculus.md),

$$
\nabla U(x)=\tau(|x|)\frac{x}{|x|}
$$

for $x\ne0$ whenever $h'(|x|)=\tau(|x|)$. A [monotone function](../../../../monotonic-function.md) has at most countably many discontinuities, so part (d) makes the exceptional radii $\widetilde\mu$-null. The origin is also $\mu$-null. Define $\mathcal T(0)=0$; thus $\mathcal T=\nabla U$ $\mu$-almost everywhere.

For every $Q$ in the [orthogonal group](../../../../orthogonal-group.md), $\mathcal T(Qx)=Q\mathcal T(x)$, including at zero. Consequently $\mathcal T_\#\mu$ is invariant under the [orthogonal group](../../../../orthogonal-group.md). Moreover $|\mathcal T(x)|=\tau(|x|)$ away from the null origin, and composition of [pushforward measures](../../../../pushforward-measure.md) gives

$$
\Phi_\#(\mathcal T_\#\mu)=\tau_\#(\Phi_\#\mu)=\widetilde\nu=\Phi_\#\nu.
$$

Part (c) therefore gives $\mathcal T_\#\mu=\nu$. The [Knott–Smith optimality criterion](../../../../knott-smith-optimality-criterion.md) makes a [transport map](../../../../transport-map.md) given by a [convex function](../../../../convex-function.md)'s [gradient](../../../../gradient.md) optimal for the quadratic [transport cost](../../../../transport-cost-function.md). Uniqueness from [Brenier's theorem](../../../../brenier-theorem.md) yields

$$
\boxed{T(x)=\mathcal T(x)=\tau(|x|)\frac{x}{|x|}\quad\mu\text{-almost everywhere}.}
$$

Since directions agree, this also identifies the optimal value:

$$
\boxed{d_2^2(\mu,\nu)=\int_0^\infty|r-\tau(r)|^2\,d\widetilde\mu(r)=d_2^2(\widetilde\mu,\widetilde\nu).}
$$

## ↑ Ancestors (12)

1. [E](../e.md)
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
