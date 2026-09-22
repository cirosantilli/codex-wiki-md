<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $q=y-x$ and $z_t=x+tq$. The definition of [pushforward measure](../../../../pushforward-measure.md) gives the [confinement energy](../../../../confinement-energy.md) $\mathcal V[\mu_t]=\int V(z_t)\,d\Pi$. The [chain rule](../../../../chain-rule.md) and [differentiation under the integral sign](../../../../differentiation-under-the-integral-sign.md), whenever justified, give

$$
\frac d{dt}\mathcal V[\mu_t]=\int\nabla V(z_t)\cdot q\,d\Pi,\qquad\boxed{\frac{d^2}{dt^2}\mathcal V[\mu_t]=\int q^TD^2V(z_t)q\,d\Pi.}
$$

For example, bounded [Hessian matrix](../../../../hessian-matrix.md) is sufficient: it gives $|\nabla V(z)|\leq C(1+|z|)$, and the first two differentiated integrands are bounded by $C'(1+|x|^2+|y|^2)$. The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) applies because $\Pi$ has finite second [absolute moments](../../../../absolute-moment.md). Compactly supported endpoints also suffice because all interpolating points lie in one compact set.

**The printed growth assumption alone does not ensure a classical second derivative.** Here is a counterexample within the stated assumptions. On the line take the bounded nonnegative [smooth function](../../../../smooth-function.md)

$$
V(x)=1-\cos(2\pi x^3),\qquad p_n=cn^{-4}\quad(n\geq1),\qquad c^{-1}=\sum_{n\geq1}n^{-4},
$$

and the [probability measures](../../../../probability-measure.md) $\mu=\sum_np_n\delta_{n-1/2}$, $\nu=\sum_np_n\delta_{n+1/2}$. Both have finite second [absolute moments](../../../../absolute-moment.md). Their translation [transport plan](../../../../transport-plan.md) is optimal: its cost is one, while every [coupling](../../../../coupling.md) has cost at least the square of its mean displacement, also one. At $t_0=1/2$, $z_{t_0}=n$, so $F(t)=\mathcal V[\mu_t]$ satisfies $F(t_0)=0$. Each summand is nonnegative, and the [Fatou lemma](../../../../fatou-s-lemma.md) gives

$$
\liminf_{h\to0}\frac{F(t_0+h)+F(t_0-h)-2F(t_0)}{h^2}\geq\sum_np_nV''(n)=36\pi^2c\sum_n1=\infty.
$$

Thus the requested classical identity requires an additional integrability assumption on the [Hessian matrix](../../../../hessian-matrix.md); quadratic growth controls the energy but not its [second derivative](../../../../second-derivative.md).

For a [confinement potential](../../../../confinement-potential.md) $V$ that is a $\lambda$-[strongly convex function](../../../../strongly-convex-function.md), the derivative formula, where valid, yields

$$
\boxed{\frac{d^2}{dt^2}\mathcal V[\mu_t]\geq\lambda\int|q|^2\,d\Pi=\lambda D^2.}
$$

The underlying [displacement convexity](../../../../displacement-convexity.md) conclusion is valid under the printed assumptions without that extra differentiation hypothesis. Apply [convexity](../../../../convex-function.md) of $V(x)-\lambda|x|^2/2$ pointwise and integrate:

$$
\boxed{\mathcal V[\mu_t]\leq(1-t)\mathcal V[\mu]+t\mathcal V[\nu]-\frac\lambda2t(1-t)D^2.}
$$

The same argument on every subinterval makes $t\mapsto\mathcal V[\mu_t]-\lambda D^2t^2/2$ [convex](../../../../convex-function.md), so the second derivative lower bound also holds in the sense of [distributions](../../../../distribution-mathematical-analysis.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
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
